# Comparing `tmp/promptflow_tracing-1.0.0-py3-none-any.whl.zip` & `tmp/promptflow_tracing-1.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20821 bytes, number of entries: 18
+Zip file size: 21795 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      412 b- defN 80-Jan-01 00:00 promptflow/tracing/__init__.py
 -rw-r--r--  2.0 unx      400 b- defN 80-Jan-01 00:00 promptflow/tracing/_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 promptflow/tracing/_integrations/__init__.py
--rw-r--r--  2.0 unx     7883 b- defN 80-Jan-01 00:00 promptflow/tracing/_integrations/_openai_injector.py
--rw-r--r--  2.0 unx    10489 b- defN 80-Jan-01 00:00 promptflow/tracing/_openai_utils.py
+-rw-r--r--  2.0 unx     8399 b- defN 80-Jan-01 00:00 promptflow/tracing/_integrations/_openai_injector.py
+-rw-r--r--  2.0 unx    10353 b- defN 80-Jan-01 00:00 promptflow/tracing/_openai_utils.py
 -rw-r--r--  2.0 unx     7470 b- defN 80-Jan-01 00:00 promptflow/tracing/_operation_context.py
--rw-r--r--  2.0 unx     3093 b- defN 80-Jan-01 00:00 promptflow/tracing/_start_trace.py
+-rw-r--r--  2.0 unx     3500 b- defN 80-Jan-01 00:00 promptflow/tracing/_start_trace.py
 -rw-r--r--  2.0 unx     1138 b- defN 80-Jan-01 00:00 promptflow/tracing/_thread_local_singleton.py
--rw-r--r--  2.0 unx    17389 b- defN 80-Jan-01 00:00 promptflow/tracing/_trace.py
--rw-r--r--  2.0 unx     7104 b- defN 80-Jan-01 00:00 promptflow/tracing/_tracer.py
+-rw-r--r--  2.0 unx    18907 b- defN 80-Jan-01 00:00 promptflow/tracing/_trace.py
+-rw-r--r--  2.0 unx     7297 b- defN 80-Jan-01 00:00 promptflow/tracing/_tracer.py
 -rw-r--r--  2.0 unx     3372 b- defN 80-Jan-01 00:00 promptflow/tracing/_utils.py
 -rw-r--r--  2.0 unx      299 b- defN 80-Jan-01 00:00 promptflow/tracing/_version.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/__init__.py
 -rw-r--r--  2.0 unx      696 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/generator_proxy.py
--rw-r--r--  2.0 unx     2034 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/trace.py
--rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 promptflow_tracing-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_tracing-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1639 b- defN 16-Jan-01 00:00 promptflow_tracing-1.0.0.dist-info/RECORD
-18 files, 65049 bytes uncompressed, 18081 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx     2091 b- defN 80-Jan-01 00:00 promptflow/tracing/contracts/trace.py
+-rw-r--r--  2.0 unx     2227 b- defN 80-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1639 b- defN 16-Jan-01 00:00 promptflow_tracing-1.8.0.dist-info/RECORD
+18 files, 68550 bytes uncompressed, 19055 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -39,17 +39,17 @@
 
 Filename: promptflow/tracing/contracts/generator_proxy.py
 Comment: 
 
 Filename: promptflow/tracing/contracts/trace.py
 Comment: 
 
-Filename: promptflow_tracing-1.0.0.dist-info/METADATA
+Filename: promptflow_tracing-1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: promptflow_tracing-1.0.0.dist-info/WHEEL
+Filename: promptflow_tracing-1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow_tracing-1.0.0.dist-info/RECORD
+Filename: promptflow_tracing-1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow/tracing/_constants.py

```diff
@@ -1,13 +1,13 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 
 class ResourceAttributesFieldName:
     SERVICE_NAME = "service.name"
-    SESSION_ID = "session.id"
+    COLLECTION = "collection"
 
 
 RESOURCE_ATTRIBUTES_SERVICE_NAME = "promptflow"
 
 PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON = "PF_TRACING_SKIP_LOCAL_SETUP"
```

## promptflow/tracing/_integrations/_openai_injector.py

