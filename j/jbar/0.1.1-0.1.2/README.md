# Comparing `tmp/jbar-0.1.1.tar.gz` & `tmp/jbar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jbar-0.1.1.tar", max compression
+gzip compressed data, was "jbar-0.1.2.tar", max compression
```

## Comparing `jbar-0.1.1.tar` & `jbar-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      513 2024-04-08 23:13:21.269535 jbar-0.1.1/README.md
--rw-r--r--   0        0        0      355 2024-04-08 23:13:37.161445 jbar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2111 2024-04-08 23:08:46.231044 jbar-0.1.1/src/jbar/__init__.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 jbar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-04-08 23:13:56.112256 jbar-0.1.2/README.md
+-rw-r--r--   0        0        0      355 2024-04-10 20:24:13.211794 jbar-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2111 2024-04-08 23:08:46.231044 jbar-0.1.2/src/jbar/__init__.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 jbar-0.1.2/PKG-INFO
```

### Comparing `jbar-0.1.1/README.md` & `jbar-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 Open `example.ipynb` in JupyterLab, VS Code, or your favorite editor
 to start developing. Changes made in `js/` will be reflected
 in the notebook.
 
 ## Publish to PyPI
 
 ```sh
+// Update version in pyproject.toml
 poetry build
 poetry publish
 ```
```

### Comparing `jbar-0.1.1/src/jbar/__init__.py` & `jbar-0.1.2/src/jbar/__init__.py`

 * *Files identical despite different names*

### Comparing `jbar-0.1.1/PKG-INFO` & `jbar-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jbar
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Jakob Troidl
 Author-email: jakob.troidl@googlemail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,11 +38,12 @@
 Open `example.ipynb` in JupyterLab, VS Code, or your favorite editor
 to start developing. Changes made in `js/` will be reflected
 in the notebook.
 
 ## Publish to PyPI
 
 ```sh
+// Update version in pyproject.toml
 poetry build
 poetry publish
 ```
```

