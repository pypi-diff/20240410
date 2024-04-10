# Comparing `tmp/nakamon-0.1.0a1.tar.gz` & `tmp/nakamon-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakamon-0.1.0a1.tar", max compression
+gzip compressed data, was "nakamon-0.1.0a2.tar", max compression
```

## Comparing `nakamon-0.1.0a1.tar` & `nakamon-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a1/README.md
--rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a1/nakamon/__init__.py
--rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a1/nakamon/damage.py
--rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a1/nakamon/nakamon.py
--rw-r--r--   0        0        0      379 2024-04-10 04:56:03.077632 nakamon-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 nakamon-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a2/README.md
+-rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a2/nakamon/__init__.py
+-rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a2/nakamon/damage.py
+-rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a2/nakamon/nakamon.py
+-rw-r--r--   0        0        0      379 2024-04-10 05:37:48.257628 nakamon-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a2/PKG-INFO
```

### Comparing `nakamon-0.1.0a1/LICENSE` & `nakamon-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a1/README.md` & `nakamon-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a1/nakamon/damage.py` & `nakamon-0.1.0a2/nakamon/damage.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a1/nakamon/nakamon.py` & `nakamon-0.1.0a2/nakamon/nakamon.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a1/PKG-INFO` & `nakamon-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: nakamon
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: 
 Author: driller
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # なかモンダメージシミュレータ
 
 ## インストール
 
 ```
```

