# Comparing `tmp/sufficiency_data_transform-0.1.2.tar.gz` & `tmp/sufficiency_data_transform-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufficiency_data_transform-0.1.2.tar", max compression
+gzip compressed data, was "sufficiency_data_transform-0.1.3.tar", max compression
```

## Comparing `sufficiency_data_transform-0.1.2.tar` & `sufficiency_data_transform-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1022 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/README.md
--rw-r--r--   0        0        0      500 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/__init__.py
--rw-r--r--   0        0        0      138 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/__main__.py
--rw-r--r--   0        0        0    19986 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/all_dim_and_fact.py
--rw-r--r--   0        0        0    21424 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/dim_maps.py
--rw-r--r--   0        0        0     3397 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/maps.py
--rw-r--r--   0        0        0     3021 2024-04-05 09:20:21.457081 sufficiency_data_transform-0.1.2/sufficiency_data_transform/utils.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 sufficiency_data_transform-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1022 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/README.md
+-rw-r--r--   0        0        0      511 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/__main__.py
+-rw-r--r--   0        0        0    19678 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/all_dim_and_fact.py
+-rw-r--r--   0        0        0    21424 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/dim_maps.py
+-rw-r--r--   0        0        0     3404 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/maps.py
+-rw-r--r--   0        0        0     2594 2024-04-10 09:43:08.025786 sufficiency_data_transform-0.1.3/sufficiency_data_transform/utils.py
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 sufficiency_data_transform-0.1.3/PKG-INFO
```

### Comparing `sufficiency_data_transform-0.1.2/README.md` & `sufficiency_data_transform-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sufficiency_data_transform-0.1.2/sufficiency_data_transform/all_dim_and_fact.py` & `sufficiency_data_transform-0.1.3/sufficiency_data_transform/all_dim_and_fact.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         "PlacementPostcodeKey",
         "OfstedProviderKey",
         "ONSAreaKey",
         "SubmissionYearDateKey",
     ]
     episodes = fillna_categorical_columns(episodes, episode_key_columns)
 
-    write_csv(episodes, fs_out, "Output data//factEpisode.csv", False)
+    write_csv(episodes, fs_out, "factEpisode.csv", False)
 
 
 def create_factOfstedInspection():
     fs_out = open_location(output_location)
     fs_ext = open_location(input_location_ext)
 
     ofsted_effectiveness = open_file(fs_out, "dimOfstedEffectiveness.csv")
@@ -495,38 +495,38 @@
 
     factOfstedInspection = pd.concat(
         [provider_level_in_year_2022_23, provider_level_at_31Aug]
     )
     factOfstedInspection = factOfstedInspection.drop_duplicates(
         subset=["URN", "Inspection date"], keep="first"
     )
+    factOfstedInspection.reset_index(drop=True, inplace=True)
 
     # create IsLatest column that indicates if inspection is the most recent one recorded for a URN
     factOfstedInspection["IsLatest"] = (
         factOfstedInspection.groupby("URN")["Inspection date"].transform("max")
         == factOfstedInspection["Inspection date"]
     )
 