```diff
@@ -17,24 +17,24 @@
 from ..contracts.trace import TraceType
 
 USER_AGENT_HEADER = "x-ms-useragent"
 PROMPTFLOW_HEADER = "ms-azure-ai-promptflow"
 IS_LEGACY_OPENAI = version("openai").startswith("0.")
 
 
-def inject_function_async(args_to_ignore=None, trace_type=TraceType.LLM):
+def inject_function_async(args_to_ignore=None, trace_type=TraceType.LLM, name=None):
     def decorator(func):
-        return _traced_async(func, args_to_ignore=args_to_ignore, trace_type=trace_type)
+        return _traced_async(func, args_to_ignore=args_to_ignore, trace_type=trace_type, name=name)
 
     return decorator
 
 
-def inject_function_sync(args_to_ignore=None, trace_type=TraceType.LLM):
+def inject_function_sync(args_to_ignore=None, trace_type=TraceType.LLM, name=None):
     def decorator(func):
-        return _traced_sync(func, args_to_ignore=args_to_ignore, trace_type=trace_type)
+        return _traced_sync(func, args_to_ignore=args_to_ignore, trace_type=trace_type, name=name)
 
     return decorator
 
 
 def get_aoai_telemetry_headers() -> dict:
     """Get the http headers for AOAI request.
 
@@ -86,68 +86,75 @@
         def wrapper(*args, **kwargs):
             inject_headers(kwargs)
             return f(*args, **kwargs)
 
     return wrapper
 
 
-def inject_async(f, trace_type):
+def inject_async(f, trace_type, name):
     wrapper_fun = inject_operation_headers(
-        (inject_function_async(["api_key", "headers", "extra_headers"], trace_type)(f))
+        (inject_function_async(["api_key", "headers", "extra_headers"], trace_type, name)(f))
     )
     wrapper_fun._original = f
     return wrapper_fun
 
 
-def inject_sync(f, trace_type):
+def inject_sync(f, trace_type, name):
     wrapper_fun = inject_operation_headers(
-        (inject_function_sync(["api_key", "headers", "extra_headers"], trace_type)(f))
+        (inject_function_sync(["api_key", "headers", "extra_headers"], trace_type, name)(f))
     )
     wrapper_fun._original = f
     return wrapper_fun
 
 
+def _legacy_openai_apis():
+    sync_apis = (
+        ("openai", "Completion", "create", TraceType.LLM, "openai_completion_legacy"),
+        ("openai", "ChatCompletion", "create", TraceType.LLM, "openai_chat_legacy"),
+        ("openai", "Embedding", "create", TraceType.EMBEDDING, "openai_embedding_legacy"),
+    )
+    async_apis = (
+        ("openai", "Completion", "acreate", TraceType.LLM, "openai_completion_legacy"),
+        ("openai", "ChatCompletion", "acreate", TraceType.LLM, "openai_chat_legacy"),
+        ("openai", "Embedding", "acreate", TraceType.EMBEDDING, "openai_embedding_legacy"),
+    )
+    return sync_apis, async_apis
+
+
+def _openai_apis():
+    sync_apis = (
+        ("openai.resources.chat", "Completions", "create", TraceType.LLM, "openai_chat"),
+        ("openai.resources", "Completions", "create", TraceType.LLM, "openai_completion"),
+        ("openai.resources", "Embeddings", "create", TraceType.EMBEDDING, "openai_embeddings"),
+    )
+    async_apis = (
+        ("openai.resources.chat", "AsyncCompletions", "create", TraceType.LLM, "openai_chat_async"),
+        ("openai.resources", "AsyncCompletions", "create", TraceType.LLM, "openai_completion_async"),
+        ("openai.resources", "AsyncEmbeddings", "create", TraceType.EMBEDDING, "openai_embeddings_async"),
+    )
+    return sync_apis, async_apis
+
+
 def _openai_api_list():
     if IS_LEGACY_OPENAI:
-        sync_apis = (
-            ("openai", "Completion", "create", TraceType.LLM),
-            ("openai", "ChatCompletion", "create", TraceType.LLM),
-            ("openai", "Embedding", "create", TraceType.EMBEDDING),
-        )
-
-        async_apis = (
-            ("openai", "Completion", "acreate", TraceType.LLM),
-            ("openai", "ChatCompletion", "acreate", TraceType.LLM),
-            ("openai", "Embedding", "acreate", TraceType.EMBEDDING),
-        )
+        sync_apis, async_apis = _legacy_openai_apis()
     else:
-        sync_apis = (
-            ("openai.resources.chat", "Completions", "create", TraceType.LLM),
-            ("openai.resources", "Completions", "create", TraceType.LLM),
-            ("openai.resources", "Embeddings", "create", TraceType.EMBEDDING),
-        )
-
-        async_apis = (
-            ("openai.resources.chat", "AsyncCompletions", "create", TraceType.LLM),
-            ("openai.resources", "AsyncCompletions", "create", TraceType.LLM),
-            ("openai.resources", "AsyncEmbeddings", "create", TraceType.EMBEDDING),
-        )
-
+        sync_apis, async_apis = _openai_apis()
     yield sync_apis, inject_sync
     yield async_apis, inject_async
 
 
 def _generate_api_and_injector(apis):
     for apis, injector in apis:
-        for module_name, class_name, method_name, trace_type in apis:
+        for module_name, class_name, method_name, trace_type, name in apis:
             try:
                 module = importlib.import_module(module_name)
                 api = getattr(module, class_name)
                 if hasattr(api, method_name):
-                    yield api, method_name, trace_type, injector
+                    yield api, method_name, trace_type, injector, name
             except AttributeError as e:
                 # Log the attribute exception with the missing class information
                 logging.warning(
                     f"AttributeError: The module '{module_name}' does not have the class '{class_name}'. {str(e)}"
                 )
             except Exception as e:
                 # Log other exceptions as a warning, as we're not sure what they might be
@@ -172,18 +179,18 @@
 def inject_openai_api():
     """This function:
     1. Modifies the create methods of the OpenAI API classes to inject logic before calling the original methods.
     It stores the original methods as _original attributes of the create methods.
     2. Updates the openai api configs from environment variables.
     """
 
-    for api, method, trace_type, injector in available_openai_apis_and_injectors():
+    for api, method, trace_type, injector, name in available_openai_apis_and_injectors():
         # Check if the create method of the openai_api class has already been modified
         if not hasattr(getattr(api, method), "_original"):
-            setattr(api, method, injector(getattr(api, method), trace_type))
+            setattr(api, method, injector(getattr(api, method), trace_type, name))
 
     if IS_LEGACY_OPENAI:
         # For the openai versions lower than 1.0.0, it reads api configs from environment variables only at
         # import time. So we need to update the openai api configs from environment variables here.
         # Please refer to this issue: https://github.com/openai/openai-python/issues/557.
         # The issue has been fixed in openai>=1.0.0.
         openai.api_key = os.environ.get("OPENAI_API_KEY", openai.api_key)
@@ -194,10 +201,10 @@
         openai.api_version = os.environ.get("OPENAI_API_VERSION", openai.api_version)
 
 
 def recover_openai_api():
     """This function restores the original create methods of the OpenAI API classes
     by assigning them back from the _original attributes of the modified methods.
     """
-    for api, method, _, _ in available_openai_apis_and_injectors():
+    for api, method, _, _, _ in available_openai_apis_and_injectors():
         if hasattr(getattr(api, method), "_original"):
             setattr(api, method, getattr(getattr(api, method), "_original"))
```

