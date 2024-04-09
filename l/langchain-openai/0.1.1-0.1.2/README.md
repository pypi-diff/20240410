# Comparing `tmp/langchain_openai-0.1.1.tar.gz` & `tmp/langchain_openai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.1.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.2.tar", max compression
```

## Comparing `langchain_openai-0.1.1.tar` & `langchain_openai-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/LICENSE
--rw-r--r--   0        0        0     1627 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/README.md
--rw-r--r--   0        0        0      371 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10420 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    42224 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6660 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24043 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/langchain_openai/py.typed
--rw-r--r--   0        0        0     2697 2024-03-22 21:42:25.924055 langchain_openai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/README.md
+-rw-r--r--   0        0        0      371 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10508 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    43553 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    23294 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8008 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24477 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2817 2024-04-09 21:56:01.847400 langchain_openai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.2/PKG-INFO
```

### Comparing `langchain_openai-0.1.1/LICENSE` & `langchain_openai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.1/README.md` & `langchain_openai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.1/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.2/langchain_openai/chat_models/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,18 @@
                 **client_params, **async_specific
             ).chat.completions
         return values
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
-        return {**self._default_params}
+        return {
+            **{"azure_deployment": self.deployment_name},
+            **super()._identifying_params,
+        }
 
     @property
     def _llm_type(self) -> str:
         return "azure-openai-chat"
 
     @property
     def lc_attributes(self) -> Dict[str, Any]:
```

### Comparing `langchain_openai-0.1.1/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.2/langchain_openai/chat_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     in, even if not explicitly saved on this class.
 
     Example:
         .. code-block:: python
 
             from langchain_openai import ChatOpenAI
 
