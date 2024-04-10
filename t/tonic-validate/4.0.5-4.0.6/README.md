# Comparing `tmp/tonic_validate-4.0.5.tar.gz` & `tmp/tonic_validate-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic_validate-4.0.5.tar", max compression
+gzip compressed data, was "tonic_validate-4.0.6.tar", max compression
```

## Comparing `tonic_validate-4.0.5.tar` & `tonic_validate-4.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1063 2024-04-05 22:11:41.013217 tonic_validate-4.0.5/LICENSE
--rw-r--r--   0        0        0    24571 2024-04-05 22:11:41.013217 tonic_validate-4.0.5/README.md
--rw-r--r--   0        0        0      771 2024-04-05 22:11:41.077217 tonic_validate-4.0.5/pyproject.toml
--rw-r--r--   0        0        0      459 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/__init__.py
--rw-r--r--   0        0        0      387 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/__init__.py
--rw-r--r--   0        0        0     2106 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/benchmark.py
--rw-r--r--   0        0        0      247 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/exceptions.py
--rw-r--r--   0        0        0     1023 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/llm_response.py
--rw-r--r--   0        0        0     2630 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/run.py
--rw-r--r--   0        0        0      314 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/classes/user_info.py
--rw-r--r--   0        0        0      805 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/config.py
--rw-r--r--   0        0        0     1483 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/__init__.py
--rw-r--r--   0        0        0     1584 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_binary_metric.py
--rw-r--r--   0        0        0     1971 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_metric.py
--rw-r--r--   0        0        0     2784 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_contains_pii_metric.py
--rw-r--r--   0        0        0     1257 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_match_metric.py
--rw-r--r--   0        0        0     1728 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/answer_similarity_metric.py
--rw-r--r--   0        0        0     1844 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/augmentation_accuracy_metric.py
--rw-r--r--   0        0        0     2354 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/augmentation_precision_metric.py
--rw-r--r--   0        0        0     1452 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/binary_metric.py
--rw-r--r--   0        0        0     1747 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/contains_text_metric.py
--rw-r--r--   0        0        0     2808 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/context_contains_pii_metric.py
--rw-r--r--   0        0        0     1786 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/context_length_metric.py
--rw-r--r--   0        0        0     1155 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/duplication_metric.py
--rw-r--r--   0        0        0     1076 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/hate_speech_content_metric.py
--rw-r--r--   0        0        0     1173 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/latency_metric.py
--rw-r--r--   0        0        0      725 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/metric.py
--rw-r--r--   0        0        0     1239 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/regex_metric.py
--rw-r--r--   0        0        0     1448 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/response_length_metric.py
--rw-r--r--   0        0        0     1795 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/metrics/retrieval_precision_metric.py
--rw-r--r--   0        0        0     4626 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/services/openai_service.py
--rw-r--r--   0        0        0    18492 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/tests/test_scorer.py
--rw-r--r--   0        0        0        0 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/http_client.py
--rw-r--r--   0        0        0    19067 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/llm_calls.py
--rw-r--r--   0        0        0     2198 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/metrics_util.py
--rw-r--r--   0        0        0      530 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/openai_cache.py
--rw-r--r--   0        0        0     4961 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/utils/telemetry.py
--rw-r--r--   0        0        0     4381 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/validate_api.py
--rw-r--r--   0        0        0    13171 2024-04-05 22:11:41.081217 tonic_validate-4.0.5/tonic_validate/validate_scorer.py
--rw-r--r--   0        0        0    25330 1970-01-01 00:00:00.000000 tonic_validate-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-10 16:24:52.697491 tonic_validate-4.0.6/LICENSE
+-rw-r--r--   0        0        0    24571 2024-04-10 16:24:52.697491 tonic_validate-4.0.6/README.md
+-rw-r--r--   0        0        0      771 2024-04-10 16:24:52.757490 tonic_validate-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0      459 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/__init__.py
+-rw-r--r--   0        0        0     2106 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/benchmark.py
+-rw-r--r--   0        0        0      247 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/exceptions.py
+-rw-r--r--   0        0        0     1023 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/llm_response.py
+-rw-r--r--   0        0        0     2630 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/run.py
+-rw-r--r--   0        0        0      314 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/classes/user_info.py
+-rw-r--r--   0        0        0      805 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/config.py
+-rw-r--r--   0        0        0     1483 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/__init__.py
+-rw-r--r--   0        0        0     1584 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_binary_metric.py
+-rw-r--r--   0        0        0     1971 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_metric.py
+-rw-r--r--   0        0        0     2784 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_contains_pii_metric.py
+-rw-r--r--   0        0        0     1257 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_match_metric.py
+-rw-r--r--   0        0        0     1728 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/answer_similarity_metric.py
+-rw-r--r--   0        0        0     1844 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/augmentation_accuracy_metric.py
+-rw-r--r--   0        0        0     2354 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/augmentation_precision_metric.py
+-rw-r--r--   0        0        0     1452 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/binary_metric.py
+-rw-r--r--   0        0        0     1747 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/contains_text_metric.py
+-rw-r--r--   0        0        0     2808 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/context_contains_pii_metric.py
+-rw-r--r--   0        0        0     1786 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/context_length_metric.py
+-rw-r--r--   0        0        0     1155 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/duplication_metric.py
+-rw-r--r--   0        0        0     1076 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/hate_speech_content_metric.py
+-rw-r--r--   0        0        0     1173 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/latency_metric.py
+-rw-r--r--   0        0        0      725 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/metric.py
+-rw-r--r--   0        0        0     1239 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/regex_metric.py
+-rw-r--r--   0        0        0     1448 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/response_length_metric.py
+-rw-r--r--   0        0        0     1795 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/metrics/retrieval_precision_metric.py
+-rw-r--r--   0        0        0     4746 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/services/openai_service.py
+-rw-r--r--   0        0        0    18492 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/tests/test_scorer.py
+-rw-r--r--   0        0        0        0 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/http_client.py
+-rw-r--r--   0        0        0    19067 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/llm_calls.py
+-rw-r--r--   0        0        0     2198 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/metrics_util.py
+-rw-r--r--   0        0        0      530 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/openai_cache.py
+-rw-r--r--   0        0        0     4961 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/utils/telemetry.py
+-rw-r--r--   0        0        0     4431 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/validate_api.py
+-rw-r--r--   0        0        0    13230 2024-04-10 16:24:52.765490 tonic_validate-4.0.6/tonic_validate/validate_scorer.py
+-rw-r--r--   0        0        0    25330 1970-01-01 00:00:00.000000 tonic_validate-4.0.6/PKG-INFO
```

### Comparing `tonic_validate-4.0.5/LICENSE` & `tonic_validate-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/README.md` & `tonic_validate-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/pyproject.toml` & `tonic_validate-4.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonic-validate"
-version = "4.0.5"
+version = "4.0.6"
 description = "RAG evaluation metrics."
 authors = ["Joe Ferrara <joeferrara@tonic.ai>", "Ethan Philpott <ephilpott@tonic.ai>", "Adam Kamor <adam@tonic.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 openai = ">=1.0.0"
```

### Comparing `tonic_validate-4.0.5/tonic_validate/classes/benchmark.py` & `tonic_validate-4.0.6/tonic_validate/classes/benchmark.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/classes/llm_response.py` & `tonic_validate-4.0.6/tonic_validate/classes/llm_response.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/classes/run.py` & `tonic_validate-4.0.6/tonic_validate/classes/run.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/config.py` & `tonic_validate-4.0.6/tonic_validate/config.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/__init__.py` & `tonic_validate-4.0.6/tonic_validate/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_binary_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_binary_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/answer_consistency_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/answer_consistency_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/answer_contains_pii_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/answer_contains_pii_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/answer_match_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/answer_match_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/answer_similarity_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/answer_similarity_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/augmentation_accuracy_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/augmentation_accuracy_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/augmentation_precision_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/augmentation_precision_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/binary_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/binary_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/contains_text_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/contains_text_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/context_contains_pii_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/context_contains_pii_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/context_length_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/context_length_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/duplication_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/duplication_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/hate_speech_content_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/hate_speech_content_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/latency_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/latency_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/regex_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/regex_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/response_length_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/response_length_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/metrics/retrieval_precision_metric.py` & `tonic_validate-4.0.6/tonic_validate/metrics/retrieval_precision_metric.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/services/openai_service.py` & `tonic_validate-4.0.6/tonic_validate/services/openai_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 class OpenAIService:
     def __init__(
         self,
         encoder: Encoding,
         model: str = "gpt-4-1106-preview",
-        starting_wait_time: float = 0.1,
-        max_retries: int = 12,
+        starting_wait_time: float = 1.0,
+        max_retries: int = 10,
         exp_delay_base: int = 2,
     ) -> None:
         """
         The OpenAIService class is a wrapper around the OpenAI and AzureOpenAI clients.
 
         Parameters
         ----------
@@ -72,14 +72,16 @@
             The response from the language model.
         """
 
         async def get_openai_response():
             num_retries = 0
             wait_time = self.starting_wait_time
             while num_retries < self.max_retries:
+                random_value = random.randrange(0, 20) * 0.01
+                wait_time_multiplier = self.exp_delay_base * (1 + random_value)
                 try:
                     completion = await self.client.chat.completions.create(
                         model=self.model,
                         messages=[
                             {
                                 "role": "system",
                                 "content": "You are a helpful assistant. Respond using markdown.",
@@ -100,19 +102,19 @@
                 except RateLimitError:
                     log_message = (
                         "hit openai.error.RateLimitError and entered retry "
                         f"logic, num_retries={num_retries}"
                     )
                     logger.debug(log_message)
                     await asyncio.sleep(wait_time)
-                    wait_time *= self.exp_delay_base * (1 + random.random())
+                    wait_time *= wait_time_multiplier
                 except Exception as e:
                     logger.warning(e)
                     await asyncio.sleep(wait_time)
-                    wait_time *= self.exp_delay_base
+                    wait_time *= wait_time_multiplier
                 num_retries += 1
             raise LLMException(
                 f"Failed to get completion response from {self.model}, max retires hit"
             )
 
         cached_response = self.cache.get(prompt)
         if cached_response is not None:
```

### Comparing `tonic_validate-4.0.5/tonic_validate/tests/test_scorer.py` & `tonic_validate-4.0.6/tonic_validate/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/utils/http_client.py` & `tonic_validate-4.0.6/tonic_validate/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/utils/llm_calls.py` & `tonic_validate-4.0.6/tonic_validate/utils/llm_calls.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/utils/metrics_util.py` & `tonic_validate-4.0.6/tonic_validate/utils/metrics_util.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/utils/openai_cache.py` & `tonic_validate-4.0.6/tonic_validate/utils/openai_cache.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/utils/telemetry.py` & `tonic_validate-4.0.6/tonic_validate/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `tonic_validate-4.0.5/tonic_validate/validate_api.py` & `tonic_validate-4.0.6/tonic_validate/validate_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,19 @@
             telemetry = Telemetry(api_key)
             telemetry.link_user()
         except Exception as _:
             pass
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def upload_run(
-        self, project_id: str, run: Run, run_metadata: Optional[Dict[str, Any]] = {}, tags: Optional[List[str]] = []
+        self,
+        project_id: str,
+        run: Run,
+        run_metadata: Optional[Dict[str, Any]] = {},
+        tags: Optional[List[str]] = [],
     ) -> str:
         """Upload a run to a Tonic Validate project.
 
         Parameters
         ----------
         project_id : str
             The ID of the project to upload the run to.
@@ -52,15 +56,15 @@
             The run to upload.
         run_metadata : Optional[Dict[str, Any]]
             Metadata to attach to the run. If the values are not strings, then they are
             converted to strings before making the request.
         tags : Optional[List[str]]
             A list of tags which can be used to identify this run.  Tags will be rendered in the UI and can also make run searchable.
         """
-        if "llm_evaluator" not in run_metadata:
+        if run_metadata and "llm_evaluator" not in run_metadata:
             run_metadata["llm_evaluator"] = run.llm_evaluator
         run_response = self.client.http_post(
             f"/projects/{project_id}/runs/with_data",
             data={
                 "run_metadata": run_metadata,
                 "tags": tags,
                 "data": [run_data.to_dict() for run_data in run.run_data],
```

### Comparing `tonic_validate-4.0.5/tonic_validate/validate_scorer.py` & `tonic_validate-4.0.6/tonic_validate/validate_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         metrics: List[Metric] = [
             AnswerSimilarityMetric(),
             AugmentationPrecisionMetric(),
             AnswerConsistencyMetric(),
         ],
         model_evaluator: str = "gpt-4-turbo-preview",
         max_parsing_retries: int = 3,
-        max_llm_retries: int = 12,
+        max_llm_retries: int = 10,
         fail_on_error: bool = False,
         quiet: bool = False,
     ):
         """
         Create a Tonic Validate scorer.
 
         Parameters
@@ -203,15 +203,20 @@
         try:
             self.telemetry.log_run(
                 len(responses), [metric.name for metric in self.metrics], run_time
             )
         except Exception as _:
             pass
 
-        return Run(overall_scores=overall_scores, run_data=run_data, llm_evaluator=self.model_evaluator, id=None)
+        return Run(
+            overall_scores=overall_scores,
+            run_data=run_data,
+            llm_evaluator=self.model_evaluator,
+            id=None,
+        )
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def score_responses(
         self,
         responses: List[LLMResponse],
         parallelism: int = DEFAULT_PARALLELISM_SCORING,
     ) -> Run:
```

### Comparing `tonic_validate-4.0.5/PKG-INFO` & `tonic_validate-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic-validate
-Version: 4.0.5
+Version: 4.0.6
 Summary: RAG evaluation metrics.
 Author: Joe Ferrara
 Author-email: joeferrara@tonic.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

