# Comparing `tmp/langchain_openai-0.1.2.tar.gz` & `tmp/langchain_openai-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.2.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.3rc1.tar", max compression
```

## Comparing `langchain_openai-0.1.2.tar` & `langchain_openai-0.1.3rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/README.md
--rw-r--r--   0        0        0      371 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    43553 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24477 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/py.typed
--rw-r--r--   0        0        0     2817 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      371 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-10 00:56:48.250765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10508 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    44617 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    23294 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8008 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24477 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2865 2024-04-10 00:56:48.254765 langchain_openai-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 langchain_openai-0.1.3rc1/PKG-INFO
```

### Comparing `langchain_openai-0.1.2/LICENSE` & `langchain_openai-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/README.md` & `langchain_openai-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/chat_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     JsonOutputParser,
     PydanticOutputParser,
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
 from langchain_core.utils import (
     convert_to_secret_str,
@@ -99,18 +101,32 @@
     elif role == "assistant":
         # Fix for azure
         # Also OpenAI returns None for tool invocations
         content = _dict.get("content", "") or ""
         additional_kwargs: Dict = {}
         if function_call := _dict.get("function_call"):
             additional_kwargs["function_call"] = dict(function_call)
-        if tool_calls := _dict.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
+        tool_calls = []
+        invalid_tool_calls = []
+        if raw_tool_calls := _dict.get("tool_calls"):
+            additional_kwargs["tool_calls"] = raw_tool_calls
+            for raw_tool_call in raw_tool_calls:
+                try:
+                    tool_calls.append(parse_tool_call(raw_tool_call, return_id=True))
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        make_invalid_tool_call(raw_tool_call, str(e))
+                    )
         return AIMessage(
-            content=content, additional_kwargs=additional_kwargs, name=name, id=id_
+            content=content,
+            additional_kwargs=additional_kwargs,
+            name=name,
+            id=id_,
+            tool_calls=tool_calls,
+            invalid_tool_calls=invalid_tool_calls,
         )
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""), name=name, id=id_)
     elif role == "function":
         return FunctionMessage(
             content=_dict.get("content", ""), name=cast(str, _dict.get("name")), id=id_
         )
@@ -184,22 +200,38 @@
     content = cast(str, _dict.get("content") or "")
     additional_kwargs: Dict = {}
     if _dict.get("function_call"):
         function_call = dict(_dict["function_call"])
         if "name" in function_call and function_call["name"] is None:
             function_call["name"] = ""
         additional_kwargs["function_call"] = function_call
-    if _dict.get("tool_calls"):
-        additional_kwargs["tool_calls"] = _dict["tool_calls"]
+    tool_call_chunks = []
+    if raw_tool_calls := _dict.get("tool_calls"):
+        additional_kwargs["tool_calls"] = raw_tool_calls
+        try:
+            tool_call_chunks = [
+                {
+                    "name": rtc["function"].get("name"),
+                    "args": rtc["function"].get("arguments"),
+                    "id": rtc.get("id"),
+                    "index": rtc["index"],
+                }
+                for rtc in raw_tool_calls
+            ]
+        except KeyError:
+            pass
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content, id=id_)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(
-            content=content, additional_kwargs=additional_kwargs, id=id_
+            content=content,
+            additional_kwargs=additional_kwargs,
+            id=id_,
+            tool_call_chunks=tool_call_chunks,
         )
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content, id=id_)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"], id=id_)
     elif role == "tool" or default_class == ToolMessageChunk:
         return ToolMessageChunk(
```

### Comparing `langchain_openai-0.1.2/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/langchain_openai/llms/azure.py` & `langchain_openai-0.1.3rc1/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/langchain_openai/llms/base.py` & `langchain_openai-0.1.3rc1/langchain_openai/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.2/pyproject.toml` & `langchain_openai-0.1.3rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.2"
+version = "0.1.3rc1"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.41"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 openai = "^1.10.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -24,15 +24,15 @@
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
 pytest-cov = "^4.1.0"
-langchain-standard-tests = {path = "../../standard-tests", develop = true}
+langchain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_openai-0.1.2/PKG-INFO` & `langchain_openai-0.1.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.2
+Version: 0.1.3rc1
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

