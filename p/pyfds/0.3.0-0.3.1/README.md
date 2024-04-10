# Comparing `tmp/pyfds-0.3.0.tar.gz` & `tmp/pyfds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfds-0.3.0.tar", last modified: Wed Apr  3 14:54:51 2024, max compression
+gzip compressed data, was "pyfds-0.3.1.tar", last modified: Wed Apr 10 14:13:02 2024, max compression
```

## Comparing `pyfds-0.3.0.tar` & `pyfds-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.749745 pyfds-0.3.0/
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.354226 pyfds-0.3.0/.github/
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.443249 pyfds-0.3.0/.github/workflows/
--rwxrwx---   0 leanderc (50967) user     (10000)     1321 2023-06-30 08:00:31.000000 pyfds-0.3.0/.github/workflows/python-package.yml
--rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.3.0/.gitignore
--rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.3.0/AUTHORS.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2810 2024-04-03 14:41:44.000000 pyfds-0.3.0/CHANGELOG.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.3.0/LICENSE
--rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-03 14:54:51.743363 pyfds-0.3.0/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      722 2024-04-03 14:45:15.000000 pyfds-0.3.0/README.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.559044 pyfds-0.3.0/doc/
--rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.3.0/doc/acoustic_flow.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.3.0/doc/acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     2551 2023-06-30 07:07:46.000000 pyfds-0.3.0/doc/conf.py
--rwxrwx---   0 leanderc (50967) user     (10000)      172 2024-01-17 13:05:40.000000 pyfds-0.3.0/doc/coupling.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.3.0/doc/electrostatics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.3.0/doc/ex_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.3.0/doc/ex_visualization.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.3.0/doc/examples.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.3.0/doc/fields.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.3.0/doc/gfx.rst
--rwxrwx---   0 leanderc (50967) user     (10000)      454 2024-01-17 13:06:27.000000 pyfds-0.3.0/doc/index.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.3.0/doc/nonlinear_acoustics.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.3.0/doc/regions.rst
--rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.3.0/doc/thermal.rst
--rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.3.0/doc/usage.rst
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.649724 pyfds-0.3.0/pyfds/
--rwxrwx---   0 leanderc (50967) user     (10000)      247 2024-01-17 09:00:31.000000 pyfds-0.3.0/pyfds/__init__.py
--rwxrwx---   0 leanderc (50967) user     (10000)     2179 2024-01-17 13:15:07.000000 pyfds-0.3.0/pyfds/acoustic_flow.py
--rwxrwx---   0 leanderc (50967) user     (10000)    12771 2024-01-10 14:09:57.000000 pyfds-0.3.0/pyfds/acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     2603 2024-01-17 13:16:14.000000 pyfds-0.3.0/pyfds/coupled_fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)    10341 2024-01-17 14:10:14.000000 pyfds-0.3.0/pyfds/coupling.py
--rwxrwx---   0 leanderc (50967) user     (10000)     4636 2024-01-10 14:13:02.000000 pyfds-0.3.0/pyfds/electrostatics.py
--rwxrwx---   0 leanderc (50967) user     (10000)    24352 2024-01-09 15:07:20.000000 pyfds-0.3.0/pyfds/fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)    17416 2024-01-10 14:13:44.000000 pyfds-0.3.0/pyfds/gfx.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8211 2024-01-10 14:10:37.000000 pyfds-0.3.0/pyfds/nonlinear_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     5190 2024-01-18 07:57:16.000000 pyfds-0.3.0/pyfds/regions.py
--rwxrwx---   0 leanderc (50967) user     (10000)     8296 2024-01-10 14:12:11.000000 pyfds-0.3.0/pyfds/thermal.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.733615 pyfds-0.3.0/pyfds.egg-info/
--rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/PKG-INFO
--rwxrwx---   0 leanderc (50967) user     (10000)      834 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/SOURCES.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        1 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/dependency_links.txt
--rwxrwx---   0 leanderc (50967) user     (10000)       84 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/requires.txt
--rwxrwx---   0 leanderc (50967) user     (10000)        6 2024-04-03 14:54:51.000000 pyfds-0.3.0/pyfds.egg-info/top_level.txt
--rwxrwx---   0 leanderc (50967) user     (10000)     1032 2023-06-29 15:49:48.000000 pyfds-0.3.0/pyproject.toml
--rwxrwx---   0 leanderc (50967) user     (10000)       38 2024-04-03 14:54:51.751370 pyfds-0.3.0/setup.cfg
--rwxrwx---   0 leanderc (50967) user     (10000)     1261 2023-06-29 15:48:20.000000 pyfds-0.3.0/setup.py
-drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-03 14:54:51.724663 pyfds-0.3.0/test/
--rwxrwx---   0 leanderc (50967) user     (10000)     3700 2023-06-30 07:12:49.000000 pyfds-0.3.0/test/test_acoustics.py
--rwxrwx---   0 leanderc (50967) user     (10000)     3788 2024-01-10 13:49:00.000000 pyfds-0.3.0/test/test_coupling.py
--rwxrwx---   0 leanderc (50967) user     (10000)     6098 2023-06-30 08:21:57.000000 pyfds-0.3.0/test/test_fields.py
--rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.3.0/test/test_regions.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.757396 pyfds-0.3.1/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.333591 pyfds-0.3.1/.github/
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.403901 pyfds-0.3.1/.github/workflows/
+-rwxrwx---   0 leanderc (50967) user     (10000)     1321 2023-06-30 08:00:31.000000 pyfds-0.3.1/.github/workflows/python-package.yml
+-rwxrwx---   0 leanderc (50967) user     (10000)     2194 2017-01-02 12:00:53.000000 pyfds-0.3.1/.gitignore
+-rwxrwx---   0 leanderc (50967) user     (10000)      118 2021-10-20 12:26:35.000000 pyfds-0.3.1/AUTHORS.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2998 2024-04-10 13:59:56.000000 pyfds-0.3.1/CHANGELOG.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     1477 2017-05-16 12:52:30.000000 pyfds-0.3.1/LICENSE
+-rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-10 14:13:02.751333 pyfds-0.3.1/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      722 2024-04-03 14:45:15.000000 pyfds-0.3.1/README.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.515369 pyfds-0.3.1/doc/
+-rwxrwx---   0 leanderc (50967) user     (10000)       79 2023-03-30 12:24:43.000000 pyfds-0.3.1/doc/acoustic_flow.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       67 2017-02-02 09:31:23.000000 pyfds-0.3.1/doc/acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     2551 2023-06-30 07:07:46.000000 pyfds-0.3.1/doc/conf.py
+-rwxrwx---   0 leanderc (50967) user     (10000)      172 2024-01-17 13:05:40.000000 pyfds-0.3.1/doc/coupling.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       82 2021-12-20 08:34:47.000000 pyfds-0.3.1/doc/electrostatics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3790 2017-06-13 12:30:59.000000 pyfds-0.3.1/doc/ex_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     3339 2017-06-12 15:06:37.000000 pyfds-0.3.1/doc/ex_visualization.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       78 2017-06-08 09:07:55.000000 pyfds-0.3.1/doc/examples.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       58 2017-01-02 09:14:37.000000 pyfds-0.3.1/doc/fields.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       49 2017-02-02 09:31:55.000000 pyfds-0.3.1/doc/gfx.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)      454 2024-01-17 13:06:27.000000 pyfds-0.3.1/doc/index.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       97 2017-06-06 12:12:26.000000 pyfds-0.3.1/doc/nonlinear_acoustics.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2017-02-02 09:30:58.000000 pyfds-0.3.1/doc/regions.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)       61 2021-12-20 08:34:52.000000 pyfds-0.3.1/doc/thermal.rst
+-rwxrwx---   0 leanderc (50967) user     (10000)     8935 2021-10-20 12:13:52.000000 pyfds-0.3.1/doc/usage.rst
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.602006 pyfds-0.3.1/pyfds/
+-rwxrwx---   0 leanderc (50967) user     (10000)      247 2024-01-17 09:00:31.000000 pyfds-0.3.1/pyfds/__init__.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     2179 2024-01-17 13:15:07.000000 pyfds-0.3.1/pyfds/acoustic_flow.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    12771 2024-01-10 14:09:57.000000 pyfds-0.3.1/pyfds/acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     2603 2024-01-17 13:16:14.000000 pyfds-0.3.1/pyfds/coupled_fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    12371 2024-04-10 13:29:20.000000 pyfds-0.3.1/pyfds/coupling.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     4636 2024-01-10 14:13:02.000000 pyfds-0.3.1/pyfds/electrostatics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    24352 2024-01-09 15:07:20.000000 pyfds-0.3.1/pyfds/fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)    17416 2024-01-10 14:13:44.000000 pyfds-0.3.1/pyfds/gfx.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8211 2024-01-10 14:10:37.000000 pyfds-0.3.1/pyfds/nonlinear_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     5190 2024-01-18 07:57:16.000000 pyfds-0.3.1/pyfds/regions.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     8296 2024-04-10 13:20:15.000000 pyfds-0.3.1/pyfds/thermal.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.741138 pyfds-0.3.1/pyfds.egg-info/
+-rwxrwxr--   0 leanderc (50967) user     (10000)     3426 2024-04-10 14:13:02.000000 pyfds-0.3.1/pyfds.egg-info/PKG-INFO
+-rwxrwx---   0 leanderc (50967) user     (10000)      834 2024-04-10 14:13:02.000000 pyfds-0.3.1/pyfds.egg-info/SOURCES.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        1 2024-04-10 14:13:02.000000 pyfds-0.3.1/pyfds.egg-info/dependency_links.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)       84 2024-04-10 14:13:02.000000 pyfds-0.3.1/pyfds.egg-info/requires.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)        6 2024-04-10 14:13:02.000000 pyfds-0.3.1/pyfds.egg-info/top_level.txt
+-rwxrwx---   0 leanderc (50967) user     (10000)     1032 2023-06-29 15:49:48.000000 pyfds-0.3.1/pyproject.toml
+-rwxrwx---   0 leanderc (50967) user     (10000)       38 2024-04-10 14:13:02.759331 pyfds-0.3.1/setup.cfg
+-rwxrwx---   0 leanderc (50967) user     (10000)     1261 2023-06-29 15:48:20.000000 pyfds-0.3.1/setup.py
+drwxrwx---   0 leanderc (50967) user     (10000)        0 2024-04-10 14:13:02.732431 pyfds-0.3.1/test/
+-rwxrwx---   0 leanderc (50967) user     (10000)     3700 2023-06-30 07:12:49.000000 pyfds-0.3.1/test/test_acoustics.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     3788 2024-04-10 14:05:58.000000 pyfds-0.3.1/test/test_coupling.py
+-rwxrwx---   0 leanderc (50967) user     (10000)     6098 2023-06-30 08:21:57.000000 pyfds-0.3.1/test/test_fields.py
+-rwxrwx---   0 leanderc (50967) user     (10000)      286 2017-02-02 09:14:25.000000 pyfds-0.3.1/test/test_regions.py
```

### Comparing `pyfds-0.3.0/.github/workflows/python-package.yml` & `pyfds-0.3.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/.gitignore` & `pyfds-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/CHANGELOG.rst` & `pyfds-0.3.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 .. _Semantic versioning: https://semver.org/
 
 
 `Unreleased`_
 =============
 
 
