# Comparing `tmp/rooms_shared_services-0.1.93.tar.gz` & `tmp/rooms_shared_services-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rooms_shared_services-0.1.93.tar", max compression
+gzip compressed data, was "rooms_shared_services-0.1.94.tar", max compression
```

## Comparing `rooms_shared_services-0.1.93.tar` & `rooms_shared_services-0.1.94.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1074 2024-01-10 20:24:32.715596 rooms_shared_services-0.1.93/LICENSE
--rw-r--r--   0        0        0      103 2024-01-10 19:47:32.069678 rooms_shared_services-0.1.93/README.md
--rw-r--r--   0        0        0     1790 2024-04-10 20:18:21.470754 rooms_shared_services-0.1.93/pyproject.toml
--rw-r--r--   0        0        0       36 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.93/rooms_shared_services/__init__.py
--rw-r--r--   0        0        0       19 2024-01-20 21:38:48.769936 rooms_shared_services-0.1.93/rooms_shared_services/src/__init__.py
--rw-r--r--   0        0        0     9379 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/abstract.py
--rw-r--r--   0        0        0      744 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/models.py
--rw-r--r--   0        0        0     2413 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/processor.py
--rw-r--r--   0        0        0      459 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/runner.py
--rw-r--r--   0        0        0      833 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/sandbox.py
--rw-r--r--   0        0        0     3764 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/storage.py
--rw-r--r--   0        0        0     1120 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/tracker.py
--rw-r--r--   0        0        0      465 2024-03-19 18:17:17.505732 rooms_shared_services-0.1.93/rooms_shared_services/src/exceptions/storage.py
--rw-r--r--   0        0        0     1635 2024-01-31 06:50:04.784461 rooms_shared_services-0.1.93/rooms_shared_services/src/fakers/fake.py
--rw-r--r--   0        0        0     1297 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/logging/http_logger.py
--rw-r--r--   0        0        0      370 2024-02-26 16:41:13.089113 rooms_shared_services-0.1.93/rooms_shared_services/src/logging/settings.py
--rw-r--r--   0        0        0      584 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.93/rooms_shared_services/src/main.py
--rw-r--r--   0        0        0       47 2024-04-10 17:35:20.839115 rooms_shared_services-0.1.93/rooms_shared_services/src/models/countries.json
--rw-r--r--   0        0        0       53 2024-04-10 17:40:03.707840 rooms_shared_services-0.1.93/rooms_shared_services/src/models/currency_rates.json
--rw-r--r--   0        0        0      773 2024-03-16 18:49:13.180657 rooms_shared_services-0.1.93/rooms_shared_services/src/models/products/categories.py
--rw-r--r--   0        0        0      361 2024-04-10 20:16:23.507971 rooms_shared_services-0.1.93/rooms_shared_services/src/models/products/product_groups.py
--rw-r--r--   0        0        0     6062 2024-04-10 18:41:25.529147 rooms_shared_services-0.1.93/rooms_shared_services/src/models/products/products.py
--rw-r--r--   0        0        0      175 2024-03-13 19:10:06.811897 rooms_shared_services-0.1.93/rooms_shared_services/src/models/texts/languages.py
--rw-r--r--   0        0        0      826 2024-03-16 15:41:04.459885 rooms_shared_services-0.1.93/rooms_shared_services/src/models/texts/translations.py
--rw-r--r--   0        0        0       93 2024-03-19 09:10:47.716373 rooms_shared_services-0.1.93/rooms_shared_services/src/money/currency_map.json
--rw-r--r--   0        0        0      122 2024-03-19 09:10:47.720373 rooms_shared_services-0.1.93/rooms_shared_services/src/money/pricing.json
--rw-r--r--   0        0        0     2453 2024-03-13 19:23:23.165046 rooms_shared_services-0.1.93/rooms_shared_services/src/product_categories/provider.py
--rw-r--r--   0        0        0     5071 2024-03-21 09:50:15.621705 rooms_shared_services-0.1.93/rooms_shared_services/src/product_categories/source.py
--rw-r--r--   0        0        0       63 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.93/rooms_shared_services/src/receivers/abstract.py
--rw-r--r--   0        0        0      808 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.93/rooms_shared_services/src/settings/delayed_tasks.py
--rw-r--r--   0        0        0      287 2024-03-16 18:07:48.579227 rooms_shared_services-0.1.93/rooms_shared_services/src/settings/product_categories.py
--rw-r--r--   0        0        0      248 2024-04-10 19:02:35.015191 rooms_shared_services-0.1.93/rooms_shared_services/src/settings/product_group_source.py
--rw-r--r--   0        0        0      314 2024-03-23 15:27:01.729619 rooms_shared_services-0.1.93/rooms_shared_services/src/settings/product_source.py
--rw-r--r--   0        0        0     6278 2024-03-19 09:10:38.408411 rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_categories/processor.py
--rw-r--r--   0        0        0     2868 2024-03-16 15:53:01.660907 rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_categories/provider.py
--rw-r--r--   0        0        0     1204 2024-03-19 09:10:38.272412 rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_pricing/processor.py
--rw-r--r--   0        0        0       23 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.93/rooms_shared_services/src/storage/__init__.py
--rw-r--r--   0        0        0      998 2024-02-29 13:26:42.839128 rooms_shared_services-0.1.93/rooms_shared_services/src/storage/abstract.py
--rw-r--r--   0        0        0    14880 2024-04-09 21:53:53.254801 rooms_shared_services-0.1.93/rooms_shared_services/src/storage/dynamodb.py
--rw-r--r--   0        0        0     2830 2024-04-10 19:26:02.732816 rooms_shared_services-0.1.93/rooms_shared_services/src/storage/models.py
--rw-r--r--   0        0        0     1004 2024-03-16 15:31:07.613112 rooms_shared_services-0.1.93/rooms_shared_services/src/translation/client.py
--rw-r--r--   0        0        0      252 2024-03-18 21:23:21.407853 rooms_shared_services-0.1.93/rooms_shared_services/src/translation/providers/abstract.py
--rw-r--r--   0        0        0      713 2024-03-16 15:10:20.760900 rooms_shared_services-0.1.93/rooms_shared_services/src/translation/providers/aws.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 rooms_shared_services-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-10 20:24:32.715596 rooms_shared_services-0.1.94/LICENSE
+-rw-r--r--   0        0        0      103 2024-01-10 19:47:32.069678 rooms_shared_services-0.1.94/README.md
+-rw-r--r--   0        0        0     1790 2024-04-10 20:23:47.953621 rooms_shared_services-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.94/rooms_shared_services/__init__.py
+-rw-r--r--   0        0        0       19 2024-01-20 21:38:48.769936 rooms_shared_services-0.1.94/rooms_shared_services/src/__init__.py
+-rw-r--r--   0        0        0     9379 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/abstract.py
+-rw-r--r--   0        0        0      744 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/models.py
+-rw-r--r--   0        0        0     2413 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/processor.py
+-rw-r--r--   0        0        0      459 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/runner.py
+-rw-r--r--   0        0        0      833 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/sandbox.py
+-rw-r--r--   0        0        0     3764 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/storage.py
+-rw-r--r--   0        0        0     1120 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/tracker.py
+-rw-r--r--   0        0        0      465 2024-03-19 18:17:17.505732 rooms_shared_services-0.1.94/rooms_shared_services/src/exceptions/storage.py
+-rw-r--r--   0        0        0     1635 2024-01-31 06:50:04.784461 rooms_shared_services-0.1.94/rooms_shared_services/src/fakers/fake.py
+-rw-r--r--   0        0        0     1297 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/logging/http_logger.py
+-rw-r--r--   0        0        0      370 2024-02-26 16:41:13.089113 rooms_shared_services-0.1.94/rooms_shared_services/src/logging/settings.py
+-rw-r--r--   0        0        0      584 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.94/rooms_shared_services/src/main.py
+-rw-r--r--   0        0        0       47 2024-04-10 17:35:20.839115 rooms_shared_services-0.1.94/rooms_shared_services/src/models/countries.json
+-rw-r--r--   0        0        0       53 2024-04-10 17:40:03.707840 rooms_shared_services-0.1.94/rooms_shared_services/src/models/currency_rates.json
+-rw-r--r--   0        0        0      773 2024-03-16 18:49:13.180657 rooms_shared_services-0.1.94/rooms_shared_services/src/models/products/categories.py
+-rw-r--r--   0        0        0      361 2024-04-10 20:16:23.507971 rooms_shared_services-0.1.94/rooms_shared_services/src/models/products/product_groups.py
+-rw-r--r--   0        0        0     6062 2024-04-10 18:41:25.529147 rooms_shared_services-0.1.94/rooms_shared_services/src/models/products/products.py
+-rw-r--r--   0        0        0      175 2024-03-13 19:10:06.811897 rooms_shared_services-0.1.94/rooms_shared_services/src/models/texts/languages.py
+-rw-r--r--   0        0        0      826 2024-03-16 15:41:04.459885 rooms_shared_services-0.1.94/rooms_shared_services/src/models/texts/translations.py
+-rw-r--r--   0        0        0       93 2024-03-19 09:10:47.716373 rooms_shared_services-0.1.94/rooms_shared_services/src/money/currency_map.json
+-rw-r--r--   0        0        0      122 2024-03-19 09:10:47.720373 rooms_shared_services-0.1.94/rooms_shared_services/src/money/pricing.json
+-rw-r--r--   0        0        0     2453 2024-03-13 19:23:23.165046 rooms_shared_services-0.1.94/rooms_shared_services/src/product_categories/provider.py
+-rw-r--r--   0        0        0     5071 2024-03-21 09:50:15.621705 rooms_shared_services-0.1.94/rooms_shared_services/src/product_categories/source.py
+-rw-r--r--   0        0        0       63 2024-01-10 20:24:32.719596 rooms_shared_services-0.1.94/rooms_shared_services/src/receivers/abstract.py
+-rw-r--r--   0        0        0      808 2024-02-29 13:48:06.333250 rooms_shared_services-0.1.94/rooms_shared_services/src/settings/delayed_tasks.py
+-rw-r--r--   0        0        0      287 2024-03-16 18:07:48.579227 rooms_shared_services-0.1.94/rooms_shared_services/src/settings/product_categories.py
+-rw-r--r--   0        0        0      248 2024-04-10 19:02:35.015191 rooms_shared_services-0.1.94/rooms_shared_services/src/settings/product_group_source.py
+-rw-r--r--   0        0        0      314 2024-03-23 15:27:01.729619 rooms_shared_services-0.1.94/rooms_shared_services/src/settings/product_source.py
+-rw-r--r--   0        0        0     6278 2024-03-19 09:10:38.408411 rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_categories/processor.py
+-rw-r--r--   0        0        0     2868 2024-03-16 15:53:01.660907 rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_categories/provider.py
+-rw-r--r--   0        0        0     1204 2024-03-19 09:10:38.272412 rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_pricing/processor.py
+-rw-r--r--   0        0        0      998 2024-02-29 13:26:42.839128 rooms_shared_services-0.1.94/rooms_shared_services/src/storage/abstract.py
+-rw-r--r--   0        0        0    14880 2024-04-09 21:53:53.254801 rooms_shared_services-0.1.94/rooms_shared_services/src/storage/dynamodb.py
+-rw-r--r--   0        0        0     2830 2024-04-10 19:26:02.732816 rooms_shared_services-0.1.94/rooms_shared_services/src/storage/models.py
+-rw-r--r--   0        0        0     1004 2024-03-16 15:31:07.613112 rooms_shared_services-0.1.94/rooms_shared_services/src/translation/client.py
+-rw-r--r--   0        0        0      252 2024-03-18 21:23:21.407853 rooms_shared_services-0.1.94/rooms_shared_services/src/translation/providers/abstract.py
+-rw-r--r--   0        0        0      713 2024-03-16 15:10:20.760900 rooms_shared_services-0.1.94/rooms_shared_services/src/translation/providers/aws.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 rooms_shared_services-0.1.94/PKG-INFO
```

### Comparing `rooms_shared_services-0.1.93/LICENSE` & `rooms_shared_services-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/pyproject.toml` & `rooms_shared_services-0.1.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 Homepage = "https://github.com/kras55/rooms_shared_services"
 Issues = "https://github.com/kras55/rooms_shared_services/issues"
 
 
 [tool.poetry]
 name = "rooms_shared_services"
