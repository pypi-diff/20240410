# Comparing `tmp/layernext-beta-3.2.0b0.tar.gz` & `tmp/layernext-beta-3.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layernext-beta-3.2.0b0.tar", last modified: Tue Apr  2 03:48:15 2024, max compression
+gzip compressed data, was "layernext-beta-3.3.0b0.tar", last modified: Wed Apr 10 05:57:14 2024, max compression
```

## Comparing `layernext-beta-3.2.0b0.tar` & `layernext-beta-3.3.0b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.388146 layernext-beta-3.2.0b0/
--rw-r--r--   0 chathushka   (501) staff       (20)     1073 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/LICENSE
--rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-04-02 03:48:15.387676 layernext-beta-3.2.0b0/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)      352 2023-10-18 12:39:57.000000 layernext-beta-3.2.0b0/README.md
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.365575 layernext-beta-3.2.0b0/layernext/
--rw-r--r--   0 chathushka   (501) staff       (20)   124538 2024-04-02 03:47:32.000000 layernext-beta-3.2.0b0/layernext/__init__.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.368327 layernext-beta-3.2.0b0/layernext/automatic_analysis/
--rw-r--r--   0 chathushka   (501) staff       (20)     8488 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3902 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7539 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)    19710 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4927 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/support.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.380866 layernext-beta-3.2.0b0/layernext/datalake/
--rw-r--r--   0 chathushka   (501) staff       (20)    23794 2024-04-02 03:46:31.000000 layernext-beta-3.2.0b0/layernext/datalake/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)    16752 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/annotation.py
--rw-r--r--   0 chathushka   (501) staff       (20)      868 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/aws_s3_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)      964 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/azure_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2307 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/constants.py
--rw-r--r--   0 chathushka   (501) staff       (20)    93524 2024-04-02 03:46:31.000000 layernext-beta-3.2.0b0/layernext/datalake/datalakeinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)        0 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/layernext/datalake/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)      470 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/file_trash.py
--rw-r--r--   0 chathushka   (501) staff       (20)    12275 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/file_upload.py
--rw-r--r--   0 chathushka   (501) staff       (20)      879 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/gcs_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1642 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/ground_truth.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1539 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/keys.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7555 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/label.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1283 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     6659 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/metadata.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1136 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/model_run.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1166 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/mongo_json_encoder.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1390 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/query.py
--rw-r--r--   0 chathushka   (501) staff       (20)      261 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2691 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)     8733 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_upload.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.383106 layernext-beta-3.2.0b0/layernext/dataset/
--rw-r--r--   0 chathushka   (501) staff       (20)     3305 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4561 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)     9171 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/datasetinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)    23610 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/sync.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.384449 layernext-beta-3.2.0b0/layernext/studio/
--rw-r--r--   0 chathushka   (501) staff       (20)     3661 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3860 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/project.py
--rw-r--r--   0 chathushka   (501) staff       (20)    13127 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/studiointerface.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.386995 layernext-beta-3.2.0b0/layernext_beta.egg-info/
--rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)     1487 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/SOURCES.txt
--rw-r--r--   0 chathushka   (501) staff       (20)        1 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/dependency_links.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       78 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/requires.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       10 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/top_level.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       38 2024-04-02 03:48:15.388650 layernext-beta-3.2.0b0/setup.cfg
--rw-r--r--   0 chathushka   (501) staff       (20)     1950 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/setup.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.386500 layernext-beta-3.2.0b0/tests/
--rw-r--r--   0 chathushka   (501) staff       (20)     1043 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/tests/test_cli.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.975846 layernext-beta-3.3.0b0/
+-rw-r--r--   0 chathushka   (501) staff       (20)     1073 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/LICENSE
+-rw-r--r--   0 chathushka   (501) staff       (20)      928 2024-04-10 05:57:14.975623 layernext-beta-3.3.0b0/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)      352 2023-10-18 12:39:57.000000 layernext-beta-3.3.0b0/README.md
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.958779 layernext-beta-3.3.0b0/layernext/
+-rw-r--r--   0 chathushka   (501) staff       (20)   124538 2024-04-10 05:56:14.000000 layernext-beta-3.3.0b0/layernext/__init__.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.960695 layernext-beta-3.3.0b0/layernext/automatic_analysis/
+-rw-r--r--   0 chathushka   (501) staff       (20)     8488 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3902 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     7539 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis_interface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    19710 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     4927 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/automatic_analysis/support.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.969828 layernext-beta-3.3.0b0/layernext/datalake/
+-rw-r--r--   0 chathushka   (501) staff       (20)    23794 2024-04-08 06:38:18.000000 layernext-beta-3.3.0b0/layernext/datalake/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    16752 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/annotation.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      868 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/aws_s3_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      964 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/azure_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     2307 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/constants.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    93969 2024-04-10 05:55:09.000000 layernext-beta-3.3.0b0/layernext/datalake/datalakeinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)        0 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/layernext/datalake/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      470 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/file_trash.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    12275 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/file_upload.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      879 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/gcs_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1642 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/ground_truth.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1539 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/keys.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     7555 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/label.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1283 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     6659 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/metadata.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1136 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/model_run.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1166 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/mongo_json_encoder.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1390 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/query.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      261 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     2696 2024-04-03 07:30:54.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_interface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     8733 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/datalake/storage_upload.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.971459 layernext-beta-3.3.0b0/layernext/dataset/
+-rw-r--r--   0 chathushka   (501) staff       (20)     3305 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     4561 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     9171 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/datasetinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    23610 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/dataset/sync.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.973453 layernext-beta-3.3.0b0/layernext/studio/
+-rw-r--r--   0 chathushka   (501) staff       (20)     3661 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3860 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/project.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    13127 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/layernext/studio/studiointerface.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.974950 layernext-beta-3.3.0b0/layernext_beta.egg-info/
+-rw-r--r--   0 chathushka   (501) staff       (20)      928 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)     1487 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)        1 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       78 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/requires.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       10 2024-04-10 05:57:14.000000 layernext-beta-3.3.0b0/layernext_beta.egg-info/top_level.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       38 2024-04-10 05:57:14.975944 layernext-beta-3.3.0b0/setup.cfg
+-rw-r--r--   0 chathushka   (501) staff       (20)     1950 2024-02-28 06:35:15.000000 layernext-beta-3.3.0b0/setup.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-10 05:57:14.975132 layernext-beta-3.3.0b0/tests/
+-rw-r--r--   0 chathushka   (501) staff       (20)     1043 2023-09-11 10:46:59.000000 layernext-beta-3.3.0b0/tests/test_cli.py
```

### Comparing `layernext-beta-3.2.0b0/LICENSE` & `layernext-beta-3.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/PKG-INFO` & `layernext-beta-3.3.0b0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.2.0b0
+Version: 3.3.0b0
 Summary: LayerNext Python SDK
 Author: LayerNext
 Author-email: <support@layernext.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: uuid
