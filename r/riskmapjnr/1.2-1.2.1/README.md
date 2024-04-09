# Comparing `tmp/riskmapjnr-1.2.tar.gz` & `tmp/riskmapjnr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riskmapjnr-1.2.tar", last modified: Tue Jan 24 09:49:45 2023, max compression
+gzip compressed data, was "riskmapjnr-1.2.1.tar", last modified: Tue Apr  9 23:10:24 2024, max compression
```

## Comparing `riskmapjnr-1.2.tar` & `riskmapjnr-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.561650 riskmapjnr-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-01-24 09:49:32.000000 riskmapjnr-1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-01-24 09:49:32.000000 riskmapjnr-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-24 09:49:32.000000 riskmapjnr-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-01-24 09:49:45.561650 riskmapjnr-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-01-24 09:49:32.000000 riskmapjnr-1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.557648 riskmapjnr-1.2/riskmapjnr/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.557648 riskmapjnr-1.2/riskmapjnr/data/
--rw-r--r--   0 runner    (1001) docker     (123)   307200 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/data/ctry_border_GLP.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   254706 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/data/fcc123_GLP.tif
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/defor_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/deforest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/defrate_per_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/dist_edge_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/get_ldefz_v.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/get_riskmap_v.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/local_defor_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    22957 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/makemap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.557648 riskmapjnr-1.2/riskmapjnr/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/misc/countpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/misc/miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/riskmapjnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/set_defor_cat_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-01-24 09:49:33.000000 riskmapjnr-1.2/riskmapjnr/validation_fcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.561650 riskmapjnr-1.2/riskmapjnr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-24 09:49:45.000000 riskmapjnr-1.2/riskmapjnr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 09:49:45.561650 riskmapjnr-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-01-24 09:49:33.000000 riskmapjnr-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 09:49:45.561650 riskmapjnr-1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-24 09:49:33.000000 riskmapjnr-1.2/test/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.288901 riskmapjnr-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-09 23:10:24.288901 riskmapjnr-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.284901 riskmapjnr-1.2.1/riskmapjnr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.284901 riskmapjnr-1.2.1/riskmapjnr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   307200 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/data/ctry_border_GLP.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)   254706 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/data/fcc123_GLP.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/defor_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/deforest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/defrate_per_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/dist_edge_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/get_ldefz_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/get_riskmap_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/local_defor_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/makemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.284901 riskmapjnr-1.2.1/riskmapjnr/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/misc/countpix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/misc/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/riskmapjnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/set_defor_cat_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/riskmapjnr/validation_fcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.288901 riskmapjnr-1.2.1/riskmapjnr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 23:10:24.000000 riskmapjnr-1.2.1/riskmapjnr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:10:24.288901 riskmapjnr-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:10:24.284901 riskmapjnr-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 23:10:20.000000 riskmapjnr-1.2.1/test/test_import.py
```

### Comparing `riskmapjnr-1.2/CHANGELOG.rst` & `riskmapjnr-1.2.1/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Changelog
 =========
 
+riskmapjnr 1.2.1
+----------------
+
+* Bug corrections.
+* Set non-forest area as NoData in ``set_defor_cat_zero.py``.
+
+* This version is used by the Qgis Deforisk plugin.
+
 riskmapjnr 1.2
 --------------
 
 * Improving documentation.
 * Bug corrections:
 
-  - Make sure that `fcc_file` is projected to compute distances.
+  - Make sure that ``fcc_file`` is projected to compute distances.
   - Let the user set Agg backend for matplotlib when DISPLAY is not found.
-  - Close and join the pool execution in `makemap()`.
+  - Close and join the pool execution in ``makemap()``.
 
 * This version is running without issues in `SEPAL <https://sepal.io>`_.
 
 riskmapjnr 1.1
 --------------
 
 * Removing unnecessary output files.
 
 riskmapjnr 1.0
 --------------
 
 * First stable release.
-* Parallel computation for `makemap()`.
+* Parallel computation for ``makemap()``.
 * Benchmark to estimate advantage of parallel computing.
 * New tutorials on large jurisdictions (countries).
 * Bug corrections:
   
   - Correction of the annual deforestation rate formula.
   - Correction of the validation step using maps at the start of the validation period.
   - Correction of the final risk map at the end of the validation period.
```

### Comparing `riskmapjnr-1.2/LICENSE` & `riskmapjnr-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/PKG-INFO` & `riskmapjnr-1.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: riskmapjnr
-Version: 1.2
-Summary: Mapping deforestation risk following JNR methodology
-Home-page: https://github.com/ghislainv/riskmapjnr
-Author: Ghislain Vieilledent
-Author-email: ghislain.vieilledent@cirad.fr
-License: GPLv3
-Keywords: carbon deforestation emissions forests jnr map probabilityredd risk tropics vcs
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: interactive
-License-File: LICENSE
-
 ..
    # ==============================================================================
    # author          :Ghislain Vieilledent
    # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
    # web             :https://ecology.ghislainv.fr
    # license         :GPLv3
    # ==============================================================================
```

### Comparing `riskmapjnr-1.2/README.rst` & `riskmapjnr-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: riskmapjnr
+Version: 1.2.1
+Summary: Mapping deforestation risk following JNR methodology
+Home-page: https://github.com/ghislainv/riskmapjnr
+Author: Ghislain Vieilledent
+Author-email: ghislain.vieilledent@cirad.fr
+License: GPLv3
+Keywords: carbon deforestation emissions forests jnr map probabilityredd risk tropics vcs
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: gdal
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: scipy
+Provides-Extra: interactive
+Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: geopandas; extra == "interactive"
+Requires-Dist: descartes; extra == "interactive"
+Requires-Dist: folium; extra == "interactive"
+Requires-Dist: tabulate; extra == "interactive"
+
 ..
    # ==============================================================================
    # author          :Ghislain Vieilledent
    # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
    # web             :https://ecology.ghislainv.fr
    # license         :GPLv3
    # ==============================================================================
```

### Comparing `riskmapjnr-1.2/riskmapjnr/__init__.py` & `riskmapjnr-1.2.1/riskmapjnr/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+"""
+riskmapjnr: mapping deforestation risk using the moving window approach.
+https://ecology.ghislainv.fr/riskmapknr/
+"""
 
