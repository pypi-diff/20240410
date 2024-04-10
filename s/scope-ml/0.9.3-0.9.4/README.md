# Comparing `tmp/scope_ml-0.9.3.tar.gz` & `tmp/scope_ml-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope_ml-0.9.3.tar", max compression
+gzip compressed data, was "scope_ml-0.9.4.tar", max compression
```

## Comparing `scope_ml-0.9.3.tar` & `scope_ml-0.9.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1082 2024-04-09 01:08:30.317262 scope_ml-0.9.3/LICENSE
--rw-r--r--   0        0        0     1427 2024-04-09 01:08:30.317262 scope_ml-0.9.3/README.md
--rw-r--r--   0        0        0    55490 2024-04-09 01:08:30.329262 scope_ml-0.9.3/config.defaults.yaml
--rw-r--r--   0        0        0     3527 2024-04-09 01:08:30.385262 scope_ml-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2755 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/__init__.py
--rw-r--r--   0        0        0      597 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/_instantiate.py
--rwxr-xr-x   0        0        0    13601 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/fritz.py
--rw-r--r--   0        0        0      883 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/models.py
--rw-r--r--   0        0        0    21602 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/nn.py
--rwxr-xr-x   0        0        0   113350 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/scope_class.py
--rw-r--r--   0        0        0    45857 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/utils.py
--rw-r--r--   0        0        0    20264 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/xgb.py
--rw-r--r--   0        0        0     4163 2024-04-09 01:08:30.385262 scope_ml-0.9.3/tools/DNN_AL_mapper.json
--rw-r--r--   0        0        0     4163 2024-04-09 01:08:30.385262 scope_ml-0.9.3/tools/XGB_AL_mapper.json
--rwxr-xr-x   0        0        0     4346 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/analyze_logs.py
--rwxr-xr-x   0        0        0    11647 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/combine_preds.py
--rwxr-xr-x   0        0        0     4338 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/combine_preds_slurm.py
--rw-r--r--   0        0        0     3775 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/alertstats.py
--rw-r--r--   0        0        0     5460 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/external_xmatch.py
--rw-r--r--   0        0        0    12658 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/lcstats.py
--rw-r--r--   0        0        0    19686 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/periodsearch.py
--rw-r--r--   0        0        0        0 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/__init__.py
--rw-r--r--   0        0        0    29593 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aov.f90
--rw-r--r--   0        0        0      545 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aovconst.f90
--rw-r--r--   0        0        0     9369 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aovsub.f90
--rw-r--r--   0        0        0      218 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/build.sh
--rw-r--r--   0        0        0     3983 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/fritz_mapper.json
--rwxr-xr-x   0        0        0    56855 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features.py
--rwxr-xr-x   0        0        0    12036 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features_job_submission.py
--rwxr-xr-x   0        0        0    20587 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features_slurm.py
--rwxr-xr-x   0        0        0    18037 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/get_features.py
--rwxr-xr-x   0        0        0    17448 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/get_quad_ids.py
--rw-r--r--   0        0        0     4334 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/golden_dataset_mapper.json
--rwxr-xr-x   0        0        0    28896 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/inference.py
--rw-r--r--   0        0        0       92 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/local_scope_radec.csv
--rw-r--r--   0        0        0       77 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/local_scope_ztfid.csv
--rwxr-xr-x   0        0        0     2652 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_inference_job_submission.py
--rwxr-xr-x   0        0        0     6811 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_inference_slurm.py
--rwxr-xr-x   0        0        0    12544 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_scope_local.py
--rwxr-xr-x   0        0        0    30136 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_download_classification.py
--rwxr-xr-x   0        0        0     6900 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_download_gcn_sources.py
--rwxr-xr-x   0        0        0     8254 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_manage_annotation.py
--rwxr-xr-x   0        0        0    34114 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_upload_classification.py
--rw-r--r--   0        0        0     3121 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_upload_disagreements.py
--rwxr-xr-x   0        0        0     3873 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/taxonomy.py
--rwxr-xr-x   0        0        0     8018 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/train_algorithm_job_submission.py
--rwxr-xr-x   0        0        0     8971 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/train_algorithm_slurm.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 scope_ml-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-10 16:31:38.197965 scope_ml-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1427 2024-04-10 16:31:38.197965 scope_ml-0.9.4/README.md
+-rw-r--r--   0        0        0    55490 2024-04-10 16:31:38.209965 scope_ml-0.9.4/config.defaults.yaml
+-rw-r--r--   0        0        0     3527 2024-04-10 16:31:38.305965 scope_ml-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2755 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/_instantiate.py
+-rwxr-xr-x   0        0        0    13601 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/fritz.py
+-rw-r--r--   0        0        0      883 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/models.py
+-rw-r--r--   0        0        0    21602 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/nn.py
+-rwxr-xr-x   0        0        0   113350 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/scope_class.py
+-rw-r--r--   0        0        0    45857 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/utils.py
+-rw-r--r--   0        0        0    20264 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/xgb.py
+-rw-r--r--   0        0        0     4163 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/DNN_AL_mapper.json
+-rw-r--r--   0        0        0     4163 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/XGB_AL_mapper.json
+-rwxr-xr-x   0        0        0     4346 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/analyze_logs.py
+-rwxr-xr-x   0        0        0    11958 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/combine_preds.py
+-rwxr-xr-x   0        0        0     4338 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/combine_preds_slurm.py
+-rw-r--r--   0        0        0     3775 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/alertstats.py
+-rw-r--r--   0        0        0     5460 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/external_xmatch.py
+-rw-r--r--   0        0        0    12658 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/lcstats.py
+-rw-r--r--   0        0        0    19686 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/periodsearch.py
+-rw-r--r--   0        0        0        0 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/__init__.py
+-rw-r--r--   0        0        0    29593 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aov.f90
+-rw-r--r--   0        0        0      545 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aovconst.f90
+-rw-r--r--   0        0        0     9369 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aovsub.f90
+-rw-r--r--   0        0        0      218 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/build.sh
+-rw-r--r--   0        0        0     3983 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/fritz_mapper.json
+-rwxr-xr-x   0        0        0    56855 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features.py
+-rwxr-xr-x   0        0        0    12036 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features_job_submission.py
+-rwxr-xr-x   0        0        0    20587 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features_slurm.py
+-rwxr-xr-x   0        0        0    18037 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/get_features.py
+-rwxr-xr-x   0        0        0    17448 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/get_quad_ids.py
+-rw-r--r--   0        0        0     4334 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/golden_dataset_mapper.json
+-rwxr-xr-x   0        0        0    28896 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/inference.py
+-rw-r--r--   0        0        0       92 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/local_scope_radec.csv
+-rw-r--r--   0        0        0       77 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/local_scope_ztfid.csv
+-rwxr-xr-x   0        0        0     2652 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_inference_job_submission.py
+-rwxr-xr-x   0        0        0     6811 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_inference_slurm.py
+-rwxr-xr-x   0        0        0    12544 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_scope_local.py
+-rwxr-xr-x   0        0        0    30136 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_download_classification.py
+-rwxr-xr-x   0        0        0     6900 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_download_gcn_sources.py
+-rwxr-xr-x   0        0        0     8254 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_manage_annotation.py
+-rwxr-xr-x   0        0        0    34114 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_upload_classification.py
+-rw-r--r--   0        0        0     3121 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_upload_disagreements.py
+-rwxr-xr-x   0        0        0     3873 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/taxonomy.py
+-rwxr-xr-x   0        0        0     8018 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/train_algorithm_job_submission.py
+-rwxr-xr-x   0        0        0     9212 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/train_algorithm_slurm.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 scope_ml-0.9.4/PKG-INFO
```

### Comparing `scope_ml-0.9.3/LICENSE` & `scope_ml-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/README.md` & `scope_ml-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/config.defaults.yaml` & `scope_ml-0.9.4/config.defaults.yaml`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/pyproject.toml` & `scope_ml-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 target-version = ['py39', 'py310', 'py311']
 skip-string-normalization = true
 
 [tool.poetry]
 name = "scope-ml"
-version = "0.9.3"
+version = "0.9.4"
 description = "SCoPe: ZTF Source Classification Project"
 readme = "README.md"
 authors = ["Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al."]
 maintainers = ["Brian F. Healy <healyb@umn.edu>"]
 license = "MIT"
 repository = "https://github.com/ZwickyTransientFacility/scope"
 documentation = "https://zwickytransientfacility.github.io/scope-docs/"
```

