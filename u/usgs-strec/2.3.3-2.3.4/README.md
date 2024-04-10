# Comparing `tmp/usgs-strec-2.3.3.tar.gz` & `tmp/usgs-strec-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-strec-2.3.3.tar", last modified: Mon Feb  5 17:51:55 2024, max compression
+gzip compressed data, was "usgs-strec-2.3.4.tar", last modified: Wed Apr 10 16:14:34 2024, max compression
```

## Comparing `usgs-strec-2.3.3.tar` & `usgs-strec-2.3.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.288653 usgs-strec-2.3.3/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      755 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       47 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)    12911 2024-02-05 17:51:55.288653 usgs-strec-2.3.3/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10865 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1360 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-02-05 17:51:55.288653 usgs-strec-2.3.3/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.272653 usgs-strec-2.3.3/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.276653 usgs-strec-2.3.3/src/strec/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:49:56.000000 usgs-strec-2.3.3/src/strec/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.276653 usgs-strec-2.3.3/src/strec/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8374 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/bin/regcalc.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/bin/strec_cfg.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9526 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/calc.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3562 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/cmt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4869 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/config.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.284653 usgs-strec-2.3.3/src/strec/data/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      877 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/REGION_GRIDS_README.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:49:56.000000 usgs-strec-2.3.3/src/strec/data/__init__.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   750725 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/active.geojson
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    23487 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/backarc.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    36449 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/domains.xlsx
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    95983 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/land.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      240 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/maximum_interface_depths.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  6086656 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/moment_tensors.db
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   138345 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/ocean.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6153 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/select.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1753 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/selectspec.conf
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   271186 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/stable.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1794 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/strec.ini
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   204430 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/subduction.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24246 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/data/volcanic.geojson
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5461 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/database.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3635 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/distance.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7142 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/gcmt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3389 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/gmreg.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2639 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/kagan.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9386 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/slab.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13186 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/sm_probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4493 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/subduction.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    23237 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/subtype.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8163 2024-02-05 17:47:52.000000 usgs-strec-2.3.3/src/strec/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-05 17:51:55.288653 usgs-strec-2.3.3/src/usgs_strec.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)    12911 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1078 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       86 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      321 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        6 2024-02-05 17:51:55.000000 usgs-strec-2.3.3/src/usgs_strec.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.469887 usgs-strec-2.3.4/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      755 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       47 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    12948 2024-04-10 16:14:34.469887 usgs-strec-2.3.4/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10865 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1389 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-10 16:14:34.469887 usgs-strec-2.3.4/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.453887 usgs-strec-2.3.4/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.457887 usgs-strec-2.3.4/src/strec/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:13:03.000000 usgs-strec-2.3.4/src/strec/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.457887 usgs-strec-2.3.4/src/strec/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8374 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/bin/regcalc.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/bin/strec_cfg.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8768 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/calc.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3562 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/cmt.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4869 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/config.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.465887 usgs-strec-2.3.4/src/strec/data/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      877 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/REGION_GRIDS_README.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:13:03.000000 usgs-strec-2.3.4/src/strec/data/__init__.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   750725 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/active.geojson
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    23487 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/backarc.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    36449 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/domains.xlsx
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    95983 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/land.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      240 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/maximum_interface_depths.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  6086656 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/moment_tensors.db
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   138345 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/ocean.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6153 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/select.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1753 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/selectspec.conf
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   271186 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/stable.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1794 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/strec.ini
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   204430 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/subduction.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24246 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/data/volcanic.geojson
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5461 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/database.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3635 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/distance.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7142 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/gcmt.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3389 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/gmreg.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2639 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/kagan.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8924 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/slab.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13186 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/sm_probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4493 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/subduction.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    23237 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/subtype.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8163 2024-04-10 16:11:14.000000 usgs-strec-2.3.4/src/strec/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-10 16:14:34.465887 usgs-strec-2.3.4/src/usgs_strec.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    12948 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1078 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       86 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      343 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        6 2024-04-10 16:14:34.000000 usgs-strec-2.3.4/src/usgs_strec.egg-info/top_level.txt
```

### Comparing `usgs-strec-2.3.3/LICENSE.md` & `usgs-strec-2.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/PKG-INFO` & `usgs-strec-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.3.3
+Version: 2.3.4
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -26,14 +26,15 @@
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: esi-utils-rupture
 Requires-Dist: geopy>=2.2.0
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: openpyxl>=3.0.9
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: rasterio>=1.2.10
+Requires-Dist: sciencebasepy>=2.0.16
 Requires-Dist: typer[all]<0.7.0
 Requires-Dist: xlrd>=2.0.1
 Requires-Dist: xlsxwriter>=3.0.1
 Requires-Dist: xlwt>=1.3.0
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
```

### Comparing `usgs-strec-2.3.3/README.md` & `usgs-strec-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/pyproject.toml` & `usgs-strec-2.3.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "configobj>=5.0.6",
     "esi-utils-rupture",
     "geopy>=2.2.0",
     "numpy>=1.21.0",
     "openpyxl>=3.0.9",
     "pandas>=1.3.5",
     "rasterio>=1.2.10",