-# ==============================================================================
-# author          :Ghislain Vieilledent
-# email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
-# web             :https://ecology.ghislainv.fr
-# python_version  :>=3
-# license         :GPLv3
-# ==============================================================================
+# Define double undescore variables
+# https://peps.python.org/pep-0008/#module-level-dunder-names
+__author__ = "Ghislain Vieilledent"
+__email__ = "ghislain.vieilledent@cirad.fr"
+__version__ = "1.2.1"
+
+# GDAL exceptions
+from osgeo import gdal
 
 # Standard library imports
 import os
 
 # Local imports
 from .defrate_per_cat import defrate_per_cat
 from .defor_cat import defor_cat
 from .deforest import deforest
 from .dist_edge_threshold import dist_values, dist_edge_threshold
 from .get_ldefz_v import get_ldefz_v
 from .get_riskmap_v import get_riskmap_v
 from .local_defor_rate import local_defor_rate
-from .misc import countpix, invlogit, make_dir, tree
+from .misc import countpix, invlogit, make_dir, tree, rescale
 from .set_defor_cat_zero import set_defor_cat_zero
 from .validation import validation
 from .validation_fcc import validation_fcc
 from .plot import fcc123, riskmap
 # Import makemap in last as it uses from . import
 from .makemap import makemap
 
+# GDAL exceptions
+gdal.UseExceptions()
+
 # EOF
```

### Comparing `riskmapjnr-1.2/riskmapjnr/data/ctry_border_GLP.gpkg` & `riskmapjnr-1.2.1/riskmapjnr/data/ctry_border_GLP.gpkg`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/data/fcc123_GLP.tif` & `riskmapjnr-1.2.1/riskmapjnr/data/fcc123_GLP.tif`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/defor_cat.py` & `riskmapjnr-1.2.1/riskmapjnr/defor_cat.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/deforest.py` & `riskmapjnr-1.2.1/riskmapjnr/deforest.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/defrate_per_cat.py` & `riskmapjnr-1.2.1/riskmapjnr/defrate_per_cat.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,39 +16,38 @@
 import pandas as pd
 
 # Local application imports
 from .misc import progress_bar, makeblock
 
 
 # defrate_per_cat
