# Comparing `tmp/GRSdriver-1.0.0.tar.gz` & `tmp/GRSdriver-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GRSdriver-1.0.0.tar", last modified: Tue Apr  9 10:33:50 2024, max compression
+gzip compressed data, was "GRSdriver-1.0.1.tar", last modified: Wed Apr 10 17:06:23 2024, max compression
```

## Comparing `GRSdriver-1.0.0.tar` & `GRSdriver-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-09 10:33:50.028164 GRSdriver-1.0.0/
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-09 10:33:50.024164 GRSdriver-1.0.0/GRSdriver/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      170 2024-04-08 16:59:28.000000 GRSdriver-1.0.0/GRSdriver/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    21581 2024-04-08 16:59:28.000000 GRSdriver-1.0.0/GRSdriver/driver_S2_SAFE.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     7659 2024-04-08 16:59:28.000000 GRSdriver-1.0.0/GRSdriver/driver_landsat_col2.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1848 2024-04-09 09:36:03.000000 GRSdriver-1.0.0/GRSdriver/run.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     8095 2024-02-12 15:04:10.000000 GRSdriver-1.0.0/GRSdriver/visual.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-09 10:33:50.028164 GRSdriver-1.0.0/GRSdriver.egg-info/
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15025 2024-04-09 10:33:50.000000 GRSdriver-1.0.0/GRSdriver.egg-info/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      367 2024-04-09 10:33:50.000000 GRSdriver-1.0.0/GRSdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-09 10:33:50.000000 GRSdriver-1.0.0/GRSdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       61 2024-04-09 10:33:50.000000 GRSdriver-1.0.0/GRSdriver.egg-info/requires.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       14 2024-04-09 10:33:50.000000 GRSdriver-1.0.0/GRSdriver.egg-info/top_level.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 GRSdriver-1.0.0/LICENSE
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15025 2024-04-09 10:33:50.028164 GRSdriver-1.0.0/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1274 2024-04-09 09:36:03.000000 GRSdriver-1.0.0/README.md
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      859 2024-04-09 10:33:45.000000 GRSdriver-1.0.0/pyproject.toml
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-09 10:33:50.028164 GRSdriver-1.0.0/rsr/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.0/rsr/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     2754 2024-02-12 15:04:09.000000 GRSdriver-1.0.0/rsr/landsat_formatting.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-09 10:33:50.028164 GRSdriver-1.0.0/setup.cfg
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1313 2024-04-09 10:03:32.000000 GRSdriver-1.0.0/setup.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:06:23.327173 GRSdriver-1.0.1/
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:06:23.327173 GRSdriver-1.0.1/GRSdriver/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)      195 2024-04-10 15:55:56.000000 GRSdriver-1.0.1/GRSdriver/__init__.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    21581 2024-04-08 16:59:28.000000 GRSdriver-1.0.1/GRSdriver/driver_S2_SAFE.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     7659 2024-04-08 16:59:28.000000 GRSdriver-1.0.1/GRSdriver/driver_landsat_col2.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1889 2024-04-10 17:05:28.000000 GRSdriver-1.0.1/GRSdriver/run.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     8096 2024-04-10 11:19:05.000000 GRSdriver-1.0.1/GRSdriver/visual.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:06:23.327173 GRSdriver-1.0.1/GRSdriver.egg-info/
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15498 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)      352 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       50 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/entry_points.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       44 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/requires.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       10 2024-04-10 17:06:23.000000 GRSdriver-1.0.1/GRSdriver.egg-info/top_level.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 GRSdriver-1.0.1/LICENSE
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15498 2024-04-10 17:06:23.327173 GRSdriver-1.0.1/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1777 2024-04-10 11:19:39.000000 GRSdriver-1.0.1/README.md
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1171 2024-04-10 17:02:46.000000 GRSdriver-1.0.1/pyproject.toml
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-10 17:06:23.327173 GRSdriver-1.0.1/setup.cfg
```

### Comparing `GRSdriver-1.0.0/GRSdriver/driver_S2_SAFE.py` & `GRSdriver-1.0.1/GRSdriver/driver_S2_SAFE.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.0/GRSdriver/driver_landsat_col2.py` & `GRSdriver-1.0.1/GRSdriver/driver_landsat_col2.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.0/GRSdriver/run.py` & `GRSdriver-1.0.1/GRSdriver/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-''' Executable to convert Sentinel-2 or Landsat 8/9 L1C images to png format
+'''
+Executable to convert Sentinel-2 or Landsat 8/9 L1C images to png format
 
 Usage:
