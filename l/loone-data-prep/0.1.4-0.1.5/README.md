# Comparing `tmp/loone_data_prep-0.1.4.tar.gz` & `tmp/loone_data_prep-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loone_data_prep-0.1.4.tar", last modified: Thu Mar 14 22:32:30 2024, max compression
+gzip compressed data, was "loone_data_prep-0.1.5.tar", last modified: Wed Apr 10 21:41:38 2024, max compression
```

## Comparing `loone_data_prep-0.1.4.tar` & `loone_data_prep-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.127251 loone_data_prep-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-14 22:32:30.127251 loone_data_prep-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.123251 loone_data_prep-0.1.4/loone_data_prep/
--rw-r--r--   0 runner    (1001) docker     (127)    35394 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/GEOGLOWS_LOONE_DATA_PREP.py
--rw-r--r--   0 runner    (1001) docker     (127)    59777 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/LOONE_DATA_PREP.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/data_analyses_fns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.123251 loone_data_prep-0.1.4/loone_data_prep/flow_data/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/S65E_total.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/forecast_bias_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/get_forecast_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/get_inflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/get_outflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/flow_data/hydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    25019 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.123251 loone_data_prep-0.1.4/loone_data_prep/water_level_data/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_level_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_level_data/get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_level_data/hydro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.123251 loone_data_prep-0.1.4/loone_data_prep/water_quality_data/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_quality_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_quality_data/get_inflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_quality_data/get_lake_wq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/water_quality_data/wq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.123251 loone_data_prep-0.1.4/loone_data_prep/weather_data/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/weather_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/weather_data/get_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/loone_data_prep/weather_data/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 22:32:30.127251 loone_data_prep-0.1.4/loone_data_prep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-14 22:32:30.000000 loone_data_prep-0.1.4/loone_data_prep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-14 22:32:30.000000 loone_data_prep-0.1.4/loone_data_prep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 22:32:30.000000 loone_data_prep-0.1.4/loone_data_prep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 22:32:30.000000 loone_data_prep-0.1.4/loone_data_prep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-14 22:32:30.000000 loone_data_prep-0.1.4/loone_data_prep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-14 22:32:22.000000 loone_data_prep-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 22:32:30.127251 loone_data_prep-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.488219 loone_data_prep-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.480219 loone_data_prep-0.1.5/loone_data_prep/
+-rw-r--r--   0 runner    (1001) docker     (127)    35394 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/GEOGLOWS_LOONE_DATA_PREP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59777 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/LOONE_DATA_PREP.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/data_analyses_fns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/loone_data_prep/flow_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/S65E_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/forecast_bias_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/get_forecast_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/get_inflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/get_outflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/flow_data/hydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25019 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/loone_data_prep/water_level_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_level_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_level_data/get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_level_data/hydro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/loone_data_prep/water_quality_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_quality_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_quality_data/get_inflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_quality_data/get_lake_wq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/water_quality_data/wq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/loone_data_prep/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/weather_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/weather_data/get_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/loone_data_prep/weather_data/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:38.484219 loone_data_prep-0.1.5/loone_data_prep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-10 21:41:38.000000 loone_data_prep-0.1.5/loone_data_prep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-10 21:41:38.000000 loone_data_prep-0.1.5/loone_data_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:41:38.000000 loone_data_prep-0.1.5/loone_data_prep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 21:41:38.000000 loone_data_prep-0.1.5/loone_data_prep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 21:41:38.000000 loone_data_prep-0.1.5/loone_data_prep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-10 21:41:34.000000 loone_data_prep-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:41:38.488219 loone_data_prep-0.1.5/setup.cfg
```

### Comparing `loone_data_prep-0.1.4/LICENSE` & `loone_data_prep-0.1.5/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD-3-Clause License
 
-Copyright (c) 2023 Aquaveo
+Copyright (c) 2024 University of South Florida
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
```

### Comparing `loone_data_prep-0.1.4/PKG-INFO` & `loone_data_prep-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-Metadata-Version: 2.1
-Name: loone_data_prep
-Version: 0.1.4
-Summary: Prepare data to run the LOONE model.
-Author-email: Michael Souffront <msouffront@aquaveo.com>, James Dolinar <jdolinar@aquaveo.com>, Osama Tarabih <osamatarabih@usf.edu>
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: rpy2
-Requires-Dist: retry
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: geoglows>=0.27.1
-
 LOONE_DATA_PREP
 # LOONE_DATA_PREP
 
 Prepare data for the LOONE water quality model.
 
-Link to LOONE model repository: [https://github.com/osamatarabih/LOONE](https://github.com/osamatarabih/LOONE)
+Line to the LOONE model: [https://pypi.org/project/loone](https://pypi.org/project/loone)
+Link to LOONE model repository: [https://github.com/Aquaveo/LOONE](https://github.com/Aquaveo/LOONE)
 
 ## Prerequisites:
 
 * R ([https://www.r-project.org/](https://www.r-project.org/))
 * R packages: dbhydroR, rio, dplyr
 
 ## Installation:
 
 ```bash
-cd /path/to/loone_data_prep/
-pip install .
+pip install loone_data_prep
+```
+
+### Development Installation:
+
+```bash
+cd /path/to/loone_data_prep/repo
+pip install -e .
 ```
 
 ### Examples
 
 **From the command line:**
 
 ```bash
```

### Comparing `loone_data_prep-0.1.4/loone_data_prep/GEOGLOWS_LOONE_DATA_PREP.py` & `loone_data_prep-0.1.5/loone_data_prep/GEOGLOWS_LOONE_DATA_PREP.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/LOONE_DATA_PREP.py` & `loone_data_prep-0.1.5/loone_data_prep/LOONE_DATA_PREP.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/data_analyses_fns.py` & `loone_data_prep-0.1.5/loone_data_prep/data_analyses_fns.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/S65E_total.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/S65E_total.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/forecast_bias_correction.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/forecast_bias_correction.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/get_forecast_flows.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/get_forecast_flows.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/get_inflows.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/get_inflows.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/get_outflows.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/get_outflows.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/flow_data/hydro.py` & `loone_data_prep-0.1.5/loone_data_prep/flow_data/hydro.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/utils.py` & `loone_data_prep-0.1.5/loone_data_prep/utils.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/water_level_data/get_all.py` & `loone_data_prep-0.1.5/loone_data_prep/water_level_data/get_all.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/water_level_data/hydro.py` & `loone_data_prep-0.1.5/loone_data_prep/water_level_data/hydro.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/water_quality_data/get_inflows.py` & `loone_data_prep-0.1.5/loone_data_prep/water_quality_data/get_inflows.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/water_quality_data/get_lake_wq.py` & `loone_data_prep-0.1.5/loone_data_prep/water_quality_data/get_lake_wq.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/water_quality_data/wq.py` & `loone_data_prep-0.1.5/loone_data_prep/water_quality_data/wq.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/weather_data/get_all.py` & `loone_data_prep-0.1.5/loone_data_prep/weather_data/get_all.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep/weather_data/weather.py` & `loone_data_prep-0.1.5/loone_data_prep/weather_data/weather.py`

 * *Files identical despite different names*

### Comparing `loone_data_prep-0.1.4/loone_data_prep.egg-info/SOURCES.txt` & `loone_data_prep-0.1.5/loone_data_prep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

