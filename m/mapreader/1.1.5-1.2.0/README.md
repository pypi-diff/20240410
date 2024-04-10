# Comparing `tmp/mapreader-1.1.5.tar.gz` & `tmp/mapreader-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.1.5.tar", last modified: Thu Apr  4 13:58:12 2024, max compression
+gzip compressed data, was "mapreader-1.2.0.tar", last modified: Wed Apr 10 09:44:51 2024, max compression
```

## Comparing `mapreader-1.1.5.tar` & `mapreader-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.739074 mapreader-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 13:58:06.000000 mapreader-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-04-04 13:58:12.739074 mapreader-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-04 13:58:06.000000 mapreader-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.739074 mapreader-1.1.5/mapreader/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 13:58:12.739074 mapreader-1.1.5/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.731074 mapreader-1.1.5/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.731074 mapreader-1.1.5/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75024 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    98833 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 13:58:12.739074 mapreader-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-04 13:58:06.000000 mapreader-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_geo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-04 13:58:06.000000 mapreader-1.1.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.129624 mapreader-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 09:44:44.000000 mapreader-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-10 09:44:51.129624 mapreader-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-10 09:44:44.000000 mapreader-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.129624 mapreader-1.2.0/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 09:44:51.129624 mapreader-1.2.0/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.121624 mapreader-1.2.0/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26473 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75056 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98833 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 09:44:44.000000 mapreader-1.2.0/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:44:50.000000 mapreader-1.2.0/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:44:51.000000 mapreader-1.2.0/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 09:44:51.129624 mapreader-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 09:44:44.000000 mapreader-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:51.125624 mapreader-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_geo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-10 09:44:44.000000 mapreader-1.2.0/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-10 09:44:44.000000 mapreader-1.2.0/versioneer.py
```

### Comparing `mapreader-1.1.5/LICENSE` & `mapreader-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/PKG-INFO` & `mapreader-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.1.5
+Version: 1.2.0
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,29 +20,29 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<4.0.0,>=3.5.0
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<2.0.0,>=1.3.4
 Requires-Dist: pyproj<4.0.0,>=3.2.0
 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1
 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1
 Requires-Dist: scikit-image>=0.18.3
 Requires-Dist: scikit-learn<2.0.0,>=1.0.1
-Requires-Dist: torch<2.0.0,>=1.10.0
-Requires-Dist: torchvision<0.12.1,>=0.11.1
+Requires-Dist: torch>=1.10.0
+Requires-Dist: torchvision<0.17.3,>=0.11.1
 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1
 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0
 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: tensorboard<3.0.0,>=2.7.0
@@ -52,23 +52,22 @@
 Requires-Dist: simplekml<2.0.0,>=1.3.6
 Requires-Dist: versioneer>=0.28
 Requires-Dist: tqdm<5.0.0
 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0
 Requires-Dist: geopandas<1.0.0
 Requires-Dist: pyogrio>=0.7.2
+Requires-Dist: cartopy>=0.22.0
 Provides-Extra: dev
-Requires-Dist: pytest<8.0.0; extra == "dev"
-Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev"
+Requires-Dist: pytest<9.0.0; extra == "dev"
+Requires-Dist: pytest-cov<6.0.0,>=4.1.0; extra == "dev"
 Requires-Dist: timm<1.0.0; extra == "dev"
 Requires-Dist: transformers<5.0.0; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev"
-Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "dev"
-Provides-Extra: geo
-Requires-Dist: cartopy>=0.20.0; extra == "geo"
+Requires-Dist: black<25.0.0,>=23.7.0; extra == "dev"
+Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "dev"
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
     <h2>A computer vision pipeline for exploring and analyzing images at scale</h2>
     </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.1.5 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.2.0 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -10,35 +10,34 @@
 Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
+Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<2.0.0,>=1.3.4 Requires-Dist:
 pyproj<4.0.0,>=3.2.0 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1 Requires-Dist: scikit-image>=0.18.3
-Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch<2.0.0,>=1.10.0
-Requires-Dist: torchvision<0.12.1,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
+Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch>=1.10.0
+Requires-Dist: torchvision<0.17.3,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0 Requires-Dist: tensorboard<3.0.0,>=2.7.0
 Requires-Dist: parhugin<0.0.4,>=0.0.3 Requires-Dist: geopy==2.1.0 Requires-
 Dist: rasterio<2.0.0,>=1.2.10 Requires-Dist: simplekml<2.0.0,>=1.3.6 Requires-
 Dist: versioneer>=0.28 Requires-Dist: tqdm<5.0.0 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Requires-Dist:
-pyogrio>=0.7.2 Provides-Extra: dev Requires-Dist: pytest<8.0.0; extra == "dev"
-Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist:
-timm<1.0.0; extra == "dev" Requires-Dist: transformers<5.0.0; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist:
-flake8<7.0.0,>=6.0.0; extra == "dev" Provides-Extra: geo Requires-Dist:
-cartopy>=0.20.0; extra == "geo"
+pyogrio>=0.7.2 Requires-Dist: cartopy>=0.22.0 Provides-Extra: dev Requires-
+Dist: pytest<9.0.0; extra == "dev" Requires-Dist: pytest-cov<6.0.0,>=4.1.0;
+extra == "dev" Requires-Dist: timm<1.0.0; extra == "dev" Requires-Dist:
+transformers<5.0.0; extra == "dev" Requires-Dist: black<25.0.0,>=23.7.0; extra
+== "dev" Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "dev"
 
                             ************ MMaappRReeaaddeerr ************
  ********** AA ccoommppuutteerr vviissiioonn ppiippeelliinnee ffoorr eexxpplloorriinngg aanndd aannaallyyzziinngg iimmaaggeess aatt ssccaallee
                                      **********
                  _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _b_a_d_g_e_]_[_D_O_I_]
        _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_L_i_v_i_n_g_-_w_i_t_h_-_m_a_c_h_i_n_e_s_/_M_a_p_R_e_a_d_e_r_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_8_G_Q_3_O_1_G_B_5_]
```

### Comparing `mapreader-1.1.5/README.md` & `mapreader-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/__init__.py` & `mapreader-1.2.0/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/annotate/annotator.py` & `mapreader-1.2.0/mapreader/annotate/annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/annotate/utils.py` & `mapreader-1.2.0/mapreader/annotate/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         try:
             pd.options.mode.chained_assignment = None
             df["pixel_groups"] = pd.qcut(
                 df[tar_param], q=10, precision=2, labels=False
             ).values
             if random_state in ["random"]:
                 df = df.groupby("pixel_groups").sample(
-                    n=10, random_state=random.randint(0, 1e6)
+                    n=10, random_state=random.randint(0, int(1e6))
                 )
             else:
                 df = df.groupby("pixel_groups").sample(n=10, random_state=random_state)
         except Exception:
             print(f"[INFO] len(df) = {len(df)}, .sample method is deactivated.")
             df = df.iloc[:num_samples]
     else:
```

### Comparing `mapreader-1.1.5/mapreader/classify/classifier.py` & `mapreader-1.2.0/mapreader/classify/classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import copy
 import os
 import random
 import socket
 import sys
 import time
+from collections.abc import Hashable, Iterable
 from datetime import datetime
-from typing import Any, Hashable, Iterable
+from typing import Any
 
 import joblib
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 import torch.nn as nn
 import torchvision
@@ -163,15 +164,15 @@
             self.best_loss = torch.tensor(np.inf)
             self.best_epoch = 0
 
             # temp file to save checkpoints during training/validation
             if not os.path.exists("./tmp_checkpoints"):
                 os.makedirs("./tmp_checkpoints")
             self.tmp_save_filename = (
-                f"./tmp_checkpoints/tmp_{random.randint(0, 1e10)}_checkpoint.pkl"
+                f"./tmp_checkpoints/tmp_{random.randint(0, int(1e10))}_checkpoint.pkl"
             )
 
             # add colors for printing/logging
             self._set_up_print_colors()
 
             # add dataloaders and labels_map
             self.dataloaders = dataloaders if dataloaders else {}
```

### Comparing `mapreader-1.1.5/mapreader/classify/custom_models.py` & `mapreader-1.2.0/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/classify/datasets.py` & `mapreader-1.2.0/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/classify/load_annotations.py` & `mapreader-1.2.0/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/data_structures.py` & `mapreader-1.2.0/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/downloader.py` & `mapreader-1.2.0/mapreader/download/downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/downloader_utils.py` & `mapreader-1.2.0/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/sheet_downloader.py` & `mapreader-1.2.0/mapreader/download/sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/tile_loading.py` & `mapreader-1.2.0/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/download/tile_merging.py` & `mapreader-1.2.0/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/load/geo_utils.py` & `mapreader-1.2.0/mapreader/load/geo_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/load/images.py` & `mapreader-1.2.0/mapreader/load/images.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/load/loader.py` & `mapreader-1.2.0/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/process/post_process.py` & `mapreader-1.2.0/mapreader/process/post_process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/process/process.py` & `mapreader-1.2.0/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.2.0/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader/utils/slice_parallel.py` & `mapreader-1.2.0/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader.egg-info/PKG-INFO` & `mapreader-1.2.0/mapreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.1.5
+Version: 1.2.0
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,29 +20,29 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<4.0.0,>=3.5.0
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<2.0.0,>=1.3.4
 Requires-Dist: pyproj<4.0.0,>=3.2.0
 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1
 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1
 Requires-Dist: scikit-image>=0.18.3
 Requires-Dist: scikit-learn<2.0.0,>=1.0.1
