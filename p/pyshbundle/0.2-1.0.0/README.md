# Comparing `tmp/pyshbundle-0.2.tar.gz` & `tmp/pyshbundle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshbundle-0.2.tar", last modified: Sat Jan 20 14:57:54 2024, max compression
+gzip compressed data, was "pyshbundle-1.0.0.tar", last modified: Wed Apr 10 16:19:16 2024, max compression
```

## Comparing `pyshbundle-0.2.tar` & `pyshbundle-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-01-20 14:57:54.736264 pyshbundle-0.2/
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1574 2024-01-03 08:58:49.000000 pyshbundle-0.2/LICENSE
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      122 2024-01-03 08:58:49.000000 pyshbundle-0.2/MANIFEST.in
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6776 2024-01-20 14:57:54.736264 pyshbundle-0.2/PKG-INFO
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5949 2024-01-03 08:58:49.000000 pyshbundle-0.2/README.md
-drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-01-20 14:57:54.736264 pyshbundle-0.2/pyshbundle/
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13336 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/GRACE_Data_Driven_Correction_Vishwakarma.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3445 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/GRACEconstants.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6596 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/GRACEpy.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4270 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/Phase_calc.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4536 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/__init__.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5050 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/basin_avg.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4486 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/clm2cs.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6102 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/clm2sc.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3852 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/cs2sc.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4932 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/eigengrav.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4118 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/gaussian.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4544 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/grule.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    10693 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/gsha.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9531 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/gshs.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9217 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/iplm.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3749 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/ispec.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5947 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/klm2sc.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4233 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/load_longterm_mean.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     2709 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/naninterp.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4930 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/neumann.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    40576 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/new_io.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4822 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/normalklm.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13394 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/plm.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1904 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/pyshbundle.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6362 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/read_GRACE_SH_paths.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    11041 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/reader_replacer.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    12907 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/reader_replacer_csr.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    12770 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/reader_replacer_itsg.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13071 2024-01-20 14:55:37.000000 pyshbundle-0.2/pyshbundle/reader_replacer_jpl.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3366 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle/sc2cs.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3597 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/tws_cal.py
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9109 2024-01-20 14:55:30.000000 pyshbundle-0.2/pyshbundle/visualisation_utils.py
-drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-01-20 14:57:54.736264 pyshbundle-0.2/pyshbundle.egg-info/
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6776 2024-01-20 14:57:54.000000 pyshbundle-0.2/pyshbundle.egg-info/PKG-INFO
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1107 2024-01-20 14:57:54.000000 pyshbundle-0.2/pyshbundle.egg-info/SOURCES.txt
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      206 2024-01-20 14:57:54.000000 pyshbundle-0.2/pyshbundle.egg-info/dependency_links.txt
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)        1 2024-01-03 08:58:50.000000 pyshbundle-0.2/pyshbundle.egg-info/not-zip-safe
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      144 2024-01-20 14:57:54.000000 pyshbundle-0.2/pyshbundle.egg-info/requires.txt
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)       11 2024-01-20 14:57:54.000000 pyshbundle-0.2/pyshbundle.egg-info/top_level.txt
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      205 2024-01-20 14:55:38.000000 pyshbundle-0.2/requirements.txt
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      391 2024-01-20 14:57:54.736264 pyshbundle-0.2/setup.cfg
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1873 2024-01-20 14:57:27.000000 pyshbundle-0.2/setup.py
-drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-01-20 14:57:54.736264 pyshbundle-0.2/tests/
--rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      402 2024-01-03 08:58:50.000000 pyshbundle-0.2/tests/test_pyshbundle.py
+drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1574 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/LICENSE
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      122 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/MANIFEST.in
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6359 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/PKG-INFO
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5494 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/README.md
+drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/pyshbundle/
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13249 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/GRACE_Data_Driven_Correction_Vishwakarma.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3445 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/GRACEconstants.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6596 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/GRACEpy.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4270 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/Phase_calc.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4395 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/__init__.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5050 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/basin_avg.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4493 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/clm2cs.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6128 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/clm2sc.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     8302 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/conv_sh.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3852 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/cs2sc.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4932 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/eigengrav.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4118 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/gaussian.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4544 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/grule.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    10702 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/gsha.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9540 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/gshs.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4486 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/hydro.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    42256 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/io.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9217 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/iplm.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3749 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/ispec.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     5947 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/klm2sc.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4233 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/load_longterm_mean.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     2709 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/naninterp.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4930 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/neumann.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     4822 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/normalklm.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13394 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/plm.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    24954 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/pysh_core.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1904 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/pyshbundle.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6362 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/read_GRACE_SH_paths.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    11041 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/reader_replacer.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    12907 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/reader_replacer_csr.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    12770 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/reader_replacer_itsg.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    13071 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/reader_replacer_jpl.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3366 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/sc2cs.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)    30401 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/shutils.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     3597 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/tws_cal.py
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     9315 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle/viz_utils.py
+drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/pyshbundle.egg-info/
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     6359 2024-04-10 16:19:16.000000 pyshbundle-1.0.0/pyshbundle.egg-info/PKG-INFO
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1181 2024-04-10 16:19:16.000000 pyshbundle-1.0.0/pyshbundle.egg-info/SOURCES.txt
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      206 2024-04-10 16:19:16.000000 pyshbundle-1.0.0/pyshbundle.egg-info/dependency_links.txt
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)        1 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/pyshbundle.egg-info/not-zip-safe
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      144 2024-04-10 16:19:16.000000 pyshbundle-1.0.0/pyshbundle.egg-info/requires.txt
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)       11 2024-04-10 16:19:16.000000 pyshbundle-1.0.0/pyshbundle.egg-info/top_level.txt
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      205 2024-04-10 16:18:10.000000 pyshbundle-1.0.0/requirements.txt
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      393 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/setup.cfg
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)     1911 2024-04-10 16:18:11.000000 pyshbundle-1.0.0/setup.py
+drwxr-xr-x   0 mn5hk     (1000) mn5hk     (1000)        0 2024-04-10 16:19:16.135091 pyshbundle-1.0.0/tests/
+-rw-r--r--   0 mn5hk     (1000) mn5hk     (1000)      402 2024-04-10 16:18:11.000000 pyshbundle-1.0.0/tests/test_pyshbundle.py
```

### Comparing `pyshbundle-0.2/LICENSE` & `pyshbundle-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/PKG-INFO` & `pyshbundle-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyshbundle
-Version: 0.2
-Summary: PySHbundle: A Python implementation of MATLAB codes SHbundle
+Version: 1.0.0
+Summary: PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle
 Home-page: https://github.com/mn5hk/pyshbundle
 Author: Amin Shakya
 Author-email: aminshk50@gmail.com
 License: GNU General Public License v3
 Keywords: pyshbundle
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,79 +16,70 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PySHbundle: A Python implementation of MATLAB codes SHbundle <br>
+# PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle <br>
 
 ![](https://visitor-badge.glitch.me/badge?page_id=mn5hk.mat2py) <br>
 
 
-PySHBundle is the python implementation of the popular SHBundle toolbox originally written using MATLAB. 
-
-TODO: Badges and and banner for the project
+PySHBundle is a tool to process GRACE L2 data. It includes python re-implementation of the popular [SHBundle](https://www.gis.uni-stuttgart.de/en/research/downloads/shbundle/) and [DataDrivenCorrection Bundle](https://www.gis.uni-stuttgart.de/en/research/downloads/datadrivencorrectionbundle/) tools originally written using MATLAB. 
 
 
 ## Usage
 
 1. Read and Load level-2 spherical harmonic data
 2. Create basin time series for TWS
 3. Perform grace data driven correction
 4. Plot spherical harmonic related plots
 
 ## 1. How to install <br>
 ### 1.1 For Users
-Currently the package is not yet finalized hence the version on PyPI is outdated and should not be used (as of now). Please follow the steps mentioned in the following section till things are finalized. <br>
-
-### 1.2 Till things get finalized
-
-1.  Fork the pyshbundle repo on GitHub.
-
-2.  Clone your fork locally:
-
-    ```shell
-    $ git clone git@github.com:your_name_here/pyshbundle.git
-    ```
-
-3.  Create a new virtual environment or conda environment to install all the necessary dependencies. using `conda` is recommended along with `jupyter lab`. Use of python 3.x is recommended
-
-    ```shell
-    $ conda create -n pyshbundle-env
-    $ conda activate pyshbundle-env
-    $ conda install -c conda-forge --file requirements_dev.txt -y
-    ```
-4. Note that the base path to the entire repo is important while importing (this is tempoary only, after PyPi module gets updated this approach will not be required) 
-   ```
-   Example base repo path -> ../open_source/pyshbundle
-
-   pyshbundle (base container repo)
-    | - pyshbundle (codes and functions reside here)
-        | - all the codes
-    | - notebooks
-    | - docs
-    | - and rest of the other folders
-   ```
-
-5. In order to use any of the functions change the current directory to the pyshbundle (base repo) then use import as usual
-   ```python
-   import os
-   os.chdir(../open_source/pyshbundle)
-
-   import pyshbundle
-   # or import individual functions
-   from pyshbundle import read_jpl
-   ```
-   after importing the fucntions this way you are all good to go.
+The module can be installed via pip python package manager. Follow the follwing steps to setup a virtual environment and start exploring the GRACE Gravity Field data.
 
+```shell
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+# install package into virtual environment
+$ pip install pyshbundle
+
+# clone the repository in order to access the notebooks and data
+$ git clone https://github.com/mn5hk/pyshbundle.git
+```
+
+### 1.2 For Devs/Contributors
+Developers can access the latest development branch and 
+```shell
+# clone the repo and fetch the dev branch
+$ git clone https://github.com/mn5hk/pyshbundle.git
+
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+
+# install the dependencies from the requirements-dev file
+$ pip install -r ../pyshbundle/requirements-dev.txt
+
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+
+# install package into virtual environment
+$ pip install ../pyshbundle/dist/<required-version>.tzr.gz
+
+# you also have the option to build the module using, be careful of 
+$ python setup.py sdist
+```
 
 ## Read the Docs
 
-Please find the docs here - [PySHBundle](https://abhimhamane.github.io/pyshbundle/)
+Please find the docs here - [PySHBundle](https://mn5hk.github.io/pyshbundle/)
 
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
@@ -130,20 +121,14 @@
 
 If you are proposing a feature:
 
 -   Explain in detail how it would work.
 -   Keep the scope as narrow as possible, to make it easier to implement.
 -   Remember that this is a volunteer-driven project, and that contributions are welcome :)
 
-## Known Issues
-
-1. New implementation of reading data has some bug. It works for CSR but not properly properly for JPL and ITSG sources. For more information check the current issues.
-2. There is some inconsistency related to importing functions it is recommended to always use `import pyshbundle` along with any of the targeted imports you want.
-
-
 ## License Statement
 
 This file is part of PySHbundle. <br>
     PySHbundle is free software: you can redistribute it and/or modify<br>
     it under the terms of the GNU General Public License as published by<br>
     the Free Software Foundation, either version 3 of the License, or<br>
     (at your option) any later version.<br>
```

### Comparing `pyshbundle-0.2/README.md` & `pyshbundle-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,63 @@
-# PySHbundle: A Python implementation of MATLAB codes SHbundle <br>
+# PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle <br>
 
 ![](https://visitor-badge.glitch.me/badge?page_id=mn5hk.mat2py) <br>
 
 
-PySHBundle is the python implementation of the popular SHBundle toolbox originally written using MATLAB. 
-
-TODO: Badges and and banner for the project
+PySHBundle is a tool to process GRACE L2 data. It includes python re-implementation of the popular [SHBundle](https://www.gis.uni-stuttgart.de/en/research/downloads/shbundle/) and [DataDrivenCorrection Bundle](https://www.gis.uni-stuttgart.de/en/research/downloads/datadrivencorrectionbundle/) tools originally written using MATLAB. 
 
 
 ## Usage
 
 1. Read and Load level-2 spherical harmonic data
 2. Create basin time series for TWS
 3. Perform grace data driven correction
 4. Plot spherical harmonic related plots
 
 ## 1. How to install <br>
 ### 1.1 For Users
-Currently the package is not yet finalized hence the version on PyPI is outdated and should not be used (as of now). Please follow the steps mentioned in the following section till things are finalized. <br>
-
-### 1.2 Till things get finalized
-
-1.  Fork the pyshbundle repo on GitHub.
-
-2.  Clone your fork locally:
-
-    ```shell
-    $ git clone git@github.com:your_name_here/pyshbundle.git
-    ```
-
-3.  Create a new virtual environment or conda environment to install all the necessary dependencies. using `conda` is recommended along with `jupyter lab`. Use of python 3.x is recommended
-
-    ```shell
-    $ conda create -n pyshbundle-env
-    $ conda activate pyshbundle-env
-    $ conda install -c conda-forge --file requirements_dev.txt -y
-    ```
-4. Note that the base path to the entire repo is important while importing (this is tempoary only, after PyPi module gets updated this approach will not be required) 
-   ```
-   Example base repo path -> ../open_source/pyshbundle
-
-   pyshbundle (base container repo)
-    | - pyshbundle (codes and functions reside here)
-        | - all the codes
-    | - notebooks
-    | - docs
-    | - and rest of the other folders
-   ```
-
-5. In order to use any of the functions change the current directory to the pyshbundle (base repo) then use import as usual
-   ```python
-   import os
-   os.chdir(../open_source/pyshbundle)
-
-   import pyshbundle
-   # or import individual functions
-   from pyshbundle import read_jpl
-   ```
-   after importing the fucntions this way you are all good to go.
+The module can be installed via pip python package manager. Follow the follwing steps to setup a virtual environment and start exploring the GRACE Gravity Field data.
 
+```shell
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+# install package into virtual environment
+$ pip install pyshbundle
+
+# clone the repository in order to access the notebooks and data
+$ git clone https://github.com/mn5hk/pyshbundle.git
+```
+
+### 1.2 For Devs/Contributors
+Developers can access the latest development branch and 
+```shell
+# clone the repo and fetch the dev branch
+$ git clone https://github.com/mn5hk/pyshbundle.git
+
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+
+# install the dependencies from the requirements-dev file
+$ pip install -r ../pyshbundle/requirements-dev.txt
+
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+
+# install package into virtual environment
+$ pip install ../pyshbundle/dist/<required-version>.tzr.gz
+
+# you also have the option to build the module using, be careful of 
+$ python setup.py sdist
+```
 
 ## Read the Docs
 
-Please find the docs here - [PySHBundle](https://abhimhamane.github.io/pyshbundle/)
+Please find the docs here - [PySHBundle](https://mn5hk.github.io/pyshbundle/)
 
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
@@ -108,20 +99,14 @@
 
 If you are proposing a feature:
 
 -   Explain in detail how it would work.
 -   Keep the scope as narrow as possible, to make it easier to implement.
 -   Remember that this is a volunteer-driven project, and that contributions are welcome :)
 
-## Known Issues
-
-1. New implementation of reading data has some bug. It works for CSR but not properly properly for JPL and ITSG sources. For more information check the current issues.
-2. There is some inconsistency related to importing functions it is recommended to always use `import pyshbundle` along with any of the targeted imports you want.
-
-
 ## License Statement
 
 This file is part of PySHbundle. <br>
     PySHbundle is free software: you can redistribute it and/or modify<br>
     it under the terms of the GNU General Public License as published by<br>
     the Free Software Foundation, either version 3 of the License, or<br>
     (at your option) any later version.<br>
```

### Comparing `pyshbundle-0.2/pyshbundle/GRACE_Data_Driven_Correction_Vishwakarma.py` & `pyshbundle-1.0.0/pyshbundle/GRACE_Data_Driven_Correction_Vishwakarma.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,17 @@
 
 import numpy as np
 import numpy.matlib as npm
 import scipy as sc
 import scipy.io
 #CS2SC, gsha, gshs, gaussian
 
-from pyshbundle.gaussian import Gaussian
-from pyshbundle.cs2sc import cs2sc
-from pyshbundle.gshs import GSHS
-from pyshbundle.gsha import gsha
-from pyshbundle.naninterp import naninterp
-from pyshbundle.Phase_calc import PhaseCalc
+from pyshbundle.conv_sh import cs2sc
+from pyshbundle.pysh_core import GSHS, gsha, PhaseCalc
+from pyshbundle.shutils import naninterp, Gaussian
 
 def deg_to_rad(deg: float):
     """Converts angle from degree to radian
 
     Args:
         deg (float): Angle in degree
 
@@ -143,15 +140,15 @@
     l = f[0][0].shape[0]
     cfield = f[0][0].shape[1]
     if cfield == l:
         flag_cs = 0
     else:
         flag_cs = 1
 
-    Weights = gaussian(l-1, GaussianR) 
+    Weights = Gaussian(l-1, GaussianR) 
     #gaussian returns weights as a list #gaussian is np.array()
     
     try: #Broadcase Weights into dimensions
         filter_ = np.ones([1,(2*(l-1))+1]) * Weights
     except:
         w0 = Weights.shape[0]
         Weights = Weights.reshape(w0,1)
@@ -163,16 +160,16 @@
         for m in range(r):
             if flag_cs == 0:
                 Ft = cs2sc(f[m][0]).astype('longdouble') 
             else:
                 Ft = f[m][0].astype('longdouble') 
                 
            
-            fFld__, _, _ = gshs(Ft * filter_, qty, 'cell', int(180/deg), 0, 0) 
-            ffFld__, _, _ = gshs((Ft * filter_ * filter_), qty, 'cell', int(180/deg), 0, 0)
+            fFld__, _, _ = GSHS(Ft * filter_, qty, 'cell', int(180/deg), 0, 0) 
+            ffFld__, _, _ = GSHS((Ft * filter_ * filter_), qty, 'cell', int(180/deg), 0, 0)
             
             if m == 0:
                 fFld = np.zeros((r,fFld__.shape[0],fFld__.shape[1]), dtype = 'longdouble') 
                 ffFld = np.zeros((r, ffFld__.shape[0], ffFld__.shape[1]), dtype = 'longdouble')
                 
             fFld[m] = fFld__
             ffFld[m] = ffFld__
@@ -208,15 +205,15 @@
     for rbasin in range(0, cid):
         #Get the basin functions ready
        
         #Basin functions, filtered basin function and transfer function Kappa
         Rb = basins[rbasin][0] 
         csRb = gsha(Rb, 'mean', 'block', long/2) 
         csF = cs2sc(csRb[0:l, 0:l]) 
-        filRb_ = gshs(csF * filter_, 'none', 'cell', int(long/2), 0, 0) 
+        filRb_ = GSHS(csF * filter_, 'none', 'cell', int(long/2), 0, 0) 
         filRb = filRb_[0]
         kappa = (1-Rb) * filRb
          
         
     
         fF = np.zeros((fFld__.shape[0],fFld__.shape[1]), dtype = 'longdouble')
         ffF = np.zeros((fFld__.shape[0],fFld__.shape[1]), dtype = 'longdouble')
@@ -276,15 +273,15 @@
     
     multp = npm.repmat(b, r, 1) 
     devint = bfDevRegAv * multp
     multp = npm.repmat(bl, r, 1)
     leakLS = tsleaktotalf * multp
     
     
-    ps = Phase_calc(tsleaktotalf,tsleaktotalff)
+    ps = PhaseCalc(tsleaktotalf,tsleaktotalff)
     
     
     
     #Compute the near true leakage
     
     for i in range(0, cid):   
         ftsleaktotal[:,i] = naninterp(tsleaktotalf[:,i]) #Replaces gaps (NaN values) with an itnerpolated value in the leakage time series from once filtered fields
```

### Comparing `pyshbundle-0.2/pyshbundle/GRACEconstants.py` & `pyshbundle-1.0.0/pyshbundle/GRACEconstants.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/GRACEpy.py` & `pyshbundle-1.0.0/pyshbundle/GRACEpy.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/Phase_calc.py` & `pyshbundle-1.0.0/pyshbundle/Phase_calc.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/__init__.py` & `pyshbundle-1.0.0/pyshbundle/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,75 +35,65 @@
     Downscaling GRACE total water storage change using 
     partial least squares regression. Scientific data, 8(1), 95.
     https://doi.org/10.1038/s41597-021-00862-6 
     """
 
 __author__ = """Amin Shakya"""
 __email__ = 'aminshk50@gmail.com'
-__version__ = '0.1.0'
+__version__ = '0.2.1'
 
 # __init__.py with initialization code
-print("Initializing PySHbundle v0.0.1")
+print("Initializing PySHbundle v0.2.1")
 
 # __init__.py with __all__
-__all__ = ['basin_avg', 
-           'clm2cs',
-           'clm2sc',
-           'eigengrav',
-           'gaussian',
-           'GRACE_Data_Driven_Correction_Vishwakarma',
-           'GRACEpy',
-           'grule',
-           'gsha',
-           'gshs',
-           'iplm',
-           'ispec',
-           'klm2sc',
+__all__ = ['GRACEpy',
            'load_longterm_mean',
-           'naninterp',
-           'neumann',
-           'new_io',
-           'normalklm',
-           'Phase_calc',
-           'plm',
+           'io',
            'read_GRACE_SH_paths',
            'reader_replacer',
            'reader_replacer_csr',
            'reader_replacer_itsg',
            'reader_replacer_jpl',
-           'sc2cs',
-           'tws_cal',
-           'visualisation_utils']
+           'viz_utils',
+           'conv_sh',
+           'shutils',
+           'hydro',
+           'pysh_core'
+           ]
 
 #Import individual modules
-from .basin_avg import BasinAvg
-from .clm2cs import clm2cs, clm2cs_new
-from .clm2sc import clm2sc, clm2sc_new
+#from .basin_avg import BasinAvg
+#from .clm2cs import clm2cs
+#from .clm2sc import clm2sc
 # from .delta_sc import eigengrav
-from .eigengrav import eigengrav
-from .gaussian import Gaussian
-from .GRACE_Data_Driven_Correction_Vishwakarma import deg_to_rad, GRACE_Data_Driven_Correction_Vishwakarma
+#rom .eigengrav import eigengrav
+#from .gaussian import Gaussian
+#from .GRACE_Data_Driven_Correction_Vishwakarma import deg_to_rad, GRACE_Data_Driven_Correction_Vishwakarma
 # from .GRACEconstants import 
 from .GRACEpy import upwcon, lovenr, lovenrPREM
-from .grule import grule
-from .gsha import gsha
-from .gshs import GSHS
-from .iplm import iplm
-from .ispec import ispec
-from .klm2sc import klm2sc #, klm2sc_new
+#from .grule import grule
+#from .gsha import gsha
+#from .gshs import GSHS
+#from .iplm import iplm
+#from .ispec import ispec
+#from .klm2sc import klm2sc #, klm2sc_new
 from .load_longterm_mean import load_longterm_mean
-from .naninterp import naninterp
-from .neumann import neumann
-from .new_io import clm2cs_new, read_jpl, parse_jpl_header, parse_jpl_data, parse_lines, read_csr, find_word, parse_csr_header, parse_csr_data, read_itsg, parse_itsg_header, parse_itsg_data, read_tn13, parse_tn13_header, parse_tn13_data, read_tn14, parse_tn14_header, parse_tn14_data, find_date_in_replacemnt_file, extract_C10_11_replcmnt_coeff, extract_C20_replcmnt_coeff, extract_C30_replcmnt_coeff, replace_zonal_coeff, klm2sc_new, sub2ind, cklm2sc_new, check_format
-from .normalklm import normalklm
-from .Phase_calc import PhaseCalc
-from .plm import PLM, secrecur, lrecur, derivALF
+#from .naninterp import naninterp
+#from .neumann import neumann
+from .io import read_jpl, parse_jpl_header, parse_jpl_data, parse_lines, read_csr, parse_csr_header, parse_csr_data, read_itsg, parse_itsg_header, parse_itsg_data, read_tn13, parse_tn13_header, parse_tn13_data, read_tn14, parse_tn14_header, parse_tn14_data, find_date_in_replacemnt_file, extract_C10_11_replcmnt_coeff, extract_C20_replcmnt_coeff, extract_C30_replcmnt_coeff, replace_zonal_coeff, cklm2sc_new, check_format
+#from .normalklm import normalklm
+#from .Phase_calc import PhaseCalc
+#from .plm import PLM, secrecur, lrecur, derivALF
 # from .pyshbundle import 
 from .read_GRACE_SH_paths import read_GRACE_SH_paths
 from .reader_replacer import reader, TIME, last_4chars, reader_replacer
 from .reader_replacer_csr import reader_replacer_csr 
 from .reader_replacer_itsg import reader_replacer_itsg 
 from .reader_replacer_jpl import reader_replacer_jpl
-from .sc2cs import sc2cs
-from .tws_cal import TWSCalc
+#from .sc2cs import sc2cs
+from .conv_sh import sc2cs, clm2cs, clm2sc, cs2sc, klm2sc
+#from .tws_cal import TWSCalc
 # from .tws_py import 
-from .visualisation_utils import sc_triplot, cs_sqplot, polar_plot, mapfield, ylm, ylm_plot, gshs_prepare
+from .hydro import TWSCalc, BasinAvg
+from .shutils import PLM, iplm, ispec, eigengrav, grule, Gaussian, neumann, naninterp, normalklm
+from .pysh_core import GSHS, gsha, GRACE_Data_Driven_Correction_Vishwakarma, PhaseCalc
+from .viz_utils import sc_triplot, cs_sqplot, polar_plot, mapfield, ylm, ylm_plot, gshs_prepare
```

### Comparing `pyshbundle-0.2/pyshbundle/basin_avg.py` & `pyshbundle-1.0.0/pyshbundle/basin_avg.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/clm2cs.py` & `pyshbundle-1.0.0/pyshbundle/clm2cs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,17 @@
 
 
 import numpy as np
 from pyshbundle.sc2cs import sc2cs
 from pyshbundle.clm2sc import clm2sc
 
 # CLM to C|S format
+'''
 def clm2cs(data):
-    """_summary_
+    """[Depricated]
 
     Args:
         data (_type_): _description_
     
     Suggestion: 
         Instead of printing "conversion complete" let's show a progress bar
     """
@@ -87,16 +88,17 @@
                     cs_mat[month,index4,index3] = slm[year][j+1 +tile*4752]
                     j = j + 1
                 j = j + 1
             month = month + 1
     print('Conversion into clm format complete')        
     #np.save('/path/SH_coeff_cs.npy', cs_mat)
     return cs_mat
+'''
 
-def clm2cs_new(data_mat: np.ndarray, lmax: int, sigma_flag=False):
+def clm2cs(data_mat: np.ndarray, lmax: int, sigma_flag=False):
     """Converts the format from CLM to |C\S|
     Under the hood uses the `clm2sc` and `sc2cs` function
 
     Args:
         data_mat (numpy.ndarray): list containing [degree;  order; clm; slm; delta clm; delta slm; start data; end date]
         lmax (int): Max Degree of the spherical harmonic expansion
         sigma_flag (boolean): Flag to return the standard deviation data in |C\S| format or not. Defaults to False
```

### Comparing `pyshbundle-0.2/pyshbundle/clm2sc.py` & `pyshbundle-1.0.0/pyshbundle/clm2sc.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,17 @@
 #       https://doi.org/10.1038/s41597-021-00862-6
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
 
 import numpy as np
 from tqdm import tqdm
 
 # CLM to /S|C\
+'''
 def clm2sc(data):
-    """Converts the spherical harmonic coefficients from clm format to /S|C\ format
+    """[Deprecated/Not required]Converts the spherical harmonic coefficients from clm format to /S|C\ format
 
     Args:
         data (list): list containing [degree;  order; clm; slm; delta clm; delta slm; start data; end date]
 
     Returns:
         np.ndarray: Spherical Harmonic Coefficients in /S|C\ format [[files or months]; [2-D matrix of /S|C\ format]]
         np.ndarray: Standard Deviations of correcponding Spherical Harmonic Coefficients in /S|C\ format [[files or months]; [2-D matrix of /S|C\ format]]
@@ -102,33 +103,31 @@
     # delete order 0 column
     sc_mat = np.delete(sc_mat, Lmax, 2)
     dev_sc_mat = np.delete(dev_sc_mat, Lmax, 2)
     print('Conversion into clm format complete')
     return sc_mat, dev_sc_mat
 
 # mean=np.mean(sc_mat[18:102], axis=0)
+'''
 
-
-def clm2sc_new(data_mat: np.ndarray, lmax: int, sigma_flag=False):
+def clm2sc(data_mat: np.ndarray, lmax: int, sigma_flag=False):
     """Converts the spherical harmonic coefficients from clm format to /S|C\ format
 
     Args:
         data_mat (numpy.ndarray): list containing [degree;  order; clm; slm; delta clm; delta slm; start data; end date]
         lmax (int): Max Degree of the spherical harmonic expansion
         sigma_flag (boolean): Flag to return the standard deviation data in /S|C\ format or not. Defaults to False
 
     Returns:
         numpy.ndarray: Spherical Harmonic Coefficients in /S|C\ format
     
     References:
         Refer to the SHBundle or PySHBundle docs for the different data storage and retrival formats.
     
-    """
-
-    
+    """    
 
     sc_mat = np.zeros((lmax+1, 2*lmax + 2))
     dev_sc_mat = np.zeros((lmax+1, 2*lmax + 2))
     
     # as per the convention
     clm = data_mat[:, 2]
     slm = data_mat[:, 3]
```

### Comparing `pyshbundle-0.2/pyshbundle/cs2sc.py` & `pyshbundle-1.0.0/pyshbundle/cs2sc.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/eigengrav.py` & `pyshbundle-1.0.0/pyshbundle/eigengrav.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/gaussian.py` & `pyshbundle-1.0.0/pyshbundle/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/grule.py` & `pyshbundle-1.0.0/pyshbundle/grule.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/gsha.py` & `pyshbundle-1.0.0/pyshbundle/gsha.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 import numpy as np
 from pyshbundle.neumann import neumann
 from pyshbundle.plm import PLM
 from scipy import sparse
 from scipy import linalg
 from pyshbundle.iplm import iplm
-from pyshbundle.sc2cs import sc2cs
+from pyshbundle.convert_sh_fmt import sc2cs
 
 def gsha(f, method: str, grid: str = None, lmax: int = -9999):
     """ GSHA - Global Spherical Harmonic Analysis
 
     Args:
         f (np.ndarray): global field of size $(l_{max} + 1) * 2 * l_{max}$ or $l_{max} * 2 * l_{max}$
         method (str): method to be used
```

### Comparing `pyshbundle-0.2/pyshbundle/gshs.py` & `pyshbundle-1.0.0/pyshbundle/gshs.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 #       https://doi.org/10.1038/s41597-021-00862-6
 
 # @author: Amin Shakya, Interdisciplinary Center for Water Research (ICWaR), Indian Institute of Science (IISc)
 
 import numpy as np
 from os import chdir, getcwd
 
-from pyshbundle.cs2sc import cs2sc
+from pyshbundle.convert_sh_fmt import cs2sc
 from pyshbundle.normalklm import normalklm
 from pyshbundle.plm import PLM
 from pyshbundle.eigengrav import eigengrav
 from pyshbundle.ispec import ispec
 
 def GSHS(field, quant = 'none', grd = 'mesh', n = -9999, h = 0, jflag = 1):
     """GSHS - Global Spherical Harmonic Synthesis
```

### Comparing `pyshbundle-0.2/pyshbundle/iplm.py` & `pyshbundle-1.0.0/pyshbundle/iplm.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/ispec.py` & `pyshbundle-1.0.0/pyshbundle/ispec.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 #       partial least squares regression. Scientific data, 8(1), 95.
 #       https://doi.org/10.1038/s41597-021-00862-6
 
 # @author: Amin Shakya, Interdisciplinary Center for Water Research (ICWaR), Indian Institute of Science (IISc)
 
 import numpy as np
 import scipy
-import scipy.fft
+from scipy.fft import ifft
 
 def ispec(a,b = -9999):
     """Returns the function F from the spectra A and B
 
     Args:
         a (_type_): cosine coefficients
         b (int, optional): sine coefficients. Defaults to -9999.
@@ -96,13 +96,13 @@
         fs  = (np.concatenate((fs,np.conj(fs[np.arange(n2-2,0,-1),:])), axis = 0))*max(n,1)
 
     else:
         n = 2 * n2 - 1                        
         fs = (a - 1j * b)/2
         fs = (np.concatenate((fs,np.conj(fs[np.arange(n2-1,0,-1),:])), axis = 0))*n
 
-    f = np.real(scipy.fft.ifft(fs.T).T)
+    f = np.real(ifft(fs.T).T)
     return f
```

### Comparing `pyshbundle-0.2/pyshbundle/klm2sc.py` & `pyshbundle-1.0.0/pyshbundle/klm2sc.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/load_longterm_mean.py` & `pyshbundle-1.0.0/pyshbundle/load_longterm_mean.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/naninterp.py` & `pyshbundle-1.0.0/pyshbundle/naninterp.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/neumann.py` & `pyshbundle-1.0.0/pyshbundle/neumann.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/new_io.py` & `pyshbundle-1.0.0/pyshbundle/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 # new implementationhek for reading files - combining some asspects from existing reader_replacer codes
 # Author: Abhishek Mhamane, MS-Research Geoinformatics, IIT Kanpur
 
 
 import julian
 import gzip
-import os
 import re
+import pkg_resources
 
 import numpy as np
 from copy import deepcopy
-from tqdm import tqdm, trange
 from datetime import datetime, timedelta
 
-from pyshbundle.sc2cs import sc2cs
-from pyshbundle.clm2sc import clm2sc
-
-
+'''
 def clm2cs_new(data):
     """This is an other implementation of clm2cs which uses the clm2sc and then converts using
     sc2cs functions
     
     Args:
         data (_type_): _description_
     
@@ -39,15 +35,15 @@
     devcs_mat = np.zeros((num_files, r, r))
 
     for ith_file in range(num_files):
         cs_mat[ith_file, :, :] = sc2cs(sc_mat[ith_file, :, :])
         devcs_mat[ith_file, :, :] = sc2cs(devsc_mat[ith_file, :, :])
 
     return cs_mat, devcs_mat
-
+'''
 
 def read_jpl(file_path: str):
     """Reads the spherical harmonic data provided by JPL
 
     Args:
         file_path (str): Absolute path to the file
     
@@ -1104,14 +1100,15 @@
         data_mat_copy[3, :] = C20
         data_mat_copy[2, :] = C11
         data_mat_copy[1, :] = C10
 
     return data_mat_copy
 
 
+'''
 def klm2sc_new(data_mat, lmax: int):
     sc_mat = np.zeros((lmax+1, 2*lmax + 2))
     dev_sc_mat = np.zeros((lmax+1, 2*lmax + 2))
     clm = data_mat[:, 2]
     slm = data_mat[:, 3]
     clm_std_dev = data_mat[:, 4]
     slm_std_dev = data_mat[:, 5]
@@ -1127,16 +1124,15 @@
         
         index2 = index2 + lmax-index1+1
 
     sc_mat=np.delete(sc_mat,lmax,axis=1)
     dev_sc_mat=np.delete(dev_sc_mat,lmax,axis=1)
 
     return sc_mat, dev_sc_mat
-
-
+'''
 
 def sub2ind(array_shape, rows, cols):
     # rows, list need to be linear array
     return rows*array_shape[1] + cols
 
 
 def cklm2sc_new(clm_mat, lmax: int):
@@ -1198,10 +1194,49 @@
 
     scmat = flat_sc.reshape(shape_sc)
 
     # with one flag include for
 
     return scmat, dev_scmat
 
+
 def check_format(scmat):
     
-    pass
+    raise NotImplementedError()
+
+def load_longterm_mean(source = "", use_sample_mean = 0):
+    """_summary_
+
+    Args:
+        source (str, optional): _description_. Defaults to "".
+        use_sample_mean (int, optional): _description_. Defaults to 0.
+
+    Raises:
+        Exception: _description_
+
+    Returns:
+        _type_: _description_
+    
+    Todo:
+        + Not sure if using "source = ''" is all right
+        + instead of base eception is can be ValueError
+    """
+    if use_sample_mean == 1:
+        print("Loading preloaded RL06 long term mean values")
+        print("Please ensure that your data is RL06 \nIf not, please manually input long term mean by setting use_sample_mean = 0")
+
+        if str.upper(source) == 'CSR':
+            long_mean = pkg_resources.resource_filename('pyshbundle', 'data/RL06_long_mean/SH_long_mean_csr.npy')
+        elif str.upper(source) == 'JPL':
+            long_mean = pkg_resources.resource_filename('pyshbundle', 'data/RL06_long_mean/SH_long_mean_itsg.npy')
+        elif str.upper(source) == 'ITSG':
+            long_mean = pkg_resources.resource_filename('pyshbundle', 'data/RL06_long_mean/SH_long_mean_jpl.npy')
+        else:
+            raise Exception("Incorrect selection of source")
+        print("Successfully loaded preloaded longterm means")
+    else:
+        print("Please download and provide the longterm GRACE SH mean values")
+        print("Instructions to download the longterm GRACE SH mean values may be referred to in https://github.com/mn5hk/pyshbundle/blob/main/docs/index.md#how-to-download-data")
+        long_mean = str(input("Enter the longterm mean for the SH values in the numpy (.npy) format"))
+        print("Successfully loaded path to long term mean:", long_mean)
+
+    return long_mean
```

### Comparing `pyshbundle-0.2/pyshbundle/normalklm.py` & `pyshbundle-1.0.0/pyshbundle/normalklm.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/plm.py` & `pyshbundle-1.0.0/pyshbundle/plm.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/pyshbundle.py` & `pyshbundle-1.0.0/pyshbundle/pyshbundle.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/read_GRACE_SH_paths.py` & `pyshbundle-1.0.0/pyshbundle/read_GRACE_SH_paths.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/reader_replacer.py` & `pyshbundle-1.0.0/pyshbundle/reader_replacer.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/reader_replacer_csr.py` & `pyshbundle-1.0.0/pyshbundle/reader_replacer_csr.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/reader_replacer_itsg.py` & `pyshbundle-1.0.0/pyshbundle/reader_replacer_itsg.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/reader_replacer_jpl.py` & `pyshbundle-1.0.0/pyshbundle/reader_replacer_jpl.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/sc2cs.py` & `pyshbundle-1.0.0/pyshbundle/sc2cs.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/tws_cal.py` & `pyshbundle-1.0.0/pyshbundle/tws_cal.py`

 * *Files identical despite different names*

### Comparing `pyshbundle-0.2/pyshbundle/visualisation_utils.py` & `pyshbundle-1.0.0/pyshbundle/viz_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 # Visualisation Utilities for PySHBundle
 # Author: Abhishek Mhamane, MS-Research Geoinformatics, IIT Kanpur (India)
 # 
 
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-import matplotlib as mpl
 import matplotlib.path as mpath
 import matplotlib.pyplot as plt
 import numpy as np
-import cartopy
 import cartopy.crs as ccrs
 
-import pyshbundle
-from pyshbundle.clm2cs import clm2cs, clm2cs_new
-from pyshbundle.sc2cs import sc2cs
-from pyshbundle.plm import PLM
-from pyshbundle.gshs import GSHS
+from pyshbundle.shutils import PLM
+from pyshbundle.pysh_core import GSHS
 
 def sc_triplot(scmat: np.ndarray, lmax: int, title: str, vmin, vmax):
     """Visualize the SH coeff. in /S|C\ triangular matrix format
 
     Args:
         scmat (np.ndarray): /S|C\ matrix data (see clm2sc)
         lmax (int): maximum degree of SH expansion
@@ -284,14 +279,28 @@
     ax.coastlines()
 
     plt.colorbar(im, orientation='vertical', shrink=0.85, pad=0.02,label=f"[...]")
 
     plt.title(f"Visualization of Spherical Harmonics - degree: {l} order: {m}")
 
 def gshs_prepare(lmax, gs, quant, grd, h, jflag, sc_coeff):
+    """_summary_
+
+    Args:
+        lmax (_type_): _description_
+        gs (_type_): _description_
+        quant (_type_): _description_
+        grd (_type_): _description_
+        h (_type_): _description_
+        jflag (_type_): _description_
+        sc_coeff (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
     n = int(180/gs)
     
     grid_y = int(180/gs)
     grid_x = int(360/gs)
 
     ff = GSHS(sc_coeff, quant, grd, n, h, jflag)[0]
```

### Comparing `pyshbundle-0.2/pyshbundle.egg-info/PKG-INFO` & `pyshbundle-1.0.0/pyshbundle.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyshbundle
-Version: 0.2
-Summary: PySHbundle: A Python implementation of MATLAB codes SHbundle
+Version: 1.0.0
+Summary: PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle
 Home-page: https://github.com/mn5hk/pyshbundle
 Author: Amin Shakya
 Author-email: aminshk50@gmail.com
 License: GNU General Public License v3
 Keywords: pyshbundle
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,79 +16,70 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PySHbundle: A Python implementation of MATLAB codes SHbundle <br>
+# PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle <br>
 
 ![](https://visitor-badge.glitch.me/badge?page_id=mn5hk.mat2py) <br>
 
 
-PySHBundle is the python implementation of the popular SHBundle toolbox originally written using MATLAB. 
-
-TODO: Badges and and banner for the project
+PySHBundle is a tool to process GRACE L2 data. It includes python re-implementation of the popular [SHBundle](https://www.gis.uni-stuttgart.de/en/research/downloads/shbundle/) and [DataDrivenCorrection Bundle](https://www.gis.uni-stuttgart.de/en/research/downloads/datadrivencorrectionbundle/) tools originally written using MATLAB. 
 
 
 ## Usage
 
 1. Read and Load level-2 spherical harmonic data
 2. Create basin time series for TWS
 3. Perform grace data driven correction
 4. Plot spherical harmonic related plots
 
 ## 1. How to install <br>
 ### 1.1 For Users
-Currently the package is not yet finalized hence the version on PyPI is outdated and should not be used (as of now). Please follow the steps mentioned in the following section till things are finalized. <br>
-
-### 1.2 Till things get finalized
-
-1.  Fork the pyshbundle repo on GitHub.
-
-2.  Clone your fork locally:
-
-    ```shell
-    $ git clone git@github.com:your_name_here/pyshbundle.git
-    ```
-
-3.  Create a new virtual environment or conda environment to install all the necessary dependencies. using `conda` is recommended along with `jupyter lab`. Use of python 3.x is recommended
-
-    ```shell
-    $ conda create -n pyshbundle-env
-    $ conda activate pyshbundle-env
-    $ conda install -c conda-forge --file requirements_dev.txt -y
-    ```
-4. Note that the base path to the entire repo is important while importing (this is tempoary only, after PyPi module gets updated this approach will not be required) 
-   ```
-   Example base repo path -> ../open_source/pyshbundle
-
-   pyshbundle (base container repo)
-    | - pyshbundle (codes and functions reside here)
-        | - all the codes
-    | - notebooks
-    | - docs
-    | - and rest of the other folders
-   ```
-
-5. In order to use any of the functions change the current directory to the pyshbundle (base repo) then use import as usual
-   ```python
-   import os
-   os.chdir(../open_source/pyshbundle)
-
-   import pyshbundle
-   # or import individual functions
-   from pyshbundle import read_jpl
-   ```
-   after importing the fucntions this way you are all good to go.
+The module can be installed via pip python package manager. Follow the follwing steps to setup a virtual environment and start exploring the GRACE Gravity Field data.
 
+```shell
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+# install package into virtual environment
+$ pip install pyshbundle
+
+# clone the repository in order to access the notebooks and data
+$ git clone https://github.com/mn5hk/pyshbundle.git
+```
+
+### 1.2 For Devs/Contributors
+Developers can access the latest development branch and 
+```shell
+# clone the repo and fetch the dev branch
+$ git clone https://github.com/mn5hk/pyshbundle.git
+
+# creating a new virtual environment
+$ python3 -m venv <name-env>
+
+# install the dependencies from the requirements-dev file
+$ pip install -r ../pyshbundle/requirements-dev.txt
+
+# activate the virtual environment environment
+$ source </location-of-virt-env/name-env/bin/activate>
+
+# install package into virtual environment
+$ pip install ../pyshbundle/dist/<required-version>.tzr.gz
+
+# you also have the option to build the module using, be careful of 
+$ python setup.py sdist
+```
 
 ## Read the Docs
 
-Please find the docs here - [PySHBundle](https://abhimhamane.github.io/pyshbundle/)
+Please find the docs here - [PySHBundle](https://mn5hk.github.io/pyshbundle/)
 
 
 ## Contributing
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
@@ -130,20 +121,14 @@
 
 If you are proposing a feature:
 
 -   Explain in detail how it would work.
 -   Keep the scope as narrow as possible, to make it easier to implement.
 -   Remember that this is a volunteer-driven project, and that contributions are welcome :)
 
-## Known Issues
-
-1. New implementation of reading data has some bug. It works for CSR but not properly properly for JPL and ITSG sources. For more information check the current issues.
-2. There is some inconsistency related to importing functions it is recommended to always use `import pyshbundle` along with any of the targeted imports you want.
-
-
 ## License Statement
 
 This file is part of PySHbundle. <br>
     PySHbundle is free software: you can redistribute it and/or modify<br>
     it under the terms of the GNU General Public License as published by<br>
     the Free Software Foundation, either version 3 of the License, or<br>
     (at your option) any later version.<br>
```

### Comparing `pyshbundle-0.2/pyshbundle.egg-info/SOURCES.txt` & `pyshbundle-1.0.0/pyshbundle.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,42 @@
 pyshbundle/GRACEconstants.py
 pyshbundle/GRACEpy.py
 pyshbundle/Phase_calc.py
 pyshbundle/__init__.py
 pyshbundle/basin_avg.py
 pyshbundle/clm2cs.py
 pyshbundle/clm2sc.py
+pyshbundle/conv_sh.py
 pyshbundle/cs2sc.py
 pyshbundle/eigengrav.py
 pyshbundle/gaussian.py
 pyshbundle/grule.py
 pyshbundle/gsha.py
 pyshbundle/gshs.py
+pyshbundle/hydro.py
+pyshbundle/io.py
 pyshbundle/iplm.py
 pyshbundle/ispec.py
 pyshbundle/klm2sc.py
 pyshbundle/load_longterm_mean.py
 pyshbundle/naninterp.py
 pyshbundle/neumann.py
-pyshbundle/new_io.py
 pyshbundle/normalklm.py
 pyshbundle/plm.py
+pyshbundle/pysh_core.py
 pyshbundle/pyshbundle.py
 pyshbundle/read_GRACE_SH_paths.py
 pyshbundle/reader_replacer.py
 pyshbundle/reader_replacer_csr.py
 pyshbundle/reader_replacer_itsg.py
 pyshbundle/reader_replacer_jpl.py
 pyshbundle/sc2cs.py
+pyshbundle/shutils.py
 pyshbundle/tws_cal.py
-pyshbundle/visualisation_utils.py
+pyshbundle/viz_utils.py
 pyshbundle.egg-info/PKG-INFO
 pyshbundle.egg-info/SOURCES.txt
 pyshbundle.egg-info/dependency_links.txt
 pyshbundle.egg-info/not-zip-safe
 pyshbundle.egg-info/requires.txt
 pyshbundle.egg-info/top_level.txt
 tests/test_pyshbundle.py
```

### Comparing `pyshbundle-0.2/setup.py` & `pyshbundle-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,25 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    description="PySHbundle: A Python implementation of MATLAB codes SHbundle",
+    description="PySHbundle: A Python implementation of GRACE Spherical Harmonics Synthesis MATLAB codes SHbundle",
     package_data={"my_package": ["data/*"]},
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='pyshbundle',
     name='pyshbundle',
     packages=find_packages(include=['pyshbundle', 'pyshbundle.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mn5hk/pyshbundle',
-    version='0.2',
+    version='1.0.0',
     zip_safe=False,
 )
```

