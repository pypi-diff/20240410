# Comparing `tmp/dtaas_cli-0.1.1.tar.gz` & `tmp/dtaas_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtaas_cli-0.1.1.tar", max compression
+gzip compressed data, was "dtaas_cli-0.1.2.tar", max compression
```

## Comparing `dtaas_cli-0.1.1.tar` & `dtaas_cli-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,8 @@
--rw-r--r--   0        0        0        0 2024-03-24 11:06:51.522935 dtaas_cli-0.1.1/README.md
--rw-r--r--   0        0        0      423 2024-04-07 08:44:38.694859 dtaas_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 06:33:13.786621 dtaas_cli-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     1231 2024-03-27 14:51:32.151684 dtaas_cli-0.1.1/src/cmd.py
--rw-r--r--   0        0        0     2938 2024-03-31 07:34:48.599674 dtaas_cli-0.1.1/src/pkg/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     2938 2024-03-24 13:03:05.962470 dtaas_cli-0.1.1/src/pkg/__pycache__/dtaas.cpython-310.pyc
--rw-r--r--   0        0        0     2692 2024-04-07 06:44:24.513176 dtaas_cli-0.1.1/src/pkg/__pycache__/users.cpython-310.pyc
--rw-r--r--   0        0        0     2205 2024-03-31 06:42:47.839095 dtaas_cli-0.1.1/src/pkg/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     2888 2024-03-31 07:23:34.069695 dtaas_cli-0.1.1/src/pkg/config.py
--rw-r--r--   0        0        0     3718 2024-04-07 06:42:56.575522 dtaas_cli-0.1.1/src/pkg/users.py
--rw-r--r--   0        0        0     2161 2024-03-31 06:41:10.590813 dtaas_cli-0.1.1/src/pkg/utils.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 dtaas_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-24 11:06:51.522935 dtaas_cli-0.1.2/README.md
+-rw-r--r--   0        0        0      423 2024-04-10 16:30:28.567515 dtaas_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 06:33:13.786621 dtaas_cli-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0     1231 2024-03-27 14:51:32.151684 dtaas_cli-0.1.2/src/cmd.py
+-rw-r--r--   0        0        0     2888 2024-03-31 07:23:34.069695 dtaas_cli-0.1.2/src/pkg/config.py
+-rw-r--r--   0        0        0     3922 2024-04-10 16:19:14.359580 dtaas_cli-0.1.2/src/pkg/users.py
+-rw-r--r--   0        0        0     2227 2024-04-10 16:02:20.456118 dtaas_cli-0.1.2/src/pkg/utils.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 dtaas_cli-0.1.2/PKG-INFO
```

### Comparing `dtaas_cli-0.1.1/src/cmd.py` & `dtaas_cli-0.1.2/src/cmd.py`

 * *Files identical despite different names*

### Comparing `dtaas_cli-0.1.1/src/pkg/config.py` & `dtaas_cli-0.1.2/src/pkg/config.py`

 * *Files identical despite different names*

### Comparing `dtaas_cli-0.1.1/src/pkg/utils.py` & `dtaas_cli-0.1.2/src/pkg/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,7 +61,11 @@
             obj[key], err = replaceAll(obj[key], mapping)
             if err is not None:
                 return None, err
 
         return obj, None
 
     return None, Exception("Config substition failed: Object format not valid")
+
+def checkError(err):
+    if err is not None:
+        raise err
```

### Comparing `dtaas_cli-0.1.1/PKG-INFO` & `dtaas_cli-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtaas-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: DTaaS CLI
 License: INTO-CPS-Association
 Author: Astitva Sehgal
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

