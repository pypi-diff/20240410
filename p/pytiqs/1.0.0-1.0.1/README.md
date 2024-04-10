# Comparing `tmp/pytiqs-1.0.0.tar.gz` & `tmp/pytiqs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.0.tar", last modified: Tue Apr  9 04:31:14 2024, max compression
+gzip compressed data, was "pytiqs-1.0.1.tar", last modified: Tue Apr  9 04:39:21 2024, max compression
```

## Comparing `pytiqs-1.0.0.tar` & `pytiqs-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:31:14.934643 pytiqs-1.0.0/
--rw-r--r--   0 nitin      (501) staff       (20)      304 2024-04-09 04:31:14.934590 pytiqs-1.0.0/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)       19 2024-04-08 12:31:10.000000 pytiqs-1.0.0/README.md
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:31:14.934417 pytiqs-1.0.0/pytiqs.egg-info/
--rw-r--r--   0 nitin      (501) staff       (20)      304 2024-04-09 04:31:14.000000 pytiqs-1.0.0/pytiqs.egg-info/PKG-INFO
--rw-r--r--   0 nitin      (501) staff       (20)      267 2024-04-09 04:31:14.000000 pytiqs-1.0.0/pytiqs.egg-info/SOURCES.txt
--rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-09 04:31:14.000000 pytiqs-1.0.0/pytiqs.egg-info/dependency_links.txt
--rw-r--r--   0 nitin      (501) staff       (20)       17 2024-04-09 04:31:14.000000 pytiqs-1.0.0/pytiqs.egg-info/requires.txt
--rw-r--r--   0 nitin      (501) staff       (20)        5 2024-04-09 04:31:14.000000 pytiqs-1.0.0/pytiqs.egg-info/top_level.txt
--rw-r--r--   0 nitin      (501) staff       (20)      575 2024-04-09 04:31:14.934876 pytiqs-1.0.0/setup.cfg
--rw-r--r--   0 nitin      (501) staff       (20)      995 2024-04-09 04:16:48.000000 pytiqs-1.0.0/setup.py
-drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:31:14.934069 pytiqs-1.0.0/tiqs/
--rw-r--r--   0 nitin      (501) staff       (20)      104 2024-04-02 04:30:57.000000 pytiqs-1.0.0/tiqs/__init__.py
--rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-09 04:30:50.000000 pytiqs-1.0.0/tiqs/__version__.py
--rw-r--r--   0 nitin      (501) staff       (20)    17659 2024-04-08 11:39:51.000000 pytiqs-1.0.0/tiqs/connect.py
--rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-02 20:18:14.000000 pytiqs-1.0.0/tiqs/constants.py
--rw-r--r--   0 nitin      (501) staff       (20)      555 2024-03-21 12:32:16.000000 pytiqs-1.0.0/tiqs/exceptions.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488705 pytiqs-1.0.1/
+-rw-r--r--   0 nitin      (501) staff       (20)      369 2024-04-09 04:39:21.488641 pytiqs-1.0.1/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)       19 2024-04-08 12:31:10.000000 pytiqs-1.0.1/README.md
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488394 pytiqs-1.0.1/pytiqs.egg-info/
+-rw-r--r--   0 nitin      (501) staff       (20)      369 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/PKG-INFO
+-rw-r--r--   0 nitin      (501) staff       (20)      267 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/SOURCES.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        1 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/dependency_links.txt
+-rw-r--r--   0 nitin      (501) staff       (20)       52 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/requires.txt
+-rw-r--r--   0 nitin      (501) staff       (20)        5 2024-04-09 04:39:21.000000 pytiqs-1.0.1/pytiqs.egg-info/top_level.txt
+-rw-r--r--   0 nitin      (501) staff       (20)      575 2024-04-09 04:39:21.489078 pytiqs-1.0.1/setup.cfg
+-rw-r--r--   0 nitin      (501) staff       (20)     1051 2024-04-09 04:38:33.000000 pytiqs-1.0.1/setup.py
+drwxr-xr-x   0 nitin      (501) staff       (20)        0 2024-04-09 04:39:21.488021 pytiqs-1.0.1/tiqs/
+-rw-r--r--   0 nitin      (501) staff       (20)      104 2024-04-02 04:30:57.000000 pytiqs-1.0.1/tiqs/__init__.py
+-rw-r--r--   0 nitin      (501) staff       (20)      232 2024-04-09 04:39:11.000000 pytiqs-1.0.1/tiqs/__version__.py
+-rw-r--r--   0 nitin      (501) staff       (20)    17659 2024-04-08 11:39:51.000000 pytiqs-1.0.1/tiqs/connect.py
+-rw-r--r--   0 nitin      (501) staff       (20)     2525 2024-04-02 20:18:14.000000 pytiqs-1.0.1/tiqs/constants.py
+-rw-r--r--   0 nitin      (501) staff       (20)      555 2024-03-21 12:32:16.000000 pytiqs-1.0.1/tiqs/exceptions.py
```

### Comparing `pytiqs-1.0.0/setup.cfg` & `pytiqs-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.0/setup.py` & `pytiqs-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,12 +26,14 @@
     author_email=about["__author_email__"],
     url=about["__url__"],
     download_url=about["__download_url__"],
     license=about["__license__"],
     packages=["tiqs"],
     install_requires=[
         "requests>=2.18.4",
+        "python-dateutil>=2.6.1",
+        "six>=1.11.0"
     ],
     tests_require=["pytest", "responses", "pytest-cov", "mock", "flake8"],
     test_suite="tests",
     setup_requires=["pytest-runner"]
 )
```

### Comparing `pytiqs-1.0.0/tiqs/connect.py` & `pytiqs-1.0.1/tiqs/connect.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.0/tiqs/constants.py` & `pytiqs-1.0.1/tiqs/constants.py`

 * *Files identical despite different names*

### Comparing `pytiqs-1.0.0/tiqs/exceptions.py` & `pytiqs-1.0.1/tiqs/exceptions.py`

 * *Files identical despite different names*

