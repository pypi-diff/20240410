# Comparing `tmp/ecopipeline-0.2.4.tar.gz` & `tmp/ecopipeline-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.4.tar", last modified: Fri Mar 22 22:53:37 2024, max compression
+gzip compressed data, was "ecopipeline-0.2.5.tar", last modified: Wed Apr 10 20:53:04 2024, max compression
```

## Comparing `ecopipeline-0.2.4.tar` & `ecopipeline-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.455947 ecopipeline-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23219 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-03-22 22:52:24.000000 ecopipeline-0.2.4/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 22:53:37.459947 ecopipeline-0.2.4/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-22 22:53:37.000000 ecopipeline-0.2.4/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-22 22:53:37.000000 ecopipeline-0.2.4/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 22:53:37.000000 ecopipeline-0.2.4/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 22:53:37.000000 ecopipeline-0.2.4/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-22 22:53:37.000000 ecopipeline-0.2.4/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.299634 ecopipeline-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.299634 ecopipeline-0.2.5/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23669 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.4/PKG-INFO` & `ecopipeline-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.4
+Version: 0.2.5
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.4/README.md` & `ecopipeline-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/setup.cfg` & `ecopipeline-0.2.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.4
+version = 0.2.5
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.4/src/ecopipeline/extract/extract.py` & `ecopipeline-0.2.5/src/ecopipeline/extract/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,25 +215,29 @@
                     norm_data.index.values[i] = norm_data.index[i] + pd.Timedelta(seconds=1)
             temp_dfs.append(norm_data)
 
     df = pd.concat(temp_dfs, ignore_index=False)
     return df
 
 
-def csv_to_df(csv_filenames: List[str], mb_prefix : bool = False) -> pd.DataFrame:
+def csv_to_df(csv_filenames: List[str], mb_prefix : bool = False, round_time_index : bool = True) -> pd.DataFrame:
     """
     Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for aquisuite data. 
 
     Parameters
     ----------  
     csv_filenames: List[str]
         List of filenames to be processed into a single dataframe 
     mb_prefix: bool
         A boolean that signifys if the data is in modbus form- if set to true, will prepend modbus prefix to each raw varriable name
-    
+    round_time_index: bool
+        A boolean that signifys if the dataframe timestamp indexes should be rounded down to the nearest minute.
+        Should be set to False if there is no column in the data frame called 'time(UTC)' to index on.
+        Defaults to True.
+        
     Returns
     ------- 
     pd.DataFrame: 
         Pandas Dataframe containing data from all files with column headers the same as the variable names in the files 
         (with prepended modbus prefix if mb_prefix = True)
     """
     temp_dfs = []
@@ -260,20 +264,21 @@
                     print(f"Error reading {file}: No 'time(UTC)' column found.")
                     continue
                 
             temp_dfs.append(data)
 
     df = pd.concat(temp_dfs, ignore_index=False) 
     
-    #round down all seconds, 99% of points come in between 0 and 30 seconds but there are a few that are higher
-    df.index = df.index.floor('T')
-    
-    #group and sort index
-    df = df.groupby(df.index).mean(numeric_only=True)
-    df.sort_index(inplace = True)
+    if round_time_index:
+        #round down all seconds, 99% of points come in between 0 and 30 seconds but there are a few that are higher
+        df.index = df.index.floor('T')
+        
+        #group and sort index
+        df = df.groupby(df.index).mean(numeric_only=True)
+        df.sort_index(inplace = True)
 
     return df
 
 def msa_to_df(csv_filenames: List[str], mb_prefix : bool = False, time_zone: str = 'US/Pacific') -> pd.DataFrame:
      """
     Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for MSA data. 
 
@@ -369,19 +374,23 @@
     -------
     dict: 
         Dictionary with key as Station Name and Value as DF of Parsed Weather Data
     """
     formatted_dfs = {}
     weather_directory = config.get_weather_dir_path()
     try:
+        print("here 3")
         noaa_dictionary = _get_noaa_dictionary(weather_directory)
+        print("here 4")
         station_ids = {noaa_dictionary[station_name]
             : station_name for station_name in station_names if station_name in noaa_dictionary}
         noaa_filenames = _download_noaa_data(station_ids, weather_directory)
+        print("here 5")
         noaa_dfs = _convert_to_df(station_ids, noaa_filenames, weather_directory)
+        print("here 6")
         formatted_dfs = _format_df(station_ids, noaa_dfs)
     except:
         # temporary solution for NOAA ftp not including 2024
         noaa_df = pd.DataFrame(index=pd.date_range(start='2024-01-01', periods=10, freq='H'))
         noaa_df['conditions'] = None
         noaa_df['airTemp_F'] = None
         noaa_df['dewPoint_F'] = None
```

### Comparing `ecopipeline-0.2.4/src/ecopipeline/load/load.py` & `ecopipeline-0.2.5/src/ecopipeline/load/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.2.5/src/ecopipeline/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.2.5/src/ecopipeline/transform/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.2.5/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/transform/transform.py` & `ecopipeline-0.2.5/src/ecopipeline/transform/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.2.5/src/ecopipeline/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.2.5/src/ecopipeline/utils/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.4/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.2.5/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.4
+Version: 0.2.5
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.4/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.2.5/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