-Requires-Dist: torch<2.0.0,>=1.10.0
-Requires-Dist: torchvision<0.12.1,>=0.11.1
+Requires-Dist: torch>=1.10.0
+Requires-Dist: torchvision<0.17.3,>=0.11.1
 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1
 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0
 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: tensorboard<3.0.0,>=2.7.0
@@ -52,23 +52,22 @@
 Requires-Dist: simplekml<2.0.0,>=1.3.6
 Requires-Dist: versioneer>=0.28
 Requires-Dist: tqdm<5.0.0
 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0
 Requires-Dist: geopandas<1.0.0
 Requires-Dist: pyogrio>=0.7.2
+Requires-Dist: cartopy>=0.22.0
 Provides-Extra: dev
-Requires-Dist: pytest<8.0.0; extra == "dev"
-Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev"
+Requires-Dist: pytest<9.0.0; extra == "dev"
+Requires-Dist: pytest-cov<6.0.0,>=4.1.0; extra == "dev"
 Requires-Dist: timm<1.0.0; extra == "dev"
 Requires-Dist: transformers<5.0.0; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev"
-Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "dev"
-Provides-Extra: geo
-Requires-Dist: cartopy>=0.20.0; extra == "geo"
+Requires-Dist: black<25.0.0,>=23.7.0; extra == "dev"
+Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "dev"
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
     <h2>A computer vision pipeline for exploring and analyzing images at scale</h2>
     </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.1.5 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.2.0 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -10,35 +10,34 @@
 Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8, <3.11 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
+Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<2.0.0,>=1.3.4 Requires-Dist:
 pyproj<4.0.0,>=3.2.0 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1 Requires-Dist: scikit-image>=0.18.3
-Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch<2.0.0,>=1.10.0
-Requires-Dist: torchvision<0.12.1,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
+Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch>=1.10.0
+Requires-Dist: torchvision<0.17.3,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0 Requires-Dist: tensorboard<3.0.0,>=2.7.0
 Requires-Dist: parhugin<0.0.4,>=0.0.3 Requires-Dist: geopy==2.1.0 Requires-
 Dist: rasterio<2.0.0,>=1.2.10 Requires-Dist: simplekml<2.0.0,>=1.3.6 Requires-
 Dist: versioneer>=0.28 Requires-Dist: tqdm<5.0.0 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Requires-Dist:
-pyogrio>=0.7.2 Provides-Extra: dev Requires-Dist: pytest<8.0.0; extra == "dev"
-Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist:
-timm<1.0.0; extra == "dev" Requires-Dist: transformers<5.0.0; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist:
-flake8<7.0.0,>=6.0.0; extra == "dev" Provides-Extra: geo Requires-Dist:
-cartopy>=0.20.0; extra == "geo"
+pyogrio>=0.7.2 Requires-Dist: cartopy>=0.22.0 Provides-Extra: dev Requires-
+Dist: pytest<9.0.0; extra == "dev" Requires-Dist: pytest-cov<6.0.0,>=4.1.0;
+extra == "dev" Requires-Dist: timm<1.0.0; extra == "dev" Requires-Dist:
+transformers<5.0.0; extra == "dev" Requires-Dist: black<25.0.0,>=23.7.0; extra
+== "dev" Requires-Dist: flake8<8.0.0,>=6.0.0; extra == "dev"
 
                             ************ MMaappRReeaaddeerr ************
  ********** AA ccoommppuutteerr vviissiioonn ppiippeelliinnee ffoorr eexxpplloorriinngg aanndd aannaallyyzziinngg iimmaaggeess aatt ssccaallee
                                      **********
                  _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _b_a_d_g_e_]_[_D_O_I_]
        _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_L_i_v_i_n_g_-_w_i_t_h_-_m_a_c_h_i_n_e_s_/_M_a_p_R_e_a_d_e_r_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_8_G_Q_3_O_1_G_B_5_]
```

### Comparing `mapreader-1.1.5/mapreader.egg-info/SOURCES.txt` & `mapreader-1.2.0/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/mapreader.egg-info/requires.txt` & `mapreader-1.2.0/mapreader.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 pyproj<4.0.0,>=3.2.0
 azure-storage-blob<13.0.0,>=12.9.0
 aiohttp<4.0.0,>=3.8.1
 Shapely<3.0.0,>=2.0.0
 nest-asyncio<2.0.0,>=1.5.1
 scikit-image>=0.18.3
 scikit-learn<2.0.0,>=1.0.1
