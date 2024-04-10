# Comparing `tmp/fifids-0.1.0.tar.gz` & `tmp/fifids-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fifids-0.1.0.tar", max compression
+gzip compressed data, was "fifids-0.1.1.tar", max compression
```

## Comparing `fifids-0.1.0.tar` & `fifids-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1147 2024-04-09 06:14:11.121075 fifids-0.1.0/README.md
--rw-r--r--   0        0        0       21 2024-04-04 16:43:15.248304 fifids-0.1.0/fifids/__init__.py
--rw-r--r--   0        0        0       22 2024-04-04 16:43:07.935097 fifids-0.1.0/fifids/api/__init__.py
--rw-r--r--   0        0        0       66 2024-04-07 07:03:11.515043 fifids-0.1.0/fifids/api/encoders/__init__.py
--rw-r--r--   0        0        0      716 2024-04-07 08:23:09.550876 fifids-0.1.0/fifids/api/encoders/label.py
--rw-r--r--   0        0        0      396 2024-04-07 08:21:06.513446 fifids-0.1.0/fifids/api/encoders/one_hot.py
--rw-r--r--   0        0        0     2232 2024-04-09 06:44:31.614417 fifids-0.1.0/fifids/api/fifi.py
--rw-r--r--   0        0        0       30 2024-04-08 13:38:50.345040 fifids-0.1.0/fifids/api/outliers/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-09 06:13:28.368976 fifids-0.1.0/fifids/api/outliers/outliers.py
--rw-r--r--   0        0        0       30 2024-04-08 14:08:25.885563 fifids-0.1.0/fifids/api/pipeline/__init__.py
--rw-r--r--   0        0        0     3865 2024-04-09 06:44:31.615187 fifids-0.1.0/fifids/api/pipeline/pipeline.py
--rw-r--r--   0        0        0     2202 2024-04-09 06:20:37.939318 fifids-0.1.0/fifids/api/plot.py
--rw-r--r--   0        0        0      111 2024-04-07 09:28:19.458902 fifids-0.1.0/fifids/api/plots/__init__.py
--rw-r--r--   0        0        0      929 2024-04-07 08:22:10.469354 fifids-0.1.0/fifids/api/plots/correlation.py
--rw-r--r--   0        0        0      466 2024-04-07 07:42:23.360074 fifids-0.1.0/fifids/api/plots/distribution.py
--rw-r--r--   0        0        0     1241 2024-04-09 06:33:55.662121 fifids-0.1.0/fifids/api/plots/time_series.py
--rw-r--r--   0        0        0       33 2024-04-04 15:26:26.969977 fifids-0.1.0/fifids/utility/__init__.py
--rw-r--r--   0        0        0      296 2024-04-04 16:11:07.326176 fifids-0.1.0/fifids/utility/pretty_print.py
--rw-r--r--   0        0        0      507 2024-04-09 09:06:40.335406 fifids-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 fifids-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1147 2024-04-09 09:08:27.179764 fifids-0.1.1/README.md
+-rw-r--r--   0        0        0       21 2024-04-04 16:43:15.248304 fifids-0.1.1/fifids/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 16:43:07.935097 fifids-0.1.1/fifids/api/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-07 07:03:11.515043 fifids-0.1.1/fifids/api/encoders/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-07 08:23:09.550876 fifids-0.1.1/fifids/api/encoders/label.py
+-rw-r--r--   0        0        0      396 2024-04-07 08:21:06.513446 fifids-0.1.1/fifids/api/encoders/one_hot.py
+-rw-r--r--   0        0        0     2232 2024-04-09 06:44:31.614417 fifids-0.1.1/fifids/api/fifi.py
+-rw-r--r--   0        0        0       30 2024-04-08 13:38:50.345040 fifids-0.1.1/fifids/api/outliers/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-09 06:13:28.368976 fifids-0.1.1/fifids/api/outliers/outliers.py
+-rw-r--r--   0        0        0       30 2024-04-08 14:08:25.885563 fifids-0.1.1/fifids/api/pipeline/__init__.py
+-rw-r--r--   0        0        0     3865 2024-04-09 06:44:31.615187 fifids-0.1.1/fifids/api/pipeline/pipeline.py
+-rw-r--r--   0        0        0     2202 2024-04-09 06:20:37.939318 fifids-0.1.1/fifids/api/plot.py
+-rw-r--r--   0        0        0      111 2024-04-07 09:28:19.458902 fifids-0.1.1/fifids/api/plots/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-07 08:22:10.469354 fifids-0.1.1/fifids/api/plots/correlation.py
+-rw-r--r--   0        0        0      466 2024-04-07 07:42:23.360074 fifids-0.1.1/fifids/api/plots/distribution.py
+-rw-r--r--   0        0        0     1241 2024-04-09 06:33:55.662121 fifids-0.1.1/fifids/api/plots/time_series.py
+-rw-r--r--   0        0        0       33 2024-04-04 15:26:26.969977 fifids-0.1.1/fifids/utility/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-04 16:11:07.326176 fifids-0.1.1/fifids/utility/pretty_print.py
+-rw-r--r--   0        0        0      506 2024-04-10 06:43:05.922859 fifids-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 fifids-0.1.1/PKG-INFO
```

### Comparing `fifids-0.1.0/README.md` & `fifids-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Fifi
 ## data science for swiss cheese brains
