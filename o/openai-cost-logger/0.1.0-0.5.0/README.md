# Comparing `tmp/openai_cost_logger-0.1.0.tar.gz` & `tmp/openai_cost_logger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_cost_logger-0.1.0.tar", last modified: Tue Apr  9 22:02:18 2024, max compression
+gzip compressed data, was "openai_cost_logger-0.5.0.tar", last modified: Mon Apr  8 14:24:45 2024, max compression
```

## Comparing `openai_cost_logger-0.1.0.tar` & `openai_cost_logger-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/setup.py
```

### Comparing `openai_cost_logger-0.1.0/LICENSE` & `openai_cost_logger-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/PKG-INFO` & `openai_cost_logger-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_cost_logger
-Version: 0.1.0
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker
 Platform: UNKNOWN
```

### Comparing `openai_cost_logger-0.1.0/README.rst` & `openai_cost_logger-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger/constants.py` & `openai_cost_logger-0.5.0/openai_cost_logger/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,33 +4,23 @@
 DEFAULT_LOG_PATH = "cost-logs"
 
 """Enum containing the tested models."""
 class Models(Enum):
     TURBO_3_5 = "gpt-3.5-turbo"
     TURBO_3_5_INSTRUCT = "gpt-3.5-turbo-instruct"
     AZURE_3_5_TURBO = "gpt-35-turbo-0125"
-    AZURE_4_TURBO = "gpt-4-0125-Preview"
-    AZURE_4 = "gpt-4-0613"
 
 """The costs of the models above (per million tokens)."""
 MODELS_COST = {
     "gpt-3.5-turbo": {
         "input": 0.5,
         "output": 1.5
     },
     "gpt-35-turbo-0125": {
         "input": 0.5,
         "output": 1.5
     },
     "gpt-3.5-turbo-instruct": {
         "input": 1.5,
         "output": 2
-    },
-    "gpt-4-0125-Preview": {
-        "input": 10,
-        "output": 30
-    },
-    "gpt-4-0613": {
-        "input": 30,
-        "output": 60
-    },
+    }
 }
```

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger.py` & `openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_viz.py` & `openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger.egg-info/PKG-INFO` & `openai_cost_logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.1.0
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker
 Platform: UNKNOWN
```

### Comparing `openai_cost_logger-0.1.0/setup.py` & `openai_cost_logger-0.5.0/setup.py`

 * *Files identical despite different names*

