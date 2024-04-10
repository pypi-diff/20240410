# Comparing `tmp/langchain_anthropic-0.1.7.tar.gz` & `tmp/langchain_anthropic-0.1.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_anthropic-0.1.7.tar", max compression
+gzip compressed data, was "langchain_anthropic-0.1.8rc1.tar", max compression
```

## Comparing `langchain_anthropic-0.1.7.tar` & `langchain_anthropic-0.1.8rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/LICENSE
--rw-r--r--   0        0        0     1215 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/README.md
--rw-r--r--   0        0        0      225 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    25121 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0     4908 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    11687 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/llms.py
--rw-r--r--   0        0        0     2194 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/output_parsers.py
--rw-r--r--   0        0        0        0 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2677 2024-04-09 21:54:55.578792 langchain_anthropic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/LICENSE
+-rw-r--r--   0        0        0     1215 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/README.md
+-rw-r--r--   0        0        0      225 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    26903 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    11687 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2493 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2723 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.8rc1/PKG-INFO
```

### Comparing `langchain_anthropic-0.1.7/LICENSE` & `langchain_anthropic-0.1.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.7/README.md` & `langchain_anthropic-0.1.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.7/langchain_anthropic/chat_models.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 import re
 import warnings
 from operator import itemgetter
 from typing import (
     Any,
     AsyncIterator,
@@ -50,15 +51,15 @@
 from langchain_core.utils import (
     build_extra_kwargs,
     convert_to_secret_str,
     get_pydantic_field_names,
 )
 from langchain_core.utils.function_calling import convert_to_openai_tool
 
-from langchain_anthropic.output_parsers import ToolsOutputParser
+from langchain_anthropic.output_parsers import ToolsOutputParser, extract_tool_calls
 
 _message_type_lookups = {
     "human": "user",
     "ai": "assistant",
     "AIMessageChunk": "assistant",
     "HumanMessageChunk": "user",
 }
@@ -343,15 +344,32 @@
     ) -> Iterator[ChatGenerationChunk]:
         params = self._format_params(messages=messages, stop=stop, **kwargs)
         if _tools_in_params(params):
             warnings.warn("stream: Tool use is not yet supported in streaming mode.")
             result = self._generate(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
-            yield cast(ChatGenerationChunk, result.generations[0])
+            message = result.generations[0].message
+            if isinstance(message, AIMessage) and message.tool_calls is not None:
+                tool_call_chunks = [
+                    {
+                        "name": tool_call["name"],
+                        "args": json.dumps(tool_call["args"]),
+                        "id": tool_call["id"],
+                        "index": idx,
+                    }
+                    for idx, tool_call in enumerate(message.tool_calls)
+                ]
+                message_chunk = AIMessageChunk(
+                    content=message.content,
+                    tool_call_chunks=tool_call_chunks,
+                )
+                yield ChatGenerationChunk(message=message_chunk)
+            else:
+                yield cast(ChatGenerationChunk, result.generations[0])
             return
         with self._client.messages.stream(**params) as stream:
             for text in stream.text_stream:
                 chunk = ChatGenerationChunk(message=AIMessageChunk(content=text))
                 if run_manager:
                     run_manager.on_llm_new_token(text, chunk=chunk)
                 yield chunk
@@ -365,15 +383,32 @@
     ) -> AsyncIterator[ChatGenerationChunk]:
         params = self._format_params(messages=messages, stop=stop, **kwargs)
         if _tools_in_params(params):
             warnings.warn("stream: Tool use is not yet supported in streaming mode.")
             result = await self._agenerate(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
-            yield cast(ChatGenerationChunk, result.generations[0])
+            message = result.generations[0].message
+            if isinstance(message, AIMessage) and message.tool_calls is not None:
+                tool_call_chunks = [
+                    {
+                        "name": tool_call["name"],
+                        "args": json.dumps(tool_call["args"]),
+                        "id": tool_call["id"],
+                        "index": idx,
+                    }
+                    for idx, tool_call in enumerate(message.tool_calls)
+                ]
+                message_chunk = AIMessageChunk(
+                    content=message.content,
+                    tool_call_chunks=tool_call_chunks,
+                )
+                yield ChatGenerationChunk(message=message_chunk)
+            else:
+                yield cast(ChatGenerationChunk, result.generations[0])
             return
         async with self._async_client.messages.stream(**params) as stream:
             async for text in stream.text_stream:
                 chunk = ChatGenerationChunk(message=AIMessageChunk(content=text))
                 if run_manager:
                     await run_manager.on_llm_new_token(text, chunk=chunk)
                 yield chunk
@@ -382,14 +417,20 @@
         data_dict = data.model_dump()
         content = data_dict["content"]
         llm_output = {
             k: v for k, v in data_dict.items() if k not in ("content", "role", "type")
         }
         if len(content) == 1 and content[0]["type"] == "text":
             msg = AIMessage(content=content[0]["text"])
+        elif any(block["type"] == "tool_use" for block in content):
+            tool_calls = extract_tool_calls(content)
+            msg = AIMessage(
+                content=content,
+                tool_calls=tool_calls,
+            )
         else:
             msg = AIMessage(content=content)
         return ChatResult(
             generations=[ChatGeneration(message=msg)],
             llm_output=llm_output,
         )
```

### Comparing `langchain_anthropic-0.1.7/langchain_anthropic/experimental.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.7/langchain_anthropic/llms.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.7/langchain_anthropic/output_parsers.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-from typing import Any, List, Optional, Type, TypedDict, cast
+from typing import Any, List, Optional, Type
 
-from langchain_core.messages import BaseMessage
+from langchain_core.messages import ToolCall
 from langchain_core.output_parsers import BaseGenerationOutputParser
 from langchain_core.outputs import ChatGeneration, Generation
 from langchain_core.pydantic_v1 import BaseModel
 
 
-class _ToolCall(TypedDict):
-    name: str
-    args: dict
-    id: str
-    index: int
-
-
 class ToolsOutputParser(BaseGenerationOutputParser):
     first_tool_only: bool = False
     args_only: bool = False
     pydantic_schemas: Optional[List[Type[BaseModel]]] = None
 
     class Config:
         extra = "forbid"
@@ -29,38 +22,48 @@
                 to be different candidate outputs for a single model input.
 
         Returns:
             Structured output.
         """
         if not result or not isinstance(result[0], ChatGeneration):
             return None if self.first_tool_only else []
-        tool_calls: List = _extract_tool_calls(result[0].message)
+        message = result[0].message
+        if isinstance(message.content, str):
+            tool_calls: List = []
+        else:
+            content: List = message.content
+            _tool_calls = [dict(tc) for tc in extract_tool_calls(content)]
+            # Map tool call id to index
+            id_to_index = {
+                block["id"]: i
+                for i, block in enumerate(content)
+                if block["type"] == "tool_use"
+            }
+            tool_calls = [{**tc, "index": id_to_index[tc["id"]]} for tc in _tool_calls]
         if self.pydantic_schemas:
             tool_calls = [self._pydantic_parse(tc) for tc in tool_calls]
         elif self.args_only:
             tool_calls = [tc["args"] for tc in tool_calls]
         else:
             pass
 
         if self.first_tool_only:
             return tool_calls[0] if tool_calls else None
         else:
-            return tool_calls
+            return [tool_call for tool_call in tool_calls]
 
-    def _pydantic_parse(self, tool_call: _ToolCall) -> BaseModel:
+    def _pydantic_parse(self, tool_call: dict) -> BaseModel:
         cls_ = {schema.__name__: schema for schema in self.pydantic_schemas or []}[
             tool_call["name"]
         ]
         return cls_(**tool_call["args"])
 
 
-def _extract_tool_calls(msg: BaseMessage) -> List[_ToolCall]:
-    if isinstance(msg.content, str):
-        return []
+def extract_tool_calls(content: List[dict]) -> List[ToolCall]:
     tool_calls = []
-    for i, block in enumerate(cast(List[dict], msg.content)):
+    for block in content:
         if block["type"] != "tool_use":
             continue
         tool_calls.append(
-            _ToolCall(name=block["name"], args=block["input"], id=block["id"], index=i)
+            ToolCall(name=block["name"], args=block["input"], id=block["id"])
         )
     return tool_calls
```

### Comparing `langchain_anthropic-0.1.7/pyproject.toml` & `langchain_anthropic-0.1.8rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-anthropic"
-version = "0.1.7"
+version = "0.1.8rc1"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.41"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 anthropic = ">=0.23.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_anthropic-0.1.7/PKG-INFO` & `langchain_anthropic-0.1.8rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-anthropic
-Version: 0.1.7
+Version: 0.1.8rc1
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

