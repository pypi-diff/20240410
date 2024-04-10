# Comparing `tmp/deltafi-2.0rc1705024454242.tar.gz` & `tmp/deltafi-2.0rc1705080991758.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1705024454242.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1705080991758.tar", max compression
```

## Comparing `deltafi-2.0rc1705024454242.tar` & `deltafi-2.0rc1705080991758.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-2.0rc1705024454242/README.md
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.608536 deltafi-2.0rc1705024454242/deltafi/__init__.py
--rw-r--r--   0        0        0     5305 2024-01-11 22:49:18.920091 deltafi-2.0rc1705024454242/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-13 13:53:29.360657 deltafi-2.0rc1705024454242/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      865 2024-01-11 22:49:18.920091 deltafi-2.0rc1705024454242/deltafi/actiontype.py
--rw-r--r--   0        0        0    12161 2023-10-24 01:56:39.336492 deltafi-2.0rc1705024454242/deltafi/domain.py
--rw-r--r--   0        0        0     1149 2023-04-24 17:42:15.589313 deltafi-2.0rc1705024454242/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-16 03:01:54.189409 deltafi-2.0rc1705024454242/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-01-11 22:49:18.922092 deltafi-2.0rc1705024454242/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-2.0rc1705024454242/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-2.0rc1705024454242/deltafi/metric.py
--rw-r--r--   0        0        0    12956 2024-01-11 22:49:18.923092 deltafi-2.0rc1705024454242/deltafi/plugin.py
--rw-r--r--   0        0        0     7330 2024-01-11 22:49:18.923092 deltafi-2.0rc1705024454242/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-2.0rc1705024454242/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-09-08 11:24:47.609536 deltafi-2.0rc1705024454242/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-09-08 11:24:47.609536 deltafi-2.0rc1705024454242/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0     1581 2023-09-08 11:24:47.609536 deltafi-2.0rc1705024454242/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-08-07 14:10:09.593662 deltafi-2.0rc1705024454242/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0    13062 2024-01-11 22:49:18.923092 deltafi-2.0rc1705024454242/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     2608 2024-01-11 22:49:18.931092 deltafi-2.0rc1705024454242/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1309 2024-01-12 01:54:20.215257 deltafi-2.0rc1705024454242/pyproject.toml
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 deltafi-2.0rc1705024454242/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:32:51.621370 deltafi-2.0rc1705080991758/README.md
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:19.408525 deltafi-2.0rc1705080991758/deltafi/__init__.py
+-rw-r--r--   0        0        0     5305 2024-01-12 17:29:57.481763 deltafi-2.0rc1705080991758/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-25 14:03:47.782289 deltafi-2.0rc1705080991758/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      865 2024-01-12 17:29:57.482763 deltafi-2.0rc1705080991758/deltafi/actiontype.py
+-rw-r--r--   0        0        0    12161 2023-10-25 14:03:47.782289 deltafi-2.0rc1705080991758/deltafi/domain.py
+-rw-r--r--   0        0        0     1149 2023-04-26 13:21:52.730906 deltafi-2.0rc1705080991758/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-15 22:01:12.726378 deltafi-2.0rc1705080991758/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-01-12 17:29:57.483763 deltafi-2.0rc1705080991758/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:32:51.623371 deltafi-2.0rc1705080991758/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:32:51.623371 deltafi-2.0rc1705080991758/deltafi/metric.py
+-rw-r--r--   0        0        0    12956 2024-01-12 17:29:57.484763 deltafi-2.0rc1705080991758/deltafi/plugin.py
+-rw-r--r--   0        0        0     7330 2024-01-12 17:29:57.486763 deltafi-2.0rc1705080991758/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-19 17:18:33.056792 deltafi-2.0rc1705080991758/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0     1581 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-10-18 22:01:19.414525 deltafi-2.0rc1705080991758/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0    13062 2024-01-12 17:21:36.473545 deltafi-2.0rc1705080991758/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     2608 2024-01-12 17:21:36.473545 deltafi-2.0rc1705080991758/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1309 2024-01-12 17:36:38.975579 deltafi-2.0rc1705080991758/pyproject.toml
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 deltafi-2.0rc1705080991758/PKG-INFO
```

### Comparing `deltafi-2.0rc1705024454242/deltafi/__init__.py` & `deltafi-2.0rc1705080991758/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/action.py` & `deltafi-2.0rc1705080991758/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/actioneventqueue.py` & `deltafi-2.0rc1705080991758/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/actiontype.py` & `deltafi-2.0rc1705080991758/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/domain.py` & `deltafi-2.0rc1705080991758/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/exception.py` & `deltafi-2.0rc1705080991758/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/genericmodel.py` & `deltafi-2.0rc1705080991758/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/input.py` & `deltafi-2.0rc1705080991758/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/logger.py` & `deltafi-2.0rc1705080991758/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/metric.py` & `deltafi-2.0rc1705080991758/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/plugin.py` & `deltafi-2.0rc1705080991758/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/result.py` & `deltafi-2.0rc1705080991758/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/storage.py` & `deltafi-2.0rc1705080991758/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/compare_helpers.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/compare_helpers.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/constants.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/framework.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/framework.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/deltafi/test_kit/transform.py` & `deltafi-2.0rc1705080991758/deltafi/test_kit/transform.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1705024454242/pyproject.toml` & `deltafi-2.0rc1705080991758/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1705024454242"
+version = "2.0rc1705080991758"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-2.0rc1705024454242/PKG-INFO` & `deltafi-2.0rc1705080991758/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1705024454242
+Version: 2.0rc1705080991758
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

