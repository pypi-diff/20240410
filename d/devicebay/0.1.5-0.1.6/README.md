# Comparing `tmp/devicebay-0.1.5.tar.gz` & `tmp/devicebay-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.5.tar", max compression
+gzip compressed data, was "devicebay-0.1.6.tar", max compression
```

## Comparing `devicebay-0.1.5.tar` & `devicebay-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.5/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.5/README.md
--rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.5/devicebay/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-09 21:33:50.707870 devicebay-0.1.5/devicebay/base.py
--rw-r--r--   0        0        0      342 2024-04-09 21:33:55.210237 devicebay-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.6/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.6/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.6/devicebay/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-09 21:33:50.707870 devicebay-0.1.6/devicebay/base.py
+-rw-r--r--   0        0        0       99 2024-04-09 21:42:18.657362 devicebay-0.1.6/devicebay/models.py
+-rw-r--r--   0        0        0      342 2024-04-09 21:42:26.034502 devicebay-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.6/PKG-INFO
```

### Comparing `devicebay-0.1.5/LICENSE` & `devicebay-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.5/devicebay/base.py` & `devicebay-0.1.6/devicebay/base.py`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.5/PKG-INFO` & `devicebay-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.5
+Version: 0.1.6
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

