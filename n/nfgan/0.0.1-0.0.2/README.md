# Comparing `tmp/nfgan-0.0.1.tar.gz` & `tmp/nfgan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfgan-0.0.1.tar", last modified: Wed Apr 10 04:05:41 2024, max compression
+gzip compressed data, was "nfgan-0.0.2.tar", last modified: Wed Apr 10 06:04:50 2024, max compression
```

## Comparing `nfgan-0.0.1.tar` & `nfgan-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 04:05:41.403180 nfgan-0.0.1/
--rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 nfgan-0.0.1/LICENSE.text
--rw-rw-rw-   0        0        0      664 2024-04-10 04:05:41.390955 nfgan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 nfgan-0.0.1/README.md
--rw-rw-rw-   0        0        0      793 2024-04-10 04:05:03.000000 nfgan-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 04:05:41.403180 nfgan-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 04:05:41.342301 nfgan-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 04:05:41.360164 nfgan-0.0.1/src/nfgan/
--rw-rw-rw-   0        0        0        0 2023-07-09 02:42:34.000000 nfgan-0.0.1/src/nfgan/Debug.py
--rw-rw-rw-   0        0        0     5355 2024-04-10 04:04:53.000000 nfgan-0.0.1/src/nfgan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 04:05:41.390955 nfgan-0.0.1/src/nfgan.egg-info/
--rw-rw-rw-   0        0        0      664 2024-04-10 04:05:41.000000 nfgan-0.0.1/src/nfgan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-10 04:05:41.000000 nfgan-0.0.1/src/nfgan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 04:05:41.000000 nfgan-0.0.1/src/nfgan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 04:05:41.000000 nfgan-0.0.1/src/nfgan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 06:04:50.272603 nfgan-0.0.2/
+-rw-rw-rw-   0        0        0     1052 2023-02-05 10:37:40.000000 nfgan-0.0.2/LICENSE.text
+-rw-rw-rw-   0        0        0      664 2024-04-10 06:04:50.269094 nfgan-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-05 07:37:25.000000 nfgan-0.0.2/README.md
+-rw-rw-rw-   0        0        0      793 2024-04-10 06:04:10.000000 nfgan-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 06:04:50.272603 nfgan-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 06:04:50.193500 nfgan-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 06:04:50.222141 nfgan-0.0.2/src/nfgan/
+-rw-rw-rw-   0        0        0        0 2023-07-09 02:42:34.000000 nfgan-0.0.2/src/nfgan/Debug.py
+-rw-rw-rw-   0        0        0        0 2024-04-10 05:56:13.000000 nfgan-0.0.2/src/nfgan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 06:04:50.256314 nfgan-0.0.2/src/nfgan.egg-info/
+-rw-rw-rw-   0        0        0      664 2024-04-10 06:04:50.000000 nfgan-0.0.2/src/nfgan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-10 06:04:50.000000 nfgan-0.0.2/src/nfgan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 06:04:50.000000 nfgan-0.0.2/src/nfgan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 06:04:50.000000 nfgan-0.0.2/src/nfgan.egg-info/top_level.txt
```

### Comparing `nfgan-0.0.1/LICENSE.text` & `nfgan-0.0.2/LICENSE.text`

 * *Files identical despite different names*

### Comparing `nfgan-0.0.1/PKG-INFO` & `nfgan-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfgan
-Version: 0.0.1
+Version: 0.0.2
 Summary: The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <neuronode.data@gmail.com>
 Project-URL: WebApp, https://nn-engine.web.app/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `nfgan-0.0.1/pyproject.toml` & `nfgan-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nfgan"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jay Singh", email="neuronode.data@gmail.com" },
 ]
 description = '''The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 WebSite : https://nn-engine.web.app/'''
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `nfgan-0.0.1/src/nfgan.egg-info/PKG-INFO` & `nfgan-0.0.2/src/nfgan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfgan
-Version: 0.0.1
+Version: 0.0.2
 Summary: The NNEngine is an advanced visual processing model that offers a comprehensive development environment for creating visually immersive experiences, the NNEngine has been extensively trained to generate high-quality humanoid graphics with remarkable realism.
 Author-email: Jay Singh <neuronode.data@gmail.com>
 Project-URL: WebApp, https://nn-engine.web.app/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