-    # Update the EndDate where isLatest is True with 2999 if EndDate is missing, otherwise keep it the same as InspectionDateKey
-    factOfstedInspection.loc[factOfstedInspection["IsLatest"] == True, "EndDateKey"] = (
-        factOfstedInspection.loc[
-            factOfstedInspection["IsLatest"] == True, "Inspection date"
-        ]
+    factOfstedInspection.sort_values(
+        by=["Inspection date"],
+        inplace=True,
+    )
+
+    # where isLatest is True, EndDate should be InspectionDate for that URN on that date/row
+    factOfstedInspection.loc[factOfstedInspection["IsLatest"], "EndDateKey"] = (
+        factOfstedInspection.loc[factOfstedInspection["IsLatest"], "Inspection date"]
+    )
+
+    # where isLatest is False, EndDate should be the next chronological inspection date for that URN
+    factOfstedInspection.loc[~factOfstedInspection["IsLatest"], "EndDateKey"] = (
+        factOfstedInspection.groupby("URN")["Inspection date"].shift(-1)
     )
-    factOfstedInspection["EndDateKey"].fillna("2999-12-31", inplace=True)
 
-    # Find the next inspection date for each row where isLatest is False
-    next_inspection_dates = factOfstedInspection.loc[
-        factOfstedInspection["IsLatest"] == False, "Inspection date"
-    ].shift(-1)
-
-    # Update the EndDate where isLatest is False with the next inspection date
-    factOfstedInspection.loc[
-        factOfstedInspection["IsLatest"] == False, "EndDateKey"
-    ] = next_inspection_dates
+    factOfstedInspection["EndDateKey"].fillna("2999-12-31", inplace=True)
 
     factOfstedInspection = factOfstedInspection.rename(columns=inspection_map)
     factOfstedInspection = factOfstedInspection[
         ["InspectionDateKey", "EndDateKey", "OwnerName", "Effectiveness", "IsLatest"]
     ]
 
     factOfstedInspection.IsLatest = factOfstedInspection.IsLatest.map(
@@ -566,17 +566,7 @@
     key_columns = ["OfstedProviderKey", "OfstedEffectivenessKey"]
     factOfstedInspection = fillna_categorical_columns(factOfstedInspection, key_columns)
 
     factOfstedInspection.reset_index(inplace=True, drop=True)
     factOfstedInspection.reset_index(inplace=True, names="factOfstedInspectionKey")
 
     write_csv(factOfstedInspection, fs_out, "factOfstedInspection.csv")
-
-
-def create_sufficiency_data():
-    create_dim_tables()
-    create_dimONSArea()
-    create_dimLookedAfterChild()
-    create_dimOfstedProvider()
-    create_dimPostcode()
-    create_factEpisode()
-    create_factOfstedInspection()
```

### Comparing `sufficiency_data_transform-0.1.2/sufficiency_data_transform/dim_maps.py` & `sufficiency_data_transform-0.1.3/sufficiency_data_transform/dim_maps.py`

 * *Files identical despite different names*

### Comparing `sufficiency_data_transform-0.1.2/sufficiency_data_transform/maps.py` & `sufficiency_data_transform-0.1.3/sufficiency_data_transform/maps.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,16 +103,15 @@
     "Kingston upon Hull": "Kingston upon Hull, City of",
     "Southend on Sea": "Southend-on-Sea",
 }
 
 episodes_map = {
     "DECOM": "EpisodeCommencedDateKey",
     "DEC": "EpisodeCeasedDateKey",
-    "YEAR": "SubmissionYearDateKey",
+    # SubmissionYearDateKey in factEpisode will come from the merge with the dimLookedAfterChild table
 }
 
 inspection_map = {
     "Inspection date": "InspectionDateKey",
-    "Inspection publication date": "EndDateKey",  # change
     "Organisation which owns the provider": "OwnerName",  # to get OfstedProviderKey
     "Overall experiences and progress of children and young people": "Effectiveness",  # to get OfstedEffectivenessKey
 }
```

### Comparing `sufficiency_data_transform-0.1.2/sufficiency_data_transform/utils.py` & `sufficiency_data_transform-0.1.3/sufficiency_data_transform/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import chardet
 import pandas as pd
 from fs import open_fs
-from io import StringIO
 import csv
+import warnings
 
 
 def remove_duplicate_columns(df):
     """
-    ---- Hacky fix-----
-    Once I changed to pyfilesystem, I was getting duplicate
-    column names. Ideally, I'd figure out why and not remove
-    them at the end like this...
+    Warns and removes duplicate columns from a DataFrame
     """
     duplicated_cols = df.columns[df.columns.duplicated()]
 
     # Drop duplicate columns if any are found
     if len(duplicated_cols) > 0:
+        warnings.warn(f"Duplicate columns found: {duplicated_cols}")
         df.drop(columns=duplicated_cols, inplace=True)
 
     return df
 
 
 def write_csv(df, fs, filename, index=False, buffer_size=1024 * 1024):
     df = remove_duplicate_columns(df)
@@ -27,30 +25,25 @@
         writer = csv.writer(stream)  # Create a CSV writer using the stream
         writer.writerow(df.columns)
         if index:
             data = df.to_records(index=index).tolist()
         else:
             data = df.to_records().tolist()
 
-        # encoded_data = [[str(x).encode() for x in row] for row in data]
-
         writer.writerows(data)
 
 
-"""    with fs.open(filename, "wb") as f:
-        writer = pd.csv.writer(f)
-        for chunk in pd.read_csv(df, chunksize=buffer_size, iterator=True):
-            writer.writerows(chunk.to_records(index=index))"""
-
-
 def open_location(path):
     return open_fs(path)
 
 
 def open_file(fs, file, encoding=None):
+    """
+    Opens a file within a pyfilesystem
+    """
     # Open the CSV file using the FS URL
     with fs.open(file, "rb") as f:
         # Read the file content into a pandas DataFrame
         if encoding:
             df = pd.read_csv(f, encoding=encoding)
         else:
             df = pd.read_csv(f)
@@ -93,21 +86,18 @@
     nan_col[dfKey] = -1
     df.loc[len(df)] = nan_col
     return df
 
 
 def generate_dim(data, filename, fs):
     write_csv(pd.DataFrame(data), fs, filename, False)
-    # pd.DataFrame(data).to_csv(filename, index=False)
 
 
 def check_encoding(fs, file_path):
     """
     Check encoding of a file
     """
     file = fs.open(file_path, "rb")
-    # result = chardet.detect(file.read())
-    # return result["encoding"]
 
     bytes_data = file.read()  # Read as bytes
     result = chardet.detect(bytes_data)  # Detect encoding on bytes
     return result["encoding"]
```

### Comparing `sufficiency_data_transform-0.1.2/PKG-INFO` & `sufficiency_data_transform-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sufficiency-data-transform
-Version: 0.1.2
+Version: 0.1.3
 Summary: temp repo for liia sufficiency data transform
 License: MIT
 Author: tab1tha
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

