# Comparing `tmp/hexkit-2.1.0.tar.gz` & `tmp/hexkit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexkit-2.1.0.tar", last modified: Tue Jan 23 08:50:04 2024, max compression
+gzip compressed data, was "hexkit-2.1.1.tar", last modified: Mon Feb  5 14:54:53 2024, max compression
```

## Comparing `hexkit-2.1.0.tar` & `hexkit-2.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.337683 hexkit-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-01-23 08:49:56.000000 hexkit-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-23 08:49:56.000000 hexkit-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-01-23 08:50:04.337683 hexkit-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-01-23 08:49:56.000000 hexkit-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-01-23 08:49:56.000000 hexkit-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 08:50:04.337683 hexkit-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.325683 hexkit-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.329683 hexkit-2.1.0/src/hexkit/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.329683 hexkit-2.1.0/src/hexkit/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/protocols/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/protocols/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/protocols/eventsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/protocols/objstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.329683 hexkit-2.1.0/src/hexkit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit/providers/akafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/akafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/akafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/akafka/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/akafka/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit/providers/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/mongodb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/mongodb/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit/providers/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit/providers/s3/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/test_files/test_file1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/test_files/test_file2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/test_files/test_file3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/test_files/test_file4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/s3/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit/providers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/providers/testing/eventpub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-01-23 08:49:56.000000 hexkit-2.1.0/src/hexkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 08:50:04.333683 hexkit-2.1.0/src/hexkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-01-23 08:50:04.000000 hexkit-2.1.0/src/hexkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-23 08:50:04.000000 hexkit-2.1.0/src/hexkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 08:50:04.000000 hexkit-2.1.0/src/hexkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-23 08:50:04.000000 hexkit-2.1.0/src/hexkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-23 08:50:04.000000 hexkit-2.1.0/src/hexkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.978558 hexkit-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-02-05 14:54:45.000000 hexkit-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-05 14:54:45.000000 hexkit-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-02-05 14:54:53.978558 hexkit-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-02-05 14:54:45.000000 hexkit-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-02-05 14:54:45.000000 hexkit-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 14:54:53.978558 hexkit-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.970558 hexkit-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.970558 hexkit-2.1.1/src/hexkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.974558 hexkit-2.1.1/src/hexkit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16421 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/protocols/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/protocols/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/protocols/eventsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/protocols/objstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.974558 hexkit-2.1.1/src/hexkit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.974558 hexkit-2.1.1/src/hexkit/providers/akafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/akafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16985 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/akafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/akafka/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/akafka/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.974558 hexkit-2.1.1/src/hexkit/providers/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/mongodb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/mongodb/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.974558 hexkit-2.1.1/src/hexkit/providers/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.978558 hexkit-2.1.1/src/hexkit/providers/s3/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/test_files/test_file1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/test_files/test_file2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/test_files/test_file3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/test_files/test_file4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/s3/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.978558 hexkit-2.1.1/src/hexkit/providers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/providers/testing/eventpub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-05 14:54:45.000000 hexkit-2.1.1/src/hexkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 14:54:53.978558 hexkit-2.1.1/src/hexkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-02-05 14:54:53.000000 hexkit-2.1.1/src/hexkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-05 14:54:53.000000 hexkit-2.1.1/src/hexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 14:54:53.000000 hexkit-2.1.1/src/hexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-05 14:54:53.000000 hexkit-2.1.1/src/hexkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-05 14:54:53.000000 hexkit-2.1.1/src/hexkit.egg-info/top_level.txt
```

### Comparing `hexkit-2.1.0/LICENSE` & `hexkit-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/PKG-INFO` & `hexkit-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-2.1.0/README.md` & `hexkit-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/pyproject.toml` & `hexkit-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "hexkit"
-version = "2.1.0"
+version = "2.1.1"
 description = "A Toolkit for Building Microservices using the Hexagonal Architecture"
 dependencies = [
     "pydantic >=2, <3",
     "pydantic_settings >=2, <3",
     "PyYAML >=6.0, <7",
 ]
```

### Comparing `hexkit-2.1.0/src/hexkit/__init__.py` & `hexkit-2.1.1/src/hexkit/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/__main__.py` & `hexkit-2.1.1/src/hexkit/__main__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/base.py` & `hexkit-2.1.1/src/hexkit/base.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/config.py` & `hexkit-2.1.1/src/hexkit/config.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/correlation.py` & `hexkit-2.1.1/src/hexkit/correlation.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/custom_types.py` & `hexkit-2.1.1/src/hexkit/custom_types.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/log.py` & `hexkit-2.1.1/src/hexkit/log.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/protocols/__init__.py` & `hexkit-2.1.1/src/hexkit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/protocols/dao.py` & `hexkit-2.1.1/src/hexkit/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/protocols/eventpub.py` & `hexkit-2.1.1/src/hexkit/protocols/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/protocols/eventsub.py` & `hexkit-2.1.1/src/hexkit/protocols/eventsub.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/protocols/objstorage.py` & `hexkit-2.1.1/src/hexkit/protocols/objstorage.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/akafka/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/akafka/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/akafka/provider.py` & `hexkit-2.1.1/src/hexkit/providers/akafka/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         try:
             correlation_id = get_correlation_id()
         except CorrelationIdContextError:
             if not self._generate_correlation_id:
                 raise
 
             correlation_id = new_correlation_id()
