# Comparing `tmp/langchain_mistralai-0.1.1.tar.gz` & `tmp/langchain_mistralai-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.1.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.2rc1.tar", max compression
```

## Comparing `langchain_mistralai-0.1.1.tar` & `langchain_mistralai-0.1.2rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/LICENSE
--rw-r--r--   0        0        0     1336 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/README.md
--rw-r--r--   0        0        0      173 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    24784 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     5961 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2391 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/LICENSE
+-rw-r--r--   0        0        0     1336 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/README.md
+-rw-r--r--   0        0        0      173 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    26092 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     5961 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2437 2024-04-10 00:56:50.656006 langchain_mistralai-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.2rc1/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.1/LICENSE` & `langchain_mistralai-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.1/README.md` & `langchain_mistralai-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.1/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.2rc1/langchain_mistralai/chat_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     SystemMessageChunk,
     ToolMessage,
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
+    make_invalid_tool_call,
+    parse_tool_call,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.runnables import Runnable, RunnableMap, RunnablePassthrough
 from langchain_core.tools import BaseTool
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 from langchain_core.utils.function_calling import convert_to_openai_tool
@@ -78,17 +80,39 @@
     _message: Dict,
 ) -> BaseMessage:
     role = _message["role"]
     assert role == "assistant", f"Expected role to be 'assistant', got {role}"
     content = cast(str, _message["content"])
 
     additional_kwargs: Dict = {}
-    if tool_calls := _message.get("tool_calls"):
-        additional_kwargs["tool_calls"] = tool_calls
-    return AIMessage(content=content, additional_kwargs=additional_kwargs)
+    tool_calls = []
+    invalid_tool_calls = []
+    if raw_tool_calls := _message.get("tool_calls"):
+        additional_kwargs["tool_calls"] = raw_tool_calls
+        for raw_tool_call in raw_tool_calls:
+            try:
+                parsed: dict = cast(
+                    dict, parse_tool_call(raw_tool_call, return_id=False)
+                )
+                tool_calls.append(
+                    {
+                        **parsed,
+                        **{"id": None},
+                    },
+                )
+            except Exception as e:
+                invalid_tool_calls.append(
+                    dict(make_invalid_tool_call(raw_tool_call, str(e)))
+                )
+    return AIMessage(
+        content=content,
+        additional_kwargs=additional_kwargs,
+        tool_calls=tool_calls,
+        invalid_tool_calls=invalid_tool_calls,
+    )
 
 
 async def _aiter_sse(
     event_source_mgr: AsyncContextManager[EventSource],
 ) -> AsyncIterator[Dict]:
     """Iterate over the server-sent events."""
     async with event_source_mgr as event_source:
@@ -129,17 +153,35 @@
 ) -> BaseMessageChunk:
     role = _delta.get("role")
     content = _delta.get("content") or ""
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         additional_kwargs: Dict = {}
-        if tool_calls := _delta.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
-        return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
+        if raw_tool_calls := _delta.get("tool_calls"):
+            additional_kwargs["tool_calls"] = raw_tool_calls
+            try:
+                tool_call_chunks = [
+                    {
+                        "name": rtc["function"].get("name"),
+                        "args": rtc["function"].get("arguments"),
+                        "id": rtc.get("id"),
+                        "index": rtc.get("index"),
+                    }
+                    for rtc in raw_tool_calls
+                ]
+            except KeyError:
+                pass
+        else:
+            tool_call_chunks = []
+        return AIMessageChunk(
+            content=content,
+            additional_kwargs=additional_kwargs,
+            tool_call_chunks=tool_call_chunks,
+        )
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role)
     else:
         return default_class(content=content)
 
@@ -159,15 +201,15 @@
                         "name": tc["function"]["name"],
                         "arguments": tc["function"]["arguments"],
                     }
                 }
                 for tc in message.additional_kwargs["tool_calls"]
             ]
         else:
-            tool_calls = None
+            tool_calls = []
         return {
             "role": "assistant",
             "content": message.content,
             "tool_calls": tool_calls,
         }
     elif isinstance(message, SystemMessage):
         return dict(role="system", content=message.content)
```

### Comparing `langchain_mistralai-0.1.1/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.2rc1/langchain_mistralai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.1/pyproject.toml` & `langchain_mistralai-0.1.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.1"
+version = "0.1.2rc1"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.41"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 tokenizers = "^0.15.1"
 httpx = ">=0.25.2,<1"
 httpx-sse = ">=0.3.1,<1"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_mistralai-0.1.1/PKG-INFO` & `langchain_mistralai-0.1.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: httpx-sse (>=0.3.1,<1)
-Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai
 Description-Content-Type: text/markdown
 
 # langchain-mistralai
```