### Comparing `scope_ml-0.9.3/scope/__init__.py` & `scope_ml-0.9.4/scope/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import os
 import site
 
 # Below code adapted from https://github.com/skyportal/skyportal/blob/main/skyportal/__init__.py
 # 2022-10-18
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 if "dev" in __version__:
     # Append last commit date and hash to dev version information, if available
 
     import subprocess
     import os.path
```

### Comparing `scope_ml-0.9.3/scope/_instantiate.py` & `scope_ml-0.9.4/scope/_instantiate.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/fritz.py` & `scope_ml-0.9.4/scope/fritz.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/models.py` & `scope_ml-0.9.4/scope/models.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/nn.py` & `scope_ml-0.9.4/scope/nn.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/scope_class.py` & `scope_ml-0.9.4/scope/scope_class.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/utils.py` & `scope_ml-0.9.4/scope/utils.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/scope/xgb.py` & `scope_ml-0.9.4/scope/xgb.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/DNN_AL_mapper.json` & `scope_ml-0.9.4/tools/DNN_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/XGB_AL_mapper.json` & `scope_ml-0.9.4/tools/XGB_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/analyze_logs.py` & `scope_ml-0.9.4/tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/combine_preds.py` & `scope_ml-0.9.4/tools/combine_preds.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,38 +101,47 @@
         fields_xgb[i]: field_paths_xgb[i] for i in range(len(fields_xgb))
     }
 
     if save:
         os.makedirs(path_to_preds / combined_preds_dirname, exist_ok=True)
 
     done_fields = [
-        str(x).split("/")[-1].split(".")[0]
+        int(str(x).split("/")[-1].split(".")[0].split("_")[1])
         for x in (path_to_preds / combined_preds_dirname).glob("field_*.parquet")
     ]
     fields_to_list = done_fields.copy()
 
     if fields_to_exclude is not None:
         fields_to_list.extend(fields_to_exclude)
 