-  GRSdriver <input_file>  [-o <ofile>] [--odir <odir>] [--rgb_bands ][--resolution res]
-  grs -h | --help
-  grs -v | --version
+  grs_driver <input_file> [--rgb_bands RGB] [-o <ofile>] [--odir <odir>] [--resolution res] [--no_clobber]
+  grs_driver -h | --help
+  grs_driver -v | --version
 
 Options:
   -h --help        Show this screen.
   -v --version     Show version.
 
   <input_file>     Input file to be processed
 
   -o ofile         Full (absolute or relative) path to output L2 image.
   --odir odir      Ouput directory [default: ./]
-  --no_clobber     Do not process <input_file> if <output_file> already exists.
+  --rgb_bands=RGB  band number to be used in RGB [default: '4,3,1']
+
   --resolution=res  spatial resolution of the scene pixels
-  --rgb_bands R,G,B  band number to be used in RGB [default: 4,3,1]
+  --no_clobber     Do not process <input_file> if <output_file> already exists.
 
 '''
 
 import os, sys
 from docopt import docopt
 import numpy as np
 import logging
-from . import __package__, __version__
+from GRSdriver import __package__, __version__
 
 
 def main():
+
     args = docopt(__doc__, version=__package__ + '_' + __version__)
     print(args)
 
     file = args['<input_file>']
 
     resolution = int(args['--resolution'])
-    R,G,B = np.array(args['--rgb_bands'])
+    RGB = np.array(args['--rgb_bands'])
     noclobber = args['--no_clobber']
 
     ##################################
     # File naming convention
     ##################################
 
     outfile = args['-o']
```

### Comparing `GRSdriver-1.0.0/GRSdriver/visual.py` & `GRSdriver-1.0.1/GRSdriver/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 # mpl.use('TkAgg')
-import hvplot.xarray
+#import hvplot.xarray
 
 import holoviews as hv
 import holoviews.operation.datashader as hd
 from holoviews.operation.datashader import rasterize, shade, spread
 from holoviews.element.tiles import EsriImagery
 from holoviews.element import tiles as hvts
 from holoviews import opts
```

### Comparing `GRSdriver-1.0.0/GRSdriver.egg-info/PKG-INFO` & `GRSdriver-1.0.1/GRSdriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.0
-Summary: Driver for L1C satellite image dedicated to GRS processor
-Home-page: 
-Author: T. Harmel
+Version: 1.0.1
+Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,22 +202,21 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/Tristanovsk/GRSdriver
-Keywords: driver,EO satellite
+Keywords: Sentinel-2,Landsat-8,Landsat-9,driver,EO satellite
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eoreader>=0.21.1
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -227,15 +224,28 @@
 
 # GRSdriver package
 ## Driver dedicated to load and prepare data for the GRS processor
 - Tool for easy loading of Sentinel-2 L1C SAFE format with accurate computation of the viewing angles
 - Applicable to Landsat 8 and 9
 - Visualization tools
 
-### Installation
+## Installation
+
+### Usual installation
+```commandline
+conda install -c conda-forge gdal
+pip install GRSdriver
+```
+
+If you have no GDAL implementation yet, please une anaconda environment and install GDAL before GRSdriver:
+```commandline
+conda install -c conda-forge gdal
+```
+
+### Installation from GRSdriver repository (enables use of the notebook and visualization tools)
 1. First clone the repository:
 ```commandline
 git clone https://github.com/Tristanovsk/GRSdriver.git
 ```
 
 2.a. You may duplicate the conda environment (optional)
 ```commandline
@@ -246,24 +256,28 @@
 ```commandline
 conda install -c conda-forge gdal
 ```
 
 3. Install GRSdriver
 ```commandline
 conda activate grssuite
+conda install -c pyviz holoviews panel
 pip install .
 ```
-You are done.
 
-### Usual installation
+4. Install and configure JupyterLab and Holoviews
 ```commandline
-conda install -c conda-forge gdal
-pip install .
+pip install holoviews datashader
+conda install -c conda-forge jupyterlab
+jupyter labextension install @pyviz/jupyterlab_pyviz
 ```
 
+You are done.
+
+
 ## Example
 
 ![example gif](docs/_static/s2driver_visual_tool_optimized.gif)
 
 
 ## 2D-fitting method for angle computation
```

### Comparing `GRSdriver-1.0.0/LICENSE` & `GRSdriver-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.0/PKG-INFO` & `GRSdriver-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.0
-Summary: Driver for L1C satellite image dedicated to GRS processor
-Home-page: 
-Author: T. Harmel
+Version: 1.0.1
+Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,22 +202,21 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/Tristanovsk/GRSdriver
-Keywords: driver,EO satellite
+Keywords: Sentinel-2,Landsat-8,Landsat-9,driver,EO satellite
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: eoreader>=0.21.1
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
@@ -227,15 +224,28 @@
 
 # GRSdriver package
 ## Driver dedicated to load and prepare data for the GRS processor
 - Tool for easy loading of Sentinel-2 L1C SAFE format with accurate computation of the viewing angles
 - Applicable to Landsat 8 and 9
 - Visualization tools
 
-### Installation
+## Installation
+
+### Usual installation
+```commandline
+conda install -c conda-forge gdal
+pip install GRSdriver
+```
+
+If you have no GDAL implementation yet, please une anaconda environment and install GDAL before GRSdriver:
+```commandline
+conda install -c conda-forge gdal
+```
+
+### Installation from GRSdriver repository (enables use of the notebook and visualization tools)
 1. First clone the repository:
 ```commandline
 git clone https://github.com/Tristanovsk/GRSdriver.git
 ```
 
 2.a. You may duplicate the conda environment (optional)
 ```commandline
@@ -246,24 +256,28 @@
 ```commandline
 conda install -c conda-forge gdal
 ```
 
 3. Install GRSdriver
 ```commandline
 conda activate grssuite
+conda install -c pyviz holoviews panel
 pip install .
 ```
-You are done.
 
-### Usual installation
+4. Install and configure JupyterLab and Holoviews
 ```commandline
-conda install -c conda-forge gdal
-pip install .
+pip install holoviews datashader
+conda install -c conda-forge jupyterlab
+jupyter labextension install @pyviz/jupyterlab_pyviz
 ```
 
+You are done.
+
+
 ## Example
 
 ![example gif](docs/_static/s2driver_visual_tool_optimized.gif)
 
 
 ## 2D-fitting method for angle computation
```

### Comparing `GRSdriver-1.0.0/README.md` & `GRSdriver-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,28 @@
 
 # GRSdriver package
 ## Driver dedicated to load and prepare data for the GRS processor
 - Tool for easy loading of Sentinel-2 L1C SAFE format with accurate computation of the viewing angles
 - Applicable to Landsat 8 and 9
 - Visualization tools
 
-### Installation
+## Installation
+
+### Usual installation
+```commandline
+conda install -c conda-forge gdal
+pip install GRSdriver
+```
+
+If you have no GDAL implementation yet, please une anaconda environment and install GDAL before GRSdriver:
+```commandline
+conda install -c conda-forge gdal
+```
+
+### Installation from GRSdriver repository (enables use of the notebook and visualization tools)
 1. First clone the repository:
 ```commandline
 git clone https://github.com/Tristanovsk/GRSdriver.git
 ```
 
 2.a. You may duplicate the conda environment (optional)
 ```commandline
@@ -21,24 +34,28 @@
 ```commandline
 conda install -c conda-forge gdal
 ```
 
 3. Install GRSdriver
 ```commandline
 conda activate grssuite
+conda install -c pyviz holoviews panel
 pip install .
 ```
-You are done.
 
-### Usual installation
+4. Install and configure JupyterLab and Holoviews
 ```commandline
-conda install -c conda-forge gdal
-pip install .
+pip install holoviews datashader
+conda install -c conda-forge jupyterlab
+jupyter labextension install @pyviz/jupyterlab_pyviz
 ```
 
+You are done.
+
+
 ## Example
 
 ![example gif](docs/_static/s2driver_visual_tool_optimized.gif)
 
 
 ## 2D-fitting method for angle computation
```

