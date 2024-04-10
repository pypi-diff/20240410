# Comparing `tmp/ASUllm-0.0.4.tar.gz` & `tmp/ASUllm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASUllm-0.0.4.tar", last modified: Tue Apr  9 23:58:28 2024, max compression
+gzip compressed data, was "ASUllm-0.0.5.tar", last modified: Wed Apr 10 15:57:48 2024, max compression
```

## Comparing `ASUllm-0.0.4.tar` & `ASUllm-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 23:58:28.438047 ASUllm-0.0.4/
--rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.4/LICENSE
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 23:58:28.437786 ASUllm-0.0.4/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.4/README.md
--rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-09 23:58:20.000000 ASUllm-0.0.4/pyproject.toml
--rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-09 23:58:28.438110 ASUllm-0.0.4/setup.cfg
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 23:58:28.434614 ASUllm-0.0.4/src/
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 23:58:28.436399 ASUllm-0.0.4/src/ASUllm/
--rw-r--r--   0 wenxing1   (503) staff       (20)      138 2024-04-09 23:58:07.000000 ASUllm-0.0.4/src/ASUllm/__init__.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1463 2024-04-09 20:54:31.000000 ASUllm-0.0.4/src/ASUllm/api.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.4/src/ASUllm/model_config.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1258 2024-04-09 23:58:05.000000 ASUllm-0.0.4/src/ASUllm/models.py
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-09 23:58:28.437501 ASUllm-0.0.4/src/ASUllm.egg-info/
--rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-09 23:58:28.000000 ASUllm-0.0.4/src/ASUllm.egg-info/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)      257 2024-04-09 23:58:28.000000 ASUllm-0.0.4/src/ASUllm.egg-info/SOURCES.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-09 23:58:28.000000 ASUllm-0.0.4/src/ASUllm.egg-info/dependency_links.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        7 2024-04-09 23:58:28.000000 ASUllm-0.0.4/src/ASUllm.egg-info/top_level.txt
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.048793 ASUllm-0.0.5/
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.046617 ASUllm-0.0.5/ASUllm/
+-rw-r--r--   0 wenxing1   (503) staff       (20)      138 2024-04-09 23:58:07.000000 ASUllm-0.0.5/ASUllm/__init__.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1463 2024-04-09 20:54:31.000000 ASUllm-0.0.5/ASUllm/api.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllm-0.0.5/ASUllm/model_config.py
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1258 2024-04-09 23:58:05.000000 ASUllm-0.0.5/ASUllm/models.py
+drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 15:57:48.048173 ASUllm-0.0.5/ASUllm.egg-info/
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)      225 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/SOURCES.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/dependency_links.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)        7 2024-04-10 15:57:48.000000 ASUllm-0.0.5/ASUllm.egg-info/top_level.txt
+-rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllm-0.0.5/LICENSE
+-rw-r--r--   0 wenxing1   (503) staff       (20)     5600 2024-04-10 15:57:48.048499 ASUllm-0.0.5/PKG-INFO
+-rw-r--r--   0 wenxing1   (503) staff       (20)     4988 2024-02-26 20:37:09.000000 ASUllm-0.0.5/README.md
+-rw-r--r--   0 wenxing1   (503) staff       (20)      593 2024-04-10 15:57:13.000000 ASUllm-0.0.5/pyproject.toml
+-rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-10 15:57:48.048889 ASUllm-0.0.5/setup.cfg
```

### Comparing `ASUllm-0.0.4/LICENSE` & `ASUllm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.4/PKG-INFO` & `ASUllm-0.0.5/ASUllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ASUllm-0.0.4/README.md` & `ASUllm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.4/pyproject.toml` & `ASUllm-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ASUllm"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
 ]
 description = "A simple python package to facilitate connection to ASU LLM API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ASUllm-0.0.4/src/ASUllm/api.py` & `ASUllm-0.0.5/ASUllm/api.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.4/src/ASUllm/model_config.py` & `ASUllm-0.0.5/ASUllm/model_config.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.4/src/ASUllm/models.py` & `ASUllm-0.0.5/ASUllm/models.py`

 * *Files identical despite different names*

### Comparing `ASUllm-0.0.4/src/ASUllm.egg-info/PKG-INFO` & `ASUllm-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllm
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

