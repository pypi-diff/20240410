# Comparing `tmp/ASUllm-0.0.2.tar.gz` & `tmp/ASUllm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASUllm-0.0.2.tar", last modified: Tue Apr  9 21:59:04 2024, max compression
+gzip compressed data, was "ASUllm-0.0.3.tar", last modified: Tue Apr  9 22:40:30 2024, max compression
```

## Comparing `ASUllm-0.0.2.tar` & `ASUllm-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:59:04.301611 ASUllm-0.0.2/
--rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.2/LICENSE
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 21:59:04.301359 ASUllm-0.0.2/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.2/README.md
--rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-09 21:58:58.000000 ASUllm-0.0.2/pyproject.toml
--rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-09 21:59:04.301860 ASUllm-0.0.2/setup.cfg
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:59:04.298912 ASUllm-0.0.2/src/
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:59:04.299935 ASUllm-0.0.2/src/ASU_LLM/
--rw-r--r--   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:42:07.000000 ASUllm-0.0.2/src/ASU_LLM/__init__.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1463 2024-04-09 20:54:31.000000 ASUllm-0.0.2/src/ASU_LLM/api.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.2/src/ASU_LLM/model_config.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1282 2024-04-09 20:54:31.000000 ASUllm-0.0.2/src/ASU_LLM/models.py
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:59:04.301093 ASUllm-0.0.2/src/ASUllm.egg-info/
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 21:59:04.000000 ASUllm-0.0.2/src/ASUllm.egg-info/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)      261 2024-04-09 21:59:04.000000 ASUllm-0.0.2/src/ASUllm.egg-info/SOURCES.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-09 21:59:04.000000 ASUllm-0.0.2/src/ASUllm.egg-info/dependency_links.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        8 2024-04-09 21:59:04.000000 ASUllm-0.0.2/src/ASUllm.egg-info/top_level.txt
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 22:40:30.713893 ASUllm-0.0.3/
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.3/LICENSE
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 22:40:30.709612 ASUllm-0.0.3/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.3/README.md
+-rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-09 22:40:16.000000 ASUllm-0.0.3/pyproject.toml
+-rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-09 22:40:30.713949 ASUllm-0.0.3/setup.cfg
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 22:40:30.706287 ASUllm-0.0.3/src/
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 22:40:30.708041 ASUllm-0.0.3/src/ASUllm/
+-rw-r--r--   0 wenxing1   (503) staff       (20)        0 2024-04-09 21:42:07.000000 ASUllm-0.0.3/src/ASUllm/__init__.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1463 2024-04-09 20:54:31.000000 ASUllm-0.0.3/src/ASUllm/api.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.3/src/ASUllm/model_config.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1282 2024-04-09 20:54:31.000000 ASUllm-0.0.3/src/ASUllm/models.py
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 22:40:30.709345 ASUllm-0.0.3/src/ASUllm.egg-info/
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 22:40:30.000000 ASUllm-0.0.3/src/ASUllm.egg-info/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)      257 2024-04-09 22:40:30.000000 ASUllm-0.0.3/src/ASUllm.egg-info/SOURCES.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-09 22:40:30.000000 ASUllm-0.0.3/src/ASUllm.egg-info/dependency_links.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        7 2024-04-09 22:40:30.000000 ASUllm-0.0.3/src/ASUllm.egg-info/top_level.txt
```

### Comparing `ASUllm-0.0.2/LICENSE` & `ASUllm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.2/PKG-INFO` & `ASUllm-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ASUllm-0.0.2/README.md` & `ASUllm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.2/pyproject.toml` & `ASUllm-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ASUllm"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
 ]
 description = "A simple python package to facilitate connection to ASU LLM API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ASUllm-0.0.2/src/ASU_LLM/api.py` & `ASUllm-0.0.3/src/ASUllm/api.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.2/src/ASU_LLM/model_config.py` & `ASUllm-0.0.3/src/ASUllm/model_config.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.2/src/ASU_LLM/models.py` & `ASUllm-0.0.3/src/ASUllm/models.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.2/src/ASUllm.egg-info/PKG-INFO` & `ASUllm-0.0.3/src/ASUllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

