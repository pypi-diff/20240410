# Comparing `tmp/reka_api-1.0.4.tar.gz` & `tmp/reka_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-1.0.4.tar", max compression
+gzip compressed data, was "reka_api-1.0.5.tar", max compression
```

## Comparing `reka_api-1.0.4.tar` & `reka_api-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    25738 2024-04-09 08:38:41.979755 reka_api-1.0.4/LICENSE
--rw-r--r--   0        0        0      149 2024-04-09 08:38:41.979755 reka_api-1.0.4/README.md
--rw-r--r--   0        0        0     1125 2024-04-09 08:38:41.979755 reka_api-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      825 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/__init__.py
--rw-r--r--   0        0        0     7357 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/chat.py
--rw-r--r--   0        0        0     2401 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/completion.py
--rw-r--r--   0        0        0     2077 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/dataset.py
--rw-r--r--   0        0        0     2223 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/driver.py
--rw-r--r--   0        0        0      694 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/job.py
--rw-r--r--   0        0        0      373 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/models.py
--rw-r--r--   0        0        0     3563 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/api/retrieval.py
--rw-r--r--   0        0        0     1141 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/errors.py
--rw-r--r--   0        0        0        0 2024-04-09 08:38:41.979755 reka_api-1.0.4/src/reka/py.typed
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    25738 2024-04-10 10:10:31.982448 reka_api-1.0.5/LICENSE
+-rw-r--r--   0        0        0      149 2024-04-10 10:10:31.982448 reka_api-1.0.5/README.md
+-rw-r--r--   0        0        0     1125 2024-04-10 10:10:31.986448 reka_api-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      825 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/__init__.py
+-rw-r--r--   0        0        0     7403 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/chat.py
+-rw-r--r--   0        0        0     2401 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/completion.py
+-rw-r--r--   0        0        0     2077 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/dataset.py
+-rw-r--r--   0        0        0     2223 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/driver.py
+-rw-r--r--   0        0        0      694 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/job.py
+-rw-r--r--   0        0        0      373 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/models.py
+-rw-r--r--   0        0        0     3563 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/api/retrieval.py
+-rw-r--r--   0        0        0     1136 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/errors.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:10:31.986448 reka_api-1.0.5/src/reka/py.typed
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-1.0.5/PKG-INFO
```

### Comparing `reka_api-1.0.4/LICENSE` & `reka_api-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/pyproject.toml` & `reka_api-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reka-api"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     "Reka Team <contact@reka.ai>",
 ]
 description = "Reka API"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `reka_api-1.0.4/src/reka/__init__.py` & `reka_api-1.0.5/src/reka/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/api/chat.py` & `reka_api-1.0.5/src/reka/api/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Chat-related server interactions (including VLM chat)"""
 
 from __future__ import annotations
 
+import base64
 from typing import Any, Dict, List, Literal, Optional, TypedDict, cast
 
 import reka.api.driver as driver
 from reka.errors import InvalidConversationError
 
 
 class ModelTurn(TypedDict):
@@ -22,21 +23,20 @@
     """A turn in a conversation authored by the human user."""
 
     text: str
     type: Literal["human"]
 
     # Optional media (image, video, or audio), can be set only for the first turn in the conversation.
     media_url: Optional[str]
-    media_type: Optional[MediaType]
 
 
 def chat(
     human: Optional[str] = None,
     media_url: Optional[str] = None,
-    media_type: Optional[MediaType] = None,
+    media_filename: Optional[str] = None,
     conversation_history: Optional[List[HumanTurn | ModelTurn]] = None,
     retrieval_dataset: Optional[str] = None,
     model_name: str = "default",
     request_output_len: Optional[int] = None,
     temperature: Optional[float] = None,
     random_seed: Optional[int] = None,
     runtime_top_k: Optional[int] = None,
@@ -65,20 +65,20 @@
     )
     print(response) # {"type": "model", "text": "Your name is John.\\n\\n"}
     ```
 
     Args:
         human: latest message from human, this is optional if using `conversation_history` instead.
         media_url: an optional URL for the media (image, video, or audio) to chat about. This may only be set for the
-            first turn (when conversation_history is empty).
-        media_type: the media type (image, video, or audio) - this should be set when media_url is set.
+            first turn (when conversation_history is empty). You can also send base64 media in the format data:image/{image_format};base64,{base64_image}
+        media_filename: alternative to the `media_url` parameter, the location of a local file.``
         conversation_history: list of dicts, where each dict has a key "type"
             indicating the speaker, either "human" or "model", and a key "text"
             containing the message from the speaker. If not set, will default to
