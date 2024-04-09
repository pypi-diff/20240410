# Comparing `tmp/kiwi_booster-0.3.8.tar.gz` & `tmp/kiwi_booster-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_booster-0.3.8.tar", max compression
+gzip compressed data, was "kiwi_booster-0.3.9.tar", max compression
```

## Comparing `kiwi_booster-0.3.8.tar` & `kiwi_booster-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.3.8/LICENSE
--rw-r--r--   0        0        0     9196 2024-04-08 20:09:19.938677 kiwi_booster-0.3.8/README.md
--rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.3.8/kiwi_booster/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.3.8/kiwi_booster/common_utils/__init__.py
--rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.3.8/kiwi_booster/common_utils/geographic.py
--rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.3.8/kiwi_booster/common_utils/json.py
--rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.3.8/kiwi_booster/common_utils/loggers.py
--rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.3.8/kiwi_booster/common_utils/requests.py
--rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.3.8/kiwi_booster/common_utils/time.py
--rw-r--r--   0        0        0     3188 2024-04-08 20:43:49.402784 kiwi_booster-0.3.8/kiwi_booster/common_utils/video.py
--rw-r--r--   0        0        0     1794 2024-04-08 20:09:19.942677 kiwi_booster-0.3.8/kiwi_booster/decorators.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.8/kiwi_booster/gcp_utils/__init__.py
--rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.3.8/kiwi_booster/gcp_utils/bigquery.py
--rw-r--r--   0        0        0     1312 2024-04-08 20:09:19.942677 kiwi_booster-0.3.8/kiwi_booster/gcp_utils/kfp.py
--rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.3.8/kiwi_booster/gcp_utils/secrets.py
--rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.3.8/kiwi_booster/gcp_utils/storage.py
--rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.3.8/kiwi_booster/mcap_utils/__init__.py
--rw-r--r--   0        0        0    11933 2024-04-08 20:09:19.942677 kiwi_booster-0.3.8/kiwi_booster/mcap_utils/decode.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.8/kiwi_booster/ml_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.3.8/kiwi_booster/ml_utils/benchmarks.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.3.8/kiwi_booster/ml_utils/prediction.py
--rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.3.8/kiwi_booster/slack_utils.py
--rw-r--r--   0        0        0     3096 2024-04-08 20:48:16.771240 kiwi_booster-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    10758 1970-01-01 00:00:00.000000 kiwi_booster-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.3.9/LICENSE
+-rw-r--r--   0        0        0     9196 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.3.9/kiwi_booster/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.3.9/kiwi_booster/common_utils/__init__.py
+-rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/common_utils/geographic.py
+-rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/common_utils/json.py
+-rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.3.9/kiwi_booster/common_utils/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.3.9/kiwi_booster/common_utils/requests.py
+-rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.3.9/kiwi_booster/common_utils/time.py
+-rw-r--r--   0        0        0     3207 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/common_utils/video.py
+-rw-r--r--   0        0        0     1794 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/__init__.py
+-rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/bigquery.py
+-rw-r--r--   0        0        0     1312 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/kfp.py
+-rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/secrets.py
+-rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/storage.py
+-rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/mcap_utils/__init__.py
+-rw-r--r--   0        0        0    11933 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/mcap_utils/decode.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.9/kiwi_booster/ml_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.3.9/kiwi_booster/ml_utils/benchmarks.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.3.9/kiwi_booster/ml_utils/prediction.py
+-rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/slack_utils.py
+-rw-r--r--   0        0        0     3095 2024-04-09 14:19:56.288992 kiwi_booster-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    10758 1970-01-01 00:00:00.000000 kiwi_booster-0.3.9/PKG-INFO
```

### Comparing `kiwi_booster-0.3.8/LICENSE` & `kiwi_booster-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/README.md` & `kiwi_booster-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/common_utils/geographic.py` & `kiwi_booster-0.3.9/kiwi_booster/common_utils/geographic.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/common_utils/json.py` & `kiwi_booster-0.3.9/kiwi_booster/common_utils/json.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/common_utils/loggers.py` & `kiwi_booster-0.3.9/kiwi_booster/common_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/common_utils/time.py` & `kiwi_booster-0.3.9/kiwi_booster/common_utils/time.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/common_utils/video.py` & `kiwi_booster-0.3.9/kiwi_booster/common_utils/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional
 
 import numpy as np
 
 try:
     import cv2
-    from moviepy.editor import AudioFileClip, VideoFileClip, concatenate_audioclip
+    from moviepy.editor import AudioFileClip, VideoFileClip, concatenate_audioclips
 except ImportError as e:
     raise ImportError(
-        "Videos dependencies are not installed. Please install them using the 'extras' option."
+        "Videos dependencies are not installed. Please install them using using pip install kiwi-booster[video]."
     ) from e
 
 
 class VideoWriter:
     """Class for writing video frames to a local file"""
 
     def __init__(self, video_path: str, fps: int, codec: str = "MP4V") -> None:
```

### Comparing `kiwi_booster-0.3.8/kiwi_booster/decorators.py` & `kiwi_booster-0.3.9/kiwi_booster/decorators.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/gcp_utils/bigquery.py` & `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/bigquery.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/gcp_utils/kfp.py` & `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/kfp.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/gcp_utils/secrets.py` & `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/gcp_utils/storage.py` & `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/storage.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/mcap_utils/decode.py` & `kiwi_booster-0.3.9/kiwi_booster/mcap_utils/decode.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/kiwi_booster/slack_utils.py` & `kiwi_booster-0.3.9/kiwi_booster/slack_utils.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.8/pyproject.toml` & `kiwi_booster-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiwi-booster"
-version = "0.3.8"
+version = "0.3.9"
 description = "Python utility functions and classes for KiwiBot AI&Robotics team"
 authors = ["Sebastian Hernandez <juan.hernandez@kiwibot.con>"]
 readme = "README.md"
 packages = [{include = "kiwi_booster"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13.0"
@@ -30,15 +30,14 @@
 python-path = "^0.1.3"
 opencv-python = { version = "^4.9.0.80", optional = true }
 moviepy = { version = "^1.0.3", optional = true } 
 
 [tool.poetry.extras]
 video = ["opencv-python", "moviepy"]
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
```

### Comparing `kiwi_booster-0.3.8/PKG-INFO` & `kiwi_booster-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi-booster
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python utility functions and classes for KiwiBot AI&Robotics team
 Author: Sebastian Hernandez
 Author-email: juan.hernandez@kiwibot.con
 Requires-Python: >=3.8,<3.13.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kiwi-booster Version: 0.3.8 Summary: Python utility
+Metadata-Version: 2.1 Name: kiwi-booster Version: 0.3.9 Summary: Python utility
 functions and classes for KiwiBot AI&Robotics team Author: Sebastian Hernandez
 Author-email: juan.hernandez@kiwibot.con Requires-Python: >=3.8,<3.13.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: video Requires-Dist: google-auth (>=2.18.0,<3.0.0) Requires-
```

