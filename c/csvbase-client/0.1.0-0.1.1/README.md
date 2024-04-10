# Comparing `tmp/csvbase-client-0.1.0.tar.gz` & `tmp/csvbase-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvbase-client-0.1.0.tar", last modified: Tue Apr  9 11:17:53 2024, max compression
+gzip compressed data, was "csvbase-client-0.1.1.tar", last modified: Wed Apr 10 06:35:45 2024, max compression
```

## Comparing `csvbase-client-0.1.0.tar` & `csvbase-client-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/
--rw-r--r--   0 cal       (1000) cal       (1000)    34523 2017-09-30 07:16:25.000000 csvbase-client-0.1.0/COPYING
--rw-r--r--   0 cal       (1000) cal       (1000)       40 2023-04-05 16:09:56.000000 csvbase-client-0.1.0/MANIFEST.in
--rw-r--r--   0 cal       (1000) cal       (1000)     4342 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/PKG-INFO
--rw-r--r--   0 cal       (1000) cal       (1000)     2995 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/README.md
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client/
--rw-r--r--   0 cal       (1000) cal       (1000)        5 2024-04-05 10:39:14.000000 csvbase-client-0.1.0/csvbase_client/VERSION
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/__init__.py
--rw-r--r--   0 cal       (1000) cal       (1000)       40 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/constants.py
--rw-r--r--   0 cal       (1000) cal       (1000)      530 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/exceptions.py
--rw-r--r--   0 cal       (1000) cal       (1000)     7318 2024-04-08 10:19:42.000000 csvbase-client-0.1.0/csvbase_client/fsspec.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client/internals/
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/internals/__init__.py
--rw-r--r--   0 cal       (1000) cal       (1000)      988 2024-02-03 15:57:46.000000 csvbase-client-0.1.0/csvbase_client/internals/auth.py
--rw-r--r--   0 cal       (1000) cal       (1000)    11948 2024-04-05 10:43:06.000000 csvbase-client-0.1.0/csvbase_client/internals/cache.py
--rw-r--r--   0 cal       (1000) cal       (1000)     4438 2024-04-08 09:41:10.000000 csvbase-client-0.1.0/csvbase_client/internals/cli.py
--rw-r--r--   0 cal       (1000) cal       (1000)     1560 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/internals/config.py
--rw-r--r--   0 cal       (1000) cal       (1000)       77 2023-08-29 09:50:35.000000 csvbase-client-0.1.0/csvbase_client/internals/dirs.py
--rw-r--r--   0 cal       (1000) cal       (1000)      866 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/internals/http.py
--rw-r--r--   0 cal       (1000) cal       (1000)     1032 2023-08-31 16:35:27.000000 csvbase-client-0.1.0/csvbase_client/internals/value_objs.py
--rw-r--r--   0 cal       (1000) cal       (1000)      855 2024-04-08 09:54:49.000000 csvbase-client-0.1.0/csvbase_client/internals/version.py
--rw-r--r--   0 cal       (1000) cal       (1000)      634 2024-02-03 12:13:20.000000 csvbase-client-0.1.0/csvbase_client/io.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client.egg-info/
--rw-r--r--   0 cal       (1000) cal       (1000)     4342 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/PKG-INFO
--rw-r--r--   0 cal       (1000) cal       (1000)      775 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/SOURCES.txt
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/dependency_links.txt
--rw-r--r--   0 cal       (1000) cal       (1000)      134 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/entry_points.txt
--rw-r--r--   0 cal       (1000) cal       (1000)      120 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/requires.txt
--rw-r--r--   0 cal       (1000) cal       (1000)       15 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/top_level.txt
--rw-r--r--   0 cal       (1000) cal       (1000)       38 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/setup.cfg
--rw-r--r--   0 cal       (1000) cal       (1000)     2114 2024-04-09 11:16:11.000000 csvbase-client-0.1.0/setup.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/tests/
--rw-r--r--   0 cal       (1000) cal       (1000)      759 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/tests/test_cache.py
--rw-r--r--   0 cal       (1000) cal       (1000)      371 2023-08-30 11:50:37.000000 csvbase-client-0.1.0/tests/test_version.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/
+-rw-r--r--   0 cal       (1000) cal       (1000)    34523 2017-09-30 07:16:25.000000 csvbase-client-0.1.1/COPYING
+-rw-r--r--   0 cal       (1000) cal       (1000)       40 2023-04-05 16:09:56.000000 csvbase-client-0.1.1/MANIFEST.in
+-rw-r--r--   0 cal       (1000) cal       (1000)     4367 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/PKG-INFO
+-rw-r--r--   0 cal       (1000) cal       (1000)     2993 2024-04-09 11:25:11.000000 csvbase-client-0.1.1/README.md
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/csvbase_client/
+-rw-r--r--   0 cal       (1000) cal       (1000)        5 2024-04-10 06:32:14.000000 csvbase-client-0.1.1/csvbase_client/VERSION
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.1/csvbase_client/__init__.py
+-rw-r--r--   0 cal       (1000) cal       (1000)       40 2024-04-05 10:25:59.000000 csvbase-client-0.1.1/csvbase_client/constants.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      530 2024-04-05 10:25:59.000000 csvbase-client-0.1.1/csvbase_client/exceptions.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     7318 2024-04-08 10:19:42.000000 csvbase-client-0.1.1/csvbase_client/fsspec.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/csvbase_client/internals/
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.1/csvbase_client/internals/__init__.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      988 2024-02-03 15:57:46.000000 csvbase-client-0.1.1/csvbase_client/internals/auth.py
+-rw-r--r--   0 cal       (1000) cal       (1000)    11948 2024-04-05 10:43:06.000000 csvbase-client-0.1.1/csvbase_client/internals/cache.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     4438 2024-04-08 09:41:10.000000 csvbase-client-0.1.1/csvbase_client/internals/cli.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     1560 2023-08-29 09:47:19.000000 csvbase-client-0.1.1/csvbase_client/internals/config.py
+-rw-r--r--   0 cal       (1000) cal       (1000)       77 2023-08-29 09:50:35.000000 csvbase-client-0.1.1/csvbase_client/internals/dirs.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      866 2024-04-05 10:25:59.000000 csvbase-client-0.1.1/csvbase_client/internals/http.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     1032 2023-08-31 16:35:27.000000 csvbase-client-0.1.1/csvbase_client/internals/value_objs.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      855 2024-04-10 06:34:13.000000 csvbase-client-0.1.1/csvbase_client/internals/version.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      634 2024-02-03 12:13:20.000000 csvbase-client-0.1.1/csvbase_client/io.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/csvbase_client.egg-info/
+-rw-r--r--   0 cal       (1000) cal       (1000)     4367 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/PKG-INFO
+-rw-r--r--   0 cal       (1000) cal       (1000)      775 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)      134 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/entry_points.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)       93 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/requires.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)       15 2024-04-10 06:35:45.000000 csvbase-client-0.1.1/csvbase_client.egg-info/top_level.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)       38 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/setup.cfg
+-rw-r--r--   0 cal       (1000) cal       (1000)     2142 2024-04-09 11:32:15.000000 csvbase-client-0.1.1/setup.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-10 06:35:45.206502 csvbase-client-0.1.1/tests/
+-rw-r--r--   0 cal       (1000) cal       (1000)      759 2024-04-05 10:25:59.000000 csvbase-client-0.1.1/tests/test_cache.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      371 2023-08-30 11:50:37.000000 csvbase-client-0.1.1/tests/test_version.py
```

### Comparing `csvbase-client-0.1.0/COPYING` & `csvbase-client-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/PKG-INFO` & `csvbase-client-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvbase-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: The command line client for csvbase
 Home-page: https://github.com/calpaterson/csvbase-client
 Author: Cal Paterson
 Author-email: cal@calpaterson.com
 Project-URL: Bug Tracker, https://github.com/calpaterson/csvbase-client/issues
 Project-URL: Documentation, https://github.com/calpaterson/csvbase-client/wiki
 Project-URL: Source Code, https://github.com/calpaterson/csvbase-client
