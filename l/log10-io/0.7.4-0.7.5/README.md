# Comparing `tmp/log10_io-0.7.4.tar.gz` & `tmp/log10_io-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.7.4.tar", max compression
+gzip compressed data, was "log10_io-0.7.5.tar", max compression
```

## Comparing `log10_io-0.7.4.tar` & `log10_io-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2024-04-05 23:28:11.370088 log10_io-0.7.4/LICENSE
--rw-r--r--   0        0        0     8934 2024-04-05 23:28:11.370088 log10_io-0.7.4/README.md
--rw-r--r--   0        0        0        0 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/__init__.py
--rw-r--r--   0        0        0     1470 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/__main__.py
--rw-r--r--   0        0        0     9386 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/bigquery.py
--rw-r--r--   0        0        0     9532 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/evals.py
--rw-r--r--   0        0        0     5399 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4153 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/langchain.py
--rw-r--r--   0        0        0     4296 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/llm.py
--rw-r--r--   0        0        0    35836 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/openai.py
--rw-r--r--   0        0        0     5343 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/utils.py
--rw-r--r--   0        0        0     2180 2024-04-05 23:28:11.378088 log10_io-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 log10_io-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-10 04:30:32.129246 log10_io-0.7.5/LICENSE
+-rw-r--r--   0        0        0     8934 2024-04-10 04:30:32.129246 log10_io-0.7.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/__init__.py
+-rw-r--r--   0        0        0     1470 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/__main__.py
+-rw-r--r--   0        0        0    10132 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/bigquery.py
+-rw-r--r--   0        0        0     9532 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/evals.py
+-rw-r--r--   0        0        0     5399 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4153 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     4880 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/langchain.py
+-rw-r--r--   0        0        0     4296 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/llm.py
+-rw-r--r--   0        0        0    34743 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/openai.py
+-rw-r--r--   0        0        0     5343 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-04-10 04:30:32.133246 log10_io-0.7.5/log10/utils.py
+-rw-r--r--   0        0        0     2180 2024-04-10 04:30:32.133246 log10_io-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 log10_io-0.7.5/PKG-INFO
```

### Comparing `log10_io-0.7.4/LICENSE` & `log10_io-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/README.md` & `log10_io-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/__main__.py` & `log10_io-0.7.5/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/_httpx_utils.py` & `log10_io-0.7.5/log10/_httpx_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import time
 import traceback
+import uuid
 from datetime import datetime, timezone
 
 import httpx
 from httpx import Request, Response
 
 from log10.llm import Log10Config
 from log10.load import get_log10_session_tags, sessionID
@@ -13,14 +14,15 @@
 
 logger: logging.Logger = logging.getLogger("LOG10")
 
 
 _log10_config = Log10Config()
 base_url = _log10_config.url
 httpx_client = httpx.Client()
+httpx_async_client = httpx.AsyncClient()
 
 
 def _get_time_diff(created_at):
     time = datetime.fromisoformat(created_at)
     now = datetime.now(timezone.utc)
     diff = now - time
     # convert the time difference to human readable format
@@ -79,27 +81,43 @@
             )
         else:
             logger.error(f"Failed with error: {http_err}")
     except Exception as err:
         logger.error(f"Failed to insert in log10: {payload} with error {err}")
 
 
+async def _try_post_request_async(url: str, payload: dict = {}) -> httpx.Response:
+    headers = {
+        "x-log10-token": _log10_config.token,
+        "x-log10-organization-id": _log10_config.org_id,
+        "Content-Type": "application/json",
+    }
+    payload["organization_id"] = _log10_config.org_id
+    try:
+        res = await httpx_async_client.post(url, headers=headers, json=payload)
+        res.raise_for_status()
+        return res
+    except httpx.HTTPStatusError as http_err:
+        if "401" in str(http_err):
+            logger.error(
+                "Failed authorization. Please verify that LOG10_TOKEN and LOG10_ORG_ID are set correctly and try again."
+                + "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details"
+            )
+        else:
+            logger.error(f"Failed with error: {http_err}")
+    except Exception as err:
+        logger.error(f"Failed to insert in log10: {payload} with error {err}")
+
+
 async def get_completion_id(request: Request):
     if "v1/chat/completions" not in str(request.url):
         logger.warning("Currently logging is only available for v1/chat/completions.")
         return
 
-    completion_url = "/api/completions"
-    res = _try_post_request(url=f"{base_url}{completion_url}")
-    try:
-        completion_id = res.json().get("completionID")
-    except Exception as e:
-        logger.error(f"Failed to get completion ID. Error: {e}. Skipping completion recording.")
-    else:
-        request.headers["x-log10-completion-id"] = completion_id
+    request.headers["x-log10-completion-id"] = str(uuid.uuid4())
 
 
 async def log_request(request: Request):
     start_time = time.time()
     request.started = start_time
     completion_id = request.headers.get("x-log10-completion-id", "")
     if not completion_id:
