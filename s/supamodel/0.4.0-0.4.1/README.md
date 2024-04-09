# Comparing `tmp/supamodel-0.4.0.tar.gz` & `tmp/supamodel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supamodel-0.4.0.tar", max compression
+gzip compressed data, was "supamodel-0.4.1.tar", max compression
```

## Comparing `supamodel-0.4.0.tar` & `supamodel-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.4.0/README.md
--rw-r--r--   0        0        0      573 2024-04-09 23:47:13.516618 supamodel-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.4.0/supamodel/__init__.py
--rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.4.0/supamodel/_abc.py
--rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.4.0/supamodel/_client.py
--rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.4.0/supamodel/_core.py
--rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.4.0/supamodel/_logging.py
--rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.4.0/supamodel/_types.py
--rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.0/supamodel/config.py
--rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.0/supamodel/enums.py
--rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.0/supamodel/errors.py
--rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.4.0/supamodel/exceptions.py
--rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.0/supamodel/supa_model.py
--rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.0/supamodel/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.0/supamodel/trading/assets.py
--rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.0/supamodel/trading/clock.py
--rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.0/supamodel/trading/exchange.py
--rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.0/supamodel/trading/market_data.py
--rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.4.0/supamodel/trading/order_management.py
--rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.4.0/supamodel/trading/portfolio.py
--rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.4.0/supamodel/utils.py
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 supamodel-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      923 2024-04-09 22:47:07.642756 supamodel-0.4.1/README.md
+-rw-r--r--   0        0        0      619 2024-04-09 23:48:24.768588 supamodel-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:17:58.633418 supamodel-0.4.1/supamodel/__init__.py
+-rw-r--r--   0        0        0     8362 2024-04-09 21:40:21.038360 supamodel-0.4.1/supamodel/_abc.py
+-rw-r--r--   0        0        0      217 2024-04-09 21:36:38.405771 supamodel-0.4.1/supamodel/_client.py
+-rw-r--r--   0        0        0     3902 2024-04-09 16:55:51.007166 supamodel-0.4.1/supamodel/_core.py
+-rw-r--r--   0        0        0      165 2024-04-09 16:51:55.116392 supamodel-0.4.1/supamodel/_logging.py
+-rw-r--r--   0        0        0      335 2024-04-09 21:36:50.396134 supamodel-0.4.1/supamodel/_types.py
+-rw-r--r--   0        0        0     1484 2024-04-09 21:08:01.785026 supamodel-0.4.1/supamodel/config.py
+-rw-r--r--   0        0        0     2284 2024-04-09 21:21:46.805022 supamodel-0.4.1/supamodel/enums.py
+-rw-r--r--   0        0        0      321 2024-04-09 17:20:12.482160 supamodel-0.4.1/supamodel/errors.py
+-rw-r--r--   0        0        0     1432 2024-04-09 21:05:41.384852 supamodel-0.4.1/supamodel/exceptions.py
+-rw-r--r--   0        0        0     8307 2024-04-09 23:43:15.347009 supamodel-0.4.1/supamodel/supa_model.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:35.833946 supamodel-0.4.1/supamodel/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:29:20.829143 supamodel-0.4.1/supamodel/trading/assets.py
+-rw-r--r--   0        0        0     3690 2024-04-09 21:24:42.417053 supamodel-0.4.1/supamodel/trading/clock.py
+-rw-r--r--   0        0        0     3436 2024-04-09 21:20:23.128058 supamodel-0.4.1/supamodel/trading/exchange.py
+-rw-r--r--   0        0        0     1347 2024-04-09 21:21:25.286277 supamodel-0.4.1/supamodel/trading/market_data.py
+-rw-r--r--   0        0        0     1866 2024-04-09 21:14:17.363708 supamodel-0.4.1/supamodel/trading/order_management.py
+-rw-r--r--   0        0        0     1833 2024-04-09 21:11:42.958490 supamodel-0.4.1/supamodel/trading/portfolio.py
+-rw-r--r--   0        0        0    11495 2024-04-09 21:42:48.641249 supamodel-0.4.1/supamodel/utils.py
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 supamodel-0.4.1/PKG-INFO
```

### Comparing `supamodel-0.4.0/README.md` & `supamodel-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/pyproject.toml` & `supamodel-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "supamodel"
-version = "0.4.0"
-description = ""
+version = "0.4.1"
+description = "Pydantic Models for Trading Algos and Supabase"
 authors = ["Kevin Hill <kivo360@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
 pendulum = ">=2.0.0,<4.0.0"
 loguru = ">=0.5.0,<1.0.0"
```

### Comparing `supamodel-0.4.0/supamodel/_abc.py` & `supamodel-0.4.1/supamodel/_abc.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/_core.py` & `supamodel-0.4.1/supamodel/_core.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/config.py` & `supamodel-0.4.1/supamodel/config.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/enums.py` & `supamodel-0.4.1/supamodel/enums.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/exceptions.py` & `supamodel-0.4.1/supamodel/exceptions.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/supa_model.py` & `supamodel-0.4.1/supamodel/supa_model.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/trading/clock.py` & `supamodel-0.4.1/supamodel/trading/clock.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/trading/exchange.py` & `supamodel-0.4.1/supamodel/trading/exchange.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/trading/market_data.py` & `supamodel-0.4.1/supamodel/trading/market_data.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/trading/order_management.py` & `supamodel-0.4.1/supamodel/trading/order_management.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/trading/portfolio.py` & `supamodel-0.4.1/supamodel/trading/portfolio.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/supamodel/utils.py` & `supamodel-0.4.1/supamodel/utils.py`

 * *Files identical despite different names*

### Comparing `supamodel-0.4.0/PKG-INFO` & `supamodel-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: supamodel
-Version: 0.4.0
-Summary: 
+Version: 0.4.1
+Summary: Pydantic Models for Trading Algos and Supabase
 Author: Kevin Hill
 Author-email: kivo360@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