-            logging.info("Generated new correlation id: %s", correlation_id)
+            logging.info("Generated new correlation ID: %s", correlation_id)
 
         validate_correlation_id(correlation_id)
 
         event_headers = [
             ("type", type_.encode("ascii")),
             ("correlation_id", correlation_id.encode("ascii")),
         ]
@@ -307,14 +307,15 @@
         *topics: Ascii,
         bootstrap_servers: str,
         security_protocol: str,
         ssl_context: Optional[ssl.SSLContext],
         client_id: str,
         group_id: str,
         auto_offset_reset: Literal["earliest"],
+        enable_auto_commit: bool,
         key_deserializer: Callable[[bytes], str],
         value_deserializer: Callable[[bytes], str],
     ):
         """
         Initialize the consumer with some config params.
 
         Args:
@@ -330,14 +331,18 @@
             key_serializer:
                 Function to deserialize the keys into strings.
             value_serializer:
                 Function to deserialize the values into strings.
         """
         ...
 
+    async def commit(self, offsets=None):
+        """Commit offsets to Kafka Broker."""
+        ...
+
     async def start(self) -> None:
         """Setup the consumer."""
         ...
 
     async def stop(self) -> None:
         """Teardown the consumer."""
         ...
@@ -386,14 +391,15 @@
             *topics,
             bootstrap_servers=",".join(config.kafka_servers),
             security_protocol=config.kafka_security_protocol,
             ssl_context=generate_ssl_context(config),
             client_id=client_id,
             group_id=config.service_name,
             auto_offset_reset="earliest",
+            enable_auto_commit=False,
             key_deserializer=lambda event_key: event_key.decode("ascii"),
             value_deserializer=lambda event_value: json.loads(
                 event_value.decode("ascii")
             ),
         )
         try:
             await consumer.start()
@@ -433,36 +439,42 @@
         try:
             type_ = get_header_value(header_name="type", headers=headers)
             correlation_id = get_header_value(
                 header_name="correlation_id", headers=headers
             )
         except EventHeaderNotFoundError as err:
             logging.warning("Ignored an event: %s. %s", event_label, err.args[0])
+            # acknowledge event receipt
+            await self._consumer.commit()
             return
 
         if type_ in self._types_whitelist:
             logging.info('Consuming event of type "%s": %s', type_, event_label)
 
             try:
                 async with set_correlation_id(correlation_id):
                     # blocks until event processing is completed:
                     await self._translator.consume(
                         payload=event.value,
                         type_=type_,
                         topic=event.topic,
                     )
+                    # acknowledge successfully processed event
+                    await self._consumer.commit()
             except Exception:
                 logging.error(
                     "A fatal error occurred while processing the event: %s",
                     event_label,
                 )
                 raise
 
         else:
             logging.info("Ignored event of type %s: %s", type_, event_label)
+            # acknowledge event receipt
+            await self._consumer.commit()
 
     async def run(self, forever: bool = True) -> None:
         """
         Start consuming events and passing them down to the translator.
         By default, it blocks forever.
         However, you can set `forever` to `False` to make it return after handling one
         event.
```

### Comparing `hexkit-2.1.0/src/hexkit/providers/akafka/testcontainer.py` & `hexkit-2.1.1/src/hexkit/providers/akafka/testcontainer.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/akafka/testutils.py` & `hexkit-2.1.1/src/hexkit/providers/akafka/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/mongodb/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/mongodb/provider.py` & `hexkit-2.1.1/src/hexkit/providers/mongodb/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/mongodb/testutils.py` & `hexkit-2.1.1/src/hexkit/providers/mongodb/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/s3/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/s3/provider.py` & `hexkit-2.1.1/src/hexkit/providers/s3/provider.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/s3/test_files/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/s3/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/s3/testutils.py` & `hexkit-2.1.1/src/hexkit/providers/s3/testutils.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/testing/__init__.py` & `hexkit-2.1.1/src/hexkit/providers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/providers/testing/eventpub.py` & `hexkit-2.1.1/src/hexkit/providers/testing/eventpub.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit/utils.py` & `hexkit-2.1.1/src/hexkit/utils.py`

 * *Files identical despite different names*

### Comparing `hexkit-2.1.0/src/hexkit.egg-info/PKG-INFO` & `hexkit-2.1.1/src/hexkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexkit
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Toolkit for Building Microservices using the Hexagonal Architecture
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/hexkit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hexkit-2.1.0/src/hexkit.egg-info/SOURCES.txt` & `hexkit-2.1.1/src/hexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