+    "sciencebasepy>=2.0.16",
     "typer[all]<0.7.0",
     "xlrd>=2.0.1",
     "xlsxwriter>=3.0.1",
     "xlwt>=1.3.0",
 ]
 
 [options.package_data]
```

### Comparing `usgs-strec-2.3.3/src/strec/bin/regcalc.py` & `usgs-strec-2.3.4/src/strec/bin/regcalc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/bin/strec_cfg.py` & `usgs-strec-2.3.4/src/strec/bin/strec_cfg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/calc.py` & `usgs-strec-2.3.4/src/strec/calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 )
 
 # local imports
 from strec.subtype import SubductionSelector, get_event_details
 from strec.utils import read_input_file
 
 LOGGER = "subselect"
+MT_COMPS = ["mpp", "mrp", "mrr", "mrt", "mtp", "mtt"]
+MT_ANGLES = ["dip", "rake", "strike"]
 
 
 def get_input_dataframe(input_file, eqinfo, event_id, hypo_columns, id_column):
     """Create a dataframe of events (possibly only one).
 
     Args:
         input_file (str or None):  Name of input CSV/Excel file or None.
@@ -94,68 +96,38 @@
               - rake (degrees)
             - NP2 Second nodal plane values:
               - strike (degrees)
               - dip (degrees)
               - rake (degrees)
     """
     # row is a pandas series object
-    isreal = row.notnull()
-
-    has_mtt = row.index.str.contains("mtt", case=False)
-    has_mpp = row.index.str.contains("mpp", case=False)
-    has_mrr = row.index.str.contains("mrr", case=False)
-    has_mrt = row.index.str.contains("mrt", case=False)
-    has_mrp = row.index.str.contains("mrp", case=False)
-    has_mtp = row.index.str.contains("mtp", case=False)
-
-    mtts = row[isreal & has_mtt]
-    mpps = row[isreal & has_mpp]
-    mrrs = row[isreal & has_mrr]
-    mrts = row[isreal & has_mrt]
-    mrps = row[isreal & has_mrp]
-    mtps = row[isreal & has_mtp]
-
-    mtt = mpp = mrr = mrt = mrp = mtp = np.nan
-    if len(mtts):
-        mtt = float(mtts[0])
-    if len(mpps):
-        mpp = float(mpps[0])
-    if len(mrrs):
-        mrr = float(mrrs[0])
-    if len(mrts):
-        mrt = float(mrts[0])
-    if len(mrps):
-        mrp = float(mrps[0])
-    if len(mtps):
-        mtp = float(mtps[0])
-
-    if not np.isnan(np.sum([mtt, mpp, mrr, mrt, mrp, mtp])):
-        tensor_params = fill_tensor_from_components(mrr, mtt, mpp, mrt, mrp, mtp)
-        return tensor_params
-
-    has_strike = row.index.str.contains("strike", case=False)
-    has_dip = row.index.str.contains("dip", case=False)
-    has_rake = row.index.str.contains("rake", case=False)
-    strikes = row[isreal & has_strike]
-    dips = row[isreal & has_dip]
-    rakes = row[isreal & has_rake]
-
-    strike = dip = rake = np.nan
-    if len(strikes):
-        strike = strikes[0]
-    if len(dips):
-        dip = dips[0]
-    if len(rakes):
-        rake = rakes[0]
-
-    if not np.isnan(strike):
-        tensor_params = fill_tensor_from_angles(strike, dip, rake)
-        return tensor_params
+    # is it a series containing moment tensor components or focal angles?
+    indices = sorted([c.lower() for c in row.index.tolist()])
+    if indices != MT_COMPS and indices != MT_ANGLES:
+        return None
+    # are all values finite (non NaN)?
+    if row.notnull().sum() < len(row):
+        return None
+    rowdict = row.to_dict()
+    rowdict = {k.lower(): v for k, v in rowdict.items()}
+    if indices == MT_COMPS:
+        tensor_params = fill_tensor_from_components(
+            rowdict["mrr"],
+            rowdict["mtt"],
+            rowdict["mpp"],
+            rowdict["mrt"],
+            rowdict["mrp"],
+            rowdict["mtp"],
+        )
+    else:
+        tensor_params = fill_tensor_from_angles(
+            rowdict["strike"], rowdict["dip"], rowdict["rake"]
+        )
 