-def defrate_per_cat(fcc_file, defor_values, riskmap_file, time_interval,
+def defrate_per_cat(fcc_file, riskmap_file, time_interval,
+                    period="calibration",
                     tab_file_defrate="defrate_per_cat.csv",
                     blk_rows=128, verbose=True):
     """Compute deforestation rates per category of deforestation risk.
 
     This function computes the historical deforestation rates for each
     category of spatial deforestation risk.
 
     :param fcc_file: Input raster file of forest cover change at three
         dates (123). 1: first period deforestation, 2: second period
         deforestation, 3: remaining forest at the end of the second
         period. No data value must be 0 (zero).
 
-    :param defor_values: Raster values to consider for
-       deforestation. Must correspond to either scalar 1 if first
-       period, or list [1, 2] if both first and second period are
-       considered.
-
     :param riskmap_file: Input raster file with categories of
-        spatial deforestation risk. This file is typically obtained
-        with function ``defor_cat()``.
+        spatial deforestation risk.
 
     :param time_interval: Time interval (in years) for forest cover
         change observations.
 
+    :param period: Either "calibration" (from t1 to t2), "validation"
+        (or "confirmation" from t2 to t3), or "historical" (full
+        historical period from t1 to t3). Default to "calibration".
+
     :param tab_file_defrate: Path to the ``.csv`` output file with
         estimates of deforestation rates per category of deforestation
         risk.
 
     :param blk_rows: If > 0, number of rows for computation by block.
 
     :param verbose: Logical. Whether to print messages or not. Default
@@ -64,14 +63,19 @@
     # Input rasters
     # ==============================================================
 
     # Get fcc raster data
     fcc_ds = gdal.Open(fcc_file)
     fcc_band = fcc_ds.GetRasterBand(1)
 
+    # Landscape variables
+    gt = fcc_ds.GetGeoTransform()
+    xres = gt[1]
+    yres = -gt[5]
+
     # Get defor_cat raster data
     defor_cat_ds = gdal.Open(riskmap_file)
     defor_cat_band = defor_cat_ds.GetRasterBand(1)
 
     # Make blocks
     blockinfo = makeblock(fcc_file, blk_rows=blk_rows)
     nblock = blockinfo[0]
@@ -82,57 +86,85 @@
     ny = blockinfo[6]
 
     # ==============================================
     # Compute deforestation rates per cat
     # ==============================================
 
     # Number of deforestation categories
-    cb = gdal.TermProgress if verbose else 0
-    stats = defor_cat_band.ComputeStatistics(False, cb)
-    n_cat = int(stats[1])  # Get the maximum
+    n_cat = 65535
     cat = [c + 1 for c in range(n_cat)]
 
     # Create a table to save the results
     data = {"cat": cat, "nfor": 0, "ndefor": 0,
-            "rate": 0}
+            "rate_obs": 0.0, "rate_mod": 0.0}
     df = pd.DataFrame(data)
 
     # Loop on blocks of data
     for b in range(nblock):
         # Progress bar
         if verbose:
             progress_bar(nblock, b + 1)
         # Position
         px = b % nblock_x
         py = b // nblock_x
         # Data
         fcc_data = fcc_band.ReadAsArray(x[px], y[py], nx[px], ny[py])
         defor_cat_data = defor_cat_band.ReadAsArray(
             x[px], y[py], nx[px], ny[py])
+        # Defor data on period
+        if period == "calibration":
+            data_for = defor_cat_data[fcc_data > 0]
+            data_defor = defor_cat_data[fcc_data == 1]
+        elif period in ["validation", "confirmation"]:
+            data_for = defor_cat_data[fcc_data > 1]
+            data_defor = defor_cat_data[fcc_data == 2]
+        elif period == "historical":
+            data_for = defor_cat_data[fcc_data > 0]
+            data_defor = defor_cat_data[np.isin(fcc_data, [1, 2])]
         # nfor_per_cat
-        data_for = defor_cat_data[fcc_data > 0]
         cat_for = pd.Categorical(data_for.flatten(), categories=cat)
         df["nfor"] += cat_for.value_counts().values
         # ndefor_per_cat
-        data_defor = defor_cat_data[np.isin(fcc_data, defor_values)]
         cat_defor = pd.Categorical(data_defor.flatten(), categories=cat)
         df["ndefor"] += cat_defor.value_counts().values
 
     # Annual deforestation rates per category
-    df["rate"] = 1 - (1 - df["ndefor"] / df["nfor"]) ** (1 / time_interval)
+    df["rate_obs"] = 1 - (1 - df["ndefor"] / df["nfor"]) ** (1 / time_interval)
+
+    # Relative spatial deforestation probability from model
+    df["rate_mod"] = ((df["cat"] - 1) * 999999 / 65534 + 1) * 1e-6
+    # Set proba of deforestation to 0 for category 1
+    df.loc[df["cat"] == 1, "rate_mod"] = 0
+
+    # Correction factor, either ndefor / sum_i p_i
+    # or theta * nfor / sum_i p_i
+    sum_ndefor = df["ndefor"].sum()
+    sum_pi = (df["nfor"] * df["rate_mod"]).sum()
+    correction_factor = sum_ndefor / sum_pi
+
+    # Absolute deforestation probability
+    df["rate_abs"] = df["rate_mod"] * correction_factor
+
+    # Time interval
+    df["time_interval"] = time_interval
+
+    # Pixel area
+    pixel_area = xres * yres / 10000
+    df["pixel_area"] = pixel_area
+
+    # Deforestation density (ha/pixel/yr)
+    df["defor_dens"] = df["rate_abs"] * pixel_area / time_interval
 
     # Export the table of results
     df.to_csv(tab_file_defrate, sep=",", header=True,
               index=False, index_label=False)
 
     # Dereference drivers
     del fcc_ds, defor_cat_ds
 
-    return None
-
 
 # # Test
 # fcc_file = "data/fcc123.tif"
 # riskmap_file = "outputs/defor_cat.tif"
 # time_interval = 10
 # tab_file_defrate = "outputs/defrate_per_cat.csv"
 # blk_rows = 128
```

### Comparing `riskmapjnr-1.2/riskmapjnr/dist_edge_threshold.py` & `riskmapjnr-1.2.1/riskmapjnr/dist_edge_threshold.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 # author          :Ghislain Vieilledent
 # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
 # web             :https://ecology.ghislainv.fr
 # python_version  :>=3
 # license         :GPLv3
 # ==============================================================================
 
-# Python virtual environment
-# conda create --name jnr-vcs -c conda-forge python gdal numpy
-# matplotlib pip scipy pandas --yes
+"""
+Compute the distance to forest edge threshold.
+"""
 
 # Third party imports
 from matplotlib import pyplot as plt
 import numpy as np
 from osgeo import gdal
 import pandas as pd
 
 # Local application imports
 from .misc import progress_bar, makeblock
-from riskmapjnr.misc import progress_bar, makeblock
+
 
 # check_fcc_file
 def check_fcc_file(fcc_file, blk_rows=128, verbose=True):
     """Perform some checks on the fcc file.
 
     Check that the fcc file:
 
@@ -52,27 +52,27 @@
     # Read fcc file
     fcc_ds = gdal.Open(fcc_file)
     fcc_band = fcc_ds.GetRasterBand(1)
 
     # ================
     # Check projection
     # ================
-    crs=fcc_ds.GetSpatialRef()
+    crs = fcc_ds.GetSpatialRef()
     if not crs.IsProjected():
         msg = ("'fcc_file' cannot be in latlon coordinates "
                "and must be projected to compute euclidean "
                "distances.")
         raise ValueError(msg)
 
     # ==================
     # Check nodata value
     # ==================
     nodata = fcc_band.GetNoDataValue()
     if nodata != 0:
-        msg = ("'fcc_file' must have 0 (zero) as NoData value.")
+        msg = "'fcc_file' must have 0 (zero) as NoData value."
         raise ValueError(msg)
 
     # ============
     # Check values
     # ============
 
     # Necessary values
@@ -113,16 +113,14 @@
 
     # Check whole values are equal to [0, 1, 2, 3]
     if not np.array_equal(np.unique(uniq_val), nece_val):
         msg = ("'fcc_file' must include values 0, 1, 2, and 3 "
                "with 0 (zero) as NoData.")
         raise ValueError(msg)
 
-    return None
-
 
 # dist_values
 def dist_values(input_file,
                 dist_file,
                 values=0,
                 verbose=True):
     """Computing the shortest distance to pixels with given values in
@@ -174,56 +172,64 @@
     # Set nodata value
     dstband.SetNoDataValue(0)
 
     # Delete objects
     srcband = None
     dstband = None
     del src_ds, dst_ds
-    return None
 
 
 # dist_edge_threshold
 def dist_edge_threshold(fcc_file,
                         defor_values,
+                        defor_threshold=99.5,
                         dist_file="dist_edge.tif",
                         dist_bins=np.arange(0, 1080, step=30),
                         tab_file_dist="perc_dist.csv",
                         fig_file_dist="perc_dist.png",
                         figsize=(6.4, 4.8),
                         dpi=100,
                         blk_rows=128,
+                        dist_file_available=False,
+                        check_fcc=True,
                         verbose=True):
     """Computing the percentage of total deforestation as a function of
     the distance to forest edge.
 
     This function computes the percentage of total deforestation as a
     function of the distance to forest edge. It returns a table with
     the cumulative percentage of deforestation as distance to forest
     edge increases. It also identifies the distance threshold for the
     distance to forest edge so that the deforestation under that
-    threshold is >= 99 % of the total deforestation in the
+    threshold is >= 99.5 % of the total deforestation in the
     landscape. The function also plots the relationship between the
     percentage of deforestation and the distance to forest edge. A
     raster of distance to forest edge will be created. The distance
     unit will be the one of the input file.
 
     :param fcc_file: Input raster file of forest cover change at three
         dates (123). 1: first period deforestation, 2: second period
         deforestation, 3: remaining forest at the end of the second
         period. No data value must be 0 (zero). The raster must be
         projected to compute Euclidean distances with the
         ``gdal_proximity()`` function.
 
     :param defor_values: Raster values to consider for
-       deforestation. Must correspond to either scalar 1 if first
-       period, or list [1, 2] if both first and second period are
-       considered.
-
-    :param dist_file: Path to the output raster file of distance to
-        forest edge. Default to ``dist_edge.tif``.
+        deforestation. Must correspond to either scalar 1 if first
+        period, or list [1, 2] if both first and second period are
+        considered.
+
+    :param defor_threshold: Deforestation threshold (in
+        percent). Default to 99.5.
+
+    :param dist_file: Path to either (i) the output raster file of
+        distance to forest edge or (ii) the input raster file of
+        distance to forest edge if ``dist_file_available`` is
+        ``True``. Raster of distance to forest edge is computed in the
+        first case only. Default to ``dist_edge.tif``.
 
     :param dist_bins: Array of bins for distances. It has to be
         1-dimensional and monotonic. The array must also include zero
         as the first value. Default to ``np.arange(0, 1080,
         step=30)``.
 
     :param tab_file_dist: Path to the table ``.csv`` file that will be
@@ -243,33 +249,42 @@
 
     :param dpi: Resolution for output image.
 
     :param blk_rows: Number of rows for block. This is used to break
         lage raster files in several blocks of data that can be hold
         in memory.
 
+    :param dist_file_available: Boolean. If ``True``, parameter
+        ``dist_file`` indicates the input raster file of distance to
+        forest edge which is not computed. Default to ``False``.
+
+    :param check_fcc: Boolean. If ``True``, performs some checks on
+        the fcc input file. Default to ``True``.
+
     :param verbose: Logical. Whether to print messages or not. Default
         to ``True``.
 
     :return: A dictionary. With ``tot_def``: total deforestation (in
         ha), ``dist_thresh``: the distance threshold, ``perc``: the
         percentage of deforestation for pixels with distance <=
         dist_thresh.
 
     """
 
     # Check fcc_file
-    check_fcc_file(fcc_file, blk_rows=blk_rows, verbose=verbose)
+    if check_fcc:
+        check_fcc_file(fcc_file, blk_rows=blk_rows, verbose=verbose)
 
     # Compute the distance to the forest edge
-    dist_values(fcc_file, dist_file, values=0, verbose=verbose)
+    if dist_file_available is not True:
+        dist_values(fcc_file, dist_file, values=0, verbose=verbose)
 
     # Create a table to save the results
-    data = {"distance": dist_bins[1:], "npix": 0, "area": 0,
-            "cum": 0, "perc": 0}
+    data = {"distance": dist_bins[1:], "npix": 0, "area": 0.0,
+            "cum": 0.0, "perc": 0.0}
     res_df = pd.DataFrame(data)
 
     # Total deforested pixels
     npix_def = 0
 
     # Make blocks
     blockinfo = makeblock(dist_file, blk_rows=blk_rows)
@@ -302,34 +317,40 @@
         # Consider only deforested pixels for distances
         dist_def = dist_data * np.isin(fcc_data, defor_values)
         dist_def = dist_def[dist_def > 0]
         # Categorize distance
         dist_cat = pd.cut(dist_def.flatten(), dist_bins, right=True)
         # Sum by category
         df = pd.DataFrame({"dist": dist_cat})
-        counts = df.groupby(df.dist).size()
+        counts = df.groupby(df.dist, observed=False).size()
         # Update data-frame
         res_df.loc[:, "npix"] += counts.values
 
     # Compute deforested areas
     gt = dist_ds.GetGeoTransform()
     pix_area = gt[1] * (-gt[5])
-    res_df.loc[:, "area"] = res_df["npix"].values * pix_area / 10000
+    area = res_df["npix"].values * pix_area / 10000
+    res_df.loc[:, "area"] = area
     tot_area_def = npix_def * pix_area / 10000
     # Cumulated deforestation
     res_df.loc[:, "cum"] = res_df["area"].cumsum().values
     # Percentage of total deforestation
     res_df.loc[:, "perc"] = 100 * res_df["cum"].values / tot_area_def
 
     # Export the table of results
     res_df.to_csv(tab_file_dist, sep=",", header=True,
                   index=False, index_label=False)
 
-    # Distance and percentage for 99% threshold
-    index_thresh = np.nonzero(res_df["perc"].values > 99)[0][0]
+    # Distance and percentage for deforestation threshold
+    try:
+        index_thresh = np.nonzero(res_df["perc"].values > defor_threshold)[0][0]
+    except IndexError:
+        raise ValueError("Increase maximal distance "
+                         "defined in argument 'dist_bins'.")
+
     dist_thresh = res_df.loc[index_thresh, "distance"]
     perc_thresh = np.around(res_df.loc[index_thresh, "perc"], 2)
 
     # Plot
     fig = plt.figure(figsize=figsize, dpi=dpi)
     plt.subplot(111)
     plt.plot(res_df["distance"], res_df["perc"], "b-")
```

### Comparing `riskmapjnr-1.2/riskmapjnr/get_ldefz_v.py` & `riskmapjnr-1.2.1/riskmapjnr/get_ldefz_v.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     we consider (i) the map of local deforestation rates on the
     historical period, (ii) the map of distance to forest edge at the
     beginning of the validation period, and (ii) the distance
     threshold estimated on the historical period.
 
     :param ldefrate_file: Input raster file of local deforestation
         rates. Deforestation rates are defined by integer values
-        between 0 and 10000 (ten thousand). This file is typically
-        obtained with function ``local_defor_rate()``.
+        between rescale_min_val (e.g. 2) and rescale_max_val
+        (e.g. 10000). This file is typically obtained with function
+        ``local_defor_rate()``.
 
     :param dist_v_file: Input raster file of distance to forest edge
         at the beginning of the validation period. This file is
         typically obtained with function ``dist_values()`` setting
         ``values="0,1"``.
 
     :param dist_thresh: The distance threshold. This distance
@@ -55,18 +56,18 @@
         value of 0.
 
     :param blk_rows: If > 0, number of rows for computation by block.
 
     :param verbose: Logical. Whether to print messages or not. Default
         to ``True``.
 
-    :return: None. A raster files of local deforestation rate at the
-    beginning of the validation period is created (see
-    ``ldefrate_with_zero_v_file``). Data range from 0 to 10000. Raster
-    type is UInt16 ([0, 65535]). NoData value is set to 65535.
+    :return: None. A raster files of local deforestation risk at the
+        beginning of the validation period is created (see
+        ``ldefrate_with_zero_v_file``). Data range from 1 to 65535. Raster
+        type is UInt16 ([0, 65535]). NoData value is set to 0.
 
     """
 
     # ================================
     # Create ldefrate_with_zero_v_file
     # ================================
 
@@ -87,15 +88,15 @@
     ldefzv_ds = driver.Create(ldefrate_with_zero_v_file, xsize, ysize, 1,
                               gdal.GDT_UInt16,
                               ["COMPRESS=LZW", "PREDICTOR=2",
                                "BIGTIFF=YES"])
     ldefzv_ds.SetProjection(ldef_ds.GetProjection())
     ldefzv_ds.SetGeoTransform(ldef_ds.GetGeoTransform())
     ldefzv_band = ldefzv_ds.GetRasterBand(1)
-    ldefzv_band.SetNoDataValue(65535)
+    ldefzv_band.SetNoDataValue(0)
 
     # Make blocks
     blockinfo = makeblock(ldefrate_file, blk_rows=blk_rows)
     nblock = blockinfo[0]
     nblock_x = blockinfo[1]
     x = blockinfo[3]
     y = blockinfo[4]
@@ -111,30 +112,29 @@
         px = b % nblock_x
         py = b // nblock_x
         # Data
         ldef_data = ldef_band.ReadAsArray(x[px], y[py], nx[px], ny[py])
         distv_data = distv_band.ReadAsArray(x[px], y[py], nx[px], ny[py])
         # Remove defor rate for fcc == 1 (corresponding to distv == 0)
         ldefzv_data = ldef_data
-        ldefzv_data[distv_data == 0] = 65535
-        # Set 0 risk beyond distance threshold
-        ldefzv_data[distv_data >= dist_thresh] = 0
+        ldefzv_data[distv_data == 0] = 0
+        # Set 1 for null risk beyond distance threshold
+        ldefzv_data[distv_data >= dist_thresh] = 1
         # Write to files
         ldefzv_band.WriteArray(ldefzv_data, x[px], y[py])
 
     # Compute statistics
     ldefzv_band.FlushCache()
     cb = gdal.TermProgress if verbose else 0
     ldefzv_band.ComputeStatistics(False, cb)
 
     # Dereference drivers
     ldefzv_band = None
     del ldef_ds, distv_ds, ldefzv_ds
 
-    return None
 
 # # Test
 # ldefrate_file = "outputs_steps/ldefrate.tif"
 # dist_v_file = "outputs_steps/dist_edge_v.tif"
 # dist_thresh = 120
 # ldefrate_with_zero_v_file = "outputs_steps/ldefrate_with_zero_v.tif"
 # blk_rows = 128
```

### Comparing `riskmapjnr-1.2/riskmapjnr/get_riskmap_v.py` & `riskmapjnr-1.2.1/riskmapjnr/get_riskmap_v.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/local_defor_rate.py` & `riskmapjnr-1.2.1/riskmapjnr/local_defor_rate.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 
 # Third party imports
 import numpy as np
 from osgeo import gdal
 import scipy.ndimage
 
 # Local application imports
-from .misc import progress_bar
+from .misc import progress_bar, rescale
 
 
 # local_defor_rate
 def local_defor_rate(fcc_file, defor_values, ldefrate_file, win_size,
-                     time_interval, blk_rows=128, verbose=True):
+                     time_interval, rescale_min_val=2,
+                     rescale_max_val=10000, blk_rows=128,
+                     verbose=True):
     """Computing the local deforestation rate using a moving window.
 
     This function computes the local deforestation rate using a moving
     window. SciPy is used for the focal analysis. The
     ``uniform_filter`` is used over the ``generic_filter``. The
     ``generic_filter`` is 40 times slower than the strides implemented
     in the ``uniform_filter``. For cells on the edge of the raster,
@@ -47,14 +49,20 @@
 
     :param win_size: Size of the moving window in number of
         cells. Must be an odd number lower or equal to ``blk_rows``.
 
     :param time_interval: Time interval (in years) for forest cover
         change observations.
 
+    :param rescale_min_val: Integer. Minimal value for rescaling. Down
+        to 1. Default to 1.
+
+    :param rescale_max_val: Integer. Maximal value for rescaling. Up
+        to 65535. Default to 10000.
+
     :param blk_rows: Number of rows for block. Must be greater or
         equal to ``win_size``. This is used to break lage raster files
         in several blocks of data that can be hold in memory.
 
     :param verbose: Logical. Whether to print messages or not. Default
         to ``True``.
 
@@ -66,15 +74,15 @@
     """
 
     # Check win_size
     win_size = int(win_size)  # Must be int for uniform_filter
     if (win_size % 2) == 0:
         msg = "'win_size' must be an odd number."
         raise ValueError(msg)