## promptflow/tracing/_openai_utils.py

```diff
@@ -53,21 +53,21 @@
         # Legacy api:
         #   https://github.com/openai/openai-python/blob/v0.28.1/openai/api_resources/chat_completion.py
         #   https://github.com/openai/openai-python/blob/v0.28.1/openai/api_resources/completion.py
         # OpenAI v1 api:
         #   https://github.com/openai/openai-python/blob/main/src/openai/resources/chat/completions.py
         #   https://github.com/openai/openai-python/blob/main/src/openai/resources/completions.py
         if (
-            name == "openai.api_resources.chat_completion.ChatCompletion.create"
-            or name == "openai.resources.chat.completions.Completions.create"  # openai v1
+            name == "openai_chat_legacy"
+            or name == "openai_chat"  # openai v1
         ):
             return self.get_openai_metrics_for_chat_api(inputs, output)
         elif (
-            name == "openai.api_resources.completion.Completion.create"
-            or name == "openai.resources.completions.Completions.create"  # openai v1
+            name == "openai_completion_legacy"
+            or name == "openai_completion"  # openai v1
         ):
             return self.get_openai_metrics_for_completion_api(inputs, output)
         else:
             self._log_warning(f"Calculating metrics for api {name} is not supported.")
 
     def _try_get_model(self, inputs, output):
         if IS_LEGACY_OPENAI:
```

