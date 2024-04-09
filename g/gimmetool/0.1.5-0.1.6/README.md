# Comparing `tmp/gimmetool-0.1.5.tar.gz` & `tmp/gimmetool-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimmetool-0.1.5.tar", max compression
+gzip compressed data, was "gimmetool-0.1.6.tar", max compression
```

## Comparing `gimmetool-0.1.5.tar` & `gimmetool-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.5/README.md
--rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.5/gimmetool/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.5/gimmetool/gimme.py
--rwxr-xr-x   0        0        0      616 2024-04-09 22:33:40.953646 gimmetool-0.1.5/gimmetool/gimme.sh
--rwxr-xr-x   0        0        0    24806 2024-04-09 22:38:16.183338 gimmetool-0.1.5/gimmetool/gimmetool.py
--rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.5/gimmetool/setup.py
--rwxr-xr-x   0        0        0      405 2024-04-09 22:37:34.604834 gimmetool-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 gimmetool-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.6/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.6/gimmetool/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.6/gimmetool/gimme.py
+-rwxr-xr-x   0        0        0      616 2024-04-09 22:33:40.953646 gimmetool-0.1.6/gimmetool/gimme.sh
+-rwxr-xr-x   0        0        0    24806 2024-04-09 22:38:16.183338 gimmetool-0.1.6/gimmetool/gimmetool.py
+-rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.6/gimmetool/setup.py
+-rwxr-xr-x   0        0        0      428 2024-04-09 22:45:15.741872 gimmetool-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 gimmetool-0.1.6/PKG-INFO
```

### Comparing `gimmetool-0.1.5/README.md` & `gimmetool-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.5/gimmetool/gimme.sh` & `gimmetool-0.1.6/gimmetool/gimme.sh`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.5/gimmetool/gimmetool.py` & `gimmetool-0.1.6/gimmetool/gimmetool.py`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.5/gimmetool/setup.py` & `gimmetool-0.1.6/gimmetool/setup.py`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.5/PKG-INFO` & `gimmetool-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: gimmetool
-Version: 0.1.5
+Version: 0.1.6
 Summary: The multi-repo manager
 Author: Jeff
 Author-email: jhilton@qualtrics.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
+Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Gimme: The Multi-Repo Manager
 
 This is a utility designed to help developers quickly hop between and manage the many repositories they keep on their workstations.
```