-Requires-Dist: python-dotenv
-Requires-Dist: azure-storage-blob
-Requires-Dist: tqdm
-Requires-Dist: PyYAML
-Requires-Dist: Deprecated
-Requires-Dist: pymongo
 
 
 # layernext-python-sdk
 
 LayerNext python API client
 
 Sync (upload/download) with LayerNext stacks via APIs from your code
```

### Comparing `layernext-beta-3.2.0b0/layernext/__init__.py` & `layernext-beta-3.3.0b0/layernext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from deprecated import deprecated
 import uuid
 from layernext.datalake.logger import get_debug_logger
 
 # Create a package-level logger
 logger = get_debug_logger(__name__)
 
-__version__ = "3.2.0b0"
+__version__ = "3.3.0b0"
 
 
 class LayerNextClient:
     """
     Python SDK of LayerNext
     """
```

### Comparing `layernext-beta-3.2.0b0/layernext/automatic_analysis/__init__.py` & `layernext-beta-3.3.0b0/layernext/automatic_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis.py` & `layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis_interface.py` & `layernext-beta-3.3.0b0/layernext/automatic_analysis/automatic_analysis_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py` & `layernext-beta-3.3.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/automatic_analysis/support.py` & `layernext-beta-3.3.0b0/layernext/automatic_analysis/support.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/__init__.py` & `layernext-beta-3.3.0b0/layernext/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/annotation.py` & `layernext-beta-3.3.0b0/layernext/datalake/annotation.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/aws_s3_client.py` & `layernext-beta-3.3.0b0/layernext/datalake/aws_s3_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/azure_client.py` & `layernext-beta-3.3.0b0/layernext/datalake/azure_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/constants.py` & `layernext-beta-3.3.0b0/layernext/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/datalakeinterface.py` & `layernext-beta-3.3.0b0/layernext/datalake/datalakeinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -2111,21 +2111,32 @@
         url = f"{self.dalalake_url}/api/client/execute/sqlQuery"
         try:
             logger.info(
                 f"run_sql_query | sending request to metalake, request_id: {request_id}, payload: {payload}"
             )
             response = requests.post(url=url, json=payload, headers=hed)
             status_code = response.status_code