+`0.3.1`_ - 2024-04-10
+=====================
+
+Added
+-----
+* Material parameter coupling with exponential expression.
+
+
 `0.3.0`_ - 2024-04-03
 =====================
 
 Added
 -----
 * Generic API for simulation of coupled fields using boundary conditions and dependent material parameters.
 * One-dimensional thermo-acoustic simulation.
@@ -128,14 +136,15 @@
 
 Added
 -----
 * First preview release.
 
 
 .. _Unreleased: https://github.com/emtpb/pyfds
+.. _0.3.1: https://github.com/emtpb/pyfds/releases/tag/0.3.1
 .. _0.3.0: https://github.com/emtpb/pyfds/releases/tag/0.3.0
 .. _0.2.0: https://github.com/emtpb/pyfds/releases/tag/0.2.0
 .. _0.1.6: https://github.com/emtpb/pyfds/releases/tag/0.1.6
 .. _0.1.5: https://github.com/emtpb/pyfds/releases/tag/0.1.5
 .. _0.1.4: https://github.com/emtpb/pyfds/releases/tag/0.1.4
 .. _0.1.3: https://github.com/emtpb/pyfds/releases/tag/0.1.3
 .. _0.1.2: https://github.com/emtpb/pyfds/releases/tag/0.1.2