## promptflow/tracing/_start_trace.py

```diff
@@ -2,66 +2,76 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 import os
 import typing
 
 from opentelemetry import trace
+from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_ENDPOINT
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
 from ._constants import (
     PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON,
     RESOURCE_ATTRIBUTES_SERVICE_NAME,
     ResourceAttributesFieldName,
 )
 from ._integrations._openai_injector import inject_openai_api
 
 
 def start_trace(
     *,
     resource_attributes: typing.Optional[dict] = None,
-    session: typing.Optional[str] = None,
+    collection: typing.Optional[str] = None,
     **kwargs,
 ):
-    """Start a tracing session.
+    """Promptflow instrumentation.
 
-    Instrument `openai`, and set tracer provider for current tracing session.
+    Instrument `openai`, and set tracer provider for current process.
 
-    :param resource_attributes: Specify the resource attributes for current tracing session.
+    :param resource_attributes: Specify the resource attributes for current process.
     :type resource_attributes: typing.Optional[dict]
-    :param session: Specify the session id for current tracing session.
-    :type session: typing.Optional[str]
+    :param collection: Specify the collection for current tracing.
+    :type collection: typing.Optional[str]
     """
+
+    # When PF_TRACING_SKIP_LOCAL_SETUP_ENVIRON is set to true, the start_trace should be skipped.
+    # An example is that user call start_trace at cloud mode. Nothing should happen.
+    if _skip_tracing_local_setup():
+        return
+
     # prepare resource.attributes and set tracer provider
     res_attrs = {ResourceAttributesFieldName.SERVICE_NAME: RESOURCE_ATTRIBUTES_SERVICE_NAME}
-    if session is not None:
-        res_attrs[ResourceAttributesFieldName.SESSION_ID] = session
+    if collection is not None:
+        res_attrs[ResourceAttributesFieldName.COLLECTION] = collection
     if isinstance(resource_attributes, dict):
         for attr_key, attr_value in resource_attributes.items():
             res_attrs[attr_key] = attr_value
     _set_tracer_provider(res_attrs)
 
-    if _skip_tracing_local_setup():
-        return
-
     if _is_devkit_installed():
         from promptflow._sdk._tracing import start_trace_with_devkit
 
         start_trace_with_devkit(
-            session_id=session,
+            collection=collection,
             attrs=kwargs.get("attributes", None),
             run=kwargs.get("run", None),
         )
 
 
 def setup_exporter_from_environ() -> None:
+
     # openai instrumentation
     inject_openai_api()
 
+    # Ignore all the setup if the endpoint is not set
+    endpoint = os.getenv(OTEL_EXPORTER_OTLP_ENDPOINT)
+    if not endpoint:
+        return
+
     if _is_devkit_installed():
         from promptflow._sdk._tracing import setup_exporter_to_pfs
 
         setup_exporter_to_pfs()
 
 
 def _skip_tracing_local_setup() -> bool:
```

## promptflow/tracing/_trace.py