-    if (win_size > blk_rows):
+    if win_size > blk_rows:
         msg = "'win_size' must be lower or equal to 'blk_rows'."
         raise ValueError(msg)
 
     # Get raster data
     in_ds = gdal.Open(fcc_file)
     in_band = in_ds.GetRasterBand(1)
     # Raster size
@@ -86,15 +94,15 @@
     out_ds = driver.Create(ldefrate_file, xsize, ysize, 1,
                            gdal.GDT_UInt16,
                            ["COMPRESS=LZW", "PREDICTOR=2",
                             "BIGTIFF=YES"])
     out_ds.SetProjection(in_ds.GetProjection())
     out_ds.SetGeoTransform(in_ds.GetGeoTransform())
     out_band = out_ds.GetRasterBand(1)
-    out_band.SetNoDataValue(65535)
+    out_band.SetNoDataValue(0)
 
     # Iteration
     iter_block = 0
 
     # Loop on blocks of data
     for i in range(0, ysize, blk_rows):
 
@@ -121,42 +129,42 @@
         # defor (during period)
         defor_data = np.zeros(in_data.shape, int)
         defor_data[np.isin(in_data, defor_values)] = 1
         # Use uniform filter to get the mean then multiply to obtain the sum
         win_defor = scipy.ndimage.uniform_filter(
             defor_data, size=win_size, mode="constant", cval=0,
             output=float) * (win_size ** 2)