----
 
 Fifi is a pypi package for quick eda and modelling made specifically for use with Jupyter Notebooks.
 Use `??` as much as possible to see the code and adapt it for your needs. The package will guide you through the usual EDA process.
 
 The package is meant be a source of cool plots or workflows and be able to use them within Jupyter without having to look at documentation every time.
 
 ## Installation
 
 ```bash
-pip install fifi
+pip install fifids
 ```
 
 ## Usage
 
 ```python
-from fifi import Fifi
+from fifids import Fifi
 import pandas as pd
 import polars as pl
 
 df = pd.read_csv("data.csv")
 # OR POLARS
 df = pl.read_csv("data.csv")
 # Note from author: eventually, right now it breaks with polars, but I'm working on it
```

### Comparing `fifids-0.1.0/fifids/api/encoders/label.py` & `fifids-0.1.1/fifids/api/encoders/label.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/fifi.py` & `fifids-0.1.1/fifids/api/fifi.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/outliers/outliers.py` & `fifids-0.1.1/fifids/api/outliers/outliers.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/pipeline/pipeline.py` & `fifids-0.1.1/fifids/api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/plot.py` & `fifids-0.1.1/fifids/api/plot.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/plots/correlation.py` & `fifids-0.1.1/fifids/api/plots/correlation.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/fifids/api/plots/time_series.py` & `fifids-0.1.1/fifids/api/plots/time_series.py`

 * *Files identical despite different names*

### Comparing `fifids-0.1.0/PKG-INFO` & `fifids-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: fifids
-Version: 0.1.0
+Version: 0.1.1
 Summary: data science for swiss cheese brains
 Author: fibleep
 Author-email: filipn924@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: shap (>=0.45.0,<0.46.0)
 Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
 Requires-Dist: xgboost (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Fifi
 ## data science for swiss cheese brains
----
 
 Fifi is a pypi package for quick eda and modelling made specifically for use with Jupyter Notebooks.
 Use `??` as much as possible to see the code and adapt it for your needs. The package will guide you through the usual EDA process.
 
 The package is meant be a source of cool plots or workflows and be able to use them within Jupyter without having to look at documentation every time.
 
 ## Installation
 
 ```bash
-pip install fifi
+pip install fifids
 ```
 
 ## Usage
 
 ```python
-from fifi import Fifi
+from fifids import Fifi
 import pandas as pd
 import polars as pl
 
 df = pd.read_csv("data.csv")
 # OR POLARS
 df = pl.read_csv("data.csv")
 # Note from author: eventually, right now it breaks with polars, but I'm working on it
```

