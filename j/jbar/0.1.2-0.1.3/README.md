# Comparing `tmp/jbar-0.1.2.tar.gz` & `tmp/jbar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jbar-0.1.2.tar", max compression
+gzip compressed data, was "jbar-0.1.3.tar", max compression
```

## Comparing `jbar-0.1.2.tar` & `jbar-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      549 2024-04-08 23:13:56.112256 jbar-0.1.2/README.md
--rw-r--r--   0        0        0      355 2024-04-10 20:24:13.211794 jbar-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2111 2024-04-08 23:08:46.231044 jbar-0.1.2/src/jbar/__init__.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 jbar-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-04-08 23:13:56.112256 jbar-0.1.3/README.md
+-rw-r--r--   0        0        0     2113 2024-04-10 20:33:39.389583 jbar-0.1.3/jbar/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-10 20:35:12.818401 jbar-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 jbar-0.1.3/PKG-INFO
```

### Comparing `jbar-0.1.2/README.md` & `jbar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jbar-0.1.2/src/jbar/__init__.py` & `jbar-0.1.3/jbar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 try:
     __version__ = importlib.metadata.version("jbar")
 except importlib.metadata.PackageNotFoundError:
     __version__ = "unknown"
 
 class BarChart(anywidget.AnyWidget):
     _esm = pathlib.Path(__file__).parent / "static" / "widget.js"
-    _css = pathlib.Path(__file__).parent / "static" / "widget.css"
+    # _css = pathlib.Path(__file__).parent / "static" / "widget.css"
     data = traitlets.Unicode().tag(sync=True)
     x = traitlets.Unicode().tag(sync=True)
     exclude = traitlets.List().tag(sync=True)
     selection = traitlets.Int().tag(sync=True)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `jbar-0.1.2/PKG-INFO` & `jbar-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jbar
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Jakob Troidl
 Author-email: jakob.troidl@googlemail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

