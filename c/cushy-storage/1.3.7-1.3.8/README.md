# Comparing `tmp/cushy_storage-1.3.7.tar.gz` & `tmp/cushy_storage-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cushy_storage-1.3.7.tar", max compression
+gzip compressed data, was "cushy_storage-1.3.8.tar", max compression
```

## Comparing `cushy_storage-1.3.7.tar` & `cushy_storage-1.3.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/LICENSE
--rw-r--r--   0        0        0     3244 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/README.md
--rw-r--r--   0        0        0      961 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/__init__.py
--rw-r--r--   0        0        0     8467 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/_core.py
--rw-r--r--   0        0        0     1287 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/base.py
--rw-r--r--   0        0        0     8825 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/orm.py
--rw-r--r--   0        0        0     2203 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/utils/__init__.py
--rw-r--r--   0        0        0     2897 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/utils/logger.py
--rw-r--r--   0        0        0     1311 2024-01-01 22:09:06.015180 cushy_storage-1.3.7/cushy_storage/utils/singleton.py
--rw-r--r--   0        0        0     1840 2024-01-01 22:09:06.019180 cushy_storage-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 cushy_storage-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/LICENSE
+-rw-r--r--   0        0        0     3244 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/README.md
+-rw-r--r--   0        0        0      961 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/__init__.py
+-rw-r--r--   0        0        0     8467 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/_core.py
+-rw-r--r--   0        0        0     1287 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/base.py
+-rw-r--r--   0        0        0     8825 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/orm.py
+-rw-r--r--   0        0        0     2203 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/utils/__init__.py
+-rw-r--r--   0        0        0     2897 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/utils/logger.py
+-rw-r--r--   0        0        0     1311 2024-04-10 11:26:45.466996 cushy_storage-1.3.8/cushy_storage/utils/singleton.py
+-rw-r--r--   0        0        0     1822 2024-04-10 11:26:45.470996 cushy_storage-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 cushy_storage-1.3.8/PKG-INFO
```

### Comparing `cushy_storage-1.3.7/LICENSE` & `cushy_storage-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/README.md` & `cushy_storage-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/__init__.py` & `cushy_storage-1.3.8/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/_core.py` & `cushy_storage-1.3.8/cushy_storage/_core.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/base.py` & `cushy_storage-1.3.8/cushy_storage/base.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/orm.py` & `cushy_storage-1.3.8/cushy_storage/orm.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/utils/__init__.py` & `cushy_storage-1.3.8/cushy_storage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/utils/logger.py` & `cushy_storage-1.3.8/cushy_storage/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/cushy_storage/utils/singleton.py` & `cushy_storage-1.3.8/cushy_storage/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cushy_storage-1.3.7/pyproject.toml` & `cushy_storage-1.3.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 
 [tool.poetry]
 authors = ["Zeeland <zeeland4work@gmail.com>"]
 description = "A data local persistence ORM framework."
 name = "cushy-storage"
 readme = "README.md"
 repository = "https://github.com/Undertone0809/cushy-storage"
-version = "1.3.7"
+version = "1.3.8"
 keywords = [
     "storage",
     "ORM",
     "serialization",
     "json",
     "cushy-storage",
     "cushy_storage",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-loguru = "^0.7.2"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pre-commit = "^3.5.0"
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
```

### Comparing `cushy_storage-1.3.7/PKG-INFO` & `cushy_storage-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.3.7
+Version: 1.3.8
 Summary: A data local persistence ORM framework.
 Home-page: https://github.com/Undertone0809/cushy-storage
 Keywords: storage,ORM,serialization,json,cushy-storage,cushy_storage
 Author: Zeeland
 Author-email: zeeland4work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Project-URL: Repository, https://github.com/Undertone0809/cushy-storage
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     cushy-storage
 </h1>
 <p align="center">
```

