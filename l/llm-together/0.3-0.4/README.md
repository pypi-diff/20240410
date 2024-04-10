# Comparing `tmp/llm-together-0.3.tar.gz` & `tmp/llm-together-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-together-0.3.tar", last modified: Sun Dec 31 14:47:17 2023, max compression
+gzip compressed data, was "llm-together-0.4.tar", last modified: Wed Apr 10 19:36:13 2024, max compression
```

## Comparing `llm-together-0.3.tar` & `llm-together-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-12-31 14:47:17.934780 llm-together-0.3/
--rw-r--r--   0 sam        (501) staff       (20)    11324 2023-12-29 21:53:46.000000 llm-together-0.3/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     2047 2023-12-31 14:47:17.934502 llm-together-0.3/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     1478 2023-12-29 21:53:46.000000 llm-together-0.3/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-12-31 14:47:17.934160 llm-together-0.3/llm_together.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     2047 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      302 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)       30 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/entry_points.txt
--rw-r--r--   0 sam        (501) staff       (20)       33 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)       13 2023-12-31 14:47:17.000000 llm-together-0.3/llm_together.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)     3967 2023-12-29 22:32:27.000000 llm-together-0.3/llm_together.py
--rw-r--r--   0 sam        (501) staff       (20)      548 2023-12-29 22:22:28.000000 llm-together-0.3/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2023-12-31 14:47:17.934820 llm-together-0.3/setup.cfg
--rw-r--r--   0 sam        (501) staff       (20)      971 2023-12-29 22:32:52.000000 llm-together-0.3/setup.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-12-31 14:47:17.933626 llm-together-0.3/tests/
--rw-r--r--   0 sam        (501) staff       (20)      769 2023-12-29 22:28:51.000000 llm-together-0.3/tests/test_llm_together.py
+drwxrwxr-x   0 kevin     (1003) kevin     (1003)        0 2024-04-10 19:36:13.861838 llm-together-0.4/
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)    11324 2023-10-06 15:36:14.000000 llm-together-0.4/LICENSE
+-rw-r--r--   0 kevin     (1003) kevin     (1003)     2054 2024-04-10 19:36:13.861838 llm-together-0.4/PKG-INFO
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)     1478 2023-10-06 15:16:52.000000 llm-together-0.4/README.md
+drwxrwxr-x   0 kevin     (1003) kevin     (1003)        0 2024-04-10 19:36:13.861838 llm-together-0.4/llm_together.egg-info/
+-rw-r--r--   0 kevin     (1003) kevin     (1003)     2054 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)      302 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)        1 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)       30 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)       40 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/requires.txt
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)       13 2024-04-10 19:36:13.000000 llm-together-0.4/llm_together.egg-info/top_level.txt
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)     3967 2024-04-10 15:31:16.000000 llm-together-0.4/llm_together.py
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)      557 2024-04-10 15:55:47.000000 llm-together-0.4/pyproject.toml
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)       38 2024-04-10 19:36:13.861838 llm-together-0.4/setup.cfg
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)      971 2024-04-10 19:32:33.000000 llm-together-0.4/setup.py
+drwxrwxr-x   0 kevin     (1003) kevin     (1003)        0 2024-04-10 19:36:13.861838 llm-together-0.4/tests/
+-rw-rw-r--   0 kevin     (1003) kevin     (1003)      769 2024-04-10 15:31:16.000000 llm-together-0.4/tests/test_llm_together.py
```

### Comparing `llm-together-0.3/LICENSE` & `llm-together-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-together-0.3/PKG-INFO` & `llm-together-0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llm-together
-Version: 0.3
+Version: 0.4
 Summary: llm together plugin
 Home-page: https://github.com/wearedevx/llm-together
 Author: Kévin Quesada
 License: MIT
 Project-URL: Homepage, https://github.com/wearedevx/llm-together
 Project-URL: Bug Tracker, https://github.com/wearedevx/llm-together/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm>=0.5
-Requires-Dist: together
+Requires-Dist: together==0.2.9
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-together
 
 [![PyPI](https://img.shields.io/pypi/v/llm-together.svg)](https://pypi.org/project/llm-together/)
 [![Changelog](https://img.shields.io/github/v/release/accudio/llm-together?include_prereleases&label=changelog)](https://github.com/wearedevx/llm-together/releases)
```

### Comparing `llm-together-0.3/README.md` & `llm-together-0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm-together-0.3/llm_together.egg-info/PKG-INFO` & `llm-together-0.4/llm_together.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llm-together
-Version: 0.3
+Version: 0.4
 Summary: llm together plugin
 Home-page: https://github.com/wearedevx/llm-together
 Author: Kévin Quesada
 License: MIT
 Project-URL: Homepage, https://github.com/wearedevx/llm-together
 Project-URL: Bug Tracker, https://github.com/wearedevx/llm-together/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: llm>=0.5
-Requires-Dist: together
+Requires-Dist: together==0.2.9
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # llm-together
 
 [![PyPI](https://img.shields.io/pypi/v/llm-together.svg)](https://pypi.org/project/llm-together/)
 [![Changelog](https://img.shields.io/github/v/release/accudio/llm-together?include_prereleases&label=changelog)](https://github.com/wearedevx/llm-together/releases)
```

### Comparing `llm-together-0.3/llm_together.py` & `llm-together-0.4/llm_together.py`

 * *Files identical despite different names*

### Comparing `llm-together-0.3/pyproject.toml` & `llm-together-0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 dynamic = ["optional-dependencies"]
 name = "llm-together"
-version = "0.3"
+version = "0.4"
 license = { text="MIT" }
 authors = [
   { name="Kévin Quesada" },
 ]
 description = "llm together plugin"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-  "llm>=0.5", "together"
+  "llm>=0.5", "together==0.2.9" 
 ]
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [project.entry-points.llm]
 together = "llm_together"
 
 [project.urls]
 "Homepage" = "https://github.com/wearedevx/llm-together"
-"Bug Tracker" = "https://github.com/wearedevx/llm-together/issues"
+"Bug Tracker" = "https://github.com/wearedevx/llm-together/issues"
```

### Comparing `llm-together-0.3/setup.py` & `llm-together-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `llm-together-0.3/tests/test_llm_together.py` & `llm-together-0.4/tests/test_llm_together.py`

 * *Files identical despite different names*

