# Comparing `tmp/NNEngine-0.0.7.tar.gz` & `tmp/NNEngine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NNEngine-0.0.7.tar", last modified: Wed Feb 21 13:20:53 2024, max compression
+gzip compressed data, was "NNEngine-0.0.9.tar", last modified: Wed Apr 10 03:50:50 2024, max compression
```

## Comparing `NNEngine-0.0.7.tar` & `NNEngine-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 13:20:53.483405 NNEngine-0.0.7/
--rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NNEngine-0.0.7/LICENSE.text
--rw-rw-rw-   0        0        0      667 2024-02-21 13:20:53.433840 NNEngine-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NNEngine-0.0.7/README.md
--rw-rw-rw-   0        0        0      796 2024-02-21 13:14:49.000000 NNEngine-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-21 13:20:53.485408 NNEngine-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-21 13:20:53.377842 NNEngine-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-02-21 13:20:53.420190 NNEngine-0.0.7/src/NNEngine.egg-info/
--rw-rw-rw-   0        0        0      667 2024-02-21 13:20:53.000000 NNEngine-0.0.7/src/NNEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2024-02-21 13:20:53.000000 NNEngine-0.0.7/src/NNEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 13:20:53.000000 NNEngine-0.0.7/src/NNEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-21 13:20:53.000000 NNEngine-0.0.7/src/NNEngine.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-21 13:20:53.417176 NNEngine-0.0.7/src/nnengine/
--rw-rw-rw-   0        0        0        0 2023-07-09 02:42:34.000000 NNEngine-0.0.7/src/nnengine/Debug.py
--rw-rw-rw-   0        0        0    16690 2024-02-21 13:20:33.000000 NNEngine-0.0.7/src/nnengine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:50.152560 NNEngine-0.0.9/
+-rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 NNEngine-0.0.9/LICENSE.text
+-rw-rw-rw-   0        0        0      667 2024-04-10 03:50:50.150229 NNEngine-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 NNEngine-0.0.9/README.md
+-rw-rw-rw-   0        0        0      796 2024-04-10 03:49:44.000000 NNEngine-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 03:50:50.152560 NNEngine-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:50.090806 NNEngine-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:50.147194 NNEngine-0.0.9/src/NNEngine.egg-info/
+-rw-rw-rw-   0        0        0      667 2024-04-10 03:50:50.000000 NNEngine-0.0.9/src/NNEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-04-10 03:50:50.000000 NNEngine-0.0.9/src/NNEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 03:50:50.000000 NNEngine-0.0.9/src/NNEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 03:50:50.000000 NNEngine-0.0.9/src/NNEngine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 03:50:50.142824 NNEngine-0.0.9/src/nnengine/
+-rw-rw-rw-   0        0        0        0 2023-07-09 02:42:34.000000 NNEngine-0.0.9/src/nnengine/Debug.py
+-rw-rw-rw-   0        0        0     5332 2024-04-10 03:49:19.000000 NNEngine-0.0.9/src/nnengine/__init__.py
```

### Comparing `NNEngine-0.0.7/LICENSE.text` & `NNEngine-0.0.9/LICENSE.text`

 * *Files identical despite different names*

### Comparing `NNEngine-0.0.7/PKG-INFO` & `NNEngine-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NNEngine
-Version: 0.0.7
+Version: 0.0.9
 Summary: The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <neuronode.data@gmail.com>
 Project-URL: WebApp, https://nn-engine.web.app/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `NNEngine-0.0.7/pyproject.toml` & `NNEngine-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NNEngine"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Jay Singh", email="neuronode.data@gmail.com" },
 ]
 description = '''The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 WebSite : https://nn-engine.web.app/'''
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `NNEngine-0.0.7/src/NNEngine.egg-info/PKG-INFO` & `NNEngine-0.0.9/src/NNEngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NNEngine
-Version: 0.0.7
+Version: 0.0.9
 Summary: The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <neuronode.data@gmail.com>
 Project-URL: WebApp, https://nn-engine.web.app/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

