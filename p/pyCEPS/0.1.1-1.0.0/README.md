# Comparing `tmp/pyCEPS-0.1.1.tar.gz` & `tmp/pyCEPS-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCEPS-0.1.1.tar", last modified: Tue Apr  2 08:03:33 2024, max compression
+gzip compressed data, was "pyCEPS-1.0.0.tar", last modified: Wed Apr 10 11:13:06 2024, max compression
```

## Comparing `pyCEPS-0.1.1.tar` & `pyCEPS-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyCEPS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 08:03:33.000000 pyCEPS-0.1.1/pyCEPS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.885007 pyCEPS-0.1.1/pyceps/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18779 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.885007 pyCEPS-0.1.1/pyceps/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/cartotypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/lesions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/precisiontypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    41578 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/datatypes/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyceps/fileio/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99276 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/cartoio.py
--rw-r--r--   0 runner    (1001) docker     (127)    25097 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/cartoutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/igb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/pathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/precisionio.py
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/precisionutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/fileio/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/pyceps/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/colormaps.json
--rw-r--r--   0 runner    (1001) docker     (127)    30881 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/pyceps/visualize/dashutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 08:03:30.000000 pyCEPS-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:03:33.889007 pyCEPS-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-02 08:03:31.000000 pyCEPS-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyCEPS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.758434 pyCEPS-1.0.0/pyceps/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20595 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.758434 pyCEPS-1.0.0/pyceps/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/cartotypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/lesions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/precisiontypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44950 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21395 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyceps/fileio/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104812 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/cartoio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25123 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/cartoutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/igb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/pathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/precisionio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/precisionutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/xmlio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyceps/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/colormaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-10 11:13:04.000000 pyCEPS-1.0.0/setup.py
```

### Comparing `pyCEPS-0.1.1/LICENSE.txt` & `pyCEPS-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/PKG-INFO` & `pyCEPS-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 0.1.1
+Version: 1.0.0
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
@@ -28,14 +28,16 @@
 Requires-Dist: dash_vtk>=0.0.9
 Requires-Dist: py7zr>=0.20.8
 
 
 # pyCEPS
 
 [![DOI](https://zenodo.org/badge/747193272.svg)](https://zenodo.org/doi/10.5281/zenodo.10606340)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPi Version](https://img.shields.io/pypi/v/pyCEPS.svg)](https://pypi.org/project/pyCEPS/)
 
 pyCEPS provides an interface to import, visualize and translate clinical
 mapping data (EAM data).
 Supported mapping systems are: CARTO<sup>&reg;</sup>3 (Biosense Webster) and
 EnSite Precision<sup>&trade;</sup> (Abbot).
 
 <img src="https://github.com/medunigraz/pyCEPS/blob/main/pyCEPS.png?raw=true" width="300" height="300">
@@ -58,60 +60,60 @@
   url          = {https://doi.org/10.5281/zenodo.10606340}
 }
 
 To cite a specific software version, visit [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10606340)
 
 ## Installation
 
-Python 3.9 or higher is required. Just use [pip](https://pip.pypa.io) to install:
+Python 3.8 or higher is required. Just use [pip](https://pip.pypa.io) to install:
 
 ```shell
 python3 -m pip install pyceps
 ```
 
 This will install all necessary dependencies and add a CLI entry point.
 To test the installation run
 
 ```shell
 pyceps --help
 ```
 
 ## Standard Workflow
 Typically, a user wants to import and translate complete EAM data sets, save
-a reduced version of the data set to disk (PKL file), and visualize the data.
+a reduced version of the data set to disk, and visualize the data.
 ```shell
 pyceps --system "carto" --study-repository "path_to_repository" --convert --visualize --save-study
 pyceps --system "precision" --study-repository "path_to_repository" --convert --visualize --save-study
 ```
 *--system* specifies the EAM system used for data acquisition.<br>
 *--study-repository* points to a (valid) data location, e.g. a ZIP archive
 (preferred), or a folder.<br>
 *--convert* automatically loads the data set in its entirety and exports all
 data to openCARP compatible formats.<br>
 *--visualize* opens a local HTML site and interactively shows the EAM data.<br>
-*--save-study* saves the (reduced) EAM data set to disk as PKL file, which can
-later used (much faster than re-importing the EAM data).
-
-To open and work with a previously generated PKL file use
+*--save-study* saves the (reduced) EAM data set to disk as .pyceps file, which 
+can be used later (much faster than re-importing the EAM data).
+ 
+To open and work with a previously generated .pyceps file use
 ```shell
-pyceps --system "carto" --pkl-file "path_to_pkl" --visualize ...
-pyceps --system "precision" --pkl-file "path_to_pkl" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
 ```
 
 ## Saving a reduced version of EAM data
 Upon import of EAM data, a data representation is built which can be saved to
 disk for later usage.
 This data object does not contain the entirety of data available in the EAM
 data set (e.g. not all ECG and EGM data is read) but can therefore be loaded
 very quickly.
-To save the data representation in PKL format to disk use
+To save the data representation in .pyceps format to disk use
 ```shell
 --save-study
 ```
-The PKL file is automatically saved in the folder above the repository path
+The file is automatically saved in the folder above the repository path
 (if EAM data resides in a folder), or in the same folder if data is imported
 from ZIP archives.
 Optionally, a different location can be given.
 
 ## Visualizing the data
 Once a data set was imported/loaded it can be visualized using a local HTML
 site to evaluate the quality of the data set:
@@ -122,35 +124,33 @@
 
 ![Local HTML sites for data visualization](https://github.com/medunigraz/pyCEPS/blob/main/dash_interface.jpeg?raw=true "Data Visualization")
 
 ## Advanced Import/Export
 To control which data, i.e. mapping procedures, are imported from an EAM data
 set and which data are exported, the commands described below can be chained
 together.
-It is also possible to add data to an existing PKL file at a later point,
+It is also possible to add data to an existing .pyceps file at a later point,
 if the study repository (original data) is still accessible. See usage of
-*--change-root* for details on how to change data location.
+*--change-root* for details on how to change data location if needed.
 
 ### Specifying the EAM system
 ```shell
 --system [carto, precision]
 ```
+This is used only when importing data from an EAM data repository.
 
 ### Specifying the data location
 ```shell
 --study-repository "path_to_repository"
---pkl-file "path_to_pkl"
+--study-file "path_to_file"
 ```
 Using these commands will gather basic information from the data set,
 (i.e. name of the study, performed mapping procedures, etc.) and display this
 information on the command line.
 
-> **To use the following commands, the used EAM system AND the data location
-> MUST be specified!**
-
 ### Specifying what to import
 To import single mapping procedures the name of the mapping procedure can be
 specified. Optional *all* can be used to import all mapping procedures (same as
 using *--convert*). 
 ```shell
 pyceps.py ... --import-map "map_name"
 pyceps.py ... --import-map "all"
@@ -181,19 +181,19 @@
 > mapping procedures.
 
 > Note: Using *--dump-point-ecgs* needs access to EAM data repository to load
 > ECG data!<br>
 > See below how to set a valid path if necessary
 
 ### Changing the location of original EAM data
-When opening EAM data from previously generated PKL files, the original EAM
+When opening EAM data from previously generated .pyceps files, the original EAM
 data set might not be accessible or the path might have changed (e.g. when
 using mounted devices).
-Information if the path stored in the PKL file is still valid is displayed upon
-loading of a PKL file.
+Information if the path stored in the .pyceps file is still valid is displayed 
+upon loading of a .pyceps file.
 To change the path to an EAM data repository use
 ```shell
 --change-root "path_to_repository"
 ```
 This will check if the new path is valid and set it accordingly.
 
 ## For Experts
@@ -201,15 +201,18 @@
 The data contained in exported data sets differs for different mapping systems.
 Exporting data via the CLI accesses only data common to every mapping system.
 To access the entirety of imported data, Python scripts have to be used.
 
 ```python
 from pyceps import CartoStudy
 
-study = CartoStudy("path_to_repository")
+study = CartoStudy("path_to_repository",
+                   pwd='password',
+                   encoding='encoding')
+study.import_study()
 # import all available maps
 study.import_maps(study.mapNames)
 ...
 ```
 
 ## License
```

### Comparing `pyCEPS-0.1.1/README.md` & `pyCEPS-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # pyCEPS
 
 [![DOI](https://zenodo.org/badge/747193272.svg)](https://zenodo.org/doi/10.5281/zenodo.10606340)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPi Version](https://img.shields.io/pypi/v/pyCEPS.svg)](https://pypi.org/project/pyCEPS/)
 
 pyCEPS provides an interface to import, visualize and translate clinical
 mapping data (EAM data).
 Supported mapping systems are: CARTO<sup>&reg;</sup>3 (Biosense Webster) and
 EnSite Precision<sup>&trade;</sup> (Abbot).
 
 <img src="https://github.com/medunigraz/pyCEPS/blob/main/pyCEPS.png?raw=true" width="300" height="300">
@@ -27,60 +29,60 @@
   url          = {https://doi.org/10.5281/zenodo.10606340}
 }
 
 To cite a specific software version, visit [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10606340)
 
 ## Installation
 
-Python 3.9 or higher is required. Just use [pip](https://pip.pypa.io) to install:
+Python 3.8 or higher is required. Just use [pip](https://pip.pypa.io) to install:
 
 ```shell
 python3 -m pip install pyceps
 ```
 
 This will install all necessary dependencies and add a CLI entry point.
 To test the installation run
 
 ```shell
 pyceps --help
 ```
 
 ## Standard Workflow
 Typically, a user wants to import and translate complete EAM data sets, save
-a reduced version of the data set to disk (PKL file), and visualize the data.
+a reduced version of the data set to disk, and visualize the data.
 ```shell
 pyceps --system "carto" --study-repository "path_to_repository" --convert --visualize --save-study
 pyceps --system "precision" --study-repository "path_to_repository" --convert --visualize --save-study
 ```
 *--system* specifies the EAM system used for data acquisition.<br>
 *--study-repository* points to a (valid) data location, e.g. a ZIP archive
 (preferred), or a folder.<br>
 *--convert* automatically loads the data set in its entirety and exports all
 data to openCARP compatible formats.<br>
 *--visualize* opens a local HTML site and interactively shows the EAM data.<br>
-*--save-study* saves the (reduced) EAM data set to disk as PKL file, which can
-later used (much faster than re-importing the EAM data).
-
-To open and work with a previously generated PKL file use
+*--save-study* saves the (reduced) EAM data set to disk as .pyceps file, which 
+can be used later (much faster than re-importing the EAM data).
+ 
+To open and work with a previously generated .pyceps file use
 ```shell
-pyceps --system "carto" --pkl-file "path_to_pkl" --visualize ...
-pyceps --system "precision" --pkl-file "path_to_pkl" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
 ```
 
 ## Saving a reduced version of EAM data
 Upon import of EAM data, a data representation is built which can be saved to
 disk for later usage.
 This data object does not contain the entirety of data available in the EAM
 data set (e.g. not all ECG and EGM data is read) but can therefore be loaded
 very quickly.
-To save the data representation in PKL format to disk use
+To save the data representation in .pyceps format to disk use
 ```shell
 --save-study
 ```
-The PKL file is automatically saved in the folder above the repository path
+The file is automatically saved in the folder above the repository path
 (if EAM data resides in a folder), or in the same folder if data is imported
 from ZIP archives.
 Optionally, a different location can be given.
 
 ## Visualizing the data
 Once a data set was imported/loaded it can be visualized using a local HTML
 site to evaluate the quality of the data set:
@@ -91,35 +93,33 @@
 
 ![Local HTML sites for data visualization](https://github.com/medunigraz/pyCEPS/blob/main/dash_interface.jpeg?raw=true "Data Visualization")
 
 ## Advanced Import/Export
 To control which data, i.e. mapping procedures, are imported from an EAM data
 set and which data are exported, the commands described below can be chained
 together.
-It is also possible to add data to an existing PKL file at a later point,
+It is also possible to add data to an existing .pyceps file at a later point,
 if the study repository (original data) is still accessible. See usage of
-*--change-root* for details on how to change data location.
+*--change-root* for details on how to change data location if needed.
 
 ### Specifying the EAM system
 ```shell
 --system [carto, precision]
 ```
+This is used only when importing data from an EAM data repository.
 
 ### Specifying the data location
 ```shell
 --study-repository "path_to_repository"
---pkl-file "path_to_pkl"
+--study-file "path_to_file"
 ```
 Using these commands will gather basic information from the data set,
 (i.e. name of the study, performed mapping procedures, etc.) and display this
 information on the command line.
 
-> **To use the following commands, the used EAM system AND the data location
-> MUST be specified!**
-
 ### Specifying what to import
 To import single mapping procedures the name of the mapping procedure can be
 specified. Optional *all* can be used to import all mapping procedures (same as
 using *--convert*). 
 ```shell
 pyceps.py ... --import-map "map_name"
 pyceps.py ... --import-map "all"
@@ -150,19 +150,19 @@
 > mapping procedures.
 
 > Note: Using *--dump-point-ecgs* needs access to EAM data repository to load
 > ECG data!<br>
 > See below how to set a valid path if necessary
 
 ### Changing the location of original EAM data
-When opening EAM data from previously generated PKL files, the original EAM
+When opening EAM data from previously generated .pyceps files, the original EAM
 data set might not be accessible or the path might have changed (e.g. when
 using mounted devices).
-Information if the path stored in the PKL file is still valid is displayed upon
-loading of a PKL file.
+Information if the path stored in the .pyceps file is still valid is displayed 
+upon loading of a .pyceps file.
 To change the path to an EAM data repository use
 ```shell
 --change-root "path_to_repository"
 ```
 This will check if the new path is valid and set it accordingly.
 
 ## For Experts
@@ -170,15 +170,18 @@
 The data contained in exported data sets differs for different mapping systems.
 Exporting data via the CLI accesses only data common to every mapping system.
 To access the entirety of imported data, Python scripts have to be used.
 
 ```python
 from pyceps import CartoStudy
 
-study = CartoStudy("path_to_repository")
+study = CartoStudy("path_to_repository",
+                   pwd='password',
+                   encoding='encoding')
+study.import_study()
 # import all available maps
 study.import_maps(study.mapNames)
 ...
 ```
 
 ## License
```

### Comparing `pyCEPS-0.1.1/pyCEPS.egg-info/PKG-INFO` & `pyCEPS-1.0.0/pyCEPS.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 0.1.1
+Version: 1.0.0
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
@@ -28,14 +28,16 @@
 Requires-Dist: dash_vtk>=0.0.9
 Requires-Dist: py7zr>=0.20.8
 
 
 # pyCEPS
 
 [![DOI](https://zenodo.org/badge/747193272.svg)](https://zenodo.org/doi/10.5281/zenodo.10606340)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPi Version](https://img.shields.io/pypi/v/pyCEPS.svg)](https://pypi.org/project/pyCEPS/)
 
 pyCEPS provides an interface to import, visualize and translate clinical
 mapping data (EAM data).
 Supported mapping systems are: CARTO<sup>&reg;</sup>3 (Biosense Webster) and
 EnSite Precision<sup>&trade;</sup> (Abbot).
 
 <img src="https://github.com/medunigraz/pyCEPS/blob/main/pyCEPS.png?raw=true" width="300" height="300">
@@ -58,60 +60,60 @@
   url          = {https://doi.org/10.5281/zenodo.10606340}
 }
 
 To cite a specific software version, visit [Zenodo](https://zenodo.org/doi/10.5281/zenodo.10606340)
 
 ## Installation
 
-Python 3.9 or higher is required. Just use [pip](https://pip.pypa.io) to install:
+Python 3.8 or higher is required. Just use [pip](https://pip.pypa.io) to install:
 
 ```shell
 python3 -m pip install pyceps
 ```
 
 This will install all necessary dependencies and add a CLI entry point.
 To test the installation run
 
 ```shell
 pyceps --help
 ```
 
 ## Standard Workflow
 Typically, a user wants to import and translate complete EAM data sets, save
-a reduced version of the data set to disk (PKL file), and visualize the data.
+a reduced version of the data set to disk, and visualize the data.
 ```shell
 pyceps --system "carto" --study-repository "path_to_repository" --convert --visualize --save-study
 pyceps --system "precision" --study-repository "path_to_repository" --convert --visualize --save-study
 ```
 *--system* specifies the EAM system used for data acquisition.<br>
 *--study-repository* points to a (valid) data location, e.g. a ZIP archive
 (preferred), or a folder.<br>
 *--convert* automatically loads the data set in its entirety and exports all
 data to openCARP compatible formats.<br>
 *--visualize* opens a local HTML site and interactively shows the EAM data.<br>
-*--save-study* saves the (reduced) EAM data set to disk as PKL file, which can
-later used (much faster than re-importing the EAM data).
-
-To open and work with a previously generated PKL file use
+*--save-study* saves the (reduced) EAM data set to disk as .pyceps file, which 
+can be used later (much faster than re-importing the EAM data).
+ 
+To open and work with a previously generated .pyceps file use
 ```shell
-pyceps --system "carto" --pkl-file "path_to_pkl" --visualize ...
-pyceps --system "precision" --pkl-file "path_to_pkl" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
+pyceps --study-file "path_to_file" --visualize ...
 ```
 
 ## Saving a reduced version of EAM data
 Upon import of EAM data, a data representation is built which can be saved to
 disk for later usage.
 This data object does not contain the entirety of data available in the EAM
 data set (e.g. not all ECG and EGM data is read) but can therefore be loaded
 very quickly.
-To save the data representation in PKL format to disk use
+To save the data representation in .pyceps format to disk use
 ```shell
 --save-study
 ```
-The PKL file is automatically saved in the folder above the repository path
+The file is automatically saved in the folder above the repository path
 (if EAM data resides in a folder), or in the same folder if data is imported
 from ZIP archives.
 Optionally, a different location can be given.
 
 ## Visualizing the data
 Once a data set was imported/loaded it can be visualized using a local HTML
 site to evaluate the quality of the data set:
@@ -122,35 +124,33 @@
 
 ![Local HTML sites for data visualization](https://github.com/medunigraz/pyCEPS/blob/main/dash_interface.jpeg?raw=true "Data Visualization")
 
 ## Advanced Import/Export
 To control which data, i.e. mapping procedures, are imported from an EAM data
 set and which data are exported, the commands described below can be chained
 together.
-It is also possible to add data to an existing PKL file at a later point,
+It is also possible to add data to an existing .pyceps file at a later point,
 if the study repository (original data) is still accessible. See usage of
-*--change-root* for details on how to change data location.
+*--change-root* for details on how to change data location if needed.
 
 ### Specifying the EAM system
 ```shell
 --system [carto, precision]
 ```
+This is used only when importing data from an EAM data repository.
 
 ### Specifying the data location
 ```shell
 --study-repository "path_to_repository"
---pkl-file "path_to_pkl"
+--study-file "path_to_file"
 ```
 Using these commands will gather basic information from the data set,
 (i.e. name of the study, performed mapping procedures, etc.) and display this
 information on the command line.
 
-> **To use the following commands, the used EAM system AND the data location
-> MUST be specified!**
-
 ### Specifying what to import
 To import single mapping procedures the name of the mapping procedure can be
 specified. Optional *all* can be used to import all mapping procedures (same as
 using *--convert*). 
 ```shell
 pyceps.py ... --import-map "map_name"
 pyceps.py ... --import-map "all"
@@ -181,19 +181,19 @@
 > mapping procedures.
 
 > Note: Using *--dump-point-ecgs* needs access to EAM data repository to load
 > ECG data!<br>
 > See below how to set a valid path if necessary
 
 ### Changing the location of original EAM data
-When opening EAM data from previously generated PKL files, the original EAM
+When opening EAM data from previously generated .pyceps files, the original EAM
 data set might not be accessible or the path might have changed (e.g. when
 using mounted devices).
-Information if the path stored in the PKL file is still valid is displayed upon
-loading of a PKL file.
+Information if the path stored in the .pyceps file is still valid is displayed 
+upon loading of a .pyceps file.
 To change the path to an EAM data repository use
 ```shell
 --change-root "path_to_repository"
 ```
 This will check if the new path is valid and set it accordingly.
 
 ## For Experts
@@ -201,15 +201,18 @@
 The data contained in exported data sets differs for different mapping systems.
 Exporting data via the CLI accesses only data common to every mapping system.
 To access the entirety of imported data, Python scripts have to be used.
 
 ```python
 from pyceps import CartoStudy
 
-study = CartoStudy("path_to_repository")
+study = CartoStudy("path_to_repository",
+                   pwd='password',
+                   encoding='encoding')
+study.import_study()
 # import all available maps
 study.import_maps(study.mapNames)
 ...
 ```
 
 ## License
```

### Comparing `pyCEPS-0.1.1/pyCEPS.egg-info/SOURCES.txt` & `pyCEPS-1.0.0/pyCEPS.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 pyceps/fileio/cartoio.py
 pyceps/fileio/cartoutils.py
 pyceps/fileio/igb.py
 pyceps/fileio/pathtools.py
 pyceps/fileio/precisionio.py
 pyceps/fileio/precisionutils.py
 pyceps/fileio/writer.py
+pyceps/fileio/xmlio.py
 pyceps/visualize/__init__.py
 pyceps/visualize/colormaps.json
 pyceps/visualize/dashapp.py
 pyceps/visualize/dashelements.py
 pyceps/visualize/dashlayout.py
 pyceps/visualize/dashutils.py
```

### Comparing `pyCEPS-0.1.1/pyceps/__init__.py` & `pyCEPS-1.0.0/pyceps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/cli.py` & `pyCEPS-1.0.0/pyceps/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Command line interface for pyEPmap
 """
-
+import argparse
 import os
 import traceback
 import shutil
 import sys
 from argparse import ArgumentParser, Action
 import logging
 import tempfile
 from typing import Tuple
+import xml.etree.ElementTree as ET
 
 from pyceps.fileio.cartoio import CartoStudy
 from pyceps.fileio.precisionio import PrecisionStudy
 
 
 logger = logging.getLogger('pyceps')
 
@@ -74,71 +75,63 @@
 
 
 def get_args():
     """Command line argument parser."""
 
     parser = ArgumentParser(
         prog='pyceps',
+        # add_help=False,
         # formatter_class=RawTextHelpFormatter,
     )
 
-    # configure clinical mapping system from which to import
-    system = parser.add_argument_group('Clinical Mapping System')
-    system.add_argument('--system',
-                        required=True,
-                        type=str.upper,
-                        choices=['CARTO', 'PRECISION'],
-                        help='Specify the clinical mapping system that '
-                             'recorded the study.'
-                        )
-
     # specify location of data
     # Note: subsequent arguments are mutually exclusive. The user must enter
     #       either one!
     group = parser.add_argument_group('Data location')
     load = group.add_mutually_exclusive_group(required=True)
     load.add_argument(
         '--study-repository',
         type=str,
         default=None,
         help='Import study from EAM repository.\n'
-             'Specify path to folder or to ZIP file containing study data.'
+             'Specify path to folder or to ZIP file containing study data.\n'
+             'IMPORTANT: use --system to specify EAM system!'
     )
     load.add_argument(
-        '--pkl-file',
+        '--study-file',
         type=str,
         default=None,
-        help='Load study from previously created .pkl file.\n'
-             'If study root saved in PKL file does not point to a valid '
+        help='Load study from previously created pyCEPS file.\n'
+             'If study root saved in pyCEPS file does not point to a valid '
              'location, it can be set with --change-root'
     )
 
     bio = parser.add_argument_group('Export')
     bio.add_argument(
         '--convert',
         type=str,
         nargs='?',
         default=None,
         const='ALL',
         help='Convenience function to export complete EAM data set.\n'
              'When importing from EAM repository all available maps are '
-             'loaded. When importing from PKL file all maps currently in PKL '
-             'are exported or --import-map might be used to import additional '
-             'map(s) before export.\n'
+             'loaded. When importing from pyCEPS file all maps currently in '
+             'the file are exported or --import-map might be used to import '
+             'additional map(s) before export.\n'
              'Alternatively a specific map name can be given.\n'
              'Calls all functions under Advanced Exports with default values.'
     )
     bio.add_argument(
         '--save-study',
         type=str,
         nargs='?',
         const='DEFAULT',
-        help='Save study as PKL file.\n'
+        help='Save study as pyCEPS file.\n'
              'Default location is folder above study root, default name is '
-             'study name e.g. <study_root>/../<study_name>.pkl\n'
+             'study name e.g. <study_root>/../<study_name>.pyceps\n'
              'Custom location and file name can be given alternatively.'
     )
 
     vis = parser.add_argument_group('Visualization')
     vis.add_argument(
         '--visualize',
         action='store_true',
@@ -166,63 +159,65 @@
         action='store_true',
         help='Save anatomical shell for current "--map" in openCARP and VTK '
              'format.\n'
              'For VTK files, all available surface parameter maps and '
              'surface labels are included.\n'
              'Note: surface maps can also be exported as .dat with '
              '"--dump-surface-map".\n'
-             'Default: <study_root>/../<map>.[pts,elem,vtk]'
+             'Default: <study_root>/../<map>.surf.[pts,elem,vtk]'
     )
     aio.add_argument(
         '--dump-point-data',
         action='store_true',
         help='Export data for recording points for current "--map" in '
              'openCARP format.\n'
              'For each mapping point following data are exported: unipolar '
              'voltages (UNI), bipolar voltages (BIP) and local activation '
-             'time (LAT), impedance (IMP, if available), and contact force ('
-             'FRC, if available).'
-             'Default: <study_root>/../<map>.ptdata.UNI.pc.dat'
+             'time (LAT), point identifier (NAME), time stamps for '
+             'annotations (LAT, REF), window of interest (WOI_START, '
+             'WOI_END), impedance (IMP, if available), and contact force '
+             '(FRC, if available).\n'
+             'Default: <study_root>/../<map>.ptdata.<parameter>.pc.dat'
     )
     aio.add_argument(
         '--dump-point-ecgs',
         type=str,
         action=OptionalListParser,
         nargs='*',
         choices=['I', 'II', 'III',
                  'aVR', 'aVL', 'aVF',
                  'V1', 'V2', 'V3', 'V4', 'V5', 'V6'],
-        help='Export ecg traces for all valid points associated '
+        help='Export ECG traces for all valid points associated '
              'with current "--map" to IGB.\n'
              'Dimension: Nx2500 (valid recorded points x ms)\n'
              'Note: Requires valid study root!\n'
              'If no traces are specified, all surface ECGs are '
              'exported by default.\n'
-             'Default: <study_root>/../<map>.ecg.V1.pc.igb'
+             'Default: <study_root>/../<map>.ecg.<lead>.pc.igb'
     )
     aio.add_argument(
         '--dump-point-egms',
         action='store_true',
-        help='Export point EGMs for all valid points associated '
-             'with current "--map".\n'
+        help='Export point EGM traces for unipolar, bipolar and reference '
+             'channels for all valid points associated with current "--map".\n'
              'Dimension: Nx2500 (valid recorded nodes x ms)\n'
-             'Default: e.g. <study_root>/../<map>.egm.BIP.is.igb'
+             'Default: e.g. <study_root>/../<map>.egm.<lead>.pc.igb'
     )
     aio.add_argument(
         '--dump-map-ecgs',
         action='store_true',
         help='Export representative 12-lead body surface ECGs associated '
              'with current "--map" to JSON.\n'
              'Default: <study_root>/../<map>.bsecg.<method>.json'
     )
     aio.add_argument(
         '--dump-surface-maps',
         action='store_true',
         help='Export surface maps associated with current "--map" to DAT.\n'
-             'Default: <study_root>/../<map>.map.BIP.dat'
+             'Default: <study_root>/../<map>.map.<parameter>.dat'
     )
     aio.add_argument(
         '--dump-lesions',
         action='store_true',
         help='Export lesion data associated with current "--map".\n'
              'Default: <study_root>/../<map>.lesions.<RFI_name>.dat'
     )
@@ -231,21 +226,21 @@
     misc.add_argument(
         '--change-root',
         type=valid_path,
         default=None,
         help='Change location of EAM data repository.\n'
              'Parent directory of "--study-xml" for Carto3 or folder for '
              'Precision. Can be absolute path to folder or ZIP file.\n'
-             'Used only when data is loaded from PKL file.'
+             'Used only when data is loaded from pyCEPS file.'
     )
     misc.add_argument(
         '--egm-from-pos',
         action='store_true',
-        help='Retrieve EGM channel names from recording positions.\n'
-             'This will add coordinates for the second unipolar EGM channel.\n'
+        help='Retrieve EGM channel names from recording positions during '
+             'import.\n'
              'Note: Requires valid study root!'
     )
     misc.add_argument(
         '--logger-level',
         type=str,
         default='INFO',
         choices=['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET'],
@@ -253,16 +248,37 @@
     )
     misc.add_argument(
         '--encoding',
         type=str,
         default='cp1252',
         help='Set encoding for file imports. Default: "cp1252".'
     )
+    misc.add_argument('--password',
+                      type=str,
+                      default='',
+                      help='Password for protected archives.'
+                      )
+
+    main_args, _ = parser.parse_known_args()
+
+    # configure clinical mapping system from which to import
+    conditional_parser = argparse.ArgumentParser(parents=[parser],
+                                                 add_help=False
+                                                 )
+    if main_args.study_repository:
+        system = conditional_parser.add_argument_group('Clinical Mapping System')
+        system.add_argument('--system',
+                            required=main_args.study_repository,
+                            type=str.upper,
+                            choices=['CARTO', 'PRECISION'],
+                            help='Specify the clinical mapping system that '
+                                 'recorded the study.'
+                            )
 
-    return parser.parse_args()
+    return conditional_parser.parse_args()
 
 
 def configure_logger(log_level: str) -> Tuple[int, str]:
     """
     Set logging console and file formats.
 
     Messages are written to a temporary file and can be saved to disk later
@@ -300,41 +316,61 @@
 def load_study(args):
     """Import study data from repository or load existing study object."""
 
     if args.study_repository:
         logger.info('importing {} study'.format(args.system))
         if args.system == 'CARTO':
             study = CartoStudy(args.study_repository,
+                               pwd=args.password,
                                encoding=args.encoding)
+            study.import_study()
         elif args.system == 'PRECISION':
             study = PrecisionStudy(args.study_repository,
+                                   pwd=args.password,
                                    encoding=args.encoding)
         else:
             raise KeyError('unknown EAM system specified!')
 
     else:
-        study_pkg = os.path.abspath(args.pkl_file)
-        logger.info('loading {} study PKL'.format(args.system))
+        study_file = os.path.abspath(args.study_file)
+        logger.info('loading study from file {}'.format(study_file))
+
         # read in study from a pkl file
         # Note: both inputs are mutually exclusive
-        if not study_pkg.lower().endswith(('.pkl', '.pkl.gz')):
+        if not study_file.lower().endswith('.pyceps'):
             # supposedly reading the carto folder directly
-            study_pkg += '.pkl'
+            study_file += '.pyceps'
 
-        if not os.path.isfile(study_pkg):
-            raise FileNotFoundError('could not find {}'.format(study_pkg))
+        if not os.path.isfile(study_file):
+            raise FileNotFoundError('could not find {}'.format(study_file))
 
         # update argument in case of later usage
-        args.study_pkg = study_pkg
+        args.study_file = study_file
 
         # now we can load the object
-        if args.system == 'CARTO':
-            study = CartoStudy.load(study_pkg, root=args.change_root)
-        elif args.system == 'PRECISION':
-            study = PrecisionStudy.load(study_pkg, root=args.change_root)
+        try:
+            with open(study_file) as fid:
+                xml_root = ET.parse(fid).getroot()
+        except ET.ParseError:
+            logger.warning('unknown file format, aborting!')
+            return None, args
+
+        # get EAM system
+        system = xml_root.get('system')
+        repo = xml_root.find('Repository')
+
+        if system.lower() == 'carto3':
+            study = CartoStudy(study_repo=repo.get('base'),
+                               pwd=args.password,
+                               encoding=repo.get('encoding'))
+            study.load(study_file, repo_path=args.change_root)
+
+        elif args.system == 'precision':
+            study = PrecisionStudy.load(study_file, root=args.change_root)
+
         else:
             raise KeyError('unknown EAM system specified!')
         # TODO: notification if root has changed (needed to process unsaved changes)
 
         # verify study root
         if not study.is_root_valid():
             # if study root was set to .pkl folder no valid root was found
@@ -416,15 +452,15 @@
     # remove invalid from list
     import_maps = [e for e in import_maps if e not in invalid_maps]
 
     # now we can import maps from EAM repo
     if import_maps:
         logger.info('need to import map(s): {}'.format(import_maps))
 
-        if args.pkl_file and not study.is_root_valid():
+        if args.study_file and not study.is_root_valid():
             logger.warning('a valid study root is necessary to import maps!')
         else:
             study.import_maps(import_maps,
                               egm_names_from_pos=args.egm_from_pos)
             # import lesion data for all loaded maps
             for map_name in study.maps.keys():
                 study.maps[map_name].import_lesions(directory=None)
@@ -473,33 +509,39 @@
     # check if additional meshes are part of the study
     if study.meshes and args.dump_mesh:
         logger.info('found additional meshes in study, exporting...')
         study.export_additional_meshes()
 
     # save study
     if not args.save_study and data_changed:
+        logger.debug('unsaved changes found!')
         user_input = input('There are unsaved changes, save them now? [Y/N] ')
         # input validation
         if user_input.lower() in ('y', 'yes'):
+            logger.debug('user selected to save changes')
             args.save_study = 'DEFAULT'
+        elif user_input.lower() in ('n', 'no'):
+            logger.debug('user selected to continue without saving changes')
         else:
             logger.warning('Unknown user input {}'.format(user_input))
 
-    pkl_loc = ''
+    pyceps_loc = ''
     if args.save_study:
-        pkl_loc = study.save(None if args.save_study == 'DEFAULT' else
-                             args.save_study)
+        pyceps_loc = study.save(None if args.save_study == 'DEFAULT' else
+                                args.save_study)
 
     # redirect log file
-    log_file = pkl_loc.replace('.pkl', '_import.log') if pkl_loc else (
-        os.path.join(
+    if pyceps_loc:
+        base_file, _ = os.path.splitext(pyceps_loc)
+        log_file = base_file + '_import.log'
+    else:
+        log_file = os.path.join(
             study.build_export_basename(''),
             study.name + '_import.log'
         )
-    )
 
     return study, log_file
 
 
 def run():
     # get CL arguments from parser
     cl_args = get_args()
```

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/__init__.py` & `pyCEPS-1.0.0/pyceps/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/cartotypes.py` & `pyCEPS-1.0.0/pyceps/datatypes/cartotypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """A class representing ablation tags from Carto3 Visitag module."""
 
     def __init__(self,
                  site_index,
                  session_index=None,
                  channel_id=None,
                  tag_index_status=None,
-                 coordinates=np.full(3, np.nan, dtype=float),
+                 coordinates=np.full(3, np.nan, dtype=np.float32),
                  avg_force=np.nan,
                  fti=np.nan,
                  max_power=np.nan,
                  max_temp=np.nan,
                  duration=np.nan,
                  base_impedance=np.nan,
                  impedance_drop=np.nan,
```

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/lesions.py` & `pyCEPS-1.0.0/pyceps/datatypes/lesions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/precisiontypes.py` & `pyCEPS-1.0.0/pyceps/datatypes/precisiontypes.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/signals.py` & `pyCEPS-1.0.0/pyceps/datatypes/signals.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/study.py` & `pyCEPS-1.0.0/pyceps/datatypes/study.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-
 # pyCEPS allows to import, visualize and translate clinical EAM data.
 #     Copyright (C) 2023  Robert Arnold
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
@@ -17,27 +16,35 @@
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import datetime
 import logging
 import os
 from typing import Iterable
 import numpy as np
-import zipfile
-import gzip
-import pickle
+import xml.etree.ElementTree as ET
 import webbrowser
-
-import py7zr
+from importlib.metadata import version, PackageNotFoundError
+try:
+    PYCEPS_VERSION = version('pyceps')
+except PackageNotFoundError:
+    PYCEPS_VERSION = '0.0.0dev'
 
 from pyceps.fileio.pathtools import Repository
 from pyceps.datatypes.surface import SurfaceSignalMap
 from pyceps.fileio import FileWriter
+from pyceps.fileio.xmlio import (xml_add_binary_numpy,
+                                 xml_add_binary_trace,
+                                 xml_add_binary_bsecg,
+                                 xml_add_binary_surface,
+                                 xml_add_binary_lesion
+                                 )
 from pyceps.interpolation import (inverse_distance_weighting,
                                   remove_redundant_points
                                   )
+from pyceps.datatypes.signals import Trace
 from pyceps.visualize import get_dash_app
 
 
 log = logging.getLogger(__name__)
 
 
 class EPStudy:
@@ -137,15 +144,15 @@
 
         self.name = ''
         self.mapNames = []
         self.mapPoints = []
         self.maps = {}
 
         # additional meshes, i.e. from CT data
-        self.meshes = []
+        self.meshes = None
 
     def import_study(self):
         raise NotImplementedError
 
     def import_maps(self, map_names=None, *args, **kwargs):
         """
         Pre-import checks. If a map is already part of the study user
@@ -212,17 +219,17 @@
 
     def is_root_valid(self, root_dir=None):
         raise NotImplementedError
 
     def set_repository(self, root_dir):
         raise NotImplementedError
 
-    @classmethod
-    def load(cls, filename, root=None):
-        raise NotImplemented
+    def load(self, file: str,  repo_path: str = ''):
+        """Load study object from .pyceps archive."""
+        raise NotImplementedError
 
     def list_maps(self, minimal=False):
         """
         Return names of maps in this study.
 
         Map names are also added to logger for command line display.
         Parameter minimal determines format: If True only map names are
@@ -276,106 +283,139 @@
 
         # check if export folder exists, create if necessary
         if not os.path.isdir(export_folder):
             os.mkdir(export_folder)
 
         return export_folder
 
-    def save(self, filepath='', gz=False):
+    def save(self, filepath=''):
         """
-        Save pickled version of study object.
+        Save study object as .pyceps archive.
         Note: File is only created if at least one map was imported!
 
         By default, the filename is the study's name, but can also be
         specified by the user.
         If the file already exists, user interaction is required to either
         overwrite file or specify a new file name.
 
-        Using HIGHEST_PROTOCOL is almost 2X faster and creates a file that
-        is ~10% smaller. Load times go down by a factor of about 3X.
-
         Parameters:
             filepath : string (optional)
                 custom path for the output file
-            gz : boolean (optional)
-                use gzip compression or not
 
         Raises:
             ValueError : If user input is not recognised
 
         Returns:
-            str : file path PKL was saved to
+            root : ET.Element
+            str : file path .pyceps was saved to
         """
 
+        if not filepath:
+            filepath = os.path.join(self.build_export_basename(''),
+                                    self.name + '.pyceps')
+        if not filepath.lower().endswith('.pyceps'):
+            filepath += '.pyceps'
+
         if not self.maps:
             log.info('No maps imported, nothing to save!')
-            return
+            return None, filepath
 
-        if filepath:
-            if filepath.lower().endswith('.pkl'):
-                filepath = filepath[:-4]
-            f_loc = os.path.abspath(filepath)
-        else:
-            f_loc = os.path.join(self.build_export_basename(''), self.name)
-
-        # handle un-pickleable attributes
-        study_base = self.repository.base
-        study_root = self.repository.root
-        if isinstance(self.repository.root, zipfile.Path):
-            self.repository.root = os.path.abspath(
-                self.repository.root.root.filename
-            )
-        if isinstance(self.repository.base, zipfile.Path):
-            self.repository.base = os.path.abspath(
-                self.repository.base.root.filename
-            )
-        if isinstance(self.repository.root, py7zr.SevenZipFile):
-            self.repository.root = os.path.abspath(
-                self.repository.root.filename
-            )
-        if isinstance(self.repository.base, py7zr.SevenZipFile):
-            self.repository.base = os.path.abspath(
-                self.repository.base.filename
-            )
-
-        f_loc += '.gz' if gz else '.pkl'
-        if os.path.isfile(f_loc):
+        # check if file already exists
+        if os.path.isfile(filepath):
             user_input = input('Study object already exists, overwrite? [Y/N]')
             # input validation
             if user_input.lower() in ('y', 'yes'):
                 pass
             elif user_input.lower() in ('n', 'no'):
                 user_input = input('Save with suffix? [Y/N] ')
                 if user_input.lower() in ('y', 'yes'):
                     suffix = ''
                     while not suffix:
                         suffix = input('Suffix: ')
-                    f_loc, ext = os.path.splitext(f_loc)
-                    f_loc = f_loc + '_' + suffix + ext
+                    filepath, ext = os.path.splitext(filepath)
+                    filepath += '_' + suffix + ext
                 elif user_input.lower() in ('n', 'no'):
-                    return
+                    return None, filepath
             else:
                 # ... error handling ...
                 print('Error: Input {} unrecognised.'.format(user_input))
                 raise ValueError
 
-        if gz:
-            f = gzip.open(f_loc, 'wb')
-        else:
-            f = open(f_loc, 'wb')
+        # build XML
+        root = ET.Element('Study',
+                          name=self.name,
+                          system=self.system,
+                          version=PYCEPS_VERSION,
+                          created=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+                          )
+
+        # add repository info
+        ET.SubElement(root, 'Repository',
+                      base=self.repository.get_base_string(),
+                      root=self.repository.get_root_string(),
+                      encoding=self.encoding
+                      )
+
+        # add additional meshes
+        if self.meshes:
+            count = str(len(self.meshes.fileNames))
+            meshes_item = ET.SubElement(root, 'AdditionalMeshes',
+                                        count=count,
+                                        )
+            xml_add_binary_numpy(meshes_item, 'fileNames',
+                                 np.array(self.meshes.fileNames))
+            xml_add_binary_numpy(meshes_item, 'registrationMatrix',
+                                 np.array(self.meshes.registrationMatrix))
+
+        # add mapping procedures
+        sep = ';'
+        procedures = ET.SubElement(root, 'Procedures',
+                                   count=str(len(self.maps.keys())),
+                                   names=sep.join(self.mapNames),
+                                   points=sep.join(
+                                       [str(x) for x in self.mapPoints]
+                                   ),
+                                   sep=str(ord(sep))
+                                   )
+        for cmap in self.maps.values():
+            proc = ET.SubElement(procedures, 'Procedure', name=cmap.name)
+
+            # add surface mesh
+            xml_add_binary_surface(proc, cmap.surface)
+
+            # add mapping points
+            points = ET.SubElement(proc, 'Points',
+                                   count=str(len(cmap.points))
+                                   )
+            for key in list(EPPoint('dummy', parent=cmap).__dict__):
+                if key == 'parent':
+                    # don't save this
+                    continue
+
+                data = [getattr(p, key) for p in cmap.points]
+                # handle maps with no points
+                if data:
+                    is_trace = (all([isinstance(e, Trace) for e in data])
+                                or (isinstance(data[0], list)
+                                    and all([isinstance(e, Trace) for e in data[0]])
+                                    )
+                                )
+                    if is_trace:
+                        xml_add_binary_trace(points, key, data)
+                        continue
+
+                xml_add_binary_numpy(points, key, np.array(data))
 
-        pickle.dump(self, f, protocol=pickle.HIGHEST_PROTOCOL)
-        f.close()
+            # add representative body surface ECGs
+            xml_add_binary_bsecg(proc, cmap.bsecg)
 
-        # restore study root
-        self.repository.root = study_root
-        self.repository.base = study_base
+            # add lesion data
+            xml_add_binary_lesion(proc, cmap.lesions)
 
-        log.info('saved study to {}'.format(f_loc))
-        return f_loc
+        return root, filepath
 
     def visualize(self, bgnd=None):
         """Visualize the study in dash."""
 
         log.info('visualizing study')
         log.warning('This will lock the console!')
 
@@ -395,15 +435,15 @@
             the parent study for this map
         surfaceFile : str
             filename of file containing the anatomical shell data
         surface : Surface
             triangulated anatomical shell
         points : list of subclass EPPoints
             the mapping points recorded during mapping procedure
-        ecg : list of BodySurfaceECG
+        bsecg : list of BodySurfaceECG
             body surface ECG data for the mapping procedure
         lesions : list of Lesion
             ablation data for this mapping procedure
 
     Methods:
         get_valid_points(return_invalid=False)
             returns valid mapping points recorded during procedure. If
@@ -477,15 +517,15 @@
 
         self.name = name
         self.parent = parent
 
         self.surfaceFile = ''
         self.surface = None
         self.points = []
-        self.ecg = []
+        self.bsecg = []
         self.lesions = []
 
     def get_valid_points(self, return_invalid=False):
         """
         Get valid points for this map.
 
         Parameters:
@@ -500,14 +540,18 @@
         if not return_invalid:
             return [point for point in self.points if point.is_valid()]
 
         return ([point for point in self.points if point.is_valid()],
                 [point for point in self.points if not point.is_valid()]
                 )
 
+    def import_map(self, *args, **kwargs):
+        """Import all relevant data."""
+        raise NotImplementedError
+
     def load_mesh(self, *args, **kwargs):
         """Load triangulated representation of the anatomical shell."""
         raise NotImplementedError
 
     def load_points(self, *args, **kwargs):
         """Load mapping points recorded during mapping procedure."""
         raise NotImplementedError
@@ -575,16 +619,17 @@
 
         # adjust array dims for compatibility
         interpolated = np.expand_dims(interpolated, 1)
 
         surf_map = SurfaceSignalMap(name=which.upper(),
                                     values=interpolated.astype(np.single),
                                     location='pointData',
-                                    description='creationDate:{}'.format(
-                                        datetime.datetime)
+                                    description='creationDate: {}'.format(
+                                        datetime.datetime.now()
+                                        .strftime("%Y-%m-%d %H:%M:%S"))
                                     )
         self.surface.add_signal_maps(surf_map)
 
     def export_mesh_vtk(self, basename='',
                         maps_to_add=None,
                         labels_to_add=None):
         """
@@ -906,41 +951,62 @@
                            .format(not_found, self.name))
 
         # export point files
         self.export_point_cloud(points=points, basename=basename)
 
         # store ecg traces as igb files
         writer = FileWriter()
-        channel_data = np.array([])
+        channel_data = {}  # key is the filename suffix including point cloud
         # save data channel-wise
         for channel in which:
             if channel.upper() == 'BIP':
-                channel_data = np.asarray([x.egmBip.data for x in points])
+                channel_data['BIP.pc'] = (
+                    np.asarray([x.egmBip.data for x in points])
+                )
+
             elif channel.upper() == 'UNI':
-                channel_data = np.asarray([x.egmUni[0].data
-                                           for x in points])
+                channel_data['UNI.pc'] = (
+                    np.asarray([x.egmUni[0].data for x in points])
+                )
+                channel_data['UNI2.upc'] = (
+                    np.asarray([x.egmUni[1].data for x in points])
+                )
+                # export 2nd unipolar point cloud
+                uni2_points = np.array([point.uniX for point in points])
+                # adjust ndarray dimensions
+                if uni2_points.ndim == 3:
+                    uni2_points = np.squeeze(uni2_points, axis=2)
+                pts_file = '{}.egm.UNI2.upc.pts'.format(basename)
+                log.info('exporting mapping points cloud to {}'
+                         .format(pts_file)
+                         )
+                writer.dump(pts_file, uni2_points)
+
             elif channel.upper() == 'REF':
-                channel_data = np.asarray([x.egmRef.data for x in points])
-            if channel_data.size == 0:
-                log.warning('no data found for channel {}, nothing to export!'
-                            .format(channel))
-            # save data to igb
-            # Note: this file cannot be loaded with the CARTO mesh but rather
-            #       with the exported mapped nodes
-            header = {'x': channel_data.shape[0],
-                      't': channel_data.shape[1],
+                channel_data['REF.pc'] = (
+                    np.asarray([x.egmRef.data for x in points])
+                )
+
+        # save data to igb
+        # Note: this file cannot be loaded with the CARTO mesh but rather
+        #       with the exported mapped nodes
+        for key, data in channel_data.items():
+            if data.size == 0:
+                log.warning('no data found for channel {}!'.format(key))
+            header = {'x': data.shape[0],
+                      't': data.shape[1],
                       'unites_t': 'ms',
                       'unites': 'mV',
-                      'dim_t': channel_data.shape[0]-1, # (num_tsteps - 1) * inc_t
+                      'dim_t': data.shape[0]-1,
                       'org_t': 0,
                       'inc_t': 1}
 
-            filename = '{}.egm.{}.pc.igb'.format(basename, channel)
-            f = writer.dump(filename, header, channel_data)
-            log.info('exported EGM trace {} to {}'.format(channel, f))
+            filename = '{}.egm.{}.igb'.format(basename, key)
+            f = writer.dump(filename, header, data)
+            log.info('exported EGM trace {} to {}'.format(key, f))
 
         return
 
     def export_point_ecg(self, basename='', which=None, points=None):
         """
         Export surface ECG traces in IGB format.
 
@@ -963,25 +1029,25 @@
                 path and filename of the exported files
         Returns:
               None
         """
 
         log.info('exporting body surface ECGs for map {}'.format(self.name))
 
-        if not self.ecg:
+        if not self.bsecg:
             log.warning('no body surface ECG data found, nothing to export...')
             return
 
         if not basename:
             basename = self.parent.build_export_basename(self.name)
             basename = os.path.join(basename, self.name)
 
         writer = FileWriter()
 
-        for bsecg in self.ecg:
+        for bsecg in self.bsecg:
             filename = '{}.bsecg.{}.json'.format(basename, bsecg.method)
 
             # build timeline
             t = np.linspace(start=0.0,
                             stop=bsecg.traces[0].data.shape[0] / 1000,
                             num=bsecg.traces[0].data.shape[0]
                             )
@@ -989,15 +1055,15 @@
             bsecg_json = dict()
             bsecg_json['t'] = t.round(decimals=3).tolist()
 
             data_dict = dict()
             for signal in bsecg.traces:
                 data_dict[signal.name] = signal.data.tolist()
 
-            bsecg_json['ecg'] = data_dict
+            bsecg_json['bsecg'] = data_dict
 
             f = writer.dump(filename, bsecg_json, indent=2)
             log.info('exported body surface ECG trace(s) {} to {}'
                      .format([t.name for t in bsecg.traces], f))
 
     def export_lesions(self, filename=''):
         """
@@ -1080,24 +1146,26 @@
     Base class representing a recording point.
 
     Attributes:
         name : str
             identifier for this recording point
         parent : subclass of EPMap
             parent mapping procedure this point belongs to
-        recX : ndarray (3, 1)
+        recX : ndarray (3, )
             coordinates at which this point was recorded
-        prjX : ndarray (3, 1)
+        prjX : ndarray (3, )
             coordinates of the closest anatomical shell vertex
         prjDistance : float
             distance between recording location and closest shell vertex
         refAnnotation : int
             annotation for reference detection in samples
         latAnnotation : int
             annotation for local activation time in samples
+        woi : ndarray (2, 1)
+            start and end timestamps of the WOI in samples
         uniVoltage : float
             peak-to-peak voltage in unipolar EGM
         bipVoltage : float
             peak-to-peak voltage in bipolar EGM
         egmBip : Trace
             bipolar EGM trace
         egmUni : Trace
@@ -1110,22 +1178,22 @@
 
     Methods:
         is_valid()
 
     """
 
     def __init__(self, name,
-                 coordinates=np.full((3, 1), np.nan, dtype=float),
+                 coordinates=np.full(3, np.nan, dtype=np.float32),
                  parent=None):
         """
         Constructor.
 
         Parameters:
             name : string
-            coordinates : ndarray (3, 1)
+            coordinates : ndarray (3, )
                 the coordinates where this point was recorded
             parent : EPMap
 
         Raises:
             TypeError : if parent is not of type EPMap
 
         """
@@ -1135,29 +1203,34 @@
                             .format(type(parent)))
 
         self.name = name
         self.parent = parent
 
         # location info
         self.recX = coordinates
-        self.prjX = np.full((3, 1), np.nan, dtype=float)
+        self.prjX = np.full((3, 1), np.nan, dtype=np.float32)
         self.prjDistance = np.nan
 
         # annotation info
         self.refAnnotation = np.nan
         self.latAnnotation = np.nan
+        self.woi = np.full((2, 1), np.iinfo(int).min, dtype=int)
 
         # voltages
         self.uniVoltage = np.nan
         self.bipVoltage = np.nan
 
         # signal traces
         self.egmBip = None
         self.egmUni = None
         self.egmRef = None
 
         self.impedance = np.nan
         self.force = np.nan
 
+    def import_point(self, *args, **kwargs):
+        """Import relevant data."""
+        raise NotImplementedError
+
     def is_valid(self):
         """Check if this point is valid."""
         raise NotImplementedError
```

### Comparing `pyCEPS-0.1.1/pyceps/datatypes/surface.py` & `pyCEPS-1.0.0/pyceps/datatypes/surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,16 @@
 
         writer = FileWriter()
         writer.dump(filename, self.values[:, 0])
 
         return filename
 
 
-Mesh = namedtuple('Mesh', ['registrationMatrix', 'fileNames'])
+Mesh = namedtuple('Mesh', ['registrationMatrix',
+                           'fileNames'])
 Mesh.__doc__ = """
 Additional meshes.
 
 Attributes:
     registrationMatrix : ndarray (4, 4)
         transformation matrix (scale, rotate, shift)
     filenames: list of str
```

### Comparing `pyCEPS-0.1.1/pyceps/exceptions.py` & `pyCEPS-1.0.0/pyceps/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/fileio/__init__.py` & `pyCEPS-1.0.0/pyceps/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/fileio/cartoio.py` & `pyCEPS-1.0.0/pyceps/fileio/cartoio.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import logging
 import zipfile
 import re
-import xml.etree.ElementTree as xml
+import xml.etree.ElementTree as ET
+from xml.dom import minidom
 import numpy as np
-import gzip
-import pickle
 import scipy.spatial.distance as sp_distance
 
 from pyceps.fileio.pathtools import Repository
 from pyceps.datatypes import EPStudy, EPMap, EPPoint, Mesh
 from pyceps.fileio import FileWriter
+from pyceps.fileio.xmlio import (xml_add_binary_numpy,
+                                 xml_load_binary_data,
+                                 xml_load_binary_surface,
+                                 xml_load_binary_trace,
+                                 xml_load_binary_bsecg,
+                                 xml_load_binary_lesion
+                                 )
 from pyceps.fileio.cartoutils import (read_mesh_file,
                                       read_ecg_file_header, read_ecg_file,
                                       read_force_file,
                                       read_visitag_file,
                                       read_electrode_pos_file)
 from pyceps.datatypes.cartotypes import (CartoUnits, Coloring, ColoringRange,
                                          SurfaceErrorTable,
@@ -125,48 +131,48 @@
         """
 
         super().__init__(system='carto3',
                          study_repo=study_repo,
                          pwd=pwd,
                          encoding=encoding)
 
-        # locate study XML
-        log.info('Locating study XML in {}...'.format(self.repository))
-        study_info = self._locate_study_xml(self.repository,
-                                            pwd=self.pwd,
-                                            encoding=self.encoding)
-        if not study_info:
-            raise FileNotFoundError
-
-        log.info('found study XML at {}'.format(self.repository.root))
-        self.studyXML = study_info['xml']
-        self.name = study_info['name']
+        self.studyXML = ''
 
         self.units = None
         self.environment = None  # TODO: is this relevant info?
         self.externalObjects = None  # TODO: is this relevant info?
         self.mappingParams = None
 
         # visitag data
         self.visitag = Visitag()
 
-        self.import_study()
-
     def import_study(self):
         """
         Load study details and basic information from study XML.
         Overrides BaseClass method.
         """
 
+        # locate study XML
+        log.info('Locating study XML in {}...'.format(self.repository))
+        study_info = self.locate_study_xml(self.repository, pwd=self.pwd,
+                                           encoding=self.encoding)
+        if not study_info:
+            log.warning('cannot locate study XML!')
+            return
+
+        log.info('found study XML at {}'.format(self.repository.root))
+        self.studyXML = study_info['xml']
+        self.name = study_info['name']
+
         log.info('accessing study XML: {}'.format(self.studyXML))
         log.info('gathering study information...')
 
         xml_path = self.repository.join(self.studyXML)
         with self.repository.open(xml_path) as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         log.debug('reading study units')
         study_units = root.find('Units')
         self.units = CartoUnits(Distance=study_units.get('Distance'),
                                 Angle=study_units.get('Angle'))
 
         log.debug('reading study coloring table')
@@ -228,27 +234,27 @@
             TagsTable=tags_table
         )
 
         log.debug('reading additional meshes')
         item = root.find('Meshes')
         if item:
             matrix = np.asarray(item.find('RegistrationMatrix').text.split(),
-                                dtype=float)
+                                dtype=np.float32)
             meshes = []
             for mesh in item.findall('Mesh'):
                 meshes.append(mesh.get('FileName'))
             self.meshes = Mesh(registrationMatrix=matrix, fileNames=meshes)
             log.info('found {} additional meshes in study'.format(len(meshes)))
 
         log.debug('reading study maps info')
         map_names = []
         map_points = []
         for item in root.iter('Map'):
             map_names.append(item.get('Name'))
-            map_points.append(item.find('CartoPoints').get('Count'))
+            map_points.append(int(item.find('CartoPoints').get('Count')))
             log.debug('found map {} with {} mapping points'
                       .format(map_names[-1], map_points[-1]))
 
         self.mapNames = map_names
         self.mapPoints = map_points
 
     def import_maps(self, map_names=None, egm_names_from_pos=False,
@@ -285,17 +291,16 @@
         # do some pre-import checks
         map_names = super().import_maps(map_names)
 
         # now load the maps
         for map_name in map_names:
             try:
                 log.info('importing map {}:'.format(map_name))
-                new_map = CartoMap(map_name, self.studyXML,
-                                   parent=self,
-                                   egm_names_from_pos=egm_names_from_pos)
+                new_map = CartoMap(map_name, self.studyXML, parent=self)
+                new_map.import_map(egm_names_from_pos=egm_names_from_pos)
                 self.maps[map_name] = new_map
             except Exception as err:
                 log.warning('failed to import map {}: {}'
                             .format(map_name, err))
                 continue
 
         return
@@ -613,72 +618,203 @@
             # add all grid points to visitag grid
             grid.add_points(grid_points)
             # add this grid to list of grids
             grid_sites.append(grid)
 
         return grid_sites
 
-    @classmethod
-    def load(cls, filename, root=None):
+    def load(self, file: str,  repo_path: str = ''):
         """
-        Load pickled version of a study. Overrides BaseClass method.
+        Load study from file. Overrides BaseClass method.
 
-        A previously saved pickled version of a CartoStudy object can be
+        A previously saved version of a CartoStudy object can be
         loaded. The objects <study_root> is set to the one stored in the
-        PKL file if valid. If not, the folder of the PKL is set as root
+        file if valid. If not, the folder of the PKL is set as root
         directory.
         The path to the Carto files can also be specified explicitly.
 
-        Note that loading to a string with pickle.loads() is about 10% faster
-        but probably consumes a lot more memory, so we'll skip that for now.
-
         Parameters:
-            filename : string
-                path to the .PKL or .GZ study file
-            root : string (optional)
-                set study root to this directory
+            file : str
+                location of .pyceps file
+            repo_path : str
+                path to repository
 
         Raises:
-            FileNotFoundError : if pickled file cannot be found
+            TypeError : If file is not Carto3
 
         Returns:
-            CartoStudy
+            None
 
         """
 
-        log.info('loading study from {}'.format(filename))
+        log.debug('loading study')
 
-        if filename.endswith('.gz'):
-            f = gzip.open(filename, 'rb')
-        else:
-            f = open(filename, 'rb')
-        obj = pickle.load(f)
-        f.close()
+        with open(file) as fid:
+            root = ET.parse(fid).getroot()
+
+        system = root.get('system')
+        if not system.lower() == "carto3":
+            raise TypeError('expected Carto3 system file, found {}'
+                            .format(system))
+
+        # load basic info
+        self.system = system
+        self.name = root.get('name')
+        self.studyXML = root.get('studyXML')
+        units = root.find('Units')
+        self.units = CartoUnits(units.get('distance'), units.get('angle'))
+
+        # load additional meshes
+        mesh_item = root.find('AdditionalMeshes')
+        if int(mesh_item.get('count')) > 0:
+            _, reg_matrix = xml_load_binary_data(
+                [x for x in mesh_item.findall('DataArray')
+                 if x.get('name') == 'registrationMatrix'][0]
+            )
+            _, file_names = xml_load_binary_data(
+                [x for x in mesh_item.findall('DataArray')
+                 if x.get('name') == 'fileNames'][0]
+            )
+            self.meshes = Mesh(registrationMatrix=reg_matrix,
+                               fileNames=file_names
+                               )
+
+        # load mapping procedures
+        proc_item = root.find('Procedures')
+        num_procedures = proc_item.get('count')
+        sep = chr(int(proc_item.get('sep')))
+        self.mapNames = proc_item.get('names').split(sep)
+        self.mapPoints = [int(x) for x in proc_item.get('points').split(sep)]
+
+        for proc in proc_item.iter('Procedure'):
+            name = proc.get('name')
+
+            new_map = CartoMap(name, self.studyXML, parent=self)
+            new_map.surfaceFile = proc.get('meshFile')
+            new_map.volume = float(proc.get('volume'))
+
+            # load mesh
+            new_map.surface = xml_load_binary_surface(proc.find('Mesh'))
+
+            # load BSECGs
+            new_map.bsecg = xml_load_binary_bsecg(proc.find('BSECGS'))
+
+            # load lesions
+            new_map.lesions = xml_load_binary_lesion(proc.find('Lesions'))
+
+            # load EGM points
+            p_data = {}
+            points_item = proc.find('Points')
+            num_points = int(points_item.get('count'))
+
+            for arr in points_item.findall('DataArray'):
+                d_name, data = xml_load_binary_data(arr)
+                p_data[d_name] = data
+            for arr in points_item.findall('Traces'):
+                d_name, data = xml_load_binary_trace(arr)
+                p_data[d_name] = data
+
+            points = []
+            for i in range(num_points):
+                new_point = CartoPoint('dummy', parent=new_map)
+                for key, value in p_data.items():
+                    if hasattr(new_point, key):
+                        setattr(new_point, key, value[i])
+                    else:
+                        log.warning('cannot set attribute "{}" for CartoPoint'
+                                    .format(key))
+                points.append(new_point)
+            new_map.points = points
+
+            # now we can add the procedure to the study
+            self.maps[name] = new_map
 
         # try to set root if explicitly given
-        if root:
-            if obj.set_repository(os.path.abspath(root)):
-                log.info('setting study root to {}'.format(root))
-                return obj
+        if repo_path:
+            if self.set_repository(os.path.abspath(repo_path)):
+                log.info('setting study root to {}'.format(repo_path))
+                return
             else:
                 log.info('cannot set study root to {}\n'
-                         'Trying to use root information from PKL'
-                         .format(root))
+                         'Trying to use root information from file'
+                         .format(repo_path))
 
         # try to re-set previous study root
-        if obj.set_repository(obj.repository.base):
+        base_path = root.find('Repository').get('root')
+        if self.set_repository(base_path):
             log.info('previous study root is still valid ({})'
-                     .format(obj.repository.root))
-            return obj
+                     .format(self.repository.root))
+            return
 
         # no valid root found so far, set to pkl directory
-        log.warning('no valid study root found. Using .pkl location!'.upper())
-        obj.repository.base = os.path.abspath(filename)
-        obj.repository.root = os.path.dirname(os.path.abspath(filename))
-        return obj
+        log.warning(
+            'no valid study root found. Using file location!'.upper())
+        self.repository.base = os.path.abspath(file)
+        self.repository.root = os.path.dirname(os.path.abspath(file))
+
+    def save(self, filepath=''):
+        """
+        Save study object as .pyceps archive.
+        Note: File is only created if at least one map was imported!
+
+        By default, the filename is the study's name, but can also be
+        specified by the user.
+        If the file already exists, user interaction is required to either
+        overwrite file or specify a new file name.
+
+        Parameters:
+            filepath : string (optional)
+                custom path for the output file
+
+        Raises:
+            ValueError : If user input is not recognised
+
+        Returns:
+            str : file path .pyceps was saved to
+        """
+
+        # add basic information to XML
+        root, filepath = super().save(filepath)
+
+        if not root:
+            # no base info was created (no maps imported), nothing to add
+            return filepath
+
+        # add Carto specific data
+        root.set('studyXML', self.studyXML)
+        ET.SubElement(root, 'Units',
+                      distance=self.units.Distance,
+                      angle=self.units.Angle
+                      )
+
+        for key, cmap in self.maps.items():
+            map_item = [p for p in root.iter('Procedure')
+                        if p.get('name') == key][0]
+
+            # add additional procedure info
+            map_item.set('meshFile', cmap.surfaceFile)
+            map_item.set('volume', str(cmap.volume))
+
+            # add additional point info
+            point_item = map_item.find('Points')
+            to_add = ['pointFile', 'ecgFile', 'forceFile', 'uniX']
+            for name in to_add:
+                data = [getattr(p, name) for p in cmap.points]
+                xml_add_binary_numpy(point_item, name, np.array(data))
+
+        # make XML pretty
+        dom = minidom.parseString(ET.tostring(root))
+        xml_string = dom.toprettyxml(encoding='utf-8')
+
+        # write XML
+        with open(filepath, 'wb') as fid:
+            fid.write(xml_string)
+
+        log.info('saved study to {}'.format(filepath))
+        return filepath
 
     def export_additional_meshes(self, filename=''):
         """
         Export additional meshes and registration matrix in study to VTK.
         Overrides BaseClass method.
 
         If additional meshes, e.g. from CT, are part of the study, they are
@@ -699,14 +835,19 @@
             filename : str (optional)
                 path to export file, export to default location if not given
 
         Returns:
             None
         """
 
+        if not self.is_root_valid():
+            log.warning('a valid study root is necessary to dump additional '
+                        'meshes!')
+            return
+
         if not self.meshes:
             log.info('no additional meshes found in study, nothing to export')
             return
 
         if not filename:
             basename = self.build_export_basename('additionalMeshes')
         else:
@@ -825,15 +966,15 @@
             # root saved in study is valid, nothing to do
             return True
         elif root_dir:
             tmp_root = Repository(root_dir, pwd=pwd)
             if not tmp_root.root:
                 # dummy repo was not initialized properly, so root is invalid
                 return False
-            return self._locate_study_xml(tmp_root, pwd=pwd) is not None
+            return self.locate_study_xml(tmp_root, pwd=pwd) is not None
 
         return False
 
     def set_repository(self, root_dir):
         """
         Change path to root directory. Overrides BaseClass method.
         If new root directory is invalid, it is not changed.
@@ -852,39 +993,38 @@
         study_root = os.path.abspath(root_dir)
         if not self.is_root_valid(study_root):
             log.warning('root directory is invalid: {}'.format(study_root))
             return False
 
         # study XML was found, check if it is the same study
         root = Repository(root_dir)
-        study_info = self._locate_study_xml(root,
-                                            pwd=self.pwd,
-                                            encoding=self.encoding)
+        study_info = self.locate_study_xml(root, pwd=self.pwd,
+                                           encoding=self.encoding)
         if not study_info:
             # should never happen...
             raise FileNotFoundError
 
-        log.info('found study XML at {}'.format(self.repository.root))
         if not self.studyXML == study_info['xml']:
             log.warning('name of study XML differs, will not change root!')
             return False
         if not self.name == study_info['name']:
             log.warning('name of study differs, will not change root!')
             return False
 
         # change study root
         self.repository = root
+        log.info('found study XML at {}'.format(self.repository.root))
 
         return True
 
     @staticmethod
-    def _locate_study_xml(repository,
-                          pwd='',
-                          regex=r'^((?!Export).)*.xml$',
-                          encoding='cp1252'):
+    def locate_study_xml(repository,
+                         pwd='',
+                         regex=r'^((?!Export).)*.xml$',
+                         encoding='cp1252'):
         """
         Locate study XML in Carto repository. A file is considered valid if
         it starts with '<Study name='.
 
         Parameters:
             repository : Repository
                 This is searched recursively
@@ -924,15 +1064,15 @@
                    or repository.is_archive(repository.join(f))
                    ]
         log.debug('found subdirectories: {}'.format(folders))
 
         for folder in folders:
             # update root location and start new search there
             repository.update_root(repository.join(folder))
-            return CartoStudy._locate_study_xml(repository)
+            return CartoStudy.locate_study_xml(repository)
 
         # XML was nowhere to be found
         return None
 
 
 class CartoMap(EPMap):
     """
@@ -959,15 +1099,15 @@
             color ranges used by Carto
         surfaceFile : str
             filename of file containing the anatomical shell data
         surface : Surface
             triangulated anatomical shell
         points : list of subclass EPPoints
             the mapping points recorded during mapping procedure
-        ecg : list of BodySurfaceECG
+        bsecg : list of BodySurfaceECG
             body surface ECG data for the mapping procedure
         lesions : list of Lesion
             ablation data for this mapping procedure
         rf : MapRF object
             force and ablation data of the mapping procedure
 
     Methods:
@@ -985,35 +1125,25 @@
         import_rf_data()
             import RF and force data
         visitag_to_lesion(visitag_sites)
             convert VisiTag ablation sites to BaseClass Lesion
 
     """
 
-    def __init__(self, name, study_xml, parent=None, egm_names_from_pos=False):
+    def __init__(self, name, study_xml, parent=None):
         """
         Constructor.
-        Load all relevant information for this mapping procedure, import EGM
-        recording points, interpolate standard surface parameter maps from
-        point data (bip voltage, uni voltage, LAT), and build representative
-        body surface ECGs.
 
         Parameters:
             name : str
                 name of the mapping procedure
             study_xml : str
                 name of the study's XML file (same as in parent)
             parent : CartoStudy (optional)
                 study this map belongs to
-            egm_names_from_pos : boolean (optional)
-                get names of egm traces from electrode positions
-
-        Raises:
-            MapAttributeError : If unable to retrieve map attributes from XML
-            MeshFileNotFoundError: If mesh file is not found in repository
 
         Returns:
             None
 
         """
 
         super().__init__(name, parent=parent)
@@ -1024,24 +1154,50 @@
         self.visible = None
         self.type = None
         self.volume = np.nan
         self.RefAnnotationConfig = None
         self.coloringRangeTable = []
         self.rf = None
 
+    def import_map(self, egm_names_from_pos=False):
+        """
+        Load all relevant information for this mapping procedure, import EGM
+        recording points, interpolate standard surface parameter maps from
+        point data (bip voltage, uni voltage, LAT), and build representative
+        body surface ECGs.
+
+        Parameters:
+            egm_names_from_pos : boolean (optional)
+                get names of egm traces from electrode positions
+
+        Raises:
+            MapAttributeError : If unable to retrieve map attributes from XML
+            MeshFileNotFoundError: If mesh file is not found in repository
+
+        Returns:
+            None
+
+        """
+
         self._import_attributes()
         self.surface = self.load_mesh()
+        # check if parent study was imported or loaded
+        # if it was loaded, some attributes are missing
+        if not self.parent.mappingParams:
+            log.info('study was probably loaded from file, need to re-import '
+                     'basic study information')
+            self.parent.import_study()
         self.points = self.load_points(
             study_tags=self.parent.mappingParams.TagsTable,
             egm_names_from_pos=egm_names_from_pos)
         # build surface maps
         self.interpolate_data('lat')
         self.interpolate_data('bip')
         self.interpolate_data('uni')
-        self.ecg = self.get_map_ecg(method=['median', 'mse', 'ccf'])
+        self.bsecg = self.get_map_ecg(method=['median', 'mse', 'ccf'])
 
     def load_mesh(self):
         """
         Load a Carto3 triangulated anatomical shell from file. Overrides
         BaseClass method.
 
         Raises:
@@ -1087,15 +1243,15 @@
             log.warning('no tag names provided for study {}: cannot '
                         'convert tag ID to tag name'.format(self.name))
 
         points = []
 
         xml_file = self.parent.repository.join(self.studyXML)
         with self.parent.repository.open(xml_file, mode='rb') as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         map_item = [x for x in root.find('Maps').findall('Map')
                     if x.get('Name') == self.name]
         if not map_item:
             log.warning('no map with name {} found in study XML'
                         .format(self.name))
             return -1
@@ -1110,15 +1266,15 @@
         )
         if not self.parent.repository.is_file(all_points_file):
             log.warning('unable to find export overview of all points {}'
                         .format(all_points_file))
             return -1
 
         with self.parent.repository.open(all_points_file, mode='rb') as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         if not root.get('Map_Name') == self.name:
             log.warning('map name {} in export file {} does not match map '
                         'name {} for import'
                         .format(root.get('Map_Name'),
                                 self.name,
                                 all_points_file)
@@ -1171,19 +1327,20 @@
                 log.info('No Point Export file found for point {}'
                          .format(point_name))
                 point_file = None
 
             log.debug('adding point {} to map {}'.format(point_name,
                                                          self.name))
             new_point = CartoPoint(point_name,
-                                   point_file,
                                    coordinates=xyz,
                                    tags=tag_names,
-                                   parent=self,
-                                   egm_names_from_pos=egm_names_from_pos)
+                                   parent=self)
+            new_point.import_point(point_file,
+                                   egm_names_from_pos=egm_names_from_pos
+                                   )
             points.append(new_point)
 
         return points
 
     def import_lesions(self, directory=None):
         """
         Import VisiTag lesion data.
@@ -1280,15 +1437,15 @@
                 woi = point.woi
             if not point.refAnnotation == ref:
                 log.warning('REF annotation changed in point {}'
                             .format(point.name))
                 # make this the new ref
                 ref = point.refAnnotation
 
-        # build representative ecg trace
+        # build representative bsecg trace
         if isinstance(method, str):
             method = [method]
         repr_ecg = []
 
         for meth in method:
             if meth.lower() == 'median':
                 ecg = np.median(data, axis=0)
@@ -1678,15 +1835,15 @@
         Returns:
             None
 
         """
 
         xml_file = self.parent.repository.join(self.studyXML)
         with self.parent.repository.open(xml_file) as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         map_item = [x for x in root.find('Maps').findall('Map')
                     if x.get('Name') == self.name]
         if not map_item:
             raise MapAttributeError('no map with name {} found in study XML'
                                     .format(self.name))
         if len(map_item) > 1:
@@ -1756,17 +1913,17 @@
     Attributes:
         name : str
             identifier for this recording point
         pointFile : str
             name of the points XML file <map_name>_<point_ID>_Point_Export.xml
         parent : CartoMap
             parent mapping procedure this point belongs to
-        recX : ndarray (3, 1)
+        recX : ndarray (3, )
             coordinates at which this point was recorded
-        prjX : ndarray (3, 1)
+        prjX : ndarray (3, )
             coordinates of the closest anatomical shell vertex
         prjDistance : float
             distance between recording location and closest shell vertex
         refAnnotation : int
             annotation for reference detection in samples
         latAnnotation : int
             annotation for local activation time in samples
@@ -1787,18 +1944,18 @@
         force : float
         barDirection : ndarray (3, 1)
             surface normal of the closest surface point
         tags : list of str
             tags assigned to this point, i.e. 'Full_name' in study's TagsTable
         ecgFile : str
             name of the points ECG file <map_name>_<point_name>_ECG_Export.txt
-        uniX : ndarray (3, 2)
-            cartesian coordinates of the unipolar recording electrodes
-            NOTE: coordinates of second unipolar electrode are NaN if
-            unipolar channel names were read from ECG file only
+        uniX : ndarray (3, )
+            cartesian coordinates of the second unipolar recording electrode
+            NOTE: coordinates of second unipolar electrode are same as recX if
+            position cannot be determined
         forceFile : str
             name of the points contact force file
             <map_name>_<point_name>_Contact_Force.txt
         force : PointForce
             contact force data for this point
 
     Methods:
@@ -1807,89 +1964,82 @@
         load(egm_names_from_pos=False)
             load all data associated with this point
         import_ecg(channel_names)
             import ECG data for this point
 
     """
 
-    def __init__(self, name, point_file,
-                 coordinates=np.full((3, 1), np.nan, dtype=float),
+    def __init__(self, name,
+                 coordinates=np.full(3, np.nan, dtype=np.float32),
                  tags=None,
-                 egm_names_from_pos=False,
                  parent=None):
         """
         Constructor.
 
         Parameters:
              name : str
                 name / identifier for this point
-            point_file : str
-                name of this points XML file
-                <map_name>_<point_name>_Point_Export.xml
-            coordinates : ndarray(3, 1)
+            coordinates : ndarray(3, )
                 cartesian coordinates of recording position
             tags: list of str (optional)
                 tags assigned to this point, i.e. 'Full_name' in study's
                 TagsTable
-            egm_names_from_pos : bool (optional)
-                get names of EGM traces from electrode positions
-                NOTE: second unipolar channel name and coordinates are only
-                valid if this is True
             parent : CartoMap
                 the map this point belongs to
 
-        Raises:
-            FileNotFoundError : if point's XML is not found
-
         Returns:
             None
 
         """
 
         super().__init__(name, coordinates=coordinates, parent=parent)
 
-        file_loc = self.parent.parent.repository.join(point_file)
-        if not self.parent.parent.repository.is_file(file_loc):
-            log.info('Points export file {} does not exist'
-                     .format(point_file))
-            raise FileNotFoundError
-
         # add Carto3 specific attributes
-        self.pointFile = point_file
+        self.pointFile = ''
         self.barDirection = None
-        self.woi = np.array([])
         self.tags = tags
         self.ecgFile = None
-        self.uniX = np.full((3, 2), np.nan, dtype=float)
+        self.uniX = np.full(3, np.nan, dtype=np.float32)
         self.forceFile = None
         self.forceData = None
 
-        self.load(egm_names_from_pos=egm_names_from_pos)
-
-    def load(self, egm_names_from_pos=False):
+    def import_point(self, point_file, egm_names_from_pos=False):
         """
         Load data associated with this point.
 
         Parameters:
+            point_file : str
+                name of this points XML file
+                <map_name>_<point_name>_Point_Export.xml
             egm_names_from_pos : boolean
                 If True, EGM electrode names are extracted from positions file.
                 This also returns name and coordinates of the second unipolar
                 channel.
 
+        Raises:
+            FileNotFoundError : if point's XML is not found
+
         Returns:
             None
 
         """
 
         log.debug('Loading point data for point {}'.format(self.name))
 
+        file_loc = self.parent.parent.repository.join(point_file)
+        if not self.parent.parent.repository.is_file(file_loc):
+            log.info('Points export file {} does not exist'
+                     .format(point_file))
+            raise FileNotFoundError
+        self.pointFile = point_file
+
         # read annotation data
         point_file = self.parent.parent.repository.join(self.pointFile)
         with self.parent.parent.repository.open(point_file) as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         annotation_item = root.find('Annotations')
         self.refAnnotation = int(annotation_item.get('Reference_Annotation'))
         self.latAnnotation = int(annotation_item.get('Map_Annotation'))
         woi_item = root.find('WOI')
         self.woi = np.asarray([woi_item.get('From'),
                                woi_item.get('To')]
@@ -1965,15 +2115,15 @@
             closest, distance, direct = self.parent.surface.get_closest_vertex(
                 [self.recX]
             )
             if closest.shape[0] != 1:
                 log.warning('found no or multiple surface vertices closest to '
                             'to point {}: {}'
                             .format(self.name, closest))
-            self.prjX = np.array(closest[0], dtype=float)
+            self.prjX = np.array(closest[0], dtype=np.float32)
             self.prjDistance = distance[0]
             self.barDirection = direct[0]
 
         # now get the force data for this point
         log.debug('reading force file for point {}'.format(self.name))
         self.forceFile = (self.pointFile.split('_Point_Export')[0]
                           + '_ContactForce.txt'
@@ -2072,15 +2222,15 @@
 
         try:
             ecg_data.shape[1]
         except IndexError:
             # array has shape (2500,) but (2500,1) is needed
             ecg_data = np.expand_dims(ecg_data, axis=1)
 
-        return ecg_data
+        return ecg_data.astype(np.float32)
 
     def _channel_names_from_ecg_header(self, ecg_header):
         """
         Get channel names for BIP, UNI and REF traces from file header.
 
         This function also tries to extract the name of the second unipolar
         channel from the bipolar channel name.
@@ -2136,34 +2286,37 @@
         """
         Get coordinates for 2nd unipolar channel from position file(s).
 
         Searches for recording coordinates in position file(s) and extracts
         coordinates of the subsequent channel. This should be the correct
         second unipolar channel for bipolar recordings.
 
-        Note: Method _channel_names_from_pos_file is more elaborate but
+        NOTE: If coordinates cannot be determined, the recording position of
+        the first unipolar channel is used!
+
+        NOTE: Method _channel_names_from_pos_file is more elaborate but
         fails often for missing channel positions in position files!
 
         Parameters:
             encoding:
 
         Returns:
-            ndarray(3, 1)
+            ndarray(3, )
                 coordinates of the second unipolar channel
 
         """
 
-        xyz_2 = np.full((3, 1), np.nan, dtype=np.float32)
+        xyz_2 = np.full(3, np.nan, dtype=np.float32)
 
         log.debug('get position of 2nd unipolar channel')
 
         # read points XML file
         point_file = self.parent.parent.repository.join(self.pointFile)
         with self.parent.parent.repository.open(point_file) as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         # get position files
         position_files = []
         for connector in root.find('Positions').findall('Connector'):
             connector_file = list(connector.attrib.values())[0]
             if connector_file.lower().endswith(
                     'ectrode_positions_onannotation.txt'):
@@ -2173,18 +2326,18 @@
             pos_file = self.parent.parent.repository.join(filename)
             if not self.parent.parent.repository.is_file(pos_file):
                 log.warning('position file {} for point {} not found'
                             .format(filename, self.name))
                 continue
 
             with self.parent.parent.repository.open(pos_file) as fid:
-                idx, time, xyz = read_electrode_pos_file(fid)
+                idx, time, xyz = read_electrode_pos_file(fid, encoding=encoding)
 
             # find electrode with the closest distance
-            dist = sp_distance.cdist(xyz, np.array([self.recX])).flatten()
+            dist = sp_distance.cdist(xyz, np.expand_dims(self.recX, axis=1).T).flatten()
             idx_closest = np.argwhere(dist == np.amin(dist)).flatten()
             if idx_closest.size != 1:
                 log.debug(
                     'found no or multiple electrodes with same minimum '
                     'distance in file {}. Trying next file...'
                     .format(filename))
                 continue
@@ -2197,16 +2350,17 @@
                 xyz_2 = xyz[idx_closest + 1, :]
             except IndexError:
                 log.debug('unable to get position of 2nd uni channel for '
                           'point {}'.format(self.name))
 
         if np.isnan(xyz_2).all():
             log.warning('coordinates for 2nd unipolar channel not found for '
-                        'point {}'
+                        'point {}, using recording position'
                         .format(self.name))
+            xyz_2 = self.recX
 
         return xyz_2
 
     def _channel_names_from_pos_file(self, egm_names, encoding='cp1252'):
         """
         Get channel names for BIP, UNI and REF traces from electrode positions.
 
@@ -2225,15 +2379,15 @@
 
         log.debug('extracting channel names from position files for point {}'
                   .format(self.name))
 
         # read points XML file
         point_file = self.parent.parent.repository.join(self.pointFile)
         with self.parent.parent.repository.open(point_file) as fid:
-            root = xml.parse(fid).getroot()
+            root = ET.parse(fid).getroot()
 
         # get position files
         position_files = []
         for connector in root.find('Positions').findall('Connector'):
             connector_file = list(connector.attrib.values())[0]
             if connector_file.lower().endswith('ectrode_positions_onannotation.txt'):
                 position_files.append(connector_file)
@@ -2290,24 +2444,24 @@
             encoding :
 
         Returns:
              egm_name_bip : string
                 name of the bipolar channel
             egm_name_uni : list of string
                 names of the unipolar channels
-            xyz_2 : ndarray (3, 1)
+            xyz_2 : ndarray (3, )
                 coordinates of the second unipolar channel
         """
 
         log.debug('find electrode that recorded point at {}'
                   .format(point_xyz))
 
         egm_name_bip = ''
         egm_name_uni = ['', '']
-        xyz_2 = np.full((3, 1), np.nan, dtype=np.float32)
+        xyz_2 = np.full(3, np.nan, dtype=np.float32)
 
         channel_number = np.nan
 
         for filename in position_files:
             pos_file = self.parent.parent.repository.join(filename)
             if not self.parent.parent.repository.is_file(pos_file):
                 log.warning('position file {} for point {} not found'
@@ -2390,15 +2544,15 @@
 
         if not egm_name_bip or not any(egm_name_uni):
             log.warning('unable to find which electrode recorded '
                         'point {} at {}!'
                         .format(self.name, point_xyz))
             return ('',
                     ['', ''],
-                    np.full((3, ), np.nan, dtype=np.float32)
+                    np.full(3, np.nan, dtype=np.float32)
                     )
 
         return egm_name_bip, egm_name_uni, xyz_2
 
     @staticmethod
     def _translate_connector_index(channel_list, electrode_index, filename):
         """
```

### Comparing `pyCEPS-0.1.1/pyceps/fileio/cartoutils.py` & `pyCEPS-1.0.0/pyceps/fileio/cartoutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,25 +99,25 @@
             _ = fid.readline()
             # there is one blank line after header
             line = fid.readline().decode(encoding=encoding)
             if line != '\r\n':
                 raise ValueError('unexpected vertices section in Carto3 '
                                  'mesh file')
 
-            verts = np.full((n_verts, 3), np.nan, dtype=float)
-            verts_normals = np.full((n_verts, 3), np.nan, dtype=float)
+            verts = np.full((n_verts, 3), np.nan, dtype=np.single)
+            verts_normals = np.full((n_verts, 3), np.nan, dtype=np.single)
             verts_group_id = np.full((n_verts, 1),
                                      np.iinfo(int).min,
                                      dtype=int)
 
             for i in range(n_verts):
                 line = fid.readline().decode(encoding=encoding)
                 values = line.split('=')[1].split()
-                verts[i, :] = np.array(values[0:3]).astype(float)
-                verts_normals[i, :] = np.array(values[3:6]).astype(float)
+                verts[i, :] = np.array(values[0:3]).astype(np.single)
+                verts_normals[i, :] = np.array(values[3:6]).astype(np.single)
                 verts_group_id[i] = int(values[6])
 
             # next line must be blank
             line = fid.readline().decode(encoding=encoding)
             if line != '\r\n':
                 raise ValueError('unexpected end of vertices section in '
                                  'mesh file')
@@ -621,20 +621,20 @@
 
     # read header information
     col_headers = fid.readline().decode(encoding=encoding).rstrip().split()
     # save current read pos for later
     last_pos = fid.tell()
     if not fid.readline().decode(encoding=encoding):
         # file is empty!
-        return np.array([], dtype=float, ndmin=2), []
+        return np.array([], dtype=np.float32, ndmin=2), []
 
     # reset reading position
     fid.seek(last_pos)
     data = np.loadtxt(fid,
-                      dtype=float,
+                      dtype=np.float32,
                       skiprows=0,
                       ndmin=2,
                       )
 
     return data, col_headers
```

### Comparing `pyCEPS-0.1.1/pyceps/fileio/igb.py` & `pyCEPS-1.0.0/pyceps/fileio/igb.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/fileio/pathtools.py` & `pyCEPS-1.0.0/pyceps/fileio/pathtools.py`

 * *Files 11% similar despite different names*

```diff
@@ -251,14 +251,32 @@
         func1 = getattr(self, self.FUNC_ID.get(type(path)) + 'is_folder')
         func2 = getattr(self, self.FUNC_ID.get(type(path)) + 'is_archive')
         if not func1(path) and not func2(path):
             raise FileExistsError()
 
         self.root = self.build_path(path)
 
+    def get_base_string(self):
+        study_base = self.base
+        if isinstance(self.base, zipfile.Path):
+            study_base = os.path.abspath(self.base.root.filename)
+        if isinstance(self.base, py7zr.SevenZipFile):
+            study_base = os.path.abspath(self.base.filename)
+
+        return study_base
+
+    def get_root_string(self):
+        study_root = self.root
+        if isinstance(self.root, zipfile.Path):
+            study_root = os.path.abspath(self.root.root.filename)
+        if isinstance(self.root, py7zr.SevenZipFile):
+            study_root = os.path.abspath(self.root.filename)
+
+        return study_root
+
     def _path_is_file(self, filepath):
         return os.path.isfile(filepath)
 
     def _zip_is_file(self, filepath):
         return filepath.exists() and filepath.is_file()
 
     def _7z_is_file(self, filepath):
```

### Comparing `pyCEPS-0.1.1/pyceps/fileio/precisionio.py` & `pyCEPS-1.0.0/pyceps/fileio/precisionio.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/fileio/precisionutils.py` & `pyCEPS-1.0.0/pyceps/fileio/precisionutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/fileio/writer.py` & `pyCEPS-1.0.0/pyceps/fileio/writer.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/interpolation.py` & `pyCEPS-1.0.0/pyceps/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/utils.py` & `pyCEPS-1.0.0/pyceps/utils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/visualize/__init__.py` & `pyCEPS-1.0.0/pyceps/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/visualize/colormaps.json` & `pyCEPS-1.0.0/pyceps/visualize/colormaps.json`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/visualize/dashapp.py` & `pyCEPS-1.0.0/pyceps/visualize/dashapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     def update_surface_ecgs(map_name):
         if not study or not map_name:
             return empty_figure(bgnd='rgb(255, 255, 255)')
 
         p_map = [m for m in study.maps.values() if m.name == map_name][0]
 
         return (empty_figure(bgnd='rgb(255, 255, 255)')
-                if not (len(p_map.ecg) > 0)
-                else get_bsecg_figure(p_map.ecg, COLORS))
+                if not (len(p_map.bsecg) > 0)
+                else get_bsecg_figure(p_map.bsecg, COLORS))
 
     @app.callback(
         Output('surface-poly', 'points'),
         Output('surface-poly', 'polys'),
         Output('mapping-points-poly', 'points', allow_duplicate=True),
         Output('mapping-points-selected', 'values', allow_duplicate=True),
         Output('mapping-points-id', 'values', allow_duplicate=True),
```

### Comparing `pyCEPS-0.1.1/pyceps/visualize/dashelements.py` & `pyCEPS-1.0.0/pyceps/visualize/dashelements.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/visualize/dashlayout.py` & `pyCEPS-1.0.0/pyceps/visualize/dashlayout.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/pyceps/visualize/dashutils.py` & `pyCEPS-1.0.0/pyceps/visualize/dashutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-0.1.1/setup.py` & `pyCEPS-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                'openCARP compatible data formats.'
                )
 LICENSE = 'GPLv3+'
 URL = 'https://github.com/medunigraz/pyCEPS'
 EMAIL = 'robert.arnold@medunigraz.at'
 AUTHOR = 'Robert Arnold'
 REQUIRES_PYTHON = '>=3.8'
-VERSION = '0.1.1'
+VERSION = '1.0.0'
 CLASSIFIERS = [
     # Trove classifiers
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

