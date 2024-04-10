# Comparing `tmp/asyncio-foundationdb-0.9.4.tar.gz` & `tmp/asyncio-foundationdb-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-foundationdb-0.9.4.tar", max compression
+gzip compressed data, was "asyncio-foundationdb-0.9.5.tar", max compression
```

## Comparing `asyncio-foundationdb-0.9.4.tar` & `asyncio-foundationdb-0.9.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.4/LICENSE
--rw-r--r--   0        0        0      675 2021-07-05 18:10:59.492638 asyncio-foundationdb-0.9.4/README.md
--rw-r--r--   0        0        0      394 2021-07-05 17:45:35.204263 asyncio-foundationdb-0.9.4/build.py
--rw-r--r--   0        0        0    37523 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.4/fdb_c.h
--rw-r--r--   0        0        0    37452 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.4/fdb_c2.h
--rw-r--r--   0        0        0     3207 2021-07-05 17:20:15.955837 asyncio-foundationdb-0.9.4/found/__init__.py
--rwxr-xr-x   0        0        0   190304 2021-07-05 18:12:07.418339 asyncio-foundationdb-0.9.4/found/_fdb.cpython-39-x86_64-linux-gnu.so
--rw-r--r--   0        0        0    17943 2021-07-05 18:09:20.967972 asyncio-foundationdb-0.9.4/found/base.py
--rw-r--r--   0        0        0     6799 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.4/found/nstore.py
--rw-r--r--   0        0        0      687 2021-07-05 20:54:18.769926 asyncio-foundationdb-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1448 2021-07-05 20:54:29.345844 asyncio-foundationdb-0.9.4/setup.py
--rw-r--r--   0        0        0     1330 2021-07-05 20:54:29.346096 asyncio-foundationdb-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.5/LICENSE
+-rw-r--r--   0        0        0      675 2021-07-05 18:10:59.492638 asyncio-foundationdb-0.9.5/README.md
+-rw-r--r--   0        0        0      394 2021-07-05 17:45:35.204263 asyncio-foundationdb-0.9.5/build.py
+-rw-r--r--   0        0        0    37523 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.5/fdb_c.h
+-rw-r--r--   0        0        0    37452 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.5/fdb_c2.h
+-rw-r--r--   0        0        0     3207 2021-07-05 17:20:15.955837 asyncio-foundationdb-0.9.5/found/__init__.py
+-rwxr-xr-x   0        0        0   190304 2021-07-05 20:55:27.515825 asyncio-foundationdb-0.9.5/found/_fdb.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0    17943 2021-07-05 18:09:20.967972 asyncio-foundationdb-0.9.5/found/base.py
+-rw-r--r--   0        0        0     6799 2021-07-05 17:09:27.853901 asyncio-foundationdb-0.9.5/found/nstore.py
+-rw-r--r--   0        0        0      687 2021-07-05 20:55:42.607365 asyncio-foundationdb-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1448 2021-07-05 20:55:45.561706 asyncio-foundationdb-0.9.5/setup.py
+-rw-r--r--   0        0        0     1330 2021-07-05 20:55:45.561959 asyncio-foundationdb-0.9.5/PKG-INFO
```

### Comparing `asyncio-foundationdb-0.9.4/LICENSE` & `asyncio-foundationdb-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/README.md` & `asyncio-foundationdb-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/fdb_c.h` & `asyncio-foundationdb-0.9.5/fdb_c.h`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/fdb_c2.h` & `asyncio-foundationdb-0.9.5/fdb_c2.h`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/found/__init__.py` & `asyncio-foundationdb-0.9.5/found/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/found/_fdb.cpython-39-x86_64-linux-gnu.so` & `asyncio-foundationdb-0.9.5/found/_fdb.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/found/base.py` & `asyncio-foundationdb-0.9.5/found/base.py`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/found/nstore.py` & `asyncio-foundationdb-0.9.5/found/nstore.py`

 * *Files identical despite different names*

### Comparing `asyncio-foundationdb-0.9.4/pyproject.toml` & `asyncio-foundationdb-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncio-foundationdb"
-version = "0.9.4"
+version = "0.9.5"
 description = "asyncio drivers for FoundationDB"
 authors = ["Amirouche <amirouche@hyper.dev>"]
 license = "Apachev2"
 readme = "README.md"
 packages = [
     { include = "found" },
 ]
```

### Comparing `asyncio-foundationdb-0.9.4/setup.py` & `asyncio-foundationdb-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cffi>=1.14.5,<2.0.0',
  'foundationdb>=6.3.16,<7.0.0',
  'immutables>=0.15,<0.16',
  'six>=1.16.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'asyncio-foundationdb',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'asyncio drivers for FoundationDB',
     'long_description': "# [asyncio-foundationdb](https://github.com/amirouche/asyncio-foundationdb/)\n\n*early draft*\n\nasyncio drivers for foundationdb tested with CPython 3.9\n\n```\npip install asyncio-foundationdb\n```\n\n```python\n> import found\n> found.api_version(630)\n> db = await found.open()\n> await db.get(b'hello')\n> await db.set(b'hello', b'world')\n> await tr.get(b'hello')\nb'world'\n```\n\n## ChangeLog\n\n### v0.9.x\n\n- feature: bump to foundationdb 6.3.15 client API\n- feature: add hooks and states\n\n### v0.8.0\n\n- breaking change: replace ``get_rangefoo`` with ``rangefoo`` as async generator\n- new: add short syntax for querying `Nstore.query(tr, patterns)`\n- chore: remove pipenv, and pre-commit\n",
     'author': 'Amirouche',
     'author_email': 'amirouche@hyper.dev',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `asyncio-foundationdb-0.9.4/PKG-INFO` & `asyncio-foundationdb-0.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-foundationdb
-Version: 0.9.4
+Version: 0.9.5
 Summary: asyncio drivers for FoundationDB
 License: Apachev2
 Author: Amirouche
 Author-email: amirouche@hyper.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