```

### Comparing `pyfds-0.3.0/LICENSE` & `pyfds-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/PKG-INFO` & `pyfds-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modular field simulation tool using finite differences.
 Home-page: https://emt.uni-paderborn.de
 Author: Leander Claes
 Author-email: Leander Claes <claes@emt.uni-paderborn.de>
 License: Copyright (c) 2017 Leander Claes
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pyfds-0.3.0/README.rst` & `pyfds-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/doc/conf.py` & `pyfds-0.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/doc/ex_acoustics.rst` & `pyfds-0.3.1/doc/ex_acoustics.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/doc/ex_visualization.rst` & `pyfds-0.3.1/doc/ex_visualization.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/doc/usage.rst` & `pyfds-0.3.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/acoustic_flow.py` & `pyfds-0.3.1/pyfds/acoustic_flow.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/acoustics.py` & `pyfds-0.3.1/pyfds/acoustics.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/coupled_fields.py` & `pyfds-0.3.1/pyfds/coupled_fields.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/coupling.py` & `pyfds-0.3.1/pyfds/coupling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging as lo
+import numpy as np
 
 from . import fields as fld
 
 __all__ = [
-    'SynchronizedFields', 'BoundaryCoupling', 'MaterialCoupling', 'MaterialCouplingPowerLaw',
+    'SynchronizedFields', 'BoundaryCoupling', 'MaterialCoupling', 'MaterialCouplingExponential',
+    'MaterialCouplingPowerLaw',
 ]
 
 logger = lo.getLogger('pyfds')
 
 
 class SynchronizedFields(fld.Field):
     """Class for simulation of coupled fields with same time stepping."""
