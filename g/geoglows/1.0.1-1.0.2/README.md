# Comparing `tmp/geoglows-1.0.1.tar.gz` & `tmp/geoglows-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.1.tar", last modified: Tue Apr  9 20:45:48 2024, max compression
+gzip compressed data, was "geoglows-1.0.2.tar", last modified: Tue Apr  9 21:02:08 2024, max compression
```

## Comparing `geoglows-1.0.1.tar` & `geoglows-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 20:45:44.000000 geoglows-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 20:45:44.000000 geoglows-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 20:45:48.479342 geoglows-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 20:45:44.000000 geoglows-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.475342 geoglows-1.0.1/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 20:45:44.000000 geoglows-1.0.1/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:45:48.479342 geoglows-1.0.1/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 20:45:48.000000 geoglows-1.0.1/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 20:45:44.000000 geoglows-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:45:48.479342 geoglows-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 20:45:44.000000 geoglows-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.709809 geoglows-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 21:02:04.000000 geoglows-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 21:02:04.000000 geoglows-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 21:02:08.705809 geoglows-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 21:02:04.000000 geoglows-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 21:02:04.000000 geoglows-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:02:08.709809 geoglows-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 21:02:04.000000 geoglows-1.0.2/setup.py
```

### Comparing `geoglows-1.0.1/LICENSE` & `geoglows-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/PKG-INFO` & `geoglows-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.1/README.md` & `geoglows-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/format_tools.py` & `geoglows-1.0.2/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.2/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.2/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.2/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.2/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/_plots/plots.py` & `geoglows-1.0.2/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/analyze.py` & `geoglows-1.0.2/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/bias.py` & `geoglows-1.0.2/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/data.py` & `geoglows-1.0.2/geoglows/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from io import StringIO
 
 import pandas as pd
 import requests
 import s3fs
 import xarray as xr
 
-from ._constants import METADATA_TABLE_LOCAL_PATH
+from ._constants import METADATA_TABLE_PATH
 from .analyze import (
     simple_forecast as calc_simple_forecast,
     forecast_stats as calc_forecast_stats,
     daily_averages as calc_daily_averages,
     monthly_averages as calc_monthly_averages,
     annual_averages as calc_annual_averages,
 )
@@ -338,18 +338,18 @@
     Retrieves the master table of stream reaches with all metadata and properties as a pandas DataFrame
     Args:
         columns: optional subset of columns names to read from the parquet
 
     Returns:
         pd.DataFrame
     """
-    if os.path.exists(METADATA_TABLE_LOCAL_PATH):
-        return pd.read_parquet(METADATA_TABLE_LOCAL_PATH, columns=columns)
+    if os.path.exists(METADATA_TABLE_PATH):
+        return pd.read_parquet(METADATA_TABLE_PATH, columns=columns)
     warn = f"""
     Local copy of geoglows v2 metadata table not found. You should download a copy for optimal performance and 
-    to make the data available when you are offline. A copy of the table will be cached at {METADATA_TABLE_LOCAL_PATH}.
+    to make the data available when you are offline. A copy of the table will be cached at {METADATA_TABLE_PATH}.
     """
     warnings.warn(warn)
     df = pd.read_parquet('https://geoglows-v2.s3-website-us-west-2.amazonaws.com/tables/package-metadata-table.parquet')
-    os.makedirs(os.path.dirname(METADATA_TABLE_LOCAL_PATH), exist_ok=True)
-    df.to_parquet(METADATA_TABLE_LOCAL_PATH)
+    os.makedirs(os.path.dirname(METADATA_TABLE_PATH), exist_ok=True)
+    df.to_parquet(METADATA_TABLE_PATH)
     return df[columns] if columns else df
```

### Comparing `geoglows-1.0.1/geoglows/streams.py` & `geoglows-1.0.2/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows/tables.py` & `geoglows-1.0.2/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.2/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.1/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.2/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.1/setup.py` & `geoglows-1.0.2/setup.py`

 * *Files identical despite different names*

