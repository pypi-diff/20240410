# Comparing `tmp/jbar-0.1.3.tar.gz` & `tmp/jbar-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jbar-0.1.3.tar", max compression
+gzip compressed data, was "jbar-0.1.4.tar", max compression
```

## Comparing `jbar-0.1.3.tar` & `jbar-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      549 2024-04-08 23:13:56.112256 jbar-0.1.3/README.md
--rw-r--r--   0        0        0     2113 2024-04-10 20:33:39.389583 jbar-0.1.3/jbar/__init__.py
--rw-r--r--   0        0        0      393 2024-04-10 20:35:12.818401 jbar-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 jbar-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-04-08 23:13:56.112256 jbar-0.1.4/README.md
+-rw-r--r--   0        0        0     2113 2024-04-10 20:33:39.389583 jbar-0.1.4/jbar/__init__.py
+-rw-r--r--   0        0        0      354 2024-04-10 20:42:48.966327 jbar-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 jbar-0.1.4/PKG-INFO
```

### Comparing `jbar-0.1.3/README.md` & `jbar-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jbar-0.1.3/jbar/__init__.py` & `jbar-0.1.4/jbar/__init__.py`

 * *Files identical despite different names*

### Comparing `jbar-0.1.3/PKG-INFO` & `jbar-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jbar
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Jakob Troidl
 Author-email: jakob.troidl@googlemail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