-        # Round to nearest inter to remove approximation due to float precision
+        # Round to nearest int to remove approximation due to float precision
         win_defor = np.rint(win_defor).astype(int)
         # for (start of first period)
         for_data = np.zeros(in_data.shape, int)
         w = np.where(in_data > 0)
         for_data[w] = 1
         # Use uniform filter to get the mean then multiply to obtain the sum
         win_for = scipy.ndimage.uniform_filter(
             for_data, size=win_size, mode="constant", cval=0,
             output=float) * (win_size ** 2)
         # Round to nearest inter to remove approximation due to float precision
         win_for = np.rint(win_for).astype(int)
         # Annual deforestation rate
-        out_data = np.ones(in_data.shape, int) * 65535
+        out_data = np.zeros(in_data.shape, int)
         theta = 1 - (1 - win_defor[w] / win_for[w]) ** (1 / time_interval)
-        out_data[w] = np.rint(9999 * theta + 1).astype(int)  # min=1, max=10000
+        # Rescale
+        out_data[w] = rescale(theta, rescale_min_val, rescale_max_val)
         if yoff == 0:
             out_band.WriteArray(out_data)
         else:
             out_band.WriteArray(out_data[(extra_lines):], 0,
                                 yoff + extra_lines)
 
     # Closing
     out_band.FlushCache()
     cb = gdal.TermProgress if verbose else 0
     out_band.ComputeStatistics(False, cb)
     del out_ds, in_ds
