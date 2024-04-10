# Comparing `tmp/uvx-0.9.2.tar.gz` & `tmp/uvx-0.9.3.tar.gz`

## Comparing `uvx-0.9.2.tar` & `uvx-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 uvx-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/_cli_support.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/_constants.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/_maybe.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/_symlinks.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/cli.py
--rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/core.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.9.2/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.9.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.9.2/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.9.2/README.md
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 uvx-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 uvx-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 uvx-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/_cli_support.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/_constants.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/_maybe.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/_python.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/_symlinks.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/cli.py
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/core.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.9.3/src/uvx/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.9.3/LICENSE.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.9.3/README.md
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 uvx-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 uvx-0.9.3/PKG-INFO
```

### Comparing `uvx-0.9.2/CHANGELOG.md` & `uvx-0.9.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.9.3 (2024-04-10)
+
+
+
 ## v0.9.2 (2024-04-10)
 
 ### Fix
 
 * **self-update:** Proper order of old and new + disable caching for self update ([`27298eb`](https://github.com/robinvandernoord/uvx/commit/27298ebfee768c163b6b63db84bd0e5af1fb4f4b))
 
 ## v0.9.1 (2024-04-10)
```

### Comparing `uvx-0.9.2/src/uvx/_python.py` & `uvx-0.9.3/src/uvx/_python.py`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/src/uvx/_symlinks.py` & `uvx-0.9.3/src/uvx/_symlinks.py`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/src/uvx/cli.py` & `uvx-0.9.3/src/uvx/cli.py`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/src/uvx/core.py` & `uvx-0.9.3/src/uvx/core.py`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/src/uvx/metadata.py` & `uvx-0.9.3/src/uvx/metadata.py`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/LICENSE.txt` & `uvx-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/README.md` & `uvx-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/pyproject.toml` & `uvx-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-0.9.2/PKG-INFO` & `uvx-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvx
-Version: 0.9.2
+Version: 0.9.3
 Summary: uvx: pipx for uv
 Project-URL: Documentation, https://github.com/robinvandernoord/uvx#readme
 Project-URL: Issues, https://github.com/robinvandernoord/uvx/issues
 Project-URL: Source, https://github.com/robinvandernoord/uvx
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

