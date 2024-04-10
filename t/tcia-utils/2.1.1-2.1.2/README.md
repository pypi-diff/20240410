# Comparing `tmp/tcia_utils-2.1.1.tar.gz` & `tmp/tcia_utils-2.1.2.tar.gz`

## Comparing `tcia_utils-2.1.1.tar` & `tcia_utils-2.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    87232 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/utils.py
--rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/wordpress.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/LICENSE
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    87292 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/src/tcia_utils/wordpress.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tcia_utils-2.1.2/PKG-INFO
```

### Comparing `tcia_utils-2.1.1/src/tcia_utils/datacite.py` & `tcia_utils-2.1.2/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/src/tcia_utils/nbia.py` & `tcia_utils-2.1.2/src/tcia_utils/nbia.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 from enum import Enum
 import matplotlib
 import matplotlib.pyplot as plt
 import plotly.express as px
 import pydicom
 import pydicom_seg
 import rt_utils
-import tkinter
-from tkinter import filedialog
 import numpy as np
 from ipywidgets import interact
 from tcia_utils.utils import searchDf
 from tcia_utils.utils import format_disk_space
 from tcia_utils.utils import remove_html_tags
 from tcia_utils.datacite import getDoi
+try:
+    import tkinter
+    from tkinter import filedialog
+except ModuleNotFoundError:
+    tkinter = None
 
 
 class StopExecution(Exception):
     def _render_traceback_(self):
         pass
```

### Comparing `tcia_utils-2.1.1/src/tcia_utils/pathdb.py` & `tcia_utils-2.1.2/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/src/tcia_utils/utils.py` & `tcia_utils-2.1.2/src/tcia_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/src/tcia_utils/wordpress.py` & `tcia_utils-2.1.2/src/tcia_utils/wordpress.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/.gitignore` & `tcia_utils-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/LICENSE` & `tcia_utils-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/README.md` & `tcia_utils-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.1/pyproject.toml` & `tcia_utils-2.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "2.1.1"
+version = "2.1.2"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-2.1.1/PKG-INFO` & `tcia_utils-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tcia_utils
-Version: 2.1.1
+Version: 2.1.2
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

