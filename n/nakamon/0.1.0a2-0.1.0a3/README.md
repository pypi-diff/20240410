# Comparing `tmp/nakamon-0.1.0a2.tar.gz` & `tmp/nakamon-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakamon-0.1.0a2.tar", max compression
+gzip compressed data, was "nakamon-0.1.0a3.tar", max compression
```

## Comparing `nakamon-0.1.0a2.tar` & `nakamon-0.1.0a3.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a2/README.md
--rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a2/nakamon/__init__.py
--rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a2/nakamon/damage.py
--rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a2/nakamon/nakamon.py
--rw-r--r--   0        0        0      379 2024-04-10 05:37:48.257628 nakamon-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a3/README.md
+-rw-r--r--   0        0        0   445554 2024-04-08 04:27:44.869120 nakamon-0.1.0a3/data/nakamon_status.csv
+-rw-r--r--   0        0        0    13822 2024-04-09 04:15:52.083469 nakamon-0.1.0a3/data/orange_skill.csv
+-rw-r--r--   0        0        0     8449 2024-04-05 00:15:11.226076 nakamon-0.1.0a3/data/red_skill.csv
+-rw-r--r--   0        0        0     4474 2024-04-09 04:11:06.526795 nakamon-0.1.0a3/data/resistance_skill.csv
+-rw-r--r--   0        0        0     5578 2024-04-08 04:44:28.569145 nakamon-0.1.0a3/data/resistance_status.csv
+-rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a3/nakamon/__init__.py
+-rw-r--r--   0        0        0     7560 2024-04-09 05:29:11.103600 nakamon-0.1.0a3/nakamon/damage.py
+-rw-r--r--   0        0        0     5357 2024-04-10 01:49:53.607644 nakamon-0.1.0a3/nakamon/nakamon.py
+-rw-r--r--   0        0        0      404 2024-04-10 05:50:13.207627 nakamon-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a3/PKG-INFO
```

### Comparing `nakamon-0.1.0a2/LICENSE` & `nakamon-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a2/README.md` & `nakamon-0.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a2/nakamon/damage.py` & `nakamon-0.1.0a3/nakamon/damage.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a2/nakamon/nakamon.py` & `nakamon-0.1.0a3/nakamon/nakamon.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a2/PKG-INFO` & `nakamon-0.1.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakamon
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Author: driller
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
```