-            an empty history. The first turn may also have "media_url" and "media_type" set.
+            an empty history. The first turn may also have "media_url" set.
         retrieval_dataset: Previously uploaded dataset to do retrieval on.
         model_name: Name of model.
         request_output_len: Completion length in tokens.
         temperature: Softmax temperature, higher is more diverse.
         random_seed: Seed to obtain different results.
         runtime_top_k: Keep only k top tokens when sampling.
         runtime_top_p: Keep only top p quantile when sampling.
@@ -95,18 +95,21 @@
         ModelTurn: A dict containing `{"type": "model", "text": <response from the model>}`. If `retrieval_dataset` is
             set, then this will also contain `"retrieved_chunks"`.
 
     """
     defined_hturn: Optional[HumanTurn] = None
     if human is not None:
         defined_hturn = {"type": "human", "text": human}
+        if media_url is not None and media_filename is not None:
+            raise ValueError("Must specify either `media_url` or `media_filename`")
+
         if media_url is not None:
             defined_hturn["media_url"] = media_url
-        if media_type is not None:
-            defined_hturn["media_type"] = media_type
+        elif media_filename is not None:
+            defined_hturn["media_url"] = _local_file_to_media_url(media_filename)
 
     full_conv = (conversation_history or []) + (
         [defined_hturn] if defined_hturn else []
     )
     _check_conversation_history(full_conv)
 
     json_dict = {
@@ -148,46 +151,44 @@
 
     Raises InvalidConversationError otherwise.
     """
     if len(conversation_history) == 0:
         raise InvalidConversationError(reason="Conversation history cannot be empty")
 
     for i, turn in enumerate(conversation_history):
-        if i > 0 and ("media_url" in turn or "media_type" in turn):
+        if i > 0 and ("media_url" in turn):
             raise InvalidConversationError(
                 reason=f"Media is only supported for the first turn, found media keys in turn {i} '{turn}'."
             )
 
         valid_key_sets = [{"type", "text"}]
         if i == 0:
-            valid_key_sets.append({"type", "text", "media_url", "media_type"})
+            valid_key_sets.append({"type", "text", "media_url"})
 
         turn_keys = set(turn.keys())
         if not any(turn_keys == valid_key_set for valid_key_set in valid_key_sets):
             expected_keys_str = " or ".join(map(str, valid_key_sets))
             raise InvalidConversationError(
                 reason=f"Expected keys {expected_keys_str} for turn {i} '{turn}', got keys {turn_keys}."
             )
 
-        valid_media_types = {"image", "video", "audio", None}
-        if not turn.get("media_type") in valid_media_types:
-            raise InvalidConversationError(
-                reason=(
-                    f"Unrecognized media_type '{turn.get('media_type')}' for turn {i} '{turn}', "
-                    f"expected one of {valid_media_types}."
-                )
-            )
-
         for key, value in turn.items():
             if not isinstance(value, str):
                 raise InvalidConversationError(
                     reason=f"Expected string for value of '{key}' in turn {i} '{turn}', got {type(value)}."
                 )
 
         expected_type = ["human", "model"][i % 2]
         if turn["type"] != expected_type:
             raise InvalidConversationError(
                 reason=(
                     f"Expected type '{expected_type}' for turn {i} '{turn}', got '{turn['type']}'. Conversations should "
                     "alternate between 'human' and 'model', starting with 'human'."
                 )
             )
+
+
+def _local_file_to_media_url(media_filename: str) -> str:
+    with open(media_filename, "rb") as f:
+        base64_media = base64.b64encode(f.read()).decode("ascii")
+
+    return f"data:application/octet-stream;base64,{base64_media}"
```

### Comparing `reka_api-1.0.4/src/reka/api/completion.py` & `reka_api-1.0.5/src/reka/api/completion.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/api/dataset.py` & `reka_api-1.0.5/src/reka/api/dataset.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/api/driver.py` & `reka_api-1.0.5/src/reka/api/driver.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/api/job.py` & `reka_api-1.0.5/src/reka/api/job.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/api/retrieval.py` & `reka_api-1.0.5/src/reka/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `reka_api-1.0.4/src/reka/errors.py` & `reka_api-1.0.5/src/reka/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Reka-specific exceptions."""
 
-from typing import Any, Optional
+from typing import Optional
 
 
 class RekaError(Exception):
     """Something wrong happened with the request."""
 
     def __init__(
         self, underlying: Optional[Exception] = None, reason: Optional[str] = None
```

### Comparing `reka_api-1.0.4/PKG-INFO` & `reka_api-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reka-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Reka API
 Home-page: https://reka.ai/
 Author: Reka Team
 Author-email: contact@reka.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