```diff
@@ -18,15 +18,15 @@
 from opentelemetry.trace.status import StatusCode
 
 from ._openai_utils import OpenAIMetricsCalculator, OpenAIResponseParser
 from ._operation_context import OperationContext
 from ._tracer import Tracer, _create_trace_from_function_call, get_node_name_from_context
 from ._utils import get_input_names_for_prompt_template, get_prompt_param_name_from_func, serialize
 from .contracts.generator_proxy import GeneratorProxy
-from .contracts.trace import TraceType
+from .contracts.trace import Trace, TraceType
 
 IS_LEGACY_OPENAI = version("openai").startswith("0.")
 
 open_telemetry_tracer = otel_trace.get_tracer("promptflow")
 
 
 class TokenCollector:
@@ -81,21 +81,21 @@
     try:
         attrs_from_context = OperationContext.get_instance()._get_otel_attributes()
         span.set_attributes(attrs_from_context)
     except Exception as e:
         logging.warning(f"Failed to enrich span with context: {e}")
 
 
-def enrich_span_with_trace(span, trace):
+def enrich_span_with_trace(span, trace: Trace):
     try:
         span.set_attributes(
             {
                 "framework": "promptflow",
                 "span_type": trace.type.value,
-                "function": trace.name,
+                "function": trace.function,
             }
         )
         node_name = get_node_name_from_context()
         if node_name:
             span.set_attribute("node_name", node_name)
         enrich_span_with_context(span)
     except Exception as e:
@@ -110,22 +110,24 @@
         if prompt_tpl_param_name is not None:
             prompt_tpl = kwargs.get(prompt_tpl_param_name)
             prompt_vars = {
                 name: kwargs.get(name) for name in get_input_names_for_prompt_template(prompt_tpl) if name in kwargs
             }
             prompt_info = {"prompt.template": prompt_tpl, "prompt.variables": serialize_attribute(prompt_vars)}
             span.set_attributes(prompt_info)
+            span.add_event("promptflow.prompt.template", {"payload": serialize_attribute(prompt_info)})
     except Exception as e:
         logging.warning(f"Failed to enrich span with prompt info: {e}")
 
 
 def enrich_span_with_input(span, input):
     try:
         serialized_input = serialize_attribute(input)
         span.set_attribute("inputs", serialized_input)
+        span.add_event("promptflow.function.inputs", {"payload": serialized_input})
     except Exception as e:
         logging.warning(f"Failed to enrich span with input: {e}")
 
     return input
 
 
 def enrich_span_with_trace_type(span, inputs, output, trace_type):
@@ -149,14 +151,17 @@
     link = Link(context)
     # If start_trace is not called, the name of the original_span will be empty.
     with open_telemetry_tracer.start_as_current_span(
         f"Iterated({original_span.name})",
         links=[link],
     ) as span:
         enrich_span_with_original_attributes(span, original_span.attributes)
+        # Enrich the new span with input before generator iteration to prevent loss of input information.
+        # The input is as an event within this span.
+        enrich_span_with_input(span, inputs)
         generator_proxy = GeneratorProxy(generator)
         yield from generator_proxy
         generator_output = generator_proxy.items
 
         # Enrich LLM span for OpenAI streaming output
         if original_span.attributes["span_type"] == "LLM" and not IS_LEGACY_OPENAI:
             from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
@@ -178,23 +183,25 @@
     except Exception as e:
         logging.warning(f"Failed to enrich span with original attributes: {e}")
 
 
 def enrich_span_with_llm(span, model, generated_message):
     try:
         span.set_attribute("llm.response.model", model)
-        span.set_attribute("llm.generated_message", generated_message)
+        span.set_attribute("llm.generated_message", serialize_attribute(generated_message))
+        span.add_event("promptflow.llm.generated_message", {"payload": serialize_attribute(generated_message)})
     except Exception as e:
         logging.warning(f"Failed to enrich span with llm: {e}")
 
 
 def enrich_span_with_output(span, output):
     try:
         serialized_output = serialize_attribute(output)
         span.set_attribute("output", serialized_output)
+        span.add_event("promptflow.function.output", {"payload": serialized_output})
     except Exception as e:
         logging.warning(f"Failed to enrich span with output: {e}")
 
 
 def enrich_span_with_openai_tokens(span, trace_type):
     try:
         tokens = token_collector.try_get_openai_tokens(span.get_span_context().span_id)
@@ -221,14 +228,15 @@
                 embeddings.append(
                     {
                         "embedding.vector": f"<{len(emb.embedding)} dimensional vector>",
                         "embedding.text": emb_text,
                     }
                 )
             span.set_attribute("embedding.embeddings", serialize_attribute(embeddings))
+            span.add_event("promptflow.embedding.embeddings", {"payload": serialize_attribute(embeddings)})
     except Exception as e:
         logging.warning(f"Failed to enrich span with embedding: {e}")
 
 
 def _is_single_input(embedding_inputs):
     # OpenAI Embedding API accepts a single string/tokenized string or a list of string/tokenized string as input.
     # For the single string/tokenized string case, we should return true, otherwise return false.
@@ -289,40 +297,52 @@
         Callable: The traced function.
     """
     wrapped_method = _traced_async if inspect.iscoroutinefunction(func) else _traced_sync
     return wrapped_method(func, args_to_ignore=args_to_ignore, trace_type=trace_type)
 
 
 def _traced_async(
-    func: Callable = None, *, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION
+    func: Callable = None,
+    *,
+    args_to_ignore: Optional[List[str]] = None,
+    trace_type=TraceType.FUNCTION,
+    name: Optional[str] = None,
 ) -> Callable:
     """
     Decorator that adds tracing to an asynchronous function.
 
     Args:
         func (Callable): The function to be traced.
         args_to_ignore (Optional[List[str]], optional): A list of argument names to be ignored in the trace.
                                                         Defaults to None.
         trace_type (TraceType, optional): The type of the trace. Defaults to TraceType.FUNCTION.
+        name (str, optional): The name of the trace, will set to func name if not provided.
 
     Returns:
         Callable: The traced function.
     """
 
     def create_trace(func, args, kwargs):
         return _create_trace_from_function_call(
-            func, args=args, kwargs=kwargs, args_to_ignore=args_to_ignore, trace_type=trace_type
+            func,
+            args=args,
+            kwargs=kwargs,
+            args_to_ignore=args_to_ignore,
+            trace_type=trace_type,
+            name=name,
         )
 
     @functools.wraps(func)
     async def wrapped(*args, **kwargs):
         trace = create_trace(func, args, kwargs)
         # For node span we set the span name to node name, otherwise we use the function name.
         span_name = get_node_name_from_context(used_for_span_name=True) or trace.name
         with open_telemetry_tracer.start_as_current_span(span_name) as span:
+            # Store otel trace id in context for correlation
+            OperationContext.get_instance()["otel_trace_id"] = f"{span.get_span_context().trace_id:032x}"
             enrich_span_with_trace(span, trace)
             enrich_span_with_prompt_info(span, func, kwargs)
 
             # Should not extract these codes to a separate function here.
             # We directly call func instead of calling Tracer.invoke,
             # because we want to avoid long stack trace when hitting an exception.
             try:
@@ -339,39 +359,54 @@
         return output
 
     wrapped.__original_function = func
 
     return wrapped
 
 
-def _traced_sync(func: Callable = None, *, args_to_ignore=None, trace_type=TraceType.FUNCTION) -> Callable:
+def _traced_sync(
+    func: Callable = None,
+    *,
+    args_to_ignore: Optional[List[str]] = None,
+    trace_type=TraceType.FUNCTION,
+    name: Optional[str] = None,
+) -> Callable:
     """
     Decorator that adds tracing to a synchronous function.
 
     Args:
         func (Callable): The function to be traced.
         args_to_ignore (Optional[List[str]], optional): A list of argument names to be ignored in the trace.
                                                         Defaults to None.
         trace_type (TraceType, optional): The type of the trace. Defaults to TraceType.FUNCTION.
+        name (str, optional): The name of the trace, will set to func name if not provided.
+
 
     Returns:
         Callable: The traced function.
     """
 
     def create_trace(func, args, kwargs):
         return _create_trace_from_function_call(
-            func, args=args, kwargs=kwargs, args_to_ignore=args_to_ignore, trace_type=trace_type
+            func,
+            args=args,
+            kwargs=kwargs,
+            args_to_ignore=args_to_ignore,
+            trace_type=trace_type,
+            name=name,
         )
 
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         trace = create_trace(func, args, kwargs)
         # For node span we set the span name to node name, otherwise we use the function name.
         span_name = get_node_name_from_context(used_for_span_name=True) or trace.name
         with open_telemetry_tracer.start_as_current_span(span_name) as span:
+            # Store otel trace id in context for correlation
+            OperationContext.get_instance()["otel_trace_id"] = f"{span.get_span_context().trace_id:032x}"
             enrich_span_with_trace(span, trace)
             enrich_span_with_prompt_info(span, func, kwargs)
 
             # Should not extract these codes to a separate function here.
             # We directly call func instead of calling Tracer.invoke,
             # because we want to avoid long stack trace when hitting an exception.
             try:
```