-    return None
 
 
 # # Test
 # ws = 7
 # local_defor_rate(fcc_file="data/fcc123_GLP.tif",
 #                  ldefrate_file="outputs/ldefrate_ws{}.tif".format(ws),
 #                  win_size=ws,
```

### Comparing `riskmapjnr-1.2/riskmapjnr/makemap.py` & `riskmapjnr-1.2.1/riskmapjnr/makemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
         res = pool.starmap_async(makemap_ws, args).get()
         ncell = res[0][2]
         csize_km = res[0][3]
         wRMSE_obj = [r[1] for r in res]
         df.loc[:, "wRMSE"] = np.array(wRMSE_obj).flatten()
         pool.close()
         pool.join()
-        
+
     # Export the table of results
     df.to_csv(tab_file_map_comp, sep=",", header=True,
               index=False, index_label=False)
 
     # Plot of wRMSE
     fig = plt.figure(figsize=figsize, dpi=dpi)
     df.set_index("ws", inplace=True)
```

### Comparing `riskmapjnr-1.2/riskmapjnr/misc/countpix.py` & `riskmapjnr-1.2.1/riskmapjnr/misc/countpix.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/misc/miscellaneous.py` & `riskmapjnr-1.2.1/riskmapjnr/misc/miscellaneous.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     :return: Return the inverse-logit of the array.
 
     """
 
     r = x
     r[x > 0] = 1.0 / (1.0 + np.exp(-x[x > 0]))
     r[x <= 0] = np.exp(x[x <= 0]) / (1 + np.exp(x[x <= 0]))
-    return (r)
+    return r
 
 
 # Function to make a directory
 def make_dir(newdir):
     """Make new directory
 
         * Already exists, silently complete
@@ -140,16 +140,16 @@
     ncol = r.RasterXSize
     nrow = r.RasterYSize
     # Number of squares
     nsquare_x = int(np.ceil(ncol / square_size))
     nsquare_y = int(np.ceil(nrow / square_size))
     nsquare = nsquare_x * nsquare_y
     # Upper-left coordinates of each square
-    x = np.arange(0, ncol, square_size, dtype=np.int).tolist()
-    y = np.arange(0, nrow, square_size, dtype=np.int).tolist()
+    x = np.arange(0, ncol, square_size, dtype=int).tolist()
+    y = np.arange(0, nrow, square_size, dtype=int).tolist()
     # Size (number of col and row) of each square
     nx = [square_size] * nsquare_x
     ny = [square_size] * nsquare_y
     # Modify last values of nx and ny
     if (ncol % square_size) > 0:
         nx[-1] = ncol % square_size
     if (nrow % square_size) > 0:
