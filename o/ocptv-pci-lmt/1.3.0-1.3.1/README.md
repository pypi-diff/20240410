# Comparing `tmp/ocptv-pci_lmt-1.3.0.tar.gz` & `tmp/ocptv-pci_lmt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocptv-pci_lmt-1.3.0.tar", last modified: Mon Apr  8 19:41:45 2024, max compression
+gzip compressed data, was "ocptv-pci_lmt-1.3.1.tar", last modified: Wed Apr 10 02:04:12 2024, max compression
```

## Comparing `ocptv-pci_lmt-1.3.0.tar` & `ocptv-pci_lmt-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/configs/test_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/pci_lmt/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/host.py
--rw-r--r--   0 runner    (1001) docker     (127)    39776 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/pcie_lane_margining.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.550220 ocptv-pci_lmt-1.3.1/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/configs/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.550220 ocptv-pci_lmt-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 02:04:12.000000 ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/src/pci_lmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39740 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/pcie_lane_margining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:04:12.554220 ocptv-pci_lmt-1.3.1/src/pci_lmt_bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-10 02:03:57.000000 ocptv-pci_lmt-1.3.1/src/pci_lmt_bin/main.py
```

### Comparing `ocptv-pci_lmt-1.3.0/LICENSE` & `ocptv-pci_lmt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/PKG-INFO` & `ocptv-pci_lmt-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocptv-pci_lmt
-Version: 1.3.0
+Version: 1.3.1
 Summary: PCI Lane Margining Tool
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ocptv-pci_lmt-1.3.0/README.md` & `ocptv-pci_lmt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/configs/test_config.json` & `ocptv-pci_lmt-1.3.1/configs/test_config.json`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/pyproject.toml` & `ocptv-pci_lmt-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ocptv-pci_lmt"
-version = "1.3.0"
+version = "1.3.1"
 description = "PCI Lane Margining Tool"
 readme = "README.md"
 authors = [
     { name = "OCP Test & Validation", email = "ocp-test-validation@OCP-All.groups.io" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -32,15 +32,15 @@
 [project.scripts]
 pci_lmt = "pci_lmt_bin.main:main"
 
 # Increment MAJOR version when you make incompatible API changes
 # Increment MINOR version when you add functionality in a backward compatible manner
 # Increment PATCH version when you make backward compatible bug fixes
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/PKG-INFO` & `ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocptv-pci_lmt
-Version: 1.3.0
+Version: 1.3.1
 Summary: PCI Lane Margining Tool
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/SOURCES.txt` & `ocptv-pci_lmt-1.3.1/src/ocptv_pci_lmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/args.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/args.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/collector.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/collector.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/config.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/config.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/constants.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/constants.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/device.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/device.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/host.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/host.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/pcie_lane_margining.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/pcie_lane_margining.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 
 # Decorator function to check the lane_errors status prior performing any
 # operations and update lane_errors status accordingly.
 def handle_lane_status(method: ty.Callable):
     def wrapper(self: "PcieDeviceLaneMargining", lane: int, *args, **kwargs):
         # Skip invoking the function if the device is faulty.
-        if self.device_error is not None:
+        if self.device_error:
             return {"error": self.device_error}
 
         # Skip invoking the function if the lane is already faulty.
         # Return the first error encountered.
-        if self.lane_errors[lane] is not None:
+        if self.lane_errors[lane]:
             return {"error": self.lane_errors[lane]}
 
         # Invoke the function and update the lane_errors if the function failed.
         ret = method(self, lane, *args, **kwargs)
-        if ret["error"] is not None:
+        if ret["error"]:
             logger.warning(f"{method} failed for BDF {self.device.bdf} lane {lane}: {ret['error']}")
             self.lane_errors[lane] = ret["error"]
         return ret
 
     return wrapper
```

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt/results.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt/results.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/main.py` & `ocptv-pci_lmt-1.3.1/src/pci_lmt_bin/main.py`

 * *Files identical despite different names*