## promptflow/tracing/_tracer.py

```diff
@@ -133,26 +133,27 @@
         return {
             "message": str(error),
             "type": type(error).__qualname__,
         }
 
 
 def _create_trace_from_function_call(
-    f, *, args=None, kwargs=None, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION
+    f, *, args=None, kwargs=None, args_to_ignore: Optional[List[str]] = None, trace_type=TraceType.FUNCTION, name=None,
 ):
     """
     Creates a trace object from a function call.
 
     Args:
         f (Callable): The function to be traced.
         args (list, optional): The positional arguments to the function. Defaults to None.
         kwargs (dict, optional): The keyword arguments to the function. Defaults to None.
         args_to_ignore (Optional[List[str]], optional): A list of argument names to be ignored in the trace.
                                                         Defaults to None.
         trace_type (TraceType, optional): The type of the trace. Defaults to TraceType.FUNCTION.
+        name (str, optional): The name of the trace. Defaults to None.
 
     Returns:
         Trace: The created trace object.
     """
     args = args or []
     kwargs = kwargs or {}
     args_to_ignore = set(args_to_ignore or [])
@@ -172,24 +173,25 @@
         pass
 
     # TODO: put parameters in self to inputs for builtin tools
     all_kwargs.pop("self", None)
     for key in args_to_ignore:
         all_kwargs.pop(key, None)
 
-    name = f.__qualname__
+    function = f.__qualname__
     if trace_type in [TraceType.LLM, TraceType.EMBEDDING] and f.__module__:
-        name = f"{f.__module__}.{name}"
+        function = f"{f.__module__}.{function}"
 
     return Trace(
-        name=name,
+        name=name or function,  # Use the function name as the trace name if not provided
         type=trace_type,
         start_time=datetime.utcnow().timestamp(),
         inputs=all_kwargs,
         children=[],
+        function=function,
     )
 
 
 def get_node_name_from_context(used_for_span_name=False):
     tracer = Tracer.active_instance()
     if tracer is not None:
         if used_for_span_name:
```