-    fields_to_do = list(set(fields_dnn_dict).difference(done_fields))
+    fields_to_do = list(
+        set([int(x.split("_")[1]) for x in fields_dnn_dict.keys()]).difference(
+            fields_to_list
+        )
+    )
     fields_to_list.extend(fields_to_do)
 
+    # Use set to drop duplicate fields before sorting
+    fields_to_list = list(set(fields_to_list))
     fields_to_list.sort()
 
     if save:
         # Write json file containing field list
         with open(path_to_preds / combined_preds_dirname / "fields.json", "w") as f:
             json.dump(fields_to_list, f)
 
     preds_to_save = None
     counter = 0
     print(f"Processing {len(fields_to_do)} fields/files...")
 
+    # Reformat fields in field_N format to match filenames
+    fields_to_do = [f"field_{x}" for x in fields_to_do]
+
     for field in fields_dnn_dict.keys():
-        if field not in done_fields:
+        if field in fields_to_do:
             if field in fields_xgb_dict.keys():
                 try:
                     dnn_preds = read_parquet(
                         fields_dnn_dict[field] / f"{field}.parquet"
                     )
                     xgb_preds = read_parquet(
                         fields_xgb_dict[field] / f"{field}.parquet"
```

### Comparing `scope_ml-0.9.3/tools/combine_preds_slurm.py` & `scope_ml-0.9.4/tools/combine_preds_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/alertstats.py` & `scope_ml-0.9.4/tools/featureGeneration/alertstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/external_xmatch.py` & `scope_ml-0.9.4/tools/featureGeneration/external_xmatch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/lcstats.py` & `scope_ml-0.9.4/tools/featureGeneration/lcstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/periodsearch.py` & `scope_ml-0.9.4/tools/featureGeneration/periodsearch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/pyaov/aov.f90` & `scope_ml-0.9.4/tools/featureGeneration/pyaov/aov.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/pyaov/aovconst.f90` & `scope_ml-0.9.4/tools/featureGeneration/pyaov/aovconst.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/featureGeneration/pyaov/aovsub.f90` & `scope_ml-0.9.4/tools/featureGeneration/pyaov/aovsub.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/fritz_mapper.json` & `scope_ml-0.9.4/tools/fritz_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/generate_features.py` & `scope_ml-0.9.4/tools/generate_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/generate_features_job_submission.py` & `scope_ml-0.9.4/tools/generate_features_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/generate_features_slurm.py` & `scope_ml-0.9.4/tools/generate_features_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/get_features.py` & `scope_ml-0.9.4/tools/get_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/get_quad_ids.py` & `scope_ml-0.9.4/tools/get_quad_ids.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/golden_dataset_mapper.json` & `scope_ml-0.9.4/tools/golden_dataset_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/inference.py` & `scope_ml-0.9.4/tools/inference.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/run_inference_job_submission.py` & `scope_ml-0.9.4/tools/run_inference_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/run_inference_slurm.py` & `scope_ml-0.9.4/tools/run_inference_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/run_scope_local.py` & `scope_ml-0.9.4/tools/run_scope_local.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/scope_download_classification.py` & `scope_ml-0.9.4/tools/scope_download_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/scope_download_gcn_sources.py` & `scope_ml-0.9.4/tools/scope_download_gcn_sources.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/scope_manage_annotation.py` & `scope_ml-0.9.4/tools/scope_manage_annotation.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/scope_upload_classification.py` & `scope_ml-0.9.4/tools/scope_upload_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/scope_upload_disagreements.py` & `scope_ml-0.9.4/tools/scope_upload_disagreements.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/taxonomy.py` & `scope_ml-0.9.4/tools/taxonomy.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/train_algorithm_job_submission.py` & `scope_ml-0.9.4/tools/train_algorithm_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.3/tools/train_algorithm_slurm.py` & `scope_ml-0.9.4/tools/train_algorithm_slurm.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,33 @@
     tags = []
     group = 'experiment'
     algorithm = 'dnn'
 
     for line in lines:
         if 'scope-train' in line:
             line_info = line.removeprefix('scope-train').split()
-            for arg in line_info.copy():
-                if '--tag' in arg:
-                    tag = arg.split('=')[1]
+            line_info_copy = line_info.copy()
+            for i in range(len(line_info_copy)):
+                arg = line_info_copy[i]
+
+                if arg == '--tag':
+                    tag = line_info_copy[i + 1]
                     tags += [tag]
                     line_info.remove(arg)
+                    line_info.remove(tag)
 
-                if '--group' in arg:
-                    group = arg.split('=')[1]
+                if arg == '--group':
+                    group = line_info_copy[i + 1]
                     line_info.remove(arg)
+                    line_info.remove(group)
 
-                if '--algorithm' in arg:
-                    algorithm = arg.split('=')[1]
+                if arg == '--algorithm':
+                    algorithm = line_info_copy[i + 1]
                     line_info.remove(arg)
+                    line_info.remove(algorithm)
 
     return tags, group, algorithm, line_info
 
 
 def get_parser():
 
     parser = argparse.ArgumentParser()
```

### Comparing `scope_ml-0.9.3/PKG-INFO` & `scope_ml-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-ml
-Version: 0.9.3
+Version: 0.9.4
 Summary: SCoPe: ZTF Source Classification Project
 Home-page: https://github.com/ZwickyTransientFacility/scope
 License: MIT
 Author: Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al.
 Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu
 Requires-Python: >=3.9,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scope-ml Version: 0.9.3 Summary: SCoPe: ZTF Source
+Metadata-Version: 2.1 Name: scope-ml Version: 0.9.4 Summary: SCoPe: ZTF Source
 Classification Project Home-page: https://github.com/ZwickyTransientFacility/
 scope License: MIT Author: Brian F. Healy, Michael W. Coughlin, Ashish A.
 Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A.
 Hillenbrand, Jan van Roestel, Paula Szkody et al. Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

