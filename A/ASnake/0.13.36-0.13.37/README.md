# Comparing `tmp/ASnake-0.13.36.tar.gz` & `tmp/ASnake-0.13.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASnake-0.13.36.tar", last modified: Wed Apr 10 15:49:43 2024, max compression
+gzip compressed data, was "ASnake-0.13.37.tar", last modified: Wed Apr 10 19:33:12 2024, max compression
```

## Comparing `ASnake-0.13.36.tar` & `ASnake-0.13.37.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/ASnake.egg-info/
--rw-r--r--   0 ahri      (1002) ahri      (1002)    14968 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      237 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/SOURCES.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/dependency_links.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       11 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/top_level.txt
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/ASnakeData/
--rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-09 12:51:58.000000 ASnake-0.13.36/ASnakeData/ASnakeAlias.bat
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 15:43:29.000000 ASnake-0.13.36/ASnakeData/megaTest.asnake
--rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-09 14:58:35.000000 ASnake-0.13.36/ASnakeData/setAlias.asnake
--rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.36/LICENSE.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)    14968 2024-04-10 15:49:43.164333 ASnake-0.13.36/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.36/README.md
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1611 2024-04-10 15:35:00.000000 ASnake-0.13.36/pyproject.toml
--rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-10 15:49:43.164333 ASnake-0.13.36/setup.cfg
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.37/LICENSE.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-10 19:33:12.597394 ASnake-0.13.37/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.37/README.md
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1495 2024-04-10 19:24:02.000000 ASnake-0.13.37/pyproject.toml
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-10 19:33:12.597394 ASnake-0.13.37/setup.cfg
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake/
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)   517000 2024-04-10 19:16:27.000000 ASnake-0.13.37/src/ASnake/ASnake.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        0 2024-04-10 18:46:25.000000 ASnake-0.13.37/src/ASnake/__init__.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    19469 2024-04-10 19:29:33.000000 ASnake-0.13.37/src/ASnake/__main__.py
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake/data/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/ASnakeAlias.bat
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/megaTest.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-10 18:07:02.000000 ASnake-0.13.37/src/ASnake/data/setAlias.asnake
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 19:33:12.597394 ASnake-0.13.37/src/ASnake.egg-info/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      405 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/SOURCES.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/dependency_links.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       46 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/entry_points.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/requires.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        7 2024-04-10 19:33:12.000000 ASnake-0.13.37/src/ASnake.egg-info/top_level.txt
```

### Comparing `ASnake-0.13.36/ASnake.egg-info/PKG-INFO` & `ASnake-0.13.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.36
+Version: 0.13.37
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,16 @@
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: sly>=0.4
+Requires-Dist: autopep8>=1.5.5
 
 # ASnake
 Optimizing Python transpiler for the ASnake programming language.
 
 A proper readme is yet to come. If you are super interested, we have a lot more info (including some draft documentation) on this Discord:
 https://discord.gg/ySDFchT
```

### Comparing `ASnake-0.13.36/ASnakeData/megaTest.asnake` & `ASnake-0.13.37/src/ASnake/data/megaTest.asnake`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.36/ASnakeData/setAlias.asnake` & `ASnake-0.13.37/src/ASnake/data/setAlias.asnake`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.36/LICENSE.txt` & `ASnake-0.13.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.36/PKG-INFO` & `ASnake-0.13.37/src/ASnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.36
+Version: 0.13.37
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,14 +221,16 @@
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: sly>=0.4
+Requires-Dist: autopep8>=1.5.5
 
 # ASnake
 Optimizing Python transpiler for the ASnake programming language.
 
 A proper readme is yet to come. If you are super interested, we have a lot more info (including some draft documentation) on this Discord:
 https://discord.gg/ySDFchT
```

### Comparing `ASnake-0.13.36/README.md` & `ASnake-0.13.37/README.md`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.36/pyproject.toml` & `ASnake-0.13.37/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-[build-system]
-requires = ["setuptools>=46.4.0", "wheel", "sly>=0.4", "autopep8>=1.5.5"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "ASnake"
-#dynamic = ["version"]
-version="0.13.36"
 authors = [
   { name="Ahri Fox"},
 ]
 description = "Python optimizing compiler for the ASnake programming language."
 readme = "README.md"
-requires-python = ">=3.6"
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Operating System :: POSIX :: Linux",
     "Development Status :: 3 - Alpha",
@@ -25,31 +18,31 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Software Development :: Version Control :: Git"
 ]
 keywords = ["programming language","transpiler","pyston","compiler"]
+requires-python = ">=3.6"
+dependencies = [
+    "sly>=0.4",
+    "autopep8>=1.5.5"
+]
+dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://asnake.org"
 Github = "https://github.com/AhriFoxSnek/ASnake"
 Issues = "https://github.com/AhriFoxSnek/ASnake/issues"
 
-[options]
-python_requires = ">=3.6"
-install_requires = [
-    "sly>=0.4",
-    "autopep8>=1.5.5"
-]
-
+[project.scripts]
+ASnake = "ASnake.ASnake:main"
 
-[tool.setuptools.package-data]
-"ASnakeData" = ["*.bat", "*.asnake", "*.py", "ASnake.py"]
+[build-system]
+requires = ["setuptools", "wheel", "sly>=0.4"]
+build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
-version = {attr = "ASnake.__version__"}
+version = {attr = "ASnake.ASnake.__version__"}
 
-[entry-points]
-console_scripts = [
-    "ASnake = ASnake:main"
-]
+[tool.setuptools.package-data]
+"ASnake.data" = ["*.bat", "*.asnake"]
```

