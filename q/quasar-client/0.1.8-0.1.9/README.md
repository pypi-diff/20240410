# Comparing `tmp/quasar_client-0.1.8.tar.gz` & `tmp/quasar_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quasar_client-0.1.8.tar", max compression
+gzip compressed data, was "quasar_client-0.1.9.tar", max compression
```

## Comparing `quasar_client-0.1.8.tar` & `quasar_client-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11353 2024-03-03 06:55:56.854539 quasar_client-0.1.8/LICENSE
--rw-r--r--   0        0        0     2302 2024-03-03 06:55:56.854539 quasar_client-0.1.8/README.md
--rw-r--r--   0        0        0      380 2024-03-03 06:55:56.854539 quasar_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       90 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/__init__.py
--rw-r--r--   0        0        0     5074 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/client.py
--rw-r--r--   0        0        0      337 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/classify.py
--rw-r--r--   0        0        0      211 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/embed.py
--rw-r--r--   0        0        0      369 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/extract.py
--rw-r--r--   0        0        0      221 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/models.py
--rw-r--r--   0        0        0      210 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/rank.py
--rw-r--r--   0        0        0      209 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/dataclasses/tag.py
--rw-r--r--   0        0        0      969 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/base.py
--rw-r--r--   0        0        0     2402 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/classifier.py
--rw-r--r--   0        0        0     1569 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/embed.py
--rw-r--r--   0        0        0     2048 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/extract.py
--rw-r--r--   0        0        0     1547 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/rank.py
--rw-r--r--   0        0        0     1846 2024-03-03 06:55:56.854539 quasar_client-0.1.8/quasar_client/resources/tagger.py
--rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 quasar_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11353 2024-03-06 08:31:50.033962 quasar_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2302 2024-03-06 08:31:50.033962 quasar_client-0.1.9/README.md
+-rw-r--r--   0        0        0      380 2024-03-06 08:31:50.033962 quasar_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-03-06 08:31:50.033962 quasar_client-0.1.9/quasar_client/__init__.py
+-rw-r--r--   0        0        0     5074 2024-03-06 08:31:50.033962 quasar_client-0.1.9/quasar_client/client.py
+-rw-r--r--   0        0        0      337 2024-03-06 08:31:50.033962 quasar_client-0.1.9/quasar_client/dataclasses/classify.py
+-rw-r--r--   0        0        0      211 2024-03-06 08:31:50.033962 quasar_client-0.1.9/quasar_client/dataclasses/embed.py
+-rw-r--r--   0        0        0      369 2024-03-06 08:31:50.033962 quasar_client-0.1.9/quasar_client/dataclasses/extract.py
+-rw-r--r--   0        0        0      221 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/dataclasses/models.py
+-rw-r--r--   0        0        0      210 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/dataclasses/rank.py
+-rw-r--r--   0        0        0      209 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/dataclasses/tag.py
+-rw-r--r--   0        0        0      969 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/base.py
+-rw-r--r--   0        0        0     2402 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/classifier.py
+-rw-r--r--   0        0        0     1904 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/embed.py
+-rw-r--r--   0        0        0     2048 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/extract.py
+-rw-r--r--   0        0        0     1547 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/rank.py
+-rw-r--r--   0        0        0     1846 2024-03-06 08:31:50.037962 quasar_client-0.1.9/quasar_client/resources/tagger.py
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 quasar_client-0.1.9/PKG-INFO
```

### Comparing `quasar_client-0.1.8/LICENSE` & `quasar_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/README.md` & `quasar_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/client.py` & `quasar_client-0.1.9/quasar_client/client.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/resources/base.py` & `quasar_client-0.1.9/quasar_client/resources/base.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/resources/classifier.py` & `quasar_client-0.1.9/quasar_client/resources/classifier.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/resources/extract.py` & `quasar_client-0.1.9/quasar_client/resources/extract.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/resources/rank.py` & `quasar_client-0.1.9/quasar_client/resources/rank.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/quasar_client/resources/tagger.py` & `quasar_client-0.1.9/quasar_client/resources/tagger.py`

 * *Files identical despite different names*

### Comparing `quasar_client-0.1.8/PKG-INFO` & `quasar_client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quasar-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Yurts Python Quasar Client
 Author: Yurts Technologies, Inc.
 Author-email: dev@yurts.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