-            model = ChatOpenAI(model_name="gpt-3.5-turbo")
+            model = ChatOpenAI(model="gpt-3.5-turbo")
     """
 
     @property
     def lc_secrets(self) -> Dict[str, str]:
         return {"openai_api_key": "OPENAI_API_KEY"}
 
     @classmethod
@@ -376,20 +376,39 @@
             "base_url": values["openai_api_base"],
             "timeout": values["request_timeout"],
             "max_retries": values["max_retries"],
             "default_headers": values["default_headers"],
             "default_query": values["default_query"],
         }
 
+        openai_proxy = values["openai_proxy"]
         if not values.get("client"):
+            if openai_proxy and not values["http_client"]:
+                try:
+                    import httpx
+                except ImportError as e:
+                    raise ImportError(
+                        "Could not import httpx python package. "
+                        "Please install it with `pip install httpx`."
+                    ) from e
+                values["http_client"] = httpx.Client(proxy=openai_proxy)
             sync_specific = {"http_client": values["http_client"]}
             values["client"] = openai.OpenAI(
                 **client_params, **sync_specific
             ).chat.completions
         if not values.get("async_client"):
+            if openai_proxy and not values["http_async_client"]:
+                try:
+                    import httpx
+                except ImportError as e:
+                    raise ImportError(
+                        "Could not import httpx python package. "
+                        "Please install it with `pip install httpx`."
+                    ) from e
+                values["http_async_client"] = httpx.AsyncClient(proxy=openai_proxy)
             async_specific = {"http_client": values["http_async_client"]}
             values["async_client"] = openai.AsyncOpenAI(
                 **client_params, **async_specific
             ).chat.completions
         return values
 
     @property
@@ -434,57 +453,56 @@
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs, "stream": True}
 
         default_chunk_class = AIMessageChunk
-        for chunk in self.client.create(messages=message_dicts, **params):
-            if not isinstance(chunk, dict):
-                chunk = chunk.model_dump()
-            if len(chunk["choices"]) == 0:
-                continue
-            choice = chunk["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
-            )
-            generation_info = {}
-            if finish_reason := choice.get("finish_reason"):
-                generation_info["finish_reason"] = finish_reason
-            logprobs = choice.get("logprobs")
-            if logprobs:
-                generation_info["logprobs"] = logprobs
-            default_chunk_class = chunk.__class__
-            chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
-            )
-            if run_manager:
-                run_manager.on_llm_new_token(chunk.text, chunk=chunk, logprobs=logprobs)
-            yield chunk
+        with self.client.create(messages=message_dicts, **params) as response:
+            for chunk in response:
+                if not isinstance(chunk, dict):
+                    chunk = chunk.model_dump()
+                if len(chunk["choices"]) == 0:
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
+                )
+                if run_manager:
+                    run_manager.on_llm_new_token(
+                        chunk.text, chunk=chunk, logprobs=logprobs
+                    )
+                yield chunk
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
-        stream: Optional[bool] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        should_stream = stream if stream is not None else self.streaming
-        if should_stream:
+        if self.streaming:
             stream_iter = self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return generate_from_stream(stream_iter)
         message_dicts, params = self._create_message_dicts(messages, stop)
-        params = {
-            **params,
-            **({"stream": stream} if stream is not None else {}),
-            **kwargs,
-        }
+        params = {**params, **kwargs}
         response = self.client.create(messages=message_dicts, **params)
         return self._create_chat_result(response)
 
     def _create_message_dicts(
         self, messages: List[BaseMessage], stop: Optional[List[str]]
     ) -> Tuple[List[Dict[str, Any]], Dict[str, Any]]:
         params = self._default_params
@@ -497,14 +515,22 @@
 
     def _create_chat_result(
         self, response: Union[dict, openai.BaseModel]
     ) -> ChatResult:
         generations = []
         if not isinstance(response, dict):
             response = response.model_dump()
+
+        # Sometimes the AI Model calling will get error, we should raise it.
+        # Otherwise, the next code 'choices.extend(response["choices"])'
+        # will throw a "TypeError: 'NoneType' object is not iterable" error
+        # to mask the true error. Because 'response["choices"]' is None.
+        if response.get("error"):
+            raise ValueError(response.get("error"))
+
         for res in response["choices"]:
             message = _convert_dict_to_message(res["message"])
             generation_info = dict(finish_reason=res.get("finish_reason"))
             if "logprobs" in res:
                 generation_info["logprobs"] = res["logprobs"]
             gen = ChatGeneration(
                 message=message,
@@ -526,62 +552,58 @@
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         message_dicts, params = self._create_message_dicts(messages, stop)
         params = {**params, **kwargs, "stream": True}
 
         default_chunk_class = AIMessageChunk
-        async for chunk in await self.async_client.create(
-            messages=message_dicts, **params
-        ):
-            if not isinstance(chunk, dict):
-                chunk = chunk.model_dump()
-            if len(chunk["choices"]) == 0:
-                continue
-            choice = chunk["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
-            )
-            generation_info = {}
-            if finish_reason := choice.get("finish_reason"):
-                generation_info["finish_reason"] = finish_reason
-            logprobs = choice.get("logprobs")
-            if logprobs:
-                generation_info["logprobs"] = logprobs
-            default_chunk_class = chunk.__class__
-            chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
-            )
-            if run_manager:
-                await run_manager.on_llm_new_token(
-                    token=chunk.text, chunk=chunk, logprobs=logprobs
+        response = await self.async_client.create(messages=message_dicts, **params)
+        async with response:
+            async for chunk in response:
+                if not isinstance(chunk, dict):
+                    chunk = chunk.model_dump()
+                if len(chunk["choices"]) == 0:
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
                 )
-            yield chunk
+                if run_manager:
+                    await run_manager.on_llm_new_token(
+                        token=chunk.text, chunk=chunk, logprobs=logprobs
+                    )
+                yield chunk
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
-        stream: Optional[bool] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        should_stream = stream if stream is not None else self.streaming
-        if should_stream:
+        if self.streaming:
             stream_iter = self._astream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return await agenerate_from_stream(stream_iter)
 
         message_dicts, params = self._create_message_dicts(messages, stop)
-        params = {
-            **params,
-            **({"stream": stream} if stream is not None else {}),
-            **kwargs,
-        }
+        params = {**params, **kwargs}
         response = await self.async_client.create(messages=message_dicts, **params)
         return self._create_chat_result(response)
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {"model_name": self.model_name, **self._default_params}
```

### Comparing `langchain_openai-0.1.1/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.2/langchain_openai/embeddings/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Azure OpenAI embeddings wrapper."""
+
 from __future__ import annotations
 
 import os
 from typing import Callable, Dict, Optional, Union
 
 import openai
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
@@ -53,14 +54,16 @@
     """A function that returns an Azure Active Directory token.
 
         Will be invoked on every request.
     """
     openai_api_version: Optional[str] = Field(default=None, alias="api_version")
     """Automatically inferred from env var `OPENAI_API_VERSION` if not provided."""
     validate_base_url: bool = True
+    chunk_size: int = 2048
+    """Maximum number of texts to embed in each batch"""
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         # Check OPENAI_KEY for backwards compatibility.
         # TODO: Remove OPENAI_API_KEY support to avoid possible conflict when using
         # other forms of azure credentials.