@@ -209,14 +211,58 @@
                 self.target_field.assemble_matrices()
                 self.last_used_factors = transfer_factors
                 if self.rel_change_threshold is not None:
                     logger.info(f"Relative change in parameters is {rel_change}.")
                     logger.info(f"Matrices reassembled in step {step}.")
 
 
+class MaterialCouplingExponential(MaterialCoupling):
+    """Class to couple the material parameters of one field to a field quantity q of another using
+    an exponential expression: p * (a + (1 - a) * exp(b * q))). The expression will always yield p
+    for q = 0. The expression will converge to p * a for negative values of b and for large
+    positive values of q as well as for positive values of b and large negative values of q."""
+
+    def __init__(self, source_component, target_field, target_parameter, a, b,
+                 rel_change_threshold=None, stepping=1):
+        """Class constructor.
+
+        Args:
+            source_component: Field component whose values are fed into the transfer function.
+            target_field: Field with material to be modified.
+            target_parameter: Name of parameter modified by the output of transfer function.
+            a: Parameter of the exponential expression. Relative limit for bounded half
+                of the expression.
+            b: Parameter in the exponent of the exponential expression.
+            rel_change_threshold: Relative change threshold for parameters changes to be applied.
+            stepping: Increase to apply coupling only each nth step.
+        """
+
+        self.a = a
+        self.b = b
+        super().__init__(
+            source_component=source_component,
+            target_field=target_field,
+            target_parameter=target_parameter,
+            transfer_function=self.transfer_function,
+            rel_change_threshold=rel_change_threshold,
+            stepping=stepping
+        )
+
+    def transfer_function(self, values):
+        """Exponential expression used as a transfer function.
+
+        Args:
+            values: Values of the source field component.
+
+        Returns:
+            Factors the material parameters are multiplied with.
+        """
+        return self.a + (1 - self.a) * np.exp(self.b * values)
+
+
 class MaterialCouplingPowerLaw(MaterialCoupling):
     """Class to couple the material parameters of one field to a field quantity q of another using
     a power law: p * (1 + factor * q ^ power)."""
 
     def __init__(self, source_component, target_field, target_parameter, power, factor,
                  rel_change_threshold=None, stepping=1):
         """Class constructor.
```

### Comparing `pyfds-0.3.0/pyfds/electrostatics.py` & `pyfds-0.3.1/pyfds/electrostatics.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/fields.py` & `pyfds-0.3.1/pyfds/fields.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/gfx.py` & `pyfds-0.3.1/pyfds/gfx.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/nonlinear_acoustics.py` & `pyfds-0.3.1/pyfds/nonlinear_acoustics.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/regions.py` & `pyfds-0.3.1/pyfds/regions.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds/thermal.py` & `pyfds-0.3.1/pyfds/thermal.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyfds.egg-info/PKG-INFO` & `pyfds-0.3.1/pyfds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modular field simulation tool using finite differences.
 Home-page: https://emt.uni-paderborn.de
 Author: Leander Claes
 Author-email: Leander Claes <claes@emt.uni-paderborn.de>
 License: Copyright (c) 2017 Leander Claes
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pyfds-0.3.0/pyfds.egg-info/SOURCES.txt` & `pyfds-0.3.1/pyfds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/pyproject.toml` & `pyfds-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/setup.py` & `pyfds-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/test/test_acoustics.py` & `pyfds-0.3.1/test/test_acoustics.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/test/test_coupling.py` & `pyfds-0.3.1/test/test_coupling.py`

 * *Files identical despite different names*

### Comparing `pyfds-0.3.0/test/test_fields.py` & `pyfds-0.3.1/test/test_fields.py`

 * *Files identical despite different names*