-            res = response.json()
-            logger.info(f"run_sql_query | request_id: {request_id}, response: {res}")
+            logger.info(
+                f"run_sql_query | request_id: {request_id}, status_code: {status_code}"
+            )
             if status_code == 200:
                 return_object = response.json()
+                logger.info(
+                    f"run_sql_query | request_id: {request_id}, response: {return_object}"
+                )
                 return return_object
             else:
-                raise Exception(f"{res['error']['message']}")
+                # if status_code == 504:
+                #     raise Exception(f"{response.text}")
+                # else:
+                try:
+                    return_object = response.json()
+                    raise Exception(f"{return_object['error']['message']}")
+                except Exception:
+                    raise Exception(f"{response.text}")
         except Exception as e:
             # Capture the traceback
             tb_str = traceback.format_exception(
                 etype=type(e), value=e, tb=e.__traceback__
             )
             traceback_str = "".join(tb_str)
             # Log the detailed error with traceback
```

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/file_upload.py` & `layernext-beta-3.3.0b0/layernext/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/gcs_client.py` & `layernext-beta-3.3.0b0/layernext/datalake/gcs_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/ground_truth.py` & `layernext-beta-3.3.0b0/layernext/datalake/ground_truth.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/keys.py` & `layernext-beta-3.3.0b0/layernext/datalake/keys.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/label.py` & `layernext-beta-3.3.0b0/layernext/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/logger.py` & `layernext-beta-3.3.0b0/layernext/datalake/logger.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/metadata.py` & `layernext-beta-3.3.0b0/layernext/datalake/metadata.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/model_run.py` & `layernext-beta-3.3.0b0/layernext/datalake/model_run.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/mongo_json_encoder.py` & `layernext-beta-3.3.0b0/layernext/datalake/mongo_json_encoder.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/query.py` & `layernext-beta-3.3.0b0/layernext/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/storage_interface.py` & `layernext-beta-3.3.0b0/layernext/datalake/storage_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 
 class StorageInterface:
 
     def __init__(self, storage_type, url_list):
         self.e_tag = ""
         # Create client based on storage type
-        if storage_type == "AWS_S3":
+        if storage_type == "aws_s3":
             from layernext.datalake.aws_s3_client import AWSS3Client
 
             self.storage_client = AWSS3Client()
-        elif storage_type == "GCP":
+        elif storage_type == "gcs":
             from layernext.datalake.gcs_client import GCSClient
 
             self.storage_client = GCSClient()
-        elif storage_type == "AZURE":
+        elif storage_type == "azure_blob":
             from layernext.datalake.azure_client import AzureClient
 
             self.storage_client = AzureClient(url_list)
         else:
             raise Exception("Invalid storage type: " + storage_type)
 
     """'
```

### Comparing `layernext-beta-3.2.0b0/layernext/datalake/storage_upload.py` & `layernext-beta-3.3.0b0/layernext/datalake/storage_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/dataset/__init__.py` & `layernext-beta-3.3.0b0/layernext/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/dataset/dataset.py` & `layernext-beta-3.3.0b0/layernext/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/dataset/datasetinterface.py` & `layernext-beta-3.3.0b0/layernext/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/dataset/sync.py` & `layernext-beta-3.3.0b0/layernext/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/studio/__init__.py` & `layernext-beta-3.3.0b0/layernext/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/studio/project.py` & `layernext-beta-3.3.0b0/layernext/studio/project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext/studio/studiointerface.py` & `layernext-beta-3.3.0b0/layernext/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/layernext_beta.egg-info/PKG-INFO` & `layernext-beta-3.3.0b0/layernext_beta.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.2.0b0
+Version: 3.3.0b0
 Summary: LayerNext Python SDK
 Author: LayerNext
 Author-email: <support@layernext.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: uuid
-Requires-Dist: python-dotenv
-Requires-Dist: azure-storage-blob
-Requires-Dist: tqdm
-Requires-Dist: PyYAML
-Requires-Dist: Deprecated
-Requires-Dist: pymongo
 
 
 # layernext-python-sdk
 
 LayerNext python API client
 
 Sync (upload/download) with LayerNext stacks via APIs from your code
```

### Comparing `layernext-beta-3.2.0b0/layernext_beta.egg-info/SOURCES.txt` & `layernext-beta-3.3.0b0/layernext_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/setup.py` & `layernext-beta-3.3.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.2.0b0/tests/test_cli.py` & `layernext-beta-3.3.0b0/tests/test_cli.py`

 * *Files identical despite different names*

