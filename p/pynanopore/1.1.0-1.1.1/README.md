# Comparing `tmp/pynanopore-1.1.0.tar.gz` & `tmp/pynanopore-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanopore-1.1.0.tar", last modified: Fri Nov  3 21:12:38 2023, max compression
+gzip compressed data, was "pynanopore-1.1.1.tar", last modified: Wed Apr 10 09:19:44 2024, max compression
```

## Comparing `pynanopore-1.1.0.tar` & `pynanopore-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:12:38.776968 pynanopore-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-11-03 21:12:38.776968 pynanopore-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-11-03 21:11:46.000000 pynanopore-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:12:38.772968 pynanopore-1.1.0/pynanopore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 21:11:46.000000 pynanopore-1.1.0/pynanopore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2023-11-03 21:11:46.000000 pynanopore-1.1.0/pynanopore/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2023-11-03 21:11:46.000000 pynanopore-1.1.0/pynanopore/dwelltime.py
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2023-11-03 21:11:46.000000 pynanopore-1.1.0/pynanopore/event_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-11-03 21:11:46.000000 pynanopore-1.1.0/pynanopore/powerspectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 21:12:38.776968 pynanopore-1.1.0/pynanopore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-11-03 21:12:38.000000 pynanopore-1.1.0/pynanopore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-11-03 21:12:38.000000 pynanopore-1.1.0/pynanopore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 21:12:38.000000 pynanopore-1.1.0/pynanopore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-03 21:12:38.000000 pynanopore-1.1.0/pynanopore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-03 21:12:38.000000 pynanopore-1.1.0/pynanopore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 21:12:38.776968 pynanopore-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-11-03 21:11:46.000000 pynanopore-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:44.272649 pynanopore-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-10 09:19:44.272649 pynanopore-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 09:19:09.000000 pynanopore-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:44.268649 pynanopore-1.1.1/pynanopore/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 09:19:09.000000 pynanopore-1.1.1/pynanopore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-10 09:19:09.000000 pynanopore-1.1.1/pynanopore/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-10 09:19:09.000000 pynanopore-1.1.1/pynanopore/dwelltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-04-10 09:19:09.000000 pynanopore-1.1.1/pynanopore/event_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-10 09:19:09.000000 pynanopore-1.1.1/pynanopore/powerspectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:19:44.272649 pynanopore-1.1.1/pynanopore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-10 09:19:44.000000 pynanopore-1.1.1/pynanopore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 09:19:44.000000 pynanopore-1.1.1/pynanopore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:19:44.000000 pynanopore-1.1.1/pynanopore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 09:19:44.000000 pynanopore-1.1.1/pynanopore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 09:19:44.000000 pynanopore-1.1.1/pynanopore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:19:44.272649 pynanopore-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-10 09:19:09.000000 pynanopore-1.1.1/setup.py
```

### Comparing `pynanopore-1.1.0/PKG-INFO` & `pynanopore-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanopore
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/jaybfn/Single-Molecule-Electrophysiology-Data-Analysis
 Author: Jayesh Arun Bafna
 Author-email: jayesh.bfn@gmail.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -13,9 +13,9 @@
 
 Pynanopore serves as a sophisticated toolkit for analyzing single molecules, designed to interpret complex states within nanopore data automatically. It accomplishes this by constructing a virtual representation of the nanopore mechanism using an electrical circuit analogy. This approach capitalizes on the initial electrical changes that occur when a molecule passes through the nanopore to measure the interactions between the pore and the molecule accurately.
 
 Tiny pores on the nanometer scale have shown promising applications in the field of biotechnology, with uses ranging from DNA sequencing to measuring forces at the single-molecule level, and even in identifying molecules by mass on a one-by-one basis. The sophisticated data analysis and modeling techniques provided by Pynanopore are key to significantly enhancing the accuracy of measuring how molecules engage with these nanopores in all these high-tech applications.
 
 
 