@@ -95,18 +98,14 @@
         values["azure_endpoint"] = values["azure_endpoint"] or os.getenv(
             "AZURE_OPENAI_ENDPOINT"
         )
         azure_ad_token = values["azure_ad_token"] or os.getenv("AZURE_OPENAI_AD_TOKEN")
         values["azure_ad_token"] = (
             convert_to_secret_str(azure_ad_token) if azure_ad_token else None
         )
-        # Azure OpenAI embedding models allow a maximum of 16 texts
-        # at a time in each batch
-        # See: https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#embeddings
-        values["chunk_size"] = min(values["chunk_size"], 16)
         # For backwards compatibility. Before openai v1, no distinction was made
         # between azure_endpoint and base_url (openai_api_base).
         openai_api_base = values["openai_api_base"]
         if openai_api_base and values["validate_base_url"]:
             if "/openai" not in openai_api_base:
                 values["openai_api_base"] += "/openai"
                 raise ValueError(
@@ -122,20 +121,24 @@
                     "Instead use `deployment` (or alias `azure_deployment`) "
                     "and `azure_endpoint`."
                 )
         client_params = {
             "api_version": values["openai_api_version"],
             "azure_endpoint": values["azure_endpoint"],
             "azure_deployment": values["deployment"],
-            "api_key": values["openai_api_key"].get_secret_value()
-            if values["openai_api_key"]
-            else None,
-            "azure_ad_token": values["azure_ad_token"].get_secret_value()
-            if values["azure_ad_token"]
-            else None,
+            "api_key": (
+                values["openai_api_key"].get_secret_value()
+                if values["openai_api_key"]
+                else None
+            ),
+            "azure_ad_token": (
+                values["azure_ad_token"].get_secret_value()
+                if values["azure_ad_token"]
+                else None
+            ),
             "azure_ad_token_provider": values["azure_ad_token_provider"],
             "organization": values["openai_organization"],
             "base_url": values["openai_api_base"],
             "timeout": values["request_timeout"],
             "max_retries": values["max_retries"],
             "default_headers": values["default_headers"],
             "default_query": values["default_query"],
```

### Comparing `langchain_openai-0.1.1/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.2/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.1/langchain_openai/llms/azure.py` & `langchain_openai-0.1.2/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.1/langchain_openai/llms/base.py` & `langchain_openai-0.1.2/langchain_openai/llms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,21 @@
             else:
                 response = self.client.create(prompt=_prompts, **params)
                 if not isinstance(response, dict):
                     # V1 client returns the response in an PyDantic object instead of
                     # dict. For the transition period, we deep convert it to dict.
                     response = response.model_dump()
 
+                # Sometimes the AI Model calling will get error, we should raise it.
+                # Otherwise, the next code 'choices.extend(response["choices"])'
+                # will throw a "TypeError: 'NoneType' object is not iterable" error
+                # to mask the true error. Because 'response["choices"]' is None.
+                if response.get("error"):
+                    raise ValueError(response.get("error"))
+
                 choices.extend(response["choices"])
                 _update_token_usage(_keys, response, token_usage)
                 if not system_fingerprint:
                     system_fingerprint = response.get("system_fingerprint")
         return self.create_llm_result(
             choices,
             prompts,
```

### Comparing `langchain_openai-0.1.1/pyproject.toml` & `langchain_openai-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.1"
+version = "0.1.2"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.33"
+langchain-core = "^0.1.41"
 openai = "^1.10.0"
 tiktoken = ">=0.5.2,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
+pytest-cov = "^4.1.0"
+langchain-standard-tests = {path = "../../standard-tests", develop = true}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -85,15 +87,15 @@
 #
 # https://docs.pytest.org/en/7.1.x/reference/reference.html
 # --strict-config       any warnings encountered while parsing the `pytest`
 #                       section of the configuration file raise errors.
 #
 # https://github.com/tophat/syrupy
 # --snapshot-warn-unused    Prints a warning on unused snapshots rather than fail the test suite.
-addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
+addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5 --cov=langchain_openai"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
   "compile: mark placeholder test used to compile integration tests without running them",
   "scheduled: mark tests to run in scheduled testing",
```

### Comparing `langchain_openai-0.1.1/PKG-INFO` & `langchain_openai-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.1
+Version: 0.1.2
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
-Requires-Dist: langchain-core (>=0.1.33,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