@@ -173,18 +173,47 @@
     step = 1 if niter <= 100 else niter // 100
     if i == 1:
         sys.stdout.write("0%")
         sys.stdout.flush()
     elif i % step == 0:
         sys.stdout.write("\r{}%".format((100 * i) // niter))
         sys.stdout.flush()
-    if (i == niter):
+    if i == niter:
         sys.stdout.write("\r100%\n")
         sys.stdout.flush()
-    return None
+
+
+# Rescale
+def rescale(value, min_val=1, max_val=10000):
+    """Rescale probability values to.
+
+    This function rescales probability values (float in [0, 1]) to
+    integer values in [min_val, max_val]. Raster data can then be of type
+    UInt16 with 0 as nodata value.
+
+    :param value: Numpy array of float values in [0, 1].
+
+    :param min_val: Integer. Minimal value for
+        rescaling. Down to 1. Default to 1.
+
+    :param max_val: Integer. Maximal value for
+        rescaling. Up to 65535. Default to 10000.
+
+    :return: Rescaled numpy array of integer values in [min_val, max_val].
+
+    """
+
+    # Transform to float (otherwise 1e-06 is set to 0)
+    value = value.astype(float)
+    # Avoid nodata value (0) for low proba
+    value[value < 1e-06] = 1e-06
+    # Rescale and round to nearest integer
+    r = ((value * 1e6 - 1) * (max_val - min_val) / 999999.0) + min_val
+    r = np.rint(r).astype(int)
+    return r
 
 
 # Tree
 # from https://stackoverflow.com/questions/9727673/
 # list-directory-tree-structure-in-python
 
 space = '    '
```

### Comparing `riskmapjnr-1.2/riskmapjnr/plot.py` & `riskmapjnr-1.2.1/riskmapjnr/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     Ymin = gt[3] + gt[5] * nrow
     Ymax = gt[3]
     extent = [Xmin, Xmax, Ymin, Ymax]
 
     # Total number of pixels
     npixels_orig = ncol * nrow
     # Check number of pixels is inferior to maxpixels
-    if (npixels_orig > maxpixels):
+    if npixels_orig > maxpixels:
         # Remove potential existing external overviews
         if os.path.isfile(input_fcc_raster + ".ovr"):
             os.remove(input_fcc_raster + ".ovr")
         # Find overview level such that npixels <= maxpixels
         i = 0
         npixels_ov = npixels_orig
         while npixels_ov > maxpixels:
@@ -177,15 +177,15 @@
         ov_arr = ov_band.ReadAsArray()
     else:
         # Get original data
         ov_arr = rasterB.ReadAsArray()
 
     # Dereference driver
     rasterB = None
-    del(rasterR)
+    del rasterR
 
     # Colormap
     colors = [(1, 1, 1, 0)]  # transparent white for 0
     cmax = 255.0  # float for division
     for i in range(3):
         col_class = tuple(np.array(col[i]) / cmax)
         colors.append(col_class)
@@ -216,15 +216,21 @@
         plt.ylim(zoom[2], zoom[3])
         ax2.set_xticks([])
         ax2.set_yticks([])
 
     # Save and return figure
     fig.tight_layout()
     fig.savefig(output_file, dpi="figure", bbox_inches="tight")
-    return(fig)
+    return fig
+
+
+def rescale_zo(x, xmin, xmax):
+    """Rescale on interval zero-one."""
+    z = (x - xmin) / (xmax - xmin)
+    return z
 
 
 # plot.riskmap
 def riskmap(input_risk_map,
             output_file="prob.png",
             maxpixels=500000,
             borders=None,
@@ -262,15 +268,15 @@
     Ymin = gt[3] + gt[5] * nrow
     Ymax = gt[3]
     extent = [Xmin, Xmax, Ymin, Ymax]
 
     # Total number of pixels
     npixels_orig = ncol * nrow
     # Check number of pixels is inferior to maxpixels
-    if (npixels_orig > maxpixels):
+    if npixels_orig > maxpixels:
         # Remove potential existing external overviews
         if os.path.isfile(input_risk_map + ".ovr"):
             os.remove(input_risk_map + ".ovr")
         # Find overview level such that npixels <= maxpixels
         i = 0
         npixels_ov = npixels_orig
         while npixels_ov > maxpixels:
@@ -285,49 +291,57 @@
         ov_arr = ov_band.ReadAsArray()
     else:
         # Get original data
         ov_arr = rasterB.ReadAsArray()
 
     # Dereference driver
     rasterB = None
-    del(rasterR)
+    del rasterR
 
     # Colormap
     colors = []
     cmax = 255.0  # float for division
-    vmax = 30.0  # float for division
+    vmin = 1.0
+    vmax = 65535.0  # float for division
     # green
-    colors.append((0, (34 / cmax, 139 / cmax, 34 / cmax, 1)))
+    colors.append((rescale_zo(1, vmin, vmax),
+                   (34 / cmax, 139 / cmax, 34 / cmax, 1)))
     # orange
-    colors.append((1 / vmax, (1, 165 / cmax, 0, 1)))
+    colors.append((rescale_zo(2, vmin, vmax),
+                   (1, 165 / cmax, 0, 1)))
     # red
-    colors.append((15 / vmax, (227 / cmax, 26 / cmax, 28 / cmax, 1)))
+    colors.append((rescale_zo(100, vmin, vmax),
+                   (227 / cmax, 26 / cmax, 28 / cmax, 1)))
     # black
-    colors.append((1, (0, 0, 0, 1)))
-    color_map = LinearSegmentedColormap.from_list(name="mycm", colors=colors,
-                                                  N=31, gamma=1.0)
-    # Set transparent color for high out-of-range values.
-    color_map.set_over(color=(1, 1, 1, 0))
+    colors.append((rescale_zo(10000, vmin, vmax),
+                   (0, 0, 0, 1)))
+    colors.append((rescale_zo(65535, vmin, vmax),
+                   (0, 0, 0, 1)))
+    color_map = LinearSegmentedColormap.from_list(
+        name="mycm", colors=colors, N=65535, gamma=1.0
+    )
+    # Set transparent color for lower out-of-range values.
+    color_map.set_under(color=(1, 1, 1, 0))
 
     # Plot raster
     fig = plt.figure(figsize=figsize, dpi=dpi)
     plt.subplot(111)
     plt.imshow(ov_arr, cmap=color_map, extent=extent,
-               vmin=0, vmax=30)
+               vmin=0.01, vmax=65535)
     if borders is not None:
         plot_layer(borders, symbol="k-", **kwargs)
 
     # Legend
     if legend is True:
-        t = np.linspace(0, 30, 7, endpoint=True)
+        t = np.linspace(0, 65535, 6, endpoint=True)
         cbar = plt.colorbar(ticks=t, orientation="vertical",
                             shrink=0.5, aspect=20)
-        vl = np.linspace(0, 30, 7, endpoint=True).astype(int)
+        vl = np.linspace(0, 1, 6, endpoint=True).astype(int)
         cbar.ax.set_yticklabels(vl)
 
     # Save image
     figure_as_image(fig, output_file)
 
     # Return figure
-    return(fig)
+    return fig
 
 # EOF
```

### Comparing `riskmapjnr-1.2/riskmapjnr/riskmapjnr.py` & `riskmapjnr-1.2.1/riskmapjnr/riskmapjnr.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 # author          :Ghislain Vieilledent
 # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
 # web             :https://ecology.ghislainv.fr
 # python_version  :>=3.6
 # license         :GPLv3
 # ==============================================================================
 
-__version__ = "1.2"
+import riskmapjnr as rmj
 
 
 def main():
     """riskmapjnr.riskmapjnr: provides entry point main().
 
     Running ``riskmapjnr`` in the terminal prints riskmapjnr
     description and version. Can be used to check that the
     ``riskmapjnr`` Python package has been correctly imported.
 
     """
-    print("# riskmapjnr: Map of deforestation risk following JNR methodology.")
-    print("# https://ecology.ghislainv.fr/riskmapjnr")
-    print("# riskmapjnr version {}.".format(__version__))
-    return None
+
+    print(rmj.__doc__)
+    print(f"version {rmj.__version__}.")
 
 # End
```

### Comparing `riskmapjnr-1.2/riskmapjnr/set_defor_cat_zero.py` & `riskmapjnr-1.2.1/riskmapjnr/set_defor_cat_zero.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,41 +20,43 @@
 # set_defor_cat_zero
 def set_defor_cat_zero(ldefrate_file,
                        dist_file,
                        dist_thresh,
                        ldefrate_with_zero_file="ldefrate_with_zero.tif",
                        blk_rows=128,
                        verbose=True):
-    """Set a value of zero (0) to pixels with zero deforestation risk. A
-    risk of deforestation of zero is assumed when distance to forest
-    edge is greater than the distance threshold.
+    """Set a value of one (1) to pixels with zero deforestation
+    risk. A null risk of deforestation is assumed when distance to
+    forest edge is greater than the distance threshold. NoData value
+    is set to zero (0).
 
     :param ldefrate_file: Input raster file of local deforestation
         rates. Deforestation rates are defined by integer values
-        between 1 and 10000 (ten thousand). This file is typically
-        obtained with function ``local_defor_rate()``.
+        between rescale_min_val (e.g. 2) and rescale_max_val
+        (e.g. 10000). This file is typically obtained with function
+        ``local_defor_rate()``.
 
     :param dist_file: Path to the distance to forest edge raster file.
 
     :param dist_thresh: The distance threshold. This distance
         threshold is used to identify pixels with zero deforestation
         risk.
 
     :param ldefrate_with_zero_file: Output raster file. Default to
         "ldefrate_with_zero.tif" in the current working
         directory. Pixels with zero deforestation risk are assigned a
-        value of 0.
+        value of 1.
 
     :param blk_rows: If > 0, number of rows for computation by block.
 
     :param verbose: Logical. Whether to print messages or not. Default
         to ``True``.
 
     :return: None. A raster file identifying pixels with zero risk of
-        deforestation (value 0) will be created (see
+        deforestation (value 1) will be created (see
         ``ldefrate_with_zero_file``).
 
     """
 
     # ==============================================================
     # Input rasters: deforestation rates and distance to forest edge
     # ==============================================================
@@ -88,29 +90,31 @@
     catzero_ds = driver.Create(
         ldefrate_with_zero_file, xsize, ysize,
         1, gdal.GDT_UInt16, ["COMPRESS=LZW",
                              "PREDICTOR=2", "BIGTIFF=YES"])
     catzero_ds.SetProjection(ldefrate_ds.GetProjection())
     catzero_ds.SetGeoTransform(ldefrate_ds.GetGeoTransform())
     catzero_band = catzero_ds.GetRasterBand(1)
-    catzero_band.SetNoDataValue(65535)
+    catzero_band.SetNoDataValue(0)
 
     # Loop on blocks of data
     for b in range(nblock):
         # Progress bar
         if verbose:
             progress_bar(nblock, b + 1)
         # Position
         px = b % nblock_x
         py = b // nblock_x
         # Data
         catzero_data = ldefrate_band.ReadAsArray(x[px], y[py], nx[px], ny[py])
         dist_data = dist_band.ReadAsArray(x[px], y[py], nx[px], ny[py])
-        # Set 0 risk beyond distance threshold
-        catzero_data[dist_data >= dist_thresh] = 0
+        # Ensure NoData when dist_data equals zero (especially for t2)
+        catzero_data[dist_data == 0] = 0
+        # Set 1 for zero risk of deforestation (beyond distance threshold)
+        catzero_data[dist_data >= dist_thresh] = 1
         catzero_band.WriteArray(catzero_data, x[px], y[py])
 
     # Compute statistics
     catzero_band.FlushCache()
     cb = gdal.TermProgress if verbose else 0
     catzero_band.ComputeStatistics(False, cb)
```

### Comparing `riskmapjnr-1.2/riskmapjnr/validation.py` & `riskmapjnr-1.2.1/riskmapjnr/validation.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr/validation_fcc.py` & `riskmapjnr-1.2.1/riskmapjnr/validation_fcc.py`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/riskmapjnr.egg-info/PKG-INFO` & `riskmapjnr-1.2.1/riskmapjnr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: riskmapjnr
-Version: 1.2
+Version: 1.2.1
 Summary: Mapping deforestation risk following JNR methodology
 Home-page: https://github.com/ghislainv/riskmapjnr
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Keywords: carbon deforestation emissions forests jnr map probabilityredd risk tropics vcs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: interactive
 License-File: LICENSE
+Requires-Dist: gdal
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: scipy
+Provides-Extra: interactive
+Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: geopandas; extra == "interactive"
+Requires-Dist: descartes; extra == "interactive"
+Requires-Dist: folium; extra == "interactive"
+Requires-Dist: tabulate; extra == "interactive"
 
 ..
    # ==============================================================================
    # author          :Ghislain Vieilledent
    # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
    # web             :https://ecology.ghislainv.fr
    # license         :GPLv3
```

### Comparing `riskmapjnr-1.2/riskmapjnr.egg-info/SOURCES.txt` & `riskmapjnr-1.2.1/riskmapjnr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riskmapjnr-1.2/setup.py` & `riskmapjnr-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,19 @@
 import io
 import re
 from setuptools import setup, find_packages
 
 
 # find_version
 def find_version():
-    with open('riskmapjnr/riskmapjnr.py') as f:
-        far = f.read()
-    version = re.search(
-        '^__version__\\s*=\\s*"(.*)"',
-        far,
-        re.M
-    ).group(1)
-    return version
+    """Finding package version."""
+    with open("riskmapjnr/__init__.py", encoding="utf-8") as init_file:
+        init_text = init_file.read()
+    far_version = re.search('^__version__\\s*=\\s*"(.*)"', init_text, re.M).group(1)
+    return far_version
 
 
 version = find_version()
 
 # reStructuredText README file
 with io.open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
```

### Comparing `riskmapjnr-1.2/test/test_import.py` & `riskmapjnr-1.2.1/test/test_import.py`

 * *Files identical despite different names*

