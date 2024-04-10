# Comparing `tmp/kvfile-1.1.1.tar.gz` & `tmp/kvfile-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvfile-1.1.1.tar", last modified: Fri Mar 22 17:09:33 2024, max compression
+gzip compressed data, was "kvfile-1.1.2.tar", last modified: Wed Apr 10 06:20:57 2024, max compression
```

## Comparing `kvfile-1.1.1.tar` & `kvfile-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-03-22 17:09:33.629444 kvfile-1.1.1/
--rw-r--r--   0 adam       (501) staff       (20)     1254 2020-10-11 18:59:21.000000 kvfile-1.1.1/.travis.yml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-03-22 17:09:33.617816 kvfile-1.1.1/.vscode/
--rw-r--r--   0 adam       (501) staff       (20)       89 2024-03-20 13:04:50.000000 kvfile-1.1.1/.vscode/settings.json
--rw-r--r--   0 adam       (501) staff       (20)     1077 2020-10-11 18:59:21.000000 kvfile-1.1.1/LICENSE.md
--rw-r--r--   0 adam       (501) staff       (20)      208 2020-10-11 18:59:21.000000 kvfile-1.1.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      516 2020-10-11 18:59:21.000000 kvfile-1.1.1/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     3874 2024-03-22 17:09:33.629222 kvfile-1.1.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3068 2020-10-11 18:59:21.000000 kvfile-1.1.1/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-03-22 17:09:33.624308 kvfile-1.1.1/kvfile/
--rw-r--r--   0 adam       (501) staff       (20)        6 2024-03-22 17:09:08.000000 kvfile-1.1.1/kvfile/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       60 2024-03-20 10:39:11.000000 kvfile-1.1.1/kvfile/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     3355 2024-03-22 12:46:38.000000 kvfile-1.1.1/kvfile/base.py
--rw-r--r--   0 adam       (501) staff       (20)     2544 2024-03-22 12:55:37.000000 kvfile-1.1.1/kvfile/cached.py
--rw-r--r--   0 adam       (501) staff       (20)      147 2024-03-22 17:09:00.000000 kvfile-1.1.1/kvfile/kvfile.py
--rw-r--r--   0 adam       (501) staff       (20)     1820 2024-03-22 12:55:30.000000 kvfile-1.1.1/kvfile/kvfile_leveldb.py
--rw-r--r--   0 adam       (501) staff       (20)     2976 2024-03-22 12:48:45.000000 kvfile-1.1.1/kvfile/kvfile_sqlite.py
--rw-r--r--   0 adam       (501) staff       (20)      189 2024-03-20 09:29:02.000000 kvfile-1.1.1/kvfile/serializer.py
--rw-r--r--   0 adam       (501) staff       (20)      194 2024-03-20 08:29:38.000000 kvfile-1.1.1/kvfile/serializer_base.py
--rw-r--r--   0 adam       (501) staff       (20)     3042 2024-03-20 08:30:08.000000 kvfile-1.1.1/kvfile/serializer_json.py
--rw-r--r--   0 adam       (501) staff       (20)      261 2024-03-20 10:30:54.000000 kvfile-1.1.1/kvfile/serializer_pickle.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-03-22 17:09:33.628140 kvfile-1.1.1/kvfile.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3874 2024-03-22 17:09:32.000000 kvfile-1.1.1/kvfile.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      532 2024-03-22 17:09:33.000000 kvfile-1.1.1/kvfile.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2024-03-22 17:09:32.000000 kvfile-1.1.1/kvfile.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2020-10-11 19:03:16.000000 kvfile-1.1.1/kvfile.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       59 2024-03-22 17:09:32.000000 kvfile-1.1.1/kvfile.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2024-03-22 17:09:32.000000 kvfile-1.1.1/kvfile.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2024-03-22 17:09:33.630698 kvfile-1.1.1/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1574 2024-01-29 09:43:55.000000 kvfile-1.1.1/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-03-22 17:09:33.627376 kvfile-1.1.1/tests/
--rw-r--r--   0 adam       (501) staff       (20)     4692 2024-03-22 12:54:07.000000 kvfile-1.1.1/tests/test_main.py
--rw-r--r--   0 adam       (501) staff       (20)      408 2020-10-11 18:59:21.000000 kvfile-1.1.1/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-04-10 06:20:57.117061 kvfile-1.1.2/
+-rw-r--r--   0 adam       (501) staff       (20)     1254 2020-10-11 18:59:21.000000 kvfile-1.1.2/.travis.yml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-04-10 06:20:57.100122 kvfile-1.1.2/.vscode/
+-rw-r--r--   0 adam       (501) staff       (20)       89 2024-03-20 13:04:50.000000 kvfile-1.1.2/.vscode/settings.json
+-rw-r--r--   0 adam       (501) staff       (20)     1077 2020-10-11 18:59:21.000000 kvfile-1.1.2/LICENSE.md
+-rw-r--r--   0 adam       (501) staff       (20)      208 2020-10-11 18:59:21.000000 kvfile-1.1.2/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      516 2020-10-11 18:59:21.000000 kvfile-1.1.2/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     3874 2024-04-10 06:20:57.116861 kvfile-1.1.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3068 2020-10-11 18:59:21.000000 kvfile-1.1.2/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-04-10 06:20:57.109540 kvfile-1.1.2/kvfile/
+-rw-r--r--   0 adam       (501) staff       (20)        6 2024-04-10 06:20:30.000000 kvfile-1.1.2/kvfile/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       60 2024-03-20 10:39:11.000000 kvfile-1.1.2/kvfile/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     3355 2024-03-22 12:46:38.000000 kvfile-1.1.2/kvfile/base.py
+-rw-r--r--   0 adam       (501) staff       (20)     2619 2024-04-10 06:20:22.000000 kvfile-1.1.2/kvfile/cached.py
+-rw-r--r--   0 adam       (501) staff       (20)      147 2024-03-22 17:09:00.000000 kvfile-1.1.2/kvfile/kvfile.py
+-rw-r--r--   0 adam       (501) staff       (20)     1820 2024-03-22 12:55:30.000000 kvfile-1.1.2/kvfile/kvfile_leveldb.py
+-rw-r--r--   0 adam       (501) staff       (20)     2976 2024-03-22 12:48:45.000000 kvfile-1.1.2/kvfile/kvfile_sqlite.py
+-rw-r--r--   0 adam       (501) staff       (20)      189 2024-03-20 09:29:02.000000 kvfile-1.1.2/kvfile/serializer.py
+-rw-r--r--   0 adam       (501) staff       (20)      194 2024-03-20 08:29:38.000000 kvfile-1.1.2/kvfile/serializer_base.py
+-rw-r--r--   0 adam       (501) staff       (20)     3042 2024-03-20 08:30:08.000000 kvfile-1.1.2/kvfile/serializer_json.py
+-rw-r--r--   0 adam       (501) staff       (20)      261 2024-03-20 10:30:54.000000 kvfile-1.1.2/kvfile/serializer_pickle.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-04-10 06:20:57.115738 kvfile-1.1.2/kvfile.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3874 2024-04-10 06:20:56.000000 kvfile-1.1.2/kvfile.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      532 2024-04-10 06:20:57.000000 kvfile-1.1.2/kvfile.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2024-04-10 06:20:56.000000 kvfile-1.1.2/kvfile.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2020-10-11 19:03:16.000000 kvfile-1.1.2/kvfile.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       59 2024-04-10 06:20:56.000000 kvfile-1.1.2/kvfile.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2024-04-10 06:20:56.000000 kvfile-1.1.2/kvfile.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2024-04-10 06:20:57.117760 kvfile-1.1.2/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1574 2024-01-29 09:43:55.000000 kvfile-1.1.2/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2024-04-10 06:20:57.114645 kvfile-1.1.2/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     4692 2024-03-22 12:54:07.000000 kvfile-1.1.2/tests/test_main.py
+-rw-r--r--   0 adam       (501) staff       (20)      408 2020-10-11 18:59:21.000000 kvfile-1.1.2/tox.ini
```

### Comparing `kvfile-1.1.1/.travis.yml` & `kvfile-1.1.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/LICENSE.md` & `kvfile-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/Makefile` & `kvfile-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/PKG-INFO` & `kvfile-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvfile
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple File-based KV-Store
 Home-page: https://github.com/akariv/kvstore
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kvfile-1.1.1/README.md` & `kvfile-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/kvfile/base.py` & `kvfile-1.1.2/kvfile/base.py`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/kvfile/cached.py` & `kvfile-1.1.2/kvfile/cached.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,23 +63,25 @@
             return self.db()._keys()
         return sorted(self.cache.keys(), reverse=reverse)
 
     def _close_db(self):
         if self._db is not None:
             self.flush()
             self.db()._close_db()
+            self._db = None
 
     def items(self, reverse=False):
         if self._db is not None:
             self.flush()
             yield from self.db().items(reverse)
         else:
             for key in self.keys(reverse):
                 yield key, self.get(key)
 
     def flush(self):
-        self.db()._set_db_batch(
-            (k, v)
-            for k, v in self.cache.items()
-            if k in self.dirty
-        )
-        self.dirty.clear()
+        if self.dirty:
+            self.db()._set_db_batch(
+                (k, v)
+                for k, v in self.cache.items()
+                if k in self.dirty
+            )
+            self.dirty.clear()
```

### Comparing `kvfile-1.1.1/kvfile/kvfile_leveldb.py` & `kvfile-1.1.2/kvfile/kvfile_leveldb.py`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/kvfile/kvfile_sqlite.py` & `kvfile-1.1.2/kvfile/kvfile_sqlite.py`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/kvfile/serializer_json.py` & `kvfile-1.1.2/kvfile/serializer_json.py`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/kvfile.egg-info/PKG-INFO` & `kvfile-1.1.2/kvfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvfile
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple File-based KV-Store
 Home-page: https://github.com/akariv/kvstore
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kvfile-1.1.1/kvfile.egg-info/SOURCES.txt` & `kvfile-1.1.2/kvfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/setup.py` & `kvfile-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `kvfile-1.1.1/tests/test_main.py` & `kvfile-1.1.2/tests/test_main.py`

 * *Files identical despite different names*

