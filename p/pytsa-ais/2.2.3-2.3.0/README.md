# Comparing `tmp/pytsa_ais-2.2.3.tar.gz` & `tmp/pytsa_ais-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsa_ais-2.2.3.tar", max compression
+gzip compressed data, was "pytsa_ais-2.3.0.tar", max compression
```

## Comparing `pytsa_ais-2.2.3.tar` & `pytsa_ais-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.2.3/LICENSE
--rw-r--r--   0        0        0    15712 2024-02-06 12:03:47.000000 pytsa_ais-2.2.3/README.md
--rw-r--r--   0        0        0      952 2024-04-09 07:39:55.675188 pytsa_ais-2.2.3/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-09 07:40:03.575188 pytsa_ais-2.2.3/pytsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.2.3/pytsa/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.2.3/pytsa/data/geometry/__init__.py
--rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/denmark.json
--rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/germany.json
--rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/netherlands_detailed.json
--rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/norway.json
--rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.2.3/pytsa/data/geometry/sweden.json
--rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/__init__.py
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/diffquants.pkl
--rw-r--r--   0        0        0     8159 2024-01-18 12:40:18.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/dquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/hquants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/squants.pkl
--rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.2.3/pytsa/data/quantiles/tquants.pkl
--rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.2.3/pytsa/decoder/__init__.py
--rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.2.3/pytsa/decoder/ais_decoder.py
--rw-r--r--   0        0        0     1548 2024-01-30 09:17:11.000000 pytsa_ais-2.2.3/pytsa/decoder/filedescriptor.py
--rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.2.3/pytsa/logger.py
--rw-r--r--   0        0        0     5956 2024-02-09 15:42:47.000000 pytsa_ais-2.2.3/pytsa/structs.py
--rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.2.3/pytsa/trajectories/__init__.py
--rw-r--r--   0        0        0     7490 2024-04-09 07:08:59.835206 pytsa_ais-2.2.3/pytsa/trajectories/inspect.py
--rw-r--r--   0        0        0     4236 2024-02-09 14:01:06.000000 pytsa_ais-2.2.3/pytsa/trajectories/rules.py
--rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.2.3/pytsa/tsea/__init__.py
--rw-r--r--   0        0        0    28174 2024-03-19 09:36:35.324947 pytsa_ais-2.2.3/pytsa/tsea/search_agent.py
--rw-r--r--   0        0        0     5336 2024-04-08 10:43:36.000000 pytsa_ais-2.2.3/pytsa/tsea/split.py
--rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.2.3/pytsa/tsea/targetship.py
--rw-r--r--   0        0        0    13571 2024-04-03 18:48:40.000000 pytsa_ais-2.2.3/pytsa/utils.py
--rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.2.3/pytsa/visualization/__init__.py
--rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.2.3/pytsa/visualization/ecdf.py
--rw-r--r--   0        0        0    13488 2024-04-02 10:43:50.989572 pytsa_ais-2.2.3/pytsa/visualization/misc.py
--rw-r--r--   0        0        0    16725 1970-01-01 00:00:00.000000 pytsa_ais-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.0/LICENSE
+-rw-r--r--   0        0        0    15712 2024-02-06 12:03:47.000000 pytsa_ais-2.3.0/README.md
+-rw-r--r--   0        0        0      952 2024-04-10 08:15:06.583351 pytsa_ais-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-10 08:15:13.299351 pytsa_ais-2.3.0/pytsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.0/pytsa/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.0/pytsa/data/geometry/__init__.py
+-rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/denmark.json
+-rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/germany.json
+-rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/netherlands_detailed.json
+-rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/norway.json
+-rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.0/pytsa/data/geometry/sweden.json
+-rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/__init__.py
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/diffquants.pkl
+-rw-r--r--   0        0        0     8159 2024-01-18 12:40:18.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/dquants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/hquants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/squants.pkl
+-rw-r--r--   0        0        0     8159 2023-12-04 07:09:51.000000 pytsa_ais-2.3.0/pytsa/data/quantiles/tquants.pkl
+-rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.0/pytsa/decoder/__init__.py
+-rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.0/pytsa/decoder/ais_decoder.py
+-rw-r--r--   0        0        0     1548 2024-01-30 09:17:11.000000 pytsa_ais-2.3.0/pytsa/decoder/filedescriptor.py
+-rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.0/pytsa/logger.py
+-rw-r--r--   0        0        0     5956 2024-02-09 15:42:47.000000 pytsa_ais-2.3.0/pytsa/structs.py
+-rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.0/pytsa/trajectories/__init__.py
+-rw-r--r--   0        0        0     7561 2024-04-09 11:43:49.471049 pytsa_ais-2.3.0/pytsa/trajectories/inspect.py
+-rw-r--r--   0        0        0     5072 2024-04-10 08:13:27.591352 pytsa_ais-2.3.0/pytsa/trajectories/rules.py
+-rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.0/pytsa/tsea/__init__.py
+-rw-r--r--   0        0        0    28174 2024-03-19 09:36:35.324947 pytsa_ais-2.3.0/pytsa/tsea/search_agent.py
+-rw-r--r--   0        0        0     5336 2024-04-08 10:43:36.000000 pytsa_ais-2.3.0/pytsa/tsea/split.py
+-rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.0/pytsa/tsea/targetship.py
+-rw-r--r--   0        0        0    13571 2024-04-03 18:48:40.000000 pytsa_ais-2.3.0/pytsa/utils.py
+-rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.0/pytsa/visualization/__init__.py
+-rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.0/pytsa/visualization/ecdf.py
+-rw-r--r--   0        0        0    13488 2024-04-02 10:43:50.989572 pytsa_ais-2.3.0/pytsa/visualization/misc.py
+-rw-r--r--   0        0        0    16725 1970-01-01 00:00:00.000000 pytsa_ais-2.3.0/PKG-INFO
```

### Comparing `pytsa_ais-2.2.3/LICENSE` & `pytsa_ais-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/README.md` & `pytsa_ais-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pyproject.toml` & `pytsa_ais-2.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytsa-ais"
-version = "2.2.3"
+version = "2.3.0"
 description = "Toolbox for extracting trajectories and monitoring vessels from raw AIS records."
 authors = ["Niklas Paulig <niklas.paulig@tu-dresden.de>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytsa_ais-2.2.3/pytsa/data/geometry/denmark.json` & `pytsa_ais-2.3.0/pytsa/data/geometry/denmark.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/geometry/germany.json` & `pytsa_ais-2.3.0/pytsa/data/geometry/germany.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/geometry/netherlands_detailed.json` & `pytsa_ais-2.3.0/pytsa/data/geometry/netherlands_detailed.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/geometry/norway.json` & `pytsa_ais-2.3.0/pytsa/data/geometry/norway.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/geometry/sweden.json` & `pytsa_ais-2.3.0/pytsa/data/geometry/sweden.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/quantiles/diffquants.pkl` & `pytsa_ais-2.3.0/pytsa/data/quantiles/diffquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/quantiles/dquants.pkl` & `pytsa_ais-2.3.0/pytsa/data/quantiles/dquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/quantiles/hquants.pkl` & `pytsa_ais-2.3.0/pytsa/data/quantiles/hquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/quantiles/squants.pkl` & `pytsa_ais-2.3.0/pytsa/data/quantiles/squants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/data/quantiles/tquants.pkl` & `pytsa_ais-2.3.0/pytsa/data/quantiles/tquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/decoder/ais_decoder.py` & `pytsa_ais-2.3.0/pytsa/decoder/ais_decoder.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/decoder/filedescriptor.py` & `pytsa_ais-2.3.0/pytsa/decoder/filedescriptor.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/logger.py` & `pytsa_ais-2.3.0/pytsa/logger.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/structs.py` & `pytsa_ais-2.3.0/pytsa/structs.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/trajectories/inspect.py` & `pytsa_ais-2.3.0/pytsa/trajectories/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     """
     Return the angle between the track
     of three AIS Messages.
     """
     _cos = cosine_of_angle_between(track)        
     return np.arccos(np.round(_cos,6)) # Round to avoid floating point errors
     
-def average_smoothness(track: Track) -> float:
+def average_smoothness(track: Track, tau: int = 1) -> float:
     """
     Calculate the average smoothness of a navigational 
     track.
 
     This function computes the average smoothness of a 
     path represented  by a list of AISMessage objects.  
     It evaluates the smoothness based on the angles 
@@ -192,16 +192,17 @@
 
     Note:
     - The function assumes that the track has at least three 
        AISMessage points to form at least one angle. If the 
        track has fewer than three points, the behavior of the 
        function is unspecified.
     """
+    assert tau > 0, "Tau must be a positive integer."
     if len(track) < 3:
         raise ValueError(
             "Average smoothness requires at "
             "least three messages per track. "
             "{} were given".format(len(track))
         )
     angles = angle_between(track)
-    normalized_angles = (angles / np.pi)**2
+    normalized_angles = (angles / np.pi)**tau
     return np.mean(normalized_angles)
```

### Comparing `pytsa_ais-2.2.3/pytsa/trajectories/rules.py` & `pytsa_ais-2.3.0/pytsa/trajectories/rules.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,18 +26,21 @@
     # Cook the recipe
     cooked = recipe.cook()
     
 The `cooked` function can now be passed to the TrajectorySplitter class
 to perform the trajectory splitting.
 
 """
-from typing import Callable
+import utm
 import numpy as np
+
+from typing import Callable
 from inspect import signature
 from functools import partial
+from scipy.spatial import ConvexHull
 
 from ..structs import Track
 
 class Recipe:
     """
     Rule recipe class.
     =================
@@ -97,34 +100,56 @@
 def spatial_deviation(track: Track, sd: tuple | float) -> bool:
     """
     Return True if the summed standard deviation of lat/lon 
     of the track of the given vessel is smaller than `sd`,
     or if `sd` is a tuple, if the standard deviation is
     within the range of `sd`.
     Unit of `sd` is [°].
+
+    Note that the standard deviation is no accurate measure
+    of the spatial deviation, as it does not take into account
+    the actual distances between the points. It is only a
+    rough measure of the spread of the points.
+    Accuracy decreases rapidly with proximity to the poles.
+
+    (Not used in the paper)
     """
     assert isinstance(sd,(tuple,float))
     if isinstance(sd,float):
         assert sd > 0
         lower, upper = 0, sd
     else:
         assert all(s > 0 for s in sd)
         lower, upper = sd
-    sdlon = np.sqrt(np.var([v.lon for v in track]))
-    sdlat = np.sqrt(np.var([v.lat for v in track]))
+    sdlon = np.std([v.lon for v in track])
+    sdlat = np.std([v.lat for v in track])
     return lower <= sdlon + sdlat <= upper
 
 def too_small_span(track: Track, span: float) -> bool:
     """
     Return True if the lateral and longitudinal span
     of the track of the given vessel is smaller than `span`.
     (Not used in the paper)
     """
     lat_span = np.ptp([v.lat for v in track])
     lon_span = np.ptp([v.lon for v in track])
     return lat_span > span and lon_span > span
 
+def convex_hull_area(track: Track, area: float) -> bool:
+    """
+    Return True if the area of the convex hull of the
+    track of the given vessel is smaller than `area`.
+    (Not used in the paper)
+    """
+    assert len(track) > 2, "Need at least 3 points to calculate convex hull"
+    res = utm.from_latlon(
+        np.array([p.lat for p in track]),
+        np.array([p.lon for p in track])
+    )
+    points = np.array([res[0],res[1]]).T
+    return ConvexHull(points).area < area
+
 # Example recipe---------------------------------------------------------------
 ExampleRecipe = Recipe(
     partial(too_few_obs, n=100),
-    partial(spatial_deviation, sd=0.1)
+    partial(convex_hull_area, area=3e4)
 )
```

### Comparing `pytsa_ais-2.2.3/pytsa/tsea/__init__.py` & `pytsa_ais-2.3.0/pytsa/tsea/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/tsea/search_agent.py` & `pytsa_ais-2.3.0/pytsa/tsea/search_agent.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/tsea/split.py` & `pytsa_ais-2.3.0/pytsa/tsea/split.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/tsea/targetship.py` & `pytsa_ais-2.3.0/pytsa/tsea/targetship.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/utils.py` & `pytsa_ais-2.3.0/pytsa/utils.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/visualization/__init__.py` & `pytsa_ais-2.3.0/pytsa/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/visualization/ecdf.py` & `pytsa_ais-2.3.0/pytsa/visualization/ecdf.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/pytsa/visualization/misc.py` & `pytsa_ais-2.3.0/pytsa/visualization/misc.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.2.3/PKG-INFO` & `pytsa_ais-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytsa-ais
-Version: 2.2.3
+Version: 2.3.0
 Summary: Toolbox for extracting trajectories and monitoring vessels from raw AIS records.
 Author: Niklas Paulig
 Author-email: niklas.paulig@tu-dresden.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

