# Comparing `tmp/segments-ai-1.7.3.tar.gz` & `tmp/segments-ai-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segments-ai-1.7.3.tar", last modified: Fri Mar 29 11:16:47 2024, max compression
+gzip compressed data, was "segments-ai-1.7.4.tar", last modified: Wed Apr 10 09:53:33 2024, max compression
```

## Comparing `segments-ai-1.7.3.tar` & `segments-ai-1.7.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.661447 segments-ai-1.7.3/
--rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.7.3/LICENSE.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.7.3/MANIFEST.in
--rw-rw-r--   0 bert      (1000) bert      (1000)     1134 2024-03-29 11:16:47.661447 segments-ai-1.7.3/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.7.3/README.md
--rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.7.3/pyproject.toml
--rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.7.3/requirements.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.7.3/requirements_dev.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.7.3/requirements_docs.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-03-29 11:16:47.661447 segments-ai-1.7.3/setup.cfg
--rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-03-29 11:15:10.000000 segments-ai-1.7.3/setup.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.657447 segments-ai-1.7.3/src/
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.661447 segments-ai-1.7.3/src/segments/
--rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.7.3/src/segments/__init__.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    87565 2024-03-15 11:08:21.000000 segments-ai-1.7.3/src/segments/client.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.661447 segments-ai-1.7.3/src/segments/data/
--rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.7.3/src/segments/data/dataset_card_template.md
--rw-rw-r--   0 bert      (1000) bert      (1000)    14548 2024-03-05 14:46:29.000000 segments-ai-1.7.3/src/segments/dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.7.3/src/segments/exceptions.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    30413 2023-11-23 10:20:03.000000 segments-ai-1.7.3/src/segments/export.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.7.3/src/segments/huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.3/src/segments/py.typed
--rw-rw-r--   0 bert      (1000) bert      (1000)    22778 2024-03-29 11:14:45.000000 segments-ai-1.7.3/src/segments/typing.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    35687 2024-01-16 09:37:31.000000 segments-ai-1.7.3/src/segments/utils.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.661447 segments-ai-1.7.3/src/segments_ai.egg-info/
--rw-r--r--   0 bert      (1000) bert      (1000)     1134 2024-03-29 11:16:47.000000 segments-ai-1.7.3/src/segments_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-03-29 11:16:47.000000 segments-ai-1.7.3/src/segments_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-03-29 11:16:47.000000 segments-ai-1.7.3/src/segments_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-03-29 11:16:47.000000 segments-ai-1.7.3/src/segments_ai.egg-info/requires.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-03-29 11:16:47.000000 segments-ai-1.7.3/src/segments_ai.egg-info/top_level.txt
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-03-29 11:16:47.661447 segments-ai-1.7.3/tests/
--rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.7.3/tests/test_client.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.7.3/tests/test_dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.3/tests/test_huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.7.3/tests/test_random.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.7.3/tests/test_utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.7.4/LICENSE.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.7.4/MANIFEST.in
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1134 2024-04-10 09:53:33.137741 segments-ai-1.7.4/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.7.4/README.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.7.4/pyproject.toml
+-rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.7.4/requirements.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.7.4/requirements_dev.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.7.4/requirements_docs.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-04-10 09:53:33.137741 segments-ai-1.7.4/setup.cfg
+-rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-04-10 09:51:52.000000 segments-ai-1.7.4/setup.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/__init__.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    87565 2024-03-15 11:08:21.000000 segments-ai-1.7.4/src/segments/client.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments/data/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.7.4/src/segments/data/dataset_card_template.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)    14548 2024-03-05 14:46:29.000000 segments-ai-1.7.4/src/segments/dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.7.4/src/segments/exceptions.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    30413 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/export.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.4/src/segments/py.typed
+-rw-rw-r--   0 bert      (1000) bert      (1000)    22856 2024-04-10 09:51:23.000000 segments-ai-1.7.4/src/segments/typing.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    35687 2024-04-07 13:40:19.000000 segments-ai-1.7.4/src/segments/utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments_ai.egg-info/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1134 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-04-10 09:53:33.000000 segments-ai-1.7.4/src/segments_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/requires.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/top_level.txt
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/tests/
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.7.4/tests/test_client.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.7.4/tests/test_dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.4/tests/test_huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.7.4/tests/test_random.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.7.4/tests/test_utils.py
```

### Comparing `segments-ai-1.7.3/LICENSE.txt` & `segments-ai-1.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/PKG-INFO` & `segments-ai-1.7.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.3
+Version: 1.7.4
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.3.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.4.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `segments-ai-1.7.3/README.md` & `segments-ai-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/pyproject.toml` & `segments-ai-1.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/setup.py` & `segments-ai-1.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from typing import List
 
 
 #############
 # Constants #
 #############
-MAJOR, MINOR, PATCH = 1, 7, 3
+MAJOR, MINOR, PATCH = 1, 7, 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 ####################
 # Helper functions #
 ####################
 # https://github.com/allenai/python-package-template
```

### Comparing `segments-ai-1.7.3/src/segments/client.py` & `segments-ai-1.7.4/src/segments/client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments/dataset.py` & `segments-ai-1.7.4/src/segments/dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments/exceptions.py` & `segments-ai-1.7.4/src/segments/exceptions.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments/export.py` & `segments-ai-1.7.4/src/segments/export.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments/huggingface.py` & `segments-ai-1.7.4/src/segments/huggingface.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments/typing.py` & `segments-ai-1.7.4/src/segments/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,20 @@
 
 # Image sequence segmentation
 class ImageSequenceSegmentationAnnotation(Annotation):
     track_id: int
     is_keyframe: bool = False
 
 
-class ImageSequenceSegmentationFrame(ImageSegmentationLabelAttributes):
+class ImageSequenceSegmentationFrame(BaseModel):
     annotations: List[ImageSequenceSegmentationAnnotation]
-    timestamp: Optional[Timestamp] = None
+    segmentation_bitmap: Optional[URL] = None
     format_version: Optional[FormatVersion] = None
+    image_attributes: Optional[ImageAttributes] = None
+    timestamp: Optional[Timestamp] = None
 
 
 class ImageSequenceSegmentationLabelAttributes(BaseModel):
     frames: List[ImageSequenceSegmentationFrame]
     format_version: Optional[FormatVersion] = None
```

### Comparing `segments-ai-1.7.3/src/segments/utils.py` & `segments-ai-1.7.4/src/segments/utils.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/src/segments_ai.egg-info/PKG-INFO` & `segments-ai-1.7.4/src/segments_ai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.3
+Version: 1.7.4
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.3.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.4.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `segments-ai-1.7.3/src/segments_ai.egg-info/SOURCES.txt` & `segments-ai-1.7.4/src/segments_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/tests/test_client.py` & `segments-ai-1.7.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/tests/test_dataset.py` & `segments-ai-1.7.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.3/tests/test_utils.py` & `segments-ai-1.7.4/tests/test_utils.py`

 * *Files identical despite different names*