-### more info comming soon!!!!
-### this app is still under development!
+#### more info comming soon!!!!
+#### this app is still under development!
```

### Comparing `pynanopore-1.1.0/README.md` & `pynanopore-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 
 Pynanopore serves as a sophisticated toolkit for analyzing single molecules, designed to interpret complex states within nanopore data automatically. It accomplishes this by constructing a virtual representation of the nanopore mechanism using an electrical circuit analogy. This approach capitalizes on the initial electrical changes that occur when a molecule passes through the nanopore to measure the interactions between the pore and the molecule accurately.
 
 Tiny pores on the nanometer scale have shown promising applications in the field of biotechnology, with uses ranging from DNA sequencing to measuring forces at the single-molecule level, and even in identifying molecules by mass on a one-by-one basis. The sophisticated data analysis and modeling techniques provided by Pynanopore are key to significantly enhancing the accuracy of measuring how molecules engage with these nanopores in all these high-tech applications.
 
 
 
-### more info comming soon!!!!
-### this app is still under development!
+#### more info comming soon!!!!
+#### this app is still under development!
```

### Comparing `pynanopore-1.1.0/pynanopore/app.py` & `pynanopore-1.1.1/pynanopore/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 import plotly.graph_objects as go
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import os
 import pyabf
 
-
-# from event_detection import ReadingData, CreatingChunks, EventDetection, Plotting 
-# from powerspectrum import PSDAnalyzer, LorentzianFitter
-# from dwelltime import DwellTime_ExponentialFit
-
 from pynanopore.event_detection import ReadingData, CreatingChunks, EventDetection, Plotting 
 from pynanopore.powerspectrum import PSDAnalyzer, LorentzianFitter
 from pynanopore.dwelltime import DwellTime_ExponentialFit
 
 # Function to load and process your data
 def process_data(file_path):
     reader = ReadingData(file_path)
```

### Comparing `pynanopore-1.1.0/pynanopore/dwelltime.py` & `pynanopore-1.1.1/pynanopore/dwelltime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 import plotly.graph_objects as go
-#from event_detection import ReadingData, CreatingChunks, EventDetection, Plotting 
-from pynanopore.event_detection import ReadingData, CreatingChunks, EventDetection, Plotting 
+from pynanopore import ReadingData, CreatingChunks, EventDetection, Plotting 
 
 class DwellTime_ExponentialFit:
     def __init__(self, events_df: pd.DataFrame, bins: int = 250) -> None:
         """Initialize the ExponentialFit class."""
         self.events_df = events_df
         self.bins = bins
         self.hist, self.bin_centers = self._prepare_histogram()
```

### Comparing `pynanopore-1.1.0/pynanopore/event_detection.py` & `pynanopore-1.1.1/pynanopore/event_detection.py`

 * *Files identical despite different names*

### Comparing `pynanopore-1.1.0/pynanopore/powerspectrum.py` & `pynanopore-1.1.1/pynanopore/powerspectrum.py`

 * *Files identical despite different names*

### Comparing `pynanopore-1.1.0/pynanopore.egg-info/PKG-INFO` & `pynanopore-1.1.1/pynanopore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanopore
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/jaybfn/Single-Molecule-Electrophysiology-Data-Analysis
 Author: Jayesh Arun Bafna
 Author-email: jayesh.bfn@gmail.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -13,9 +13,9 @@
 
 Pynanopore serves as a sophisticated toolkit for analyzing single molecules, designed to interpret complex states within nanopore data automatically. It accomplishes this by constructing a virtual representation of the nanopore mechanism using an electrical circuit analogy. This approach capitalizes on the initial electrical changes that occur when a molecule passes through the nanopore to measure the interactions between the pore and the molecule accurately.
 
 Tiny pores on the nanometer scale have shown promising applications in the field of biotechnology, with uses ranging from DNA sequencing to measuring forces at the single-molecule level, and even in identifying molecules by mass on a one-by-one basis. The sophisticated data analysis and modeling techniques provided by Pynanopore are key to significantly enhancing the accuracy of measuring how molecules engage with these nanopores in all these high-tech applications.
 
 
 
-### more info comming soon!!!!
-### this app is still under development!
+#### more info comming soon!!!!
+#### this app is still under development!
```

### Comparing `pynanopore-1.1.0/setup.py` & `pynanopore-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(
     name="pynanopore",
-    version="1.1.0",
+    version="1.1.1",
     packages=['pynanopore'],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url= "https://github.com/jaybfn/Single-Molecule-Electrophysiology-Data-Analysis",
     author = "Jayesh Arun Bafna",
     author_email = "jayesh.bfn@gmail.com",
     license= "MIT",
```