## promptflow/tracing/contracts/trace.py

```diff
@@ -48,7 +48,8 @@
     start_time: Optional[float] = None  # The timestamp of the start time
     end_time: Optional[float] = None  # The timestamp of the end time
     error: Optional[str] = None
     children: Optional[List["Trace"]] = None
     node_name: Optional[str] = None  # The node name of the trace, used for flow level trace
     parent_id: str = ""  # The parent trace id of the trace
     id: str = ""  # The trace id
+    function: str = ""  # The function name of the trace
```

## Comparing `promptflow_tracing-1.0.0.dist-info/METADATA` & `promptflow_tracing-1.8.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptflow-tracing
-Version: 1.0.0
+Version: 1.8.0
 Summary: Prompt flow tracing
 Home-page: https://microsoft.github.io/promptflow/
 License: MIT
 Keywords: telemetry
 Author: Microsoft Corporation
 Author-email: aml-pt-eng@microsoft.com
 Requires-Python: >=3.8,<4.0
@@ -23,15 +23,21 @@
 Requires-Dist: tiktoken (>=0.4.0)
 Project-URL: Bug Reports, https://github.com/microsoft/promptflow/issues
 Project-URL: Repository, https://github.com/microsoft/promptflow
 Description-Content-Type: text/markdown
 
 # Prompt flow tracing
 
