# Comparing `tmp/powerflex-logging-utilities-1.3.0.tar.gz` & `tmp/powerflex-logging-utilities-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerflex-logging-utilities-1.3.0.tar", last modified: Wed Aug 16 21:19:50 2023, max compression
+gzip compressed data, was "powerflex-logging-utilities-1.3.1.tar", last modified: Wed Apr 10 17:17:36 2024, max compression
```

## Comparing `powerflex-logging-utilities-1.3.0.tar` & `powerflex-logging-utilities-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-16 21:19:50.188985 powerflex-logging-utilities-1.3.0/
--rw-r--r--   0 user      (1000) user      (1000)     1071 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     8046 2023-08-16 21:19:50.188985 powerflex-logging-utilities-1.3.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     6780 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)      100 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-08-16 21:19:50.188985 powerflex-logging-utilities-1.3.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     2124 2023-08-15 03:04:22.000000 powerflex-logging-utilities-1.3.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-16 21:19:50.178985 powerflex-logging-utilities-1.3.0/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-16 21:19:50.181985 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/
--rw-r--r--   0 user      (1000) user      (1000)        6 2023-08-15 03:06:31.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/VERSION
--rw-r--r--   0 user      (1000) user      (1000)      310 2023-08-15 03:03:57.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      118 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/default_log_format.py
--rw-r--r--   0 user      (1000) user      (1000)     1180 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/forbid_toplevel_logging.py
--rw-r--r--   0 user      (1000) user      (1000)     5575 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/init_loggers.py
--rw-r--r--   0 user      (1000) user      (1000)     1013 2023-08-15 03:06:31.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/json_formatter.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-16 21:19:50.187985 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/
--rw-r--r--   0 user      (1000) user      (1000)     3378 2023-08-15 03:04:22.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      333 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/format_exception.py
--rw-r--r--   0 user      (1000) user      (1000)     3234 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/nats.py
--rw-r--r--   0 user      (1000) user      (1000)     1203 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_slow_callbacks.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/py.typed
--rw-r--r--   0 user      (1000) user      (1000)      927 2023-08-15 02:12:41.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/trace_logger.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-16 21:19:50.182985 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     8046 2023-08-16 21:19:50.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      996 2023-08-16 21:19:50.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-08-16 21:19:50.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      221 2023-08-16 21:19:50.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-08-16 21:19:50.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-08-15 02:16:45.000000 powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/zip-safe
+drwxr-xr-x   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:17:36.116085 powerflex-logging-utilities-1.3.1/
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     1071 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/LICENSE
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     8567 2024-04-10 17:17:36.116085 powerflex-logging-utilities-1.3.1/PKG-INFO
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     6780 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/README.md
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      100 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/pyproject.toml
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)       38 2024-04-10 17:17:36.116085 powerflex-logging-utilities-1.3.1/setup.cfg
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     2124 2024-04-10 17:12:11.000000 powerflex-logging-utilities-1.3.1/setup.py
+drwxr-xr-x   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:17:36.109418 powerflex-logging-utilities-1.3.1/src/
+drwxr-xr-x   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:17:36.112752 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)        6 2024-04-10 17:14:32.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/VERSION
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      310 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/__init__.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      118 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/default_log_format.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     1180 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/forbid_toplevel_logging.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     5575 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/init_loggers.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     1013 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/json_formatter.py
+drwxr-xr-x   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:17:36.112752 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     3378 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/__init__.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      333 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/format_exception.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     3234 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/nats.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     1203 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_slow_callbacks.py
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/py.typed
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      927 2024-04-10 17:10:59.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/trace_logger.py
+drwxr-xr-x   0 FeLiNa    (1000) felina    (1000)        0 2024-04-10 17:17:36.112752 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)     8567 2024-04-10 17:17:36.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      996 2024-04-10 17:17:36.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)        1 2024-04-10 17:17:36.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)      221 2024-04-10 17:17:36.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/requires.txt
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)       28 2024-04-10 17:17:36.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/top_level.txt
+-rw-r--r--   0 FeLiNa    (1000) felina    (1000)        1 2024-04-10 17:16:46.000000 powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/zip-safe
```

### Comparing `powerflex-logging-utilities-1.3.0/LICENSE` & `powerflex-logging-utilities-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/PKG-INFO` & `powerflex-logging-utilities-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: powerflex-logging-utilities
-Version: 1.3.0
-Summary: Helpful code for logging in Python
-Home-page: https://github.com/edf-re/powerflex_logging_utilities_py
-License: MIT License
-Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_logging_utilities_py/issues
-Keywords: NATS,NATS request,aiodebug,async,JSON logging
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Utilities
-Requires-Python: >2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
-Description-Content-Type: text/markdown
-Provides-Extra: pydantic
-Provides-Extra: pydantic2
-Provides-Extra: nats-and-pydantic
-Provides-Extra: nats-and-pydantic2
-License-File: LICENSE
-
 # powerflex-logging-utilities
 
 <!-- Badges (images) related to Python package information -->
 [![PyPI - Version](https://img.shields.io/pypi/v/powerflex-logging-utilities) ![PyPI - License](https://img.shields.io/pypi/l/powerflex-logging-utilities) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/powerflex-logging-utilities) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/powerflex-logging-utilities)](https://pypi.org/project/powerflex-logging-utilities/)
 
 Helpful code for logging in Python by PowerFlex.
```

### Comparing `powerflex-logging-utilities-1.3.0/README.md` & `powerflex-logging-utilities-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+Metadata-Version: 2.1
+Name: powerflex-logging-utilities
+Version: 1.3.1
+Summary: Helpful code for logging in Python
+Home-page: https://github.com/edf-re/powerflex_logging_utilities_py
+License: MIT License
+Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_logging_utilities_py/issues
+Keywords: NATS,NATS request,aiodebug,async,JSON logging
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Utilities
+Requires-Python: >2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiodebug>=2.3.0
+Requires-Dist: python-json-logger>=2.0.0
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=1.9; extra == "pydantic"
+Provides-Extra: pydantic2
+Requires-Dist: pydantic>=2; extra == "pydantic2"
+Requires-Dist: pydantic_settings>=2; extra == "pydantic2"
+Provides-Extra: nats-and-pydantic
+Requires-Dist: nats-py>=2; extra == "nats-and-pydantic"
+Requires-Dist: pydantic; extra == "nats-and-pydantic"
+Provides-Extra: nats-and-pydantic2
+Requires-Dist: nats-py>=2; extra == "nats-and-pydantic2"
+Requires-Dist: pydantic>=2; extra == "nats-and-pydantic2"
+Requires-Dist: pydantic_settings>=2; extra == "nats-and-pydantic2"
+
 # powerflex-logging-utilities
 
 <!-- Badges (images) related to Python package information -->
 [![PyPI - Version](https://img.shields.io/pypi/v/powerflex-logging-utilities) ![PyPI - License](https://img.shields.io/pypi/l/powerflex-logging-utilities) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/powerflex-logging-utilities) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/powerflex-logging-utilities)](https://pypi.org/project/powerflex-logging-utilities/)
 
 Helpful code for logging in Python by PowerFlex.
```

### Comparing `powerflex-logging-utilities-1.3.0/setup.py` & `powerflex-logging-utilities-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "Issue Tracker": "https://github.com/edf-re/powerflex_logging_utilities_py/issues",
     },
     keywords=["NATS", "NATS request", "aiodebug", "async", "JSON logging"],
     # Only 3.8+
     python_requires=">2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*",
     install_requires=[
         "aiodebug>=2.3.0",
-        "python-json-logger>=2.0.4",
+        "python-json-logger>=2.0.0",
     ],
     extras_require={
         "pydantic": ["pydantic>=1.9"],
         "pydantic2": ["pydantic>=2", "pydantic_settings>=2"],
         "nats-and-pydantic": ["nats-py>=2", "pydantic"],
         "nats-and-pydantic2": ["nats-py>=2", "pydantic>=2", "pydantic_settings>=2"],
     },
```

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/forbid_toplevel_logging.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/forbid_toplevel_logging.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/init_loggers.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/init_loggers.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/json_formatter.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/json_formatter.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/__init__.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_level_listener/nats.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_level_listener/nats.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/log_slow_callbacks.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/log_slow_callbacks.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities/trace_logger.py` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities/trace_logger.py`

 * *Files identical despite different names*

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/PKG-INFO` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerflex-logging-utilities
-Version: 1.3.0
+Version: 1.3.1
 Summary: Helpful code for logging in Python
 Home-page: https://github.com/edf-re/powerflex_logging_utilities_py
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_logging_utilities_py/issues
 Keywords: NATS,NATS request,aiodebug,async,JSON logging
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
@@ -17,19 +17,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiodebug>=2.3.0
+Requires-Dist: python-json-logger>=2.0.0
 Provides-Extra: pydantic
+Requires-Dist: pydantic>=1.9; extra == "pydantic"
 Provides-Extra: pydantic2
+Requires-Dist: pydantic>=2; extra == "pydantic2"
+Requires-Dist: pydantic_settings>=2; extra == "pydantic2"
 Provides-Extra: nats-and-pydantic
+Requires-Dist: nats-py>=2; extra == "nats-and-pydantic"
+Requires-Dist: pydantic; extra == "nats-and-pydantic"
 Provides-Extra: nats-and-pydantic2
-License-File: LICENSE
+Requires-Dist: nats-py>=2; extra == "nats-and-pydantic2"
+Requires-Dist: pydantic>=2; extra == "nats-and-pydantic2"
+Requires-Dist: pydantic_settings>=2; extra == "nats-and-pydantic2"
 
 # powerflex-logging-utilities
 
 <!-- Badges (images) related to Python package information -->
 [![PyPI - Version](https://img.shields.io/pypi/v/powerflex-logging-utilities) ![PyPI - License](https://img.shields.io/pypi/l/powerflex-logging-utilities) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/powerflex-logging-utilities) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/powerflex-logging-utilities)](https://pypi.org/project/powerflex-logging-utilities/)
 
 Helpful code for logging in Python by PowerFlex.
```

### Comparing `powerflex-logging-utilities-1.3.0/src/powerflex_logging_utilities.egg-info/SOURCES.txt` & `powerflex-logging-utilities-1.3.1/src/powerflex_logging_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

