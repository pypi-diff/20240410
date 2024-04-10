# Comparing `tmp/visionone-filesecurity-1.1.0.tar.gz` & `tmp/visionone-filesecurity-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionone-filesecurity-1.1.0.tar", last modified: Thu Apr  4 04:43:40 2024, max compression
+gzip compressed data, was "visionone-filesecurity-1.1.1.tar", last modified: Wed Apr 10 19:06:55 2024, max compression
```

## Comparing `visionone-filesecurity-1.1.0.tar` & `visionone-filesecurity-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-04 04:43:39.000000 visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/amaas/grpc/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_aio_client_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_client_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-04 04:42:32.000000 visionone-filesecurity-1.1.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:43:40.734266 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 04:43:40.000000 visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.970519 visionone-filesecurity-1.1.1/amaas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/amaas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-10 19:06:54.000000 visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-10 19:06:54.000000 visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-10 19:06:54.000000 visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/amaas/grpc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/tests/test_aio_client_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/tests/test_client_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-10 19:05:47.000000 visionone-filesecurity-1.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:06:55.974519 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 19:06:55.000000 visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/top_level.txt
```

### Comparing `visionone-filesecurity-1.1.0/LICENSE` & `visionone-filesecurity-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/Makefile` & `visionone-filesecurity-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/__init__.py` & `visionone-filesecurity-1.1.1/amaas/grpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 LOG_LEVEL = os.environ.get('LOG_LEVEL', 'INFO')
 logger.setLevel(LOG_LEVEL)
 logger.propagate = False
 
-timeout_in_seconds = 180
+timeout_in_seconds = int(os.environ.get('TM_AM_SCAN_TIMEOUT_SECS', 300))
 
 
 class _Pipeline:
     """
     Class to allow a single element pipeline between producer and consumer.
     """
```

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/aio/__init__.py` & `visionone-filesecurity-1.1.1/amaas/grpc/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 LOG_LEVEL = os.environ.get('LOG_LEVEL', 'INFO')
 logger.setLevel(LOG_LEVEL)
 logger.propagate = False
 
-timeout_in_seconds = 180
+timeout_in_seconds = int(os.environ.get('TM_AM_SCAN_TIMEOUT_SECS', 300))
 
 
 def init_by_region(region, api_key, enable_tls=True, ca_cert=None):
     return _init_by_region_util(region, api_key, enable_tls, ca_cert, True)
 
 
 def init(host, api_key=None, enable_tls=False, ca_cert=None):
```

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/exception/__init__.py` & `visionone-filesecurity-1.1.1/amaas/grpc/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.py` & `visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2.pyi` & `visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/protos/scan_pb2_grpc.py` & `visionone-filesecurity-1.1.1/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/amaas/grpc/util.py` & `visionone-filesecurity-1.1.1/amaas/grpc/util.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/setup.py` & `visionone-filesecurity-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/tests/test_aio_client_sdk.py` & `visionone-filesecurity-1.1.1/tests/test_aio_client_sdk.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/tests/test_client_sdk.py` & `visionone-filesecurity-1.1.1/tests/test_client_sdk.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/tests/test_util.py` & `visionone-filesecurity-1.1.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `visionone-filesecurity-1.1.0/visionone_filesecurity.egg-info/SOURCES.txt` & `visionone-filesecurity-1.1.1/visionone_filesecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

