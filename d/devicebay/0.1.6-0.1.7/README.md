# Comparing `tmp/devicebay-0.1.6.tar.gz` & `tmp/devicebay-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devicebay-0.1.6.tar", max compression
+gzip compressed data, was "devicebay-0.1.7.tar", max compression
```

## Comparing `devicebay-0.1.6.tar` & `devicebay-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.6/LICENSE
--rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.6/README.md
--rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.6/devicebay/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-09 21:33:50.707870 devicebay-0.1.6/devicebay/base.py
--rw-r--r--   0        0        0       99 2024-04-09 21:42:18.657362 devicebay-0.1.6/devicebay/models.py
--rw-r--r--   0        0        0      342 2024-04-09 21:42:26.034502 devicebay-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 02:39:38.878817 devicebay-0.1.7/LICENSE
+-rw-r--r--   0        0        0       35 2024-04-09 02:39:38.878906 devicebay-0.1.7/README.md
+-rw-r--r--   0        0        0       89 2024-04-09 17:05:39.050602 devicebay-0.1.7/devicebay/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-09 22:04:05.303203 devicebay-0.1.7/devicebay/base.py
+-rw-r--r--   0        0        0       99 2024-04-09 21:42:18.657362 devicebay-0.1.7/devicebay/models.py
+-rw-r--r--   0        0        0      342 2024-04-09 22:05:35.555794 devicebay-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 devicebay-0.1.7/PKG-INFO
```

### Comparing `devicebay-0.1.6/LICENSE` & `devicebay-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `devicebay-0.1.6/devicebay/base.py` & `devicebay-0.1.7/devicebay/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
     @abstractmethod
     def view(self, background: bool = False) -> None:
         pass
 
     @classmethod
     @abstractmethod
-    def config(cls) -> Type[C]:
+    def config_type(cls) -> Type[C]:
         pass
 
     @classmethod
     @abstractmethod
-    def provision_config(cls) -> Type[P]:
+    def provision_config_type(cls) -> Type[P]:
         pass
 
     @classmethod
     def serve(cls) -> None:
         pass
```

### Comparing `devicebay-0.1.6/PKG-INFO` & `devicebay-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devicebay
-Version: 0.1.6
+Version: 0.1.7
 Summary: Devices for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