@@ -121,15 +139,15 @@
         "orig_module": orig_module,
         "orig_qualname": orig_qualname,
         "request": request.content.decode("utf-8"),
         "session_id": sessionID,
     }
     if get_log10_session_tags():
         log_row["tags"] = get_log10_session_tags()
-    _try_post_request(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
+    await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
 
 
 class _LogResponse(Response):
     async def aiter_bytes(self, *args, **kwargs):
         full_response = ""
         finished = False
         async for chunk in super().aiter_bytes(*args, **kwargs):
@@ -201,15 +219,15 @@
                 "stacktrace": json.dumps(stacktrace),
                 "kind": "chat",
                 "request": self.request.content.decode("utf-8"),
                 "session_id": sessionID,
             }
             if get_log10_session_tags():
                 log_row["tags"] = get_log10_session_tags()
-            _try_post_request(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
+            await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
 
 
 class _LogTransport(httpx.AsyncBaseTransport):
     def __init__(self, transport: httpx.AsyncBaseTransport):
         self.transport = transport
 
     async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
@@ -242,15 +260,15 @@
                 "stacktrace": json.dumps(stacktrace),
                 "kind": "chat",
                 "request": request.content.decode("utf-8"),
                 "session_id": sessionID,
             }
             if get_log10_session_tags():
                 log_row["tags"] = get_log10_session_tags()
-            _try_post_request(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
+            await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
             return response
         elif response.headers.get("content-type") == "text/event-stream":
             return _LogResponse(
                 status_code=response.status_code,
                 headers=response.headers,
                 stream=response.stream,
                 extensions=response.extensions,
```

### Comparing `log10_io-0.7.4/log10/agents/camel.py` & `log10_io-0.7.5/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/agents/scrape_summarizer.py` & `log10_io-0.7.5/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/anthropic.py` & `log10_io-0.7.5/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/bigquery.py` & `log10_io-0.7.5/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/completions/completions.py` & `log10_io-0.7.5/log10/completions/completions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/evals.py` & `log10_io-0.7.5/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.7.5/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/feedback/autofeedback.py` & `log10_io-0.7.5/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/feedback/feedback.py` & `log10_io-0.7.5/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/feedback/feedback_task.py` & `log10_io-0.7.5/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/langchain.py` & `log10_io-0.7.5/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/litellm.py` & `log10_io-0.7.5/log10/litellm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/llm.py` & `log10_io-0.7.5/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/load.py` & `log10_io-0.7.5/log10/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import logging
 import os
 import queue
 import threading
 import time
 import traceback
+import uuid
 from contextlib import contextmanager
 from copy import deepcopy
 from importlib.metadata import version
 
 import backoff
 import requests
 from dotenv import load_dotenv
@@ -34,15 +35,14 @@
 # log10, bigquery
 target_service = os.environ.get("LOG10_DATA_STORE", "log10")
 
 if target_service == "bigquery":
     from log10.bigquery import initialize_bigquery
 
     bigquery_client, bigquery_table = initialize_bigquery()
-    import uuid
     from datetime import datetime, timezone
 elif target_service is None:
     target_service = "log10"  # default to log10
 
 
 def is_openai_v1() -> bool:
     """Return whether OpenAI API is v1 or more."""
@@ -98,43 +98,17 @@
         raise
 
 
 post_session_request = functools.partial(post_request, url + "/api/sessions", {})
 
 
 def get_session_id():
-    if target_service == "bigquery":
-        return str(uuid.uuid4())
-
-    session_id = None
-    try:
-        res = post_session_request()
-        session_id = res.json()["sessionID"]
-    except requests.HTTPError as http_err:
-        if "401" in str(http_err):
-            logging.warn(
-                "Failed anthorization. Please verify that LOG10_TOKEN and LOG10_ORG_ID are set correctly and try again."
-                + "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details"
-            )
-        else:
-            logging.warn(f"Failed to create LOG10 session. Error: {http_err}")
-    except requests.ConnectionError:
-        logging.warn(
-            "Invalid LOG10_URL. Please verify that LOG10_URL is set correctly and try again."
-            + "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details"
-        )
-    except Exception as e:
-        logging.warn(
-            "Failed to create LOG10 session: "
-            + str(e)
-            + "\nLikely cause: LOG10 env vars missing or not picked up correctly!"
-            + "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details"
-        )
-
-    return session_id
+    id = str(uuid.uuid4())
+    logger.debug(f"Session ID: {id}")
+    return id
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
 last_completion_response = None
 global_tags = []
```

### Comparing `log10_io-0.7.4/log10/mosaicml.py` & `log10_io-0.7.5/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/openai.py` & `log10_io-0.7.5/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/prompt_analyzer.py` & `log10_io-0.7.5/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/schemas/bigquery.json` & `log10_io-0.7.5/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/together.py` & `log10_io-0.7.5/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/tools.py` & `log10_io-0.7.5/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/log10/utils.py` & `log10_io-0.7.5/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.4/pyproject.toml` & `log10_io-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.7.4"
+version = "0.7.5"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `log10_io-0.7.4/PKG-INFO` & `log10_io-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.7.4
+Version: 0.7.5
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

