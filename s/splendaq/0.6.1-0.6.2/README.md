# Comparing `tmp/splendaq-0.6.1.tar.gz` & `tmp/splendaq-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendaq-0.6.1.tar", last modified: Thu Nov  9 17:39:01 2023, max compression
+gzip compressed data, was "splendaq-0.6.2.tar", last modified: Wed Apr 10 18:58:52 2024, max compression
```

## Comparing `splendaq-0.6.1.tar` & `splendaq-0.6.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.484175 splendaq-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.472175 splendaq-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.476175 splendaq-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-11-09 17:38:51.000000 splendaq-0.6.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-09 17:38:51.000000 splendaq-0.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-11-09 17:38:51.000000 splendaq-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-09 17:38:51.000000 splendaq-0.6.1/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-09 17:38:51.000000 splendaq-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-09 17:38:51.000000 splendaq-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-09 17:39:01.484175 splendaq-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-09 17:38:51.000000 splendaq-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-09 17:38:51.000000 splendaq-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-09 17:39:01.484175 splendaq-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-09 17:38:51.000000 splendaq-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.472175 splendaq-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.476175 splendaq-0.6.1/src/splendaq/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.480175 splendaq-0.6.1/src/splendaq/control/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/control/_hps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/control/_sr560.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.480175 splendaq-0.6.1/src/splendaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/daq/_log_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    25592 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/daq/_offline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/daq/_oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/daq/_sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.480175 splendaq-0.6.1/src/splendaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7841 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.484175 splendaq-0.6.1/src/splendaq/io/_liconvert/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/_liconvert/COPYING.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   716536 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_linux
--rwxr-xr-x   0 runner    (1001) docker     (127)   629104 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_macos
--rw-r--r--   0 runner    (1001) docker     (127)   689928 2023-11-09 17:38:51.000000 splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_windows.exe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.476175 splendaq-0.6.1/src/splendaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-09 17:39:01.000000 splendaq-0.6.1/src/splendaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.476175 splendaq-0.6.1/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.484175 splendaq-0.6.1/tutorials/daq/
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/daq/dc_oscilloscope.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12596 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/daq/event_building.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/daq/logging_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/daq/running_the_sequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/daq/sequencer_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 17:39:01.484175 splendaq-0.6.1/tutorials/io/
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/io/read_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2023-11-09 17:38:51.000000 splendaq-0.6.1/tutorials/io/write_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-10 18:58:47.000000 splendaq-0.6.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 18:58:47.000000 splendaq-0.6.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 18:58:47.000000 splendaq-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 18:58:47.000000 splendaq-0.6.2/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 18:58:47.000000 splendaq-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 18:58:47.000000 splendaq-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-10 18:58:52.896850 splendaq-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-10 18:58:47.000000 splendaq-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 18:58:47.000000 splendaq-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-10 18:58:52.896850 splendaq-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 18:58:47.000000 splendaq-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/src/splendaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.888850 splendaq-0.6.2/src/splendaq/control/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/_hps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/control/_sr560.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25592 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_offline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/daq/_sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.892850 splendaq-0.6.2/src/splendaq/io/_liconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/COPYING.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   716536 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_linux
+-rwxr-xr-x   0 runner    (1001) docker     (127)   629104 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_macos
+-rw-r--r--   0 runner    (1001) docker     (127)   689928 2024-04-10 18:58:47.000000 splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_windows.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/src/splendaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 18:58:52.000000 splendaq-0.6.2/src/splendaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.884850 splendaq-0.6.2/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/tutorials/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/dc_oscilloscope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/event_building.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/logging_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/running_the_sequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/daq/sequencer_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:58:52.896850 splendaq-0.6.2/tutorials/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/io/read_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-10 18:58:47.000000 splendaq-0.6.2/tutorials/io/write_files.ipynb
```

### Comparing `splendaq-0.6.1/.github/workflows/python-package.yml` & `splendaq-0.6.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/.github/workflows/python-publish.yml` & `splendaq-0.6.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/.gitignore` & `splendaq-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/LICENSE` & `splendaq-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/PKG-INFO` & `splendaq-0.6.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,24 @@
-Metadata-Version: 2.1
-Name: splendaq
-Version: 0.6.1
-Summary: Generalized offline data acquisition with a focus on the Moku
-Home-page: https://github.com/splendor-collab/splendaq
-Author: SPLENDOR Collaboration
-Maintainer: SPLENDOR Collaboration
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: moku>=3.0.0
-Requires-Dist: h5py
-Requires-Dist: pyyaml
-Requires-Dist: pyserial
-
 # `splendaq`
 
 [![Python package](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml/badge.svg)](https://github.com/splendor-collab/splendaq/actions/workflows/python-package.yml) [![PyPI](https://img.shields.io/pypi/v/splendaq)](https://pypi.org/project/splendaq/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub](https://img.shields.io/github/license/splendor-collab/splendaq)](https://github.com/splendor-collab/splendaq/blob/main/LICENSE) [![arXiv](https://img.shields.io/badge/arXiv-2310.01279-<COLOR>.svg)](https://arxiv.org/abs/2310.01279)
 
 
 Package for general data acquisition with a focus on the Moku device by [Liquid Instruments](https://www.liquidinstruments.com/).
 
 If you use this package for your research, please cite our paper as below:
 ```
-@misc{watkins2023splendaq,
-      title={SPLENDAQ: A Detector-Agnostic Data Acquisition System for Small-Scale Physics Experiments}, 
-      author={S. L. Watkins},
-      year={2023},
-      eprint={2310.01279},
-      archivePrefix={arXiv},
-      primaryClass={physics.ins-det}
+@article{Watkins:2023rgt,
+    author = "Watkins, Samuel L.",
+    title = "{SPLENDAQ: A Detector-Agnostic Data Acquisition System for Small-Scale Physics Experiments}",
+    eprint = "2310.01279",
+    archivePrefix = "arXiv",
+    primaryClass = "physics.ins-det",
+    reportNumber = "LA-UR-23-31174",
+    doi = "10.1007/s10909-023-03021-w",
+    journal = "J. Low Temp. Phys.",
+    volume = "214",
+    number = "3-4",
+    pages = "133--142",
+    year = "2024"
 }
 ```
```

### Comparing `splendaq-0.6.1/setup.cfg` & `splendaq-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/_cli.py` & `splendaq-0.6.2/src/splendaq/_cli.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/control/_hps.py` & `splendaq-0.6.2/src/splendaq/control/_hps.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/control/_sr560.py` & `splendaq-0.6.2/src/splendaq/control/_sr560.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/daq/_log_data.py` & `splendaq-0.6.2/src/splendaq/daq/_log_data.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/daq/_offline_trigger.py` & `splendaq-0.6.2/src/splendaq/daq/_offline_trigger.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/daq/_oscilloscope.py` & `splendaq-0.6.2/src/splendaq/daq/_oscilloscope.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/daq/_sequencer.py` & `splendaq-0.6.2/src/splendaq/daq/_sequencer.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/io/_io.py` & `splendaq-0.6.2/src/splendaq/io/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 import os
 import sys
+import copy
 from pathlib import Path
 from datetime import datetime
 import numpy as np
 from scipy.io import loadmat
 import h5py
 
 
@@ -153,23 +154,32 @@
             set when initializing, or if a different file will be read.
         metadata : kwargs
             All of the corresponding metadata for the events in the
             HDF5 file.
 
         """
 
+        current_metadata_size = 0
+
         if filename is not None:
             self.filename = filename
         elif self.filename is None:
             raise ValueError("No filename specified.")
 
         with h5py.File(self.filename, mode='w') as hf:
-            hf.create_dataset('data', data=data, compression='gzip')
+            hf.create_dataset(
+                'data',
+                data=data,
+                compression='gzip',
+                track_order=True,
+            )
             for key in metadata:
-                if sys.getsizeof(metadata[key]) < 64000:
+                size_of_key = sys.getsizeof(copy.deepcopy(metadata[key]))
+                if current_metadata_size + size_of_key < 64000:
+                    current_metadata_size += size_of_key
                     hf.attrs[key] = metadata[key]
                 else:
                     hf.create_dataset(
                         key, data=metadata[key], compression='gzip',
                     )
```

### Comparing `splendaq-0.6.1/src/splendaq/io/_liconvert/COPYING.txt` & `splendaq-0.6.2/src/splendaq/io/_liconvert/COPYING.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_linux` & `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_linux`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_macos` & `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_macos`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq/io/_liconvert/liconvert_windows.exe` & `splendaq-0.6.2/src/splendaq/io/_liconvert/liconvert_windows.exe`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/src/splendaq.egg-info/SOURCES.txt` & `splendaq-0.6.2/src/splendaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/daq/dc_oscilloscope.ipynb` & `splendaq-0.6.2/tutorials/daq/dc_oscilloscope.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/daq/event_building.ipynb` & `splendaq-0.6.2/tutorials/daq/event_building.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/daq/logging_data.ipynb` & `splendaq-0.6.2/tutorials/daq/logging_data.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/daq/running_the_sequencer.ipynb` & `splendaq-0.6.2/tutorials/daq/running_the_sequencer.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/daq/sequencer_settings.yaml` & `splendaq-0.6.2/tutorials/daq/sequencer_settings.yaml`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/io/read_files.ipynb` & `splendaq-0.6.2/tutorials/io/read_files.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.6.1/tutorials/io/write_files.ipynb` & `splendaq-0.6.2/tutorials/io/write_files.ipynb`

 * *Files identical despite different names*

