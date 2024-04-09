# Comparing `tmp/poetry_kit-0.1.2.tar.gz` & `tmp/poetry_kit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_kit-0.1.2.tar", max compression
+gzip compressed data, was "poetry_kit-0.1.3.tar", max compression
```

## Comparing `poetry_kit-0.1.2.tar` & `poetry_kit-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rwxr-xr-x   0        0        0        0 2024-04-09 22:15:31.542678 poetry_kit-0.1.2/poetry_kit/__init__.py
--rwxr-xr-x   0        0        0      251 2024-04-09 23:04:57.662607 poetry_kit-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0      314 2024-04-09 23:04:48.126709 poetry_kit-0.1.2/readme.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 poetry_kit-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2024-04-09 22:15:31.542678 poetry_kit-0.1.3/poetry_kit/__init__.py
+-rwxr-xr-x   0        0        0      254 2024-04-09 23:05:20.678362 poetry_kit-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0      314 2024-04-09 23:04:48.126709 poetry_kit-0.1.3/readme.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 poetry_kit-0.1.3/PKG-INFO
```

### Comparing `poetry_kit-0.1.2/PKG-INFO` & `poetry_kit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-kit
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: volts (>=1.0.9,<2.0.0)
```