@@ -14,50 +14,49 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: click
 Requires-Dist: platformdirs
 Requires-Dist: pyappcache>=0.10.0
 Requires-Dist: requests
 Requires-Dist: toml
-Requires-Dist: importlib_resources; python_version < "3.9"
+Requires-Dist: importlib_resources
 Requires-Dist: fsspec
 Requires-Dist: rich
 Requires-Dist: humanize
 
 <div align="center">
     <img alt="csvbase logo" src="https://github.com/calpaterson/csvbase/raw/main/csvbase/web/static/logo/128x128.png">
 </div>
 
 # csvbase-client
 
 The command line client and pandas integration for [csvbase](https://csvbase.com/).
 
 ## Status
 
-This tool is very early alpha and suitable for testing.
-
-Semantic versioning is followed, see the [changelog](CHANGELOG.md).
+Semantic versioning is followed, see the [changelog](https://github.com/calpaterson/csvbase-client/blob/main/CHANGELOG.md).
 
 ## Usage
 
 ### Get a table
 
 In pandas:
 
 ```python
 >>> import pandas as pd
->>>  pd.read_csv("csvbase://meripaterson/stock-exchanges")
+>>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
 >>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
      csvbase_row_id      Continent                   Country                                     Name   MIC Last changed
 0                 1         Africa                   Lesotho                                    HYBSE   NaN   2019-03-25
 1                 2           Asia                Kazakhstan    Astana International Financial Centre  AIXK   2018-11-18
 2                 3         Africa              South Africa                                    ZAR X  ZARX   2018-11-18
 3                 4  South America                 Argentina             Bolsas y Mercados Argentinos   NaN   2018-04-02
 4                 5  North America  United States of America                  Delaware Board of Trade   NaN   2018-04-02
```

### Comparing `csvbase-client-0.1.0/README.md` & `csvbase-client-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 
 # csvbase-client
 
 The command line client and pandas integration for [csvbase](https://csvbase.com/).
 
 ## Status
 
-This tool is very early alpha and suitable for testing.
-
-Semantic versioning is followed, see the [changelog](CHANGELOG.md).
+Semantic versioning is followed, see the [changelog](https://github.com/calpaterson/csvbase-client/blob/main/CHANGELOG.md).
 
 ## Usage
 
 ### Get a table
 
 In pandas:
 
 ```python
 >>> import pandas as pd
->>>  pd.read_csv("csvbase://meripaterson/stock-exchanges")
+>>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
 >>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
      csvbase_row_id      Continent                   Country                                     Name   MIC Last changed
 0                 1         Africa                   Lesotho                                    HYBSE   NaN   2019-03-25
 1                 2           Asia                Kazakhstan    Astana International Financial Centre  AIXK   2018-11-18
 2                 3         Africa              South Africa                                    ZAR X  ZARX   2018-11-18
 3                 4  South America                 Argentina             Bolsas y Mercados Argentinos   NaN   2018-04-02
 4                 5  North America  United States of America                  Delaware Board of Trade   NaN   2018-04-02
```

### Comparing `csvbase-client-0.1.0/csvbase_client/exceptions.py` & `csvbase-client-0.1.1/csvbase_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/fsspec.py` & `csvbase-client-0.1.1/csvbase_client/fsspec.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/auth.py` & `csvbase-client-0.1.1/csvbase_client/internals/auth.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/cache.py` & `csvbase-client-0.1.1/csvbase_client/internals/cache.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/cli.py` & `csvbase-client-0.1.1/csvbase_client/internals/cli.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/config.py` & `csvbase-client-0.1.1/csvbase_client/internals/config.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/http.py` & `csvbase-client-0.1.1/csvbase_client/internals/http.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/value_objs.py` & `csvbase-client-0.1.1/csvbase_client/internals/value_objs.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client/internals/version.py` & `csvbase-client-0.1.1/csvbase_client/internals/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 def get_hardcoded_version() -> str:
     """Return the hardcoded version number.
 
     This is used when we're not in a valid package, for example when built by Nuitka.
 
     """
-    return "0.1.0"
+    return "0.1.1"
```

### Comparing `csvbase-client-0.1.0/csvbase_client/io.py` & `csvbase-client-0.1.1/csvbase_client/io.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/csvbase_client.egg-info/PKG-INFO` & `csvbase-client-0.1.1/csvbase_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvbase-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: The command line client for csvbase
 Home-page: https://github.com/calpaterson/csvbase-client
 Author: Cal Paterson
 Author-email: cal@calpaterson.com
 Project-URL: Bug Tracker, https://github.com/calpaterson/csvbase-client/issues
 Project-URL: Documentation, https://github.com/calpaterson/csvbase-client/wiki
 Project-URL: Source Code, https://github.com/calpaterson/csvbase-client
@@ -14,50 +14,49 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: click
 Requires-Dist: platformdirs
 Requires-Dist: pyappcache>=0.10.0
 Requires-Dist: requests
 Requires-Dist: toml
-Requires-Dist: importlib_resources; python_version < "3.9"
+Requires-Dist: importlib_resources
 Requires-Dist: fsspec
 Requires-Dist: rich
 Requires-Dist: humanize
 
 <div align="center">
     <img alt="csvbase logo" src="https://github.com/calpaterson/csvbase/raw/main/csvbase/web/static/logo/128x128.png">
 </div>
 
 # csvbase-client
 
 The command line client and pandas integration for [csvbase](https://csvbase.com/).
 
 ## Status
 
-This tool is very early alpha and suitable for testing.
-
-Semantic versioning is followed, see the [changelog](CHANGELOG.md).
+Semantic versioning is followed, see the [changelog](https://github.com/calpaterson/csvbase-client/blob/main/CHANGELOG.md).
 
 ## Usage
 
 ### Get a table
 
 In pandas:
 
 ```python
 >>> import pandas as pd
->>>  pd.read_csv("csvbase://meripaterson/stock-exchanges")
+>>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
 >>> pd.read_csv("csvbase://meripaterson/stock-exchanges")
      csvbase_row_id      Continent                   Country                                     Name   MIC Last changed
 0                 1         Africa                   Lesotho                                    HYBSE   NaN   2019-03-25
 1                 2           Asia                Kazakhstan    Astana International Financial Centre  AIXK   2018-11-18
 2                 3         Africa              South Africa                                    ZAR X  ZARX   2018-11-18
 3                 4  South America                 Argentina             Bolsas y Mercados Argentinos   NaN   2018-04-02
 4                 5  North America  United States of America                  Delaware Board of Trade   NaN   2018-04-02
```

### Comparing `csvbase-client-0.1.0/csvbase_client.egg-info/SOURCES.txt` & `csvbase-client-0.1.1/csvbase_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.1.0/setup.py` & `csvbase-client-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,29 @@
     package_data={"csvbase_client": ["VERSION"]},
     install_requires=[
         "click",
         "platformdirs",
         "pyappcache>=0.10.0",
         "requests",
         "toml",
-        "importlib_resources; python_version<'3.9'",
+        "importlib_resources",
         "fsspec",
         "rich",
         "humanize",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         c,
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Utilities",
     ],
     project_urls={
         "Bug Tracker": "https://github.com/calpaterson/csvbase-client/issues",
         "Documentation": "https://github.com/calpaterson/csvbase-client/wiki",
         "Source Code": "https://github.com/calpaterson/csvbase-client",
         "Changelog": "https://github.com/calpaterson/csvbase-client/blob/main/CHANGELOG.md",
```

### Comparing `csvbase-client-0.1.0/tests/test_cache.py` & `csvbase-client-0.1.1/tests/test_cache.py`

 * *Files identical despite different names*