-Prompt flow tracing.
+[![Python package](https://img.shields.io/pypi/v/promptflow-tracing)](https://pypi.org/project/promptflow-tracing/)
+[![SDK](https://img.shields.io/badge/SDK-reference-blue)](https://microsoft.github.io/promptflow/reference/python-library-reference/promptflow-tracing/promptflow.tracing.html)
+[![License: MIT](https://img.shields.io/github/license/microsoft/promptflow)](https://github.com/microsoft/promptflow/blob/main/LICENSE)
+
+## Introduction
+
+The `promptflow-tracing` package offers tracing capabilities to capture and illustrate the internal execution processes of both DAG flow and Flex flow. It is designed to be compatible with [OpenTelemetry](https://opentelemetry.io/). This makes it a valuable tool for Flex flow developers who use various frameworks (such as langchain, semantic kernel, OpenAI, and various agents) to build LLM-based applications. By using promptflow-tracing, developers can achieve comprehensive observability of their LLM applications.
 
 # Release History
 
 ## 1.0.0 (2024.03.21)
 
 - Compatible with promptflow 1.7.0.
```

## Comparing `promptflow_tracing-1.0.0.dist-info/RECORD` & `promptflow_tracing-1.8.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 promptflow/tracing/__init__.py,sha256=2RELQpoR4iNv5RbG3ThHKY_a6snK9m0amicO4iT2K4g,412
-promptflow/tracing/_constants.py,sha256=-4NBjMdO4B9mkoI6YYzd9Fw5Q3XBSKcbbokjwjJdIAk,400
+promptflow/tracing/_constants.py,sha256=N3eGPmPv84Opjvg-FEm9KFR-a0WPugD1qHA_onWw5GQ,400
 promptflow/tracing/_integrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-promptflow/tracing/_integrations/_openai_injector.py,sha256=zjzWESIcrWMRXUMKNpKXn24LLHq45BZN8Eok5P6SfxU,7883
-promptflow/tracing/_openai_utils.py,sha256=aJf6NWqSKSWieAvL9pSYKqNthE5LD7BEW4R-cFjuqlc,10489
+promptflow/tracing/_integrations/_openai_injector.py,sha256=Ivtl_WKqIqA2_GbR_VSqty-5FhVrwYf9IzpW07kk4fQ,8399
+promptflow/tracing/_openai_utils.py,sha256=-2L9tCJ3Hvhr75akFuhL264qFeWpynRrx2nX9FOQa68,10353
 promptflow/tracing/_operation_context.py,sha256=bYqAoamY3kiz2JHR23uxhVAP1pS1F_3ULwfRFuQav3g,7470
-promptflow/tracing/_start_trace.py,sha256=pZ-YZo6QDhqWpoHeLq2tUaAqtyGAfh2iZ6ncvw2MvO8,3093
+promptflow/tracing/_start_trace.py,sha256=r8rWLt3kjilAkqaAJ1wfVlfoRhOjlsfsVM2CmcTwl4g,3500
 promptflow/tracing/_thread_local_singleton.py,sha256=JPTGjbpG1LpMEUh-fqgXDz3-It5zlI3R1db4bHrIH4Y,1138
-promptflow/tracing/_trace.py,sha256=AgWeEkui0lzcxNqe8dYp3YlUPvWrX1RXXd7uzoX4e0s,17389
-promptflow/tracing/_tracer.py,sha256=IKhn1F4OiPGMBDIzn5WX9gf9s-gxiiowsArfujkKdHA,7104
+promptflow/tracing/_trace.py,sha256=r7vNqAtqg5y7-Fic6J_-PjN62upt0_2TO_H6UjN0-_g,18907
+promptflow/tracing/_tracer.py,sha256=wy_W-X4ikkst2nMANKSGwojK9ywvd82OMEZ-GNC9QDA,7297
 promptflow/tracing/_utils.py,sha256=sZrYjG-3YgxSMVZGRWF0KHz-vRMSBKIrk9REfmTGnFo,3372
 promptflow/tracing/_version.py,sha256=v7XN-ZZdY9fb-B9aAIoxmqWjMrrkdEPiOIDdEx3nOEc,299
 promptflow/tracing/contracts/__init__.py,sha256=vV8bhHRJHrJVbMOhR8jvnWF0_ZwCRQiSsUwf0X04gtg,262
 promptflow/tracing/contracts/generator_proxy.py,sha256=0vrOocScGwAwuEAimqMNbATCH_F6Iz-iMN6KhJnMosA,696
-promptflow/tracing/contracts/trace.py,sha256=svrrPS3p-OM5-XipMDC5QyZ6C80GRUfAe8QRZ7WSDTE,2034
-promptflow_tracing-1.0.0.dist-info/METADATA,sha256=ehwzv2M3bsR0IJunPR6paf0A5jKD6iHgekMXCaQbFlI,1281
-promptflow_tracing-1.0.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-promptflow_tracing-1.0.0.dist-info/RECORD,,
+promptflow/tracing/contracts/trace.py,sha256=ZBcMYUbfmOdeXufvTH5x-phAa4BziGLjBxNrjzLYUTo,2091
+promptflow_tracing-1.8.0.dist-info/METADATA,sha256=ittFCEp7zYBYsXa-iWybqoXS7gI46xnVGhdF7H7mH2g,2227
+promptflow_tracing-1.8.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+promptflow_tracing-1.8.0.dist-info/RECORD,,
```