-version = "0.1.93"
+version = "0.1.94"
 description = ""
 authors = ["kras55 <dkras5577@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.7"
 pydantic = "^2.5.2"
```

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/abstract.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/abstract.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/models.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/models.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/processor.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/processor.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/sandbox.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/sandbox.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/storage.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/storage.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/delayed_tasks/tracker.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/delayed_tasks/tracker.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/fakers/fake.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/fakers/fake.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/logging/http_logger.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/logging/http_logger.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/main.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/main.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/models/products/categories.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/models/products/categories.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/models/products/products.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/models/products/products.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/models/texts/translations.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/models/texts/translations.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/product_categories/provider.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/product_categories/provider.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/product_categories/source.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/product_categories/source.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/settings/delayed_tasks.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/settings/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_categories/processor.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_categories/processor.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_categories/provider.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_categories/provider.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/sources/product_pricing/processor.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/sources/product_pricing/processor.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/storage/abstract.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/storage/dynamodb.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/storage/dynamodb.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/storage/models.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/storage/models.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/translation/client.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/translation/client.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/rooms_shared_services/src/translation/providers/aws.py` & `rooms_shared_services-0.1.94/rooms_shared_services/src/translation/providers/aws.py`

 * *Files identical despite different names*

### Comparing `rooms_shared_services-0.1.93/PKG-INFO` & `rooms_shared_services-0.1.94/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rooms-shared-services
-Version: 0.1.93
+Version: 0.1.94
 Summary: 
 Author: kras55
 Author-email: dkras5577@gmail.com
 Requires-Python: ==3.11.7
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
```