-torch<2.0.0,>=1.10.0
-torchvision<0.12.1,>=0.11.1
+torch>=1.10.0
+torchvision<0.17.3,>=0.11.1
 jupyter<2.0.0,>=1.0.0
 ipykernel<7.0.0,>=6.5.1
 ipywidgets<9.0.0,>=8.0.0
 ipyannotate==0.1.0-beta.0
 Cython<0.30.0,>=0.29.24
 PyYAML<7.0,>=6.0
 tensorboard<3.0.0,>=2.7.0
@@ -23,18 +23,16 @@
 simplekml<2.0.0,>=1.3.6
 versioneer>=0.28
 tqdm<5.0.0
 torchinfo<2.0.0
 openpyxl<4.0.0
 geopandas<1.0.0
 pyogrio>=0.7.2
+cartopy>=0.22.0
 
 [dev]
-pytest<8.0.0
-pytest-cov<5.0.0,>=4.1.0
+pytest<9.0.0
+pytest-cov<6.0.0,>=4.1.0
 timm<1.0.0
 transformers<5.0.0
-black<24.0.0,>=23.7.0
-flake8<7.0.0,>=6.0.0
-
-[geo]
-cartopy>=0.20.0
+black<25.0.0,>=23.7.0
+flake8<8.0.0,>=6.0.0
```

### Comparing `mapreader-1.1.5/setup.py` & `mapreader-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,60 +22,57 @@
     long_description_content_type="text/markdown",
     zip_safe=False,
     url="https://github.com/Living-with-machines/MapReader",
     download_url="https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip",
     packages=setuptools.find_packages(),
     include_package_data=True,
     platforms="OS Independent",
-    python_requires=">=3.8, <3.11",
+    python_requires=">=3.9",
     install_requires=[
         "matplotlib>=3.5.0,<4.0.0",
         "numpy>=1.21.5,<2.0.0",
         "pandas>=1.3.4,<2.0.0",
         "pyproj>=3.2.0,<4.0.0",
         "azure-storage-blob>=12.9.0,<13.0.0",
         "aiohttp>=3.8.1,<4.0.0",
         "Shapely>=2.0.0,<3.0.0",
         "nest-asyncio>=1.5.1,<2.0.0",
         "scikit-image>=0.18.3",
         "scikit-learn>=1.0.1,<2.0.0",
-        "torch>=1.10.0,<2.0.0",
-        "torchvision>=0.11.1,<0.12.1",
+        "torch>=1.10.0",
+        "torchvision>=0.11.1,<0.17.3",
         "jupyter>=1.0.0,<2.0.0",
         "ipykernel>=6.5.1,<7.0.0",
         "ipywidgets>=8.0.0,<9.0.0",
         "ipyannotate==0.1.0-beta.0",
         "Cython>=0.29.24,<0.30.0",
-        # "proj>=0.2.0,<0.3.0",
         "PyYAML>=6.0,<7.0",
         "tensorboard>=2.7.0,<3.0.0",
         "parhugin>=0.0.3,<0.0.4",
         "geopy==2.1.0",
         "rasterio>=1.2.10,<2.0.0",
         "simplekml>=1.3.6,<2.0.0",
         "versioneer>=0.28",
         "tqdm<5.0.0",
         "torchinfo<2.0.0",
         "openpyxl<4.0.0",
         "geopandas<1.0.0",
         "pyogrio>=0.7.2",
+        "cartopy>=0.22.0",
     ],
     extras_require={
         "dev": [
-            "pytest<8.0.0",
-            "pytest-cov>=4.1.0,<5.0.0",
+            "pytest<9.0.0",
+            "pytest-cov>=4.1.0,<6.0.0",
             "timm<1.0.0",
             "transformers<5.0.0",
-            "black>=23.7.0,<24.0.0",
-            "flake8>=6.0.0,<7.0.0",
+            "black>=23.7.0,<25.0.0",
+            "flake8>=6.0.0,<8.0.0",
         ],
-        "geo": [
-            "cartopy>=0.20.0"
-        ],
-    },  
+    },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Intended Audience :: End Users/Desktop",
```

### Comparing `mapreader-1.1.5/tests/test_annotator.py` & `mapreader-1.2.0/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/tests/test_geo_pipeline.py` & `mapreader-1.2.0/tests/test_geo_pipeline.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/tests/test_post_processing.py` & `mapreader-1.2.0/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/tests/test_sheet_downloader.py` & `mapreader-1.2.0/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.5/versioneer.py` & `mapreader-1.2.0/versioneer.py`

 * *Files identical despite different names*

