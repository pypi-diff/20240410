# Comparing `tmp/testsolar-testtool-sdk-0.1.4.tar.gz` & `tmp/testsolar-testtool-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testsolar-testtool-sdk-0.1.4.tar", last modified: Wed Apr 10 06:21:57 2024, max compression
+gzip compressed data, was "testsolar-testtool-sdk-0.1.5.tar", last modified: Wed Apr 10 08:21:45 2024, max compression
```

## Comparing `testsolar-testtool-sdk-0.1.4.tar` & `testsolar-testtool-sdk-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.439765 testsolar-testtool-sdk-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.439765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/testresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/pipe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 06:21:57.000000 testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:21:57.443765 testsolar-testtool-sdk-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-10 06:21:23.000000 testsolar-testtool-sdk-0.1.4/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.790774 testsolar-testtool-sdk-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.790774 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/pipe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 08:21:45.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 08:21:45.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:21:45.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 08:21:45.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 08:21:45.000000 testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:21:45.794774 testsolar-testtool-sdk-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-10 08:21:20.000000 testsolar-testtool-sdk-0.1.5/tests/test_report.py
```

### Comparing `testsolar-testtool-sdk-0.1.4/LICENSE` & `testsolar-testtool-sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/model/testresult.py` & `testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/model/testresult.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/pipe_reader.py` & `testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/pipe_reader.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk/reporter.py` & `testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk/reporter.py`

 * *Files identical despite different names*

### Comparing `testsolar-testtool-sdk-0.1.4/src/testsolar_testtool_sdk.egg-info/SOURCES.txt` & `testsolar-testtool-sdk-0.1.5/src/testsolar_testtool_sdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 src/testsolar_testtool_sdk/__init__.py
 src/testsolar_testtool_sdk/pipe_reader.py
+src/testsolar_testtool_sdk/py.typed
 src/testsolar_testtool_sdk/reporter.py
 src/testsolar_testtool_sdk.egg-info/PKG-INFO
 src/testsolar_testtool_sdk.egg-info/SOURCES.txt
 src/testsolar_testtool_sdk.egg-info/dependency_links.txt
 src/testsolar_testtool_sdk.egg-info/requires.txt
 src/testsolar_testtool_sdk.egg-info/top_level.txt
 src/testsolar_testtool_sdk/model/__init__.py
```

### Comparing `testsolar-testtool-sdk-0.1.4/tests/test_report.py` & `testsolar-testtool-sdk-0.1.5/tests/test_report.py`

 * *Files identical despite different names*

