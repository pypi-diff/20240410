# Comparing `tmp/sling-1.2.2.tar.gz` & `tmp/sling-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sling-1.2.2.tar", last modified: Sun Mar 31 20:23:49 2024, max compression
+gzip compressed data, was "sling-1.2.3.tar", last modified: Wed Apr 10 17:18:14 2024, max compression
```

## Comparing `sling-1.2.2.tar` & `sling-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:23:49.736868 sling-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-31 20:20:32.000000 sling-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-31 20:23:49.736868 sling-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-31 20:23:46.000000 sling-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 20:23:46.000000 sling-1.2.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 20:23:49.736868 sling-1.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2134 2024-03-31 20:20:32.000000 sling-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:23:49.736868 sling-1.2.2/sling/
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-03-31 20:20:32.000000 sling-1.2.2/sling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 20:23:49.736868 sling-1.2.2/sling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 20:23:49.000000 sling-1.2.2/sling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 17:15:10.000000 sling-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-10 17:18:14.472063 sling-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 17:18:10.000000 sling-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:18:10.000000 sling-1.2.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:18:14.472063 sling-1.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-10 17:15:10.000000 sling-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/sling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-10 17:15:10.000000 sling-1.2.3/sling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/sling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/top_level.txt
```

### Comparing `sling-1.2.2/PKG-INFO` & `sling-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.2
+Version: 1.2.3
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

### Comparing `sling-1.2.2/README.md` & `sling-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sling-1.2.2/setup.py` & `sling-1.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     install_requires = [f'sling-linux-amd64=={SLING_VERSION}']
 elif platform.system() == 'Windows':
   if platform.machine() == 'aarch64':
     install_requires = [f'sling-windows-arm64=={SLING_VERSION}']
   else:
     install_requires = [f'sling-windows-amd64=={SLING_VERSION}']
 elif platform.system() == 'Darwin':
-  install_requires = [f'sling-mac-universal=={SLING_VERSION}']
+  if platform.machine() == 'aarch64':
+    install_requires = [f'sling-mac-arm64=={SLING_VERSION}']
+  else:
+    install_requires = [f'sling-mac-amd64=={SLING_VERSION}']
 else:
   raise Exception(f'platform "{platform.system()}" ({platform.system()}) not supported.')
 
 setup(
   name='sling',
   version=SLING_VERSION,
   description='Slings data from a source to a target',
```

### Comparing `sling-1.2.2/sling/__init__.py` & `sling-1.2.3/sling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,34 @@
 
 # For development
 SLING_BASE = os.path.join(os.path.dirname(__file__), '..', '..', 'sling_base')
 insert = lambda f: sys.path.insert(1, os.path.join(SLING_BASE, f))
 insert('sling-windows-amd64')
 insert('sling-linux-amd64')
 insert('sling-linux-arm64')
-insert('sling-mac-universal')
+insert('sling-mac-amd64')
+insert('sling-mac-arm64')
 
 SLING_BIN = None
 
 if platform.system() == 'Linux':
   if platform.machine() == 'aarch64':
     exec('from sling_linux_arm64 import SLING_BIN')
   else:
     exec('from sling_linux_amd64 import SLING_BIN')
 elif platform.system() == 'Windows':
   if platform.machine() == 'aarch64':
     exec('from sling_windows_arm64 import SLING_BIN')
   else:
     exec('from sling_windows_amd64 import SLING_BIN')
 elif platform.system() == 'Darwin':
-  exec('from sling_mac_universal import SLING_BIN')
+  if platform.machine() == 'aarch64':
+    exec('from sling_mac_arm64 import SLING_BIN')
+  else:
+    exec('from sling_mac_amd64 import SLING_BIN')
 
 #################################################################
 
 is_package = lambda text: any([
     text in line.lower()
     for line in traceback.format_stack()[:-1]])
```

### Comparing `sling-1.2.2/sling.egg-info/PKG-INFO` & `sling-1.2.3/sling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.2
+Version: 1.2.3
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

