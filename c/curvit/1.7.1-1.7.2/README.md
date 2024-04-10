# Comparing `tmp/curvit-1.7.1.tar.gz` & `tmp/curvit-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.7.1.tar", last modified: Thu Feb 15 14:00:57 2024, max compression
+gzip compressed data, was "curvit-1.7.2.tar", last modified: Wed Apr 10 07:43:25 2024, max compression
```

## Comparing `curvit-1.7.1.tar` & `curvit-1.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-02-15 14:00:57.717325 curvit-1.7.1/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.7.1/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1817 2024-02-15 14:00:57.717325 curvit-1.7.1/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.7.1/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-02-15 14:00:57.715325 curvit-1.7.1/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.7.1/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.7.1/curvit/check_curvit_variability_V.0.4.py
--rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    78005 2024-02-15 13:47:39.000000 curvit-1.7.1/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.7.1/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.7.1/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-02-15 14:00:57.716325 curvit-1.7.1/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1817 2024-02-15 14:00:57.000000 curvit-1.7.1/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2024-02-15 14:00:57.000000 curvit-1.7.1/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2024-02-15 14:00:57.000000 curvit-1.7.1/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2024-02-15 14:00:57.000000 curvit-1.7.1/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2024-02-15 14:00:57.000000 curvit-1.7.1/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2024-02-15 14:00:57.717325 curvit-1.7.1/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      847 2024-02-15 13:28:36.000000 curvit-1.7.1/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-10 07:43:25.935258 curvit-1.7.2/
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.7.2/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1815 2024-04-10 07:43:25.934258 curvit-1.7.2/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1182 2024-04-10 06:49:20.000000 curvit-1.7.2/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-10 07:43:25.869257 curvit-1.7.2/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.7.2/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.7.2/curvit/check_curvit_variability_V.0.4.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)    78443 2024-04-10 06:47:04.000000 curvit-1.7.2/curvit/curvit.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.7.2/curvit/profile_curvit.py
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.7.2/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2024-04-10 07:43:25.934258 curvit-1.7.2/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1815 2024-04-10 07:43:25.000000 curvit-1.7.2/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2024-04-10 07:43:25.000000 curvit-1.7.2/curvit.egg-info/SOURCES.txt
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)        1 2024-04-10 07:43:25.000000 curvit-1.7.2/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2024-04-10 07:43:25.000000 curvit-1.7.2/curvit.egg-info/requires.txt
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)        7 2024-04-10 07:43:25.000000 curvit-1.7.2/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2024-04-10 07:43:25.935258 curvit-1.7.2/setup.cfg
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      847 2024-04-10 06:49:02.000000 curvit-1.7.2/setup.py
```

### Comparing `curvit-1.7.1/LICENSE` & `curvit-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.7.1/PKG-INFO` & `curvit-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.7.1
+Version: 1.7.2
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 <a href="https://ascl.net/2101.013"><img src="https://img.shields.io/badge/ascl-2101.013-blue.svg?colorB=262255" alt="ascl:2101.013" /></a>
 <a href="https://pypi.org/project/curvit/"><img src="https://img.shields.io/pypi/v/curvit?color=262255"/></a>
 [![Documentation Status](https://readthedocs.org/projects/curvit/badge/?version=latest)](https://curvit.readthedocs.io/en/latest/?badge=latest)
 
 ### **Curvit documention is at https://curvit.readthedocs.io**
 
 
-Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.  
+Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.
 
 The software paper manuscript is accessible at https://arxiv.org/abs/2101.06377
 
 ## Installation
 
 Curvit is on the Python Package Index (PyPI) and you can install the package using [pip](https://pip.pypa.io/en/stable/) as follows:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.7.1 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.7.2 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: matplotlib Requires-Dist: astropy Requires-Dist: photutils
 Requires-Dist: scipy Requires-Dist: scikit-image Requires-Dist: aafitrans
```

### Comparing `curvit-1.7.1/README.md` & `curvit-1.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <a href="https://ascl.net/2101.013"><img src="https://img.shields.io/badge/ascl-2101.013-blue.svg?colorB=262255" alt="ascl:2101.013" /></a>
 <a href="https://pypi.org/project/curvit/"><img src="https://img.shields.io/pypi/v/curvit?color=262255"/></a>
 [![Documentation Status](https://readthedocs.org/projects/curvit/badge/?version=latest)](https://curvit.readthedocs.io/en/latest/?badge=latest)
 
 ### **Curvit documention is at https://curvit.readthedocs.io**
 
 
-Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.  
+Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.
 
 The software paper manuscript is accessible at https://arxiv.org/abs/2101.06377
 
 ## Installation
 
 Curvit is on the Python Package Index (PyPI) and you can install the package using [pip](https://pip.pypa.io/en/stable/) as follows:
```

### Comparing `curvit-1.7.1/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.7.2/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.7.1/curvit/curvit.py` & `curvit-1.7.2/curvit/curvit.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,14 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License."""
 
 
-import matplotlib
-
-# Force matplotlib to not use any Xwindows backend.
-matplotlib.use("Agg")
-
 import os
 import sys
 import ntpath
 import random
 import numpy as np
 import matplotlib.pyplot as plt
 
@@ -370,15 +365,20 @@
 
     obj_fx = fx[mask]
     obj_fy = fy[mask]
 
     obj_circle = plt.Circle((pos_x, pos_y), cir_rad, color="k", fill=False)
 
     plt.hist2d(obj_fx, obj_fy, bins=sub_size * 2, norm=LogNorm())
+    plt.tick_params(axis="both", labelsize=15)
+    plt.title("radius = %spx" % (cir_rad), fontsize=15)
     plt.gcf().gca().add_artist(obj_circle)
+    cbar = plt.colorbar()
+    cbar.ax.tick_params(labelsize=15)
+    cbar.set_label("Counts", fontsize=15)
     source_png_name = os.path.join(path_to_events_list, sub_name + events_list + ".png")
     plt.savefig(source_png_name, format="png", bbox_inches="tight")
     plt.clf()
     return source_png_name
 
 
 # To find positions of interest (using daofind algorithm).
@@ -723,15 +723,15 @@
         return
 
     coo_file = os.path.join(path_to_events_list, "sources_" + events_list + ".coo")
     np.savetxt(coo_file, uA, fmt="%4.2f\t%4.2f")
     print("\nDetected source coordinates saved in file:\n* {}".format(coo_file))
 
     # To automatically choose background region.
-    plt.figure(figsize=(10.5, 10))
+    plt.figure(figsize=(12.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
             fx,
             fy,
             time,
             photons,
             radius,
@@ -739,16 +739,18 @@
             sky_radius,
             ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
-
-    plt.tick_params(axis="both", labelsize=fontsize)
+    plt.tick_params(axis="both", labelsize=15)
+    cbar = plt.colorbar()
+    cbar.ax.tick_params(labelsize=15)
+    cbar.set_label("Counts", fontsize=15)
 
     for u in uA:
         plt.annotate("Source", u, size=13, color="black", fontweight="bold")
 
         obj_circle = plt.Circle(u, 100, color="k", fill=False)
         plt.gcf().gca().add_artist(obj_circle)
 
@@ -838,15 +840,15 @@
         T = met_to_mjd(T)
 
         plt.title(
             "X = %s, Y = %s, bin = %ss, radius = %spx" % (xp, yp, bwidth, radius),
             fontsize=fontsize,
         )
 
-        plt.xlabel("Time (Julian Date)", fontsize=fontsize)
+        plt.xlabel("Time (modified Julian date)", fontsize=fontsize)
         plt.ylabel("Counts per second", fontsize=fontsize)
         plt.tick_params(axis="both", labelsize=fontsize)
 
         weighted_counts, bin_edges = np.histogram(
             T, bins=nbin, range=(time_start, till_here), weights=W
         )
 
@@ -1028,15 +1030,15 @@
 
     ::
 
         Background CPS (scaled to aperture area): 0.02155 ± 0.00425
 
         -------------------------- curve --------------------------
         source: source_2636.71_907.91_AS1G06_084T01_9000000710uvtFIIPC00F1_l2ce.png
-                source_zoomed__2636.71_907.91_AS1G06_084T01_9000000710uvtFIIPC00F1_l2ce.png
+                source_zoomed_2636.71_907.91_AS1G06_084T01_9000000710uvtFIIPC00F1_l2ce.png
         data: curve_2636.71_907.91_AS1G06_084T01_9000000710uvtFIIPC00F1_l2ce.dat
         plot: curve_2636.71_907.91_AS1G06_084T01_9000000710uvtFIIPC00F1_l2ce.png
 
         Done!
 
     """
 
@@ -1063,15 +1065,15 @@
     if sanity < 1:
         return
 
     path_to_events_list, events_list = ntpath.split(events_list)
     events_list = modify_string(events_list)
 
     # To automatically choose background region.
-    plt.figure(figsize=(10.5, 10))
+    plt.figure(figsize=(12.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
             fx,
             fy,
             time,
             photons,
             radius,
@@ -1079,16 +1081,18 @@
             sky_radius,
             ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
-
-    plt.tick_params(axis="both", labelsize=fontsize)
+    plt.tick_params(axis="both", labelsize=15)
+    cbar = plt.colorbar()
+    cbar.ax.tick_params(labelsize=15)
+    cbar.set_label("Counts", fontsize=15)
 
     plt.annotate("Source", (xp, yp), size=13, color="black", fontweight="bold")
 
     obj_circle = plt.Circle((xp, yp), 100, color="k", fill=False)
     plt.gcf().gca().add_artist(obj_circle)
 
     if background == "manual":
@@ -1174,15 +1178,15 @@
     till_here = met_to_mjd(till_here)
     time_start = met_to_mjd(time.min())
     unique_time = met_to_mjd(unique_time)
 
     # Binning stuff, plotting stuff.
     plt.figure(figsize=(8, 5))
     plt.title("bin = %ss, radius = %spx" % (bwidth, radius), fontsize=fontsize)
-    plt.xlabel("Time (Julian Date)", fontsize=fontsize)
+    plt.xlabel("Time (modified Julian Date)", fontsize=fontsize)
     plt.ylabel("Counts per second", fontsize=fontsize)
     plt.tick_params(axis="both", labelsize=fontsize)
 
     u_counts, u_bin_edges = np.histogram(
         unique_time, bins=nbin, range=(time_start, till_here)
     )
 
@@ -1406,15 +1410,15 @@
     if sanity < 1:
         return
 
     path_to_events_list, events_list = ntpath.split(events_list)
     events_list = modify_string(events_list)
 
     # To automatically choose background region.
-    plt.figure(figsize=(10.5, 10))
+    plt.figure(figsize=(12.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
             fx,
             fy,
             time,
             photons,
             radius,
@@ -1422,16 +1426,18 @@
             sky_radius,
             ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
-
-    plt.tick_params(axis="both", labelsize=fontsize)
+    plt.tick_params(axis="both", labelsize=15)
+    cbar = plt.colorbar()
+    cbar.ax.tick_params(labelsize=15)
+    cbar.set_label("Counts", fontsize=15)
 
     plt.annotate("Source", (xp, yp), size=13, color="black", fontweight="bold")
 
     obj_circle = plt.Circle((xp, yp), 100, color="k", fill=False)
     plt.gcf().gca().add_artist(obj_circle)
 
     if background == "manual":
@@ -1535,15 +1541,15 @@
 
     time_start = ranges[0]
     till_here = ranges[-1]
 
     # Binning stuff, plotting stuff.
     plt.figure(figsize=(8, 5))
     plt.title("radius = %spx" % (radius), fontsize=fontsize)
-    plt.xlabel("Time (Julian Date)", fontsize=fontsize)
+    plt.xlabel("Time (modified Julian Date)", fontsize=fontsize)
     plt.ylabel("Counts per second", fontsize=fontsize)
     plt.tick_params(axis="both", labelsize=fontsize)
 
     u_counts, u_bin_edges = np.histogram(
         unique_time,
         bins=ranges,
     )
```

### Comparing `curvit-1.7.1/curvit/test_curvit.py` & `curvit-1.7.2/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.7.1/curvit.egg-info/PKG-INFO` & `curvit-1.7.2/curvit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.7.1
+Version: 1.7.2
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 <a href="https://ascl.net/2101.013"><img src="https://img.shields.io/badge/ascl-2101.013-blue.svg?colorB=262255" alt="ascl:2101.013" /></a>
 <a href="https://pypi.org/project/curvit/"><img src="https://img.shields.io/pypi/v/curvit?color=262255"/></a>
 [![Documentation Status](https://readthedocs.org/projects/curvit/badge/?version=latest)](https://curvit.readthedocs.io/en/latest/?badge=latest)
 
 ### **Curvit documention is at https://curvit.readthedocs.io**
 
 
-Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.  
+Curvit is an open-source python package to generate light curves from UVIT (Ultraviolet Imaging Telescope) data.
 
 The software paper manuscript is accessible at https://arxiv.org/abs/2101.06377
 
 ## Installation
 
 Curvit is on the Python Package Index (PyPI) and you can install the package using [pip](https://pip.pypa.io/en/stable/) as follows:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.7.1 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.7.2 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: matplotlib Requires-Dist: astropy Requires-Dist: photutils
 Requires-Dist: scipy Requires-Dist: scikit-image Requires-Dist: aafitrans
```

### Comparing `curvit-1.7.1/setup.py` & `curvit-1.7.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit",
-    version="1.7.1",
+    version="1.7.2",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```

