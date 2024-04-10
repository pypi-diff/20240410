# Comparing `tmp/sciveo-0.0.43.tar.gz` & `tmp/sciveo-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.43.tar", last modified: Wed Apr 10 18:23:54 2024, max compression
+gzip compressed data, was "sciveo-0.0.44.tar", last modified: Wed Apr 10 19:57:00 2024, max compression
```

## Comparing `sciveo-0.0.43.tar` & `sciveo-0.0.44.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.772595 sciveo-0.0.43/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 18:23:54.772448 sciveo-0.0.43/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5712 2024-03-17 11:37:08.000000 sciveo-0.0.43/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.749954 sciveo-0.0.43/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1360 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.756538 sciveo-0.0.43/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.43/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.43/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.764542 sciveo-0.0.43/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.43/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.43/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.43/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.43/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.766273 sciveo-0.0.43/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.43/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2023-12-12 14:35:14.000000 sciveo-0.0.43/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.43/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1552 2024-04-08 15:42:14.000000 sciveo-0.0.43/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.43/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.43/sciveo/common/tools/synchronized.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.770579 sciveo-0.0.43/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.43/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.43/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.43/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.770895 sciveo-0.0.43/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.43/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3721 2024-04-10 18:13:35.000000 sciveo-0.0.43/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-10 18:20:38.000000 sciveo-0.0.43/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.755941 sciveo-0.0.43/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 18:23:54.000000 sciveo-0.0.43/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      879 2024-04-10 18:23:54.000000 sciveo-0.0.43/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-10 18:23:54.000000 sciveo-0.0.43/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-10 18:23:54.000000 sciveo-0.0.43/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-10 18:23:54.000000 sciveo-0.0.43/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-10 18:23:54.772757 sciveo-0.0.43/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.43/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 18:23:54.772018 sciveo-0.0.43/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.43/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      577 2024-04-09 13:03:08.000000 sciveo-0.0.43/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.43/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.43/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.638592 sciveo-0.0.44/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 19:57:00.638370 sciveo-0.0.44/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5712 2024-03-17 11:37:08.000000 sciveo-0.0.44/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.616259 sciveo-0.0.44/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1360 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.629045 sciveo-0.0.44/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.44/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.44/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.630873 sciveo-0.0.44/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.44/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.44/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.633405 sciveo-0.0.44/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.44/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2023-12-12 14:35:14.000000 sciveo-0.0.44/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.44/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1552 2024-04-08 15:42:14.000000 sciveo-0.0.44/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.44/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.44/sciveo/common/tools/synchronized.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.635310 sciveo-0.0.44/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.44/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.44/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.635895 sciveo-0.0.44/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3650 2024-04-10 19:31:28.000000 sciveo-0.0.44/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-10 19:29:12.000000 sciveo-0.0.44/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.627963 sciveo-0.0.44/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      879 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-10 19:57:00.638719 sciveo-0.0.44/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.44/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.637551 sciveo-0.0.44/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.44/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.44/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.44/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.44/test/test_sampling.py
```

### Comparing `sciveo-0.0.43/PKG-INFO` & `sciveo-0.0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.43
+Version: 0.0.44
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
```

### Comparing `sciveo-0.0.43/README.md` & `sciveo-0.0.44/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/__init__.py` & `sciveo-0.0.44/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/api/base.py` & `sciveo-0.0.44/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/api/upload.py` & `sciveo-0.0.44/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/configuration.py` & `sciveo-0.0.44/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/model.py` & `sciveo-0.0.44/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/optimizers.py` & `sciveo-0.0.44/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/sampling.py` & `sciveo-0.0.44/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/tools/daemon.py` & `sciveo-0.0.44/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/tools/formating.py` & `sciveo-0.0.44/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/tools/hardware.py` & `sciveo-0.0.44/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/tools/logger.py` & `sciveo-0.0.44/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/common/tools/synchronized.py` & `sciveo-0.0.44/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/content/dataset.py` & `sciveo-0.0.44/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/content/experiment.py` & `sciveo-0.0.44/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/content/project.py` & `sciveo-0.0.44/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/content/runner.py` & `sciveo-0.0.44/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/sciveo/monitoring/monitor.py` & `sciveo-0.0.44/sciveo/monitoring/monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import os
 import subprocess
 import time
 import datetime
 import socket
 import psutil
+import uuid
 import numpy as np
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.daemon import DaemonBase
 from sciveo.common.tools.hardware import *
 from sciveo.common.tools.formating import format_memory_size
 from sciveo.api.base import APIRemoteClient
@@ -77,18 +78,15 @@
     self.data["RAM"]["total"] = memory.total
     self.data["RAM"]["free"] = memory.free
     self.data["RAM"]["print"] = f"total: {format_memory_size(memory.total)} used: {format_memory_size(memory.used)}"
 
   def getserial(self):
     machine_serial = None
     try:
-      with open('/proc/cpuinfo','r') as fp:
-        for line in fp:
-          if line.startswith('Serial'):
-            machine_serial = line[10:26]
+      machine_serial = f"{socket.gethostname()}-{uuid.getnode()}"
     except Exception:
       pass
     if machine_serial is None:
       try:
         machine_serial = socket.gethostname()
       except Exception:
         pass
@@ -126,12 +124,12 @@
     except Exception as e:
       pass
 
 
 
 
 if __name__ == "__main__":
-  mon = BaseMonitor(period=30)
+  mon = BaseMonitor(period=10)
   mon.start()
 
   while(True):
     time.sleep(30)
```

### Comparing `sciveo-0.0.43/sciveo.egg-info/PKG-INFO` & `sciveo-0.0.44/sciveo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.43
+Version: 0.0.44
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
```

### Comparing `sciveo-0.0.43/sciveo.egg-info/SOURCES.txt` & `sciveo-0.0.44/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/test/test_configuration.py` & `sciveo-0.0.44/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/test/test_runner.py` & `sciveo-0.0.44/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.43/test/test_sampling.py` & `sciveo-0.0.44/test/test_sampling.py`

 * *Files identical despite different names*

