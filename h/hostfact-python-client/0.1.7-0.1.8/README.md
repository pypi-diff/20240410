# Comparing `tmp/hostfact_python_client-0.1.7.tar.gz` & `tmp/hostfact_python_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostfact_python_client-0.1.7.tar", max compression
+gzip compressed data, was "hostfact_python_client-0.1.8.tar", max compression
```

## Comparing `hostfact_python_client-0.1.7.tar` & `hostfact_python_client-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2021-06-18 14:58:33.930562 hostfact_python_client-0.1.7/hostfact_python_client/__init__.py
--rw-r--r--   0        0        0     4298 2023-08-23 05:10:12.695610 hostfact_python_client-0.1.7/hostfact_python_client/hostfact_client.py
--rw-r--r--   0        0        0     1131 2021-06-18 14:58:33.930784 hostfact_python_client-0.1.7/hostfact_python_client/utilities.py
--rw-r--r--   0        0        0      431 2023-08-23 05:15:00.612043 hostfact_python_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 hostfact_python_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-06-18 14:58:33.930562 hostfact_python_client-0.1.8/hostfact_python_client/__init__.py
+-rw-r--r--   0        0        0     4298 2024-04-09 22:27:42.193798 hostfact_python_client-0.1.8/hostfact_python_client/hostfact_client.py
+-rw-r--r--   0        0        0     1131 2021-06-18 14:58:33.930784 hostfact_python_client-0.1.8/hostfact_python_client/utilities.py
+-rw-r--r--   0        0        0      431 2024-04-09 22:29:35.044910 hostfact_python_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 hostfact_python_client-0.1.8/PKG-INFO
```

### Comparing `hostfact_python_client-0.1.7/hostfact_python_client/hostfact_client.py` & `hostfact_python_client-0.1.8/hostfact_python_client/hostfact_client.py`

 * *Files identical despite different names*

### Comparing `hostfact_python_client-0.1.7/hostfact_python_client/utilities.py` & `hostfact_python_client-0.1.8/hostfact_python_client/utilities.py`

 * *Files identical despite different names*