-    return None
+    return tensor_params
 
 
 def check_moment_row(row):
     """Check row of dataframe for presence of moment tensor information.
 
     Args:
         row (pandas Series): Series possibly containing moment tensor data
```

### Comparing `usgs-strec-2.3.3/src/strec/cmt.py` & `usgs-strec-2.3.4/src/strec/cmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/config.py` & `usgs-strec-2.3.4/src/strec/config.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/REGION_GRIDS_README.txt` & `usgs-strec-2.3.4/src/strec/data/REGION_GRIDS_README.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/active.geojson` & `usgs-strec-2.3.4/src/strec/data/active.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/backarc.geojson` & `usgs-strec-2.3.4/src/strec/data/backarc.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/domains.xlsx` & `usgs-strec-2.3.4/src/strec/data/domains.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/land.geojson` & `usgs-strec-2.3.4/src/strec/data/land.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/moment_tensors.db` & `usgs-strec-2.3.4/src/strec/data/moment_tensors.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/ocean.geojson` & `usgs-strec-2.3.4/src/strec/data/ocean.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/select.conf` & `usgs-strec-2.3.4/src/strec/data/select.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/selectspec.conf` & `usgs-strec-2.3.4/src/strec/data/selectspec.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/stable.geojson` & `usgs-strec-2.3.4/src/strec/data/stable.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/strec.ini` & `usgs-strec-2.3.4/src/strec/data/strec.ini`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/subduction.geojson` & `usgs-strec-2.3.4/src/strec/data/subduction.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/data/volcanic.geojson` & `usgs-strec-2.3.4/src/strec/data/volcanic.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/database.py` & `usgs-strec-2.3.4/src/strec/database.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/distance.py` & `usgs-strec-2.3.4/src/strec/distance.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/gcmt.py` & `usgs-strec-2.3.4/src/strec/gcmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/gmreg.py` & `usgs-strec-2.3.4/src/strec/gmreg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/kagan.py` & `usgs-strec-2.3.4/src/strec/kagan.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/slab.py` & `usgs-strec-2.3.4/src/strec/slab.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 # stdlib imports
 import logging
 import pathlib
+import re
 import tarfile
 import zipfile
 from io import BytesIO
 
 # third party imports
 import numpy as np
 import pandas as pd
 import rasterio
 import requests
+import sciencebasepy as pysb
 from rasterio.windows import Window
 
 MAX_INTERFACE_DEPTH = 70  # depth beyond which any tectonic regime has to be intraslab
 
 # Slab 1.0 does not have depth uncertainty, so we make this a constant
 DEFAULT_DEPTH_ERROR = 10
 
-ITEM_TEMPLATE = "http://www.sciencebase.gov/catalog/file/get/[ITEMID]"
+ITEM_TEMPLATE = "https://www.sciencebase.gov/catalog/item/{itemid}?format=json"
+# ITEM_TEMPLATE = "http://www.sciencebase.gov/catalog/file/get/[ITEMID]"
 SEARCH_URL = "https://www.sciencebase.gov/catalog/items?s=Search&q=slab2&format=json"
 KEYWORDS = ["subduction", "model", "slab2"]
+SLABGRID_REGEX = "dep|str|dip|unc"
 
 
 def get_slab_grids(path):
     if not path.exists():
         path.mkdir(parents=True)
     response = requests.get(SEARCH_URL)
     jdict = response.json()
+    nfiles = 0
     for item in jdict["items"]:
         ititle = item["title"].lower()
         # is this the droid we're looking for?
         if not item["hasChildren"]:
             continue
         score = 0
         for keyword in KEYWORDS:
             if keyword in ititle:
                 score += 1
         if score < 2:
             continue
         itemid = item["id"]
-        item_url = ITEM_TEMPLATE.replace("[ITEMID]", itemid)
-        response = requests.get(item_url)
-        bytes = BytesIO(response.content)
-        nfiles = 0
-        with zipfile.ZipFile(bytes, "r") as myzip:
-            for name in myzip.namelist():
-                if not name.endswith("tar.gz"):
+        sb = pysb.SbSession()
+        slab_children = sb.get_child_ids(itemid)
+        for child_id in slab_children:
+            slab_child = sb.get_item(child_id)
+            _, region = slab_child["title"].split(",")
+            print(f"Downloading grids for {region.strip()}...")
+            for tfile in slab_child["files"]:
+                fname = tfile["name"]
+                if not fname.endswith(".grd"):
                     continue
-                tarbytes = myzip.read(name)
-                try:
-                    my_tarfile = path / name
-                    with open(my_tarfile, "wb") as tar:
-                        tar.write(tarbytes)
-                    with tarfile.open(my_tarfile, "r") as mytar:
-                        for member_str in mytar.getnames():
-                            if not member_str.endswith(".grd"):
-                                continue
-                            outfile = path / pathlib.Path(member_str).name
-                            member = mytar.getmember(member_str)
-                            logging.info(f"Unpacking slab grid {member_str}...")
-                            with mytar.extractfile(member) as in_object:
-                                with open(outfile, "wb") as out_object:
-                                    out_object.write(in_object.read())
-                                    nfiles += 1
-                except Exception as e:
-                    return (
-                        False,
-                        f"Unable to download Slab2 grids from {SEARCH_URL} - error {str(e)}.",
-                    )
+                if re.search(SLABGRID_REGEX, fname) is not None:
+                    print(f"\tRetrieving {fname}...")
+                    url = tfile["downloadUri"]
+                    response = requests.get(url)
+                    outfile = path / fname
+                    with open(outfile, "wb") as fout:
+                        fout.write(response.content)
+                    nfiles += 1
+
     return (True, f"Downloaded {nfiles} grid files from {SEARCH_URL} to {path}")
 
 
 class GridSlab(object):
     """Represents USGS Slab model grids for a given subduction zone."""
 
     def __init__(self, depth_file, dip_file, strike_file, error_file):
```

### Comparing `usgs-strec-2.3.3/src/strec/sm_probs.py` & `usgs-strec-2.3.4/src/strec/sm_probs.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/subduction.py` & `usgs-strec-2.3.4/src/strec/subduction.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/subtype.py` & `usgs-strec-2.3.4/src/strec/subtype.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/strec/utils.py` & `usgs-strec-2.3.4/src/strec/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.3.3/src/usgs_strec.egg-info/PKG-INFO` & `usgs-strec-2.3.4/src/usgs_strec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.3.3
+Version: 2.3.4
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -26,14 +26,15 @@
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: esi-utils-rupture
 Requires-Dist: geopy>=2.2.0
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: openpyxl>=3.0.9
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: rasterio>=1.2.10
+Requires-Dist: sciencebasepy>=2.0.16
 Requires-Dist: typer[all]<0.7.0
 Requires-Dist: xlrd>=2.0.1
 Requires-Dist: xlsxwriter>=3.0.1
 Requires-Dist: xlwt>=1.3.0
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
```

### Comparing `usgs-strec-2.3.3/src/usgs_strec.egg-info/SOURCES.txt` & `usgs-strec-2.3.4/src/usgs_strec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

