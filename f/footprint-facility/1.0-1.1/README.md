# Comparing `tmp/footprint_facility-1.0.tar.gz` & `tmp/footprint_facility-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footprint_facility-1.0.tar", last modified: Tue Mar 26 19:27:41 2024, max compression
+gzip compressed data, was "footprint_facility-1.1.tar", last modified: Wed Apr 10 18:35:43 2024, max compression
```

## Comparing `footprint_facility-1.0.tar` & `footprint_facility-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-03-26 19:27:41.212756 footprint_facility-1.0/
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       61 2024-03-25 21:12:39.000000 footprint_facility-1.0/MANIFEST.in
--rw-r--r--   0 pidancier  (1000) pidancier  (1000)    25803 2024-03-26 19:27:41.212756 footprint_facility-1.0/PKG-INFO
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    25291 2024-03-25 21:12:39.000000 footprint_facility-1.0/README.md
-drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-03-26 19:27:41.212756 footprint_facility-1.0/footprint_facility/
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      601 2024-03-26 19:12:34.000000 footprint_facility-1.0/footprint_facility/__init__.py
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      495 2024-03-26 19:27:41.212756 footprint_facility-1.0/footprint_facility/_version.py
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    16405 2024-03-25 21:12:39.000000 footprint_facility-1.0/footprint_facility/footprint_facility.py
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    18748 2024-03-25 21:12:39.000000 footprint_facility-1.0/footprint_facility/test_footprint_facility.py
-drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-03-26 19:27:41.212756 footprint_facility-1.0/footprint_facility.egg-info/
--rw-r--r--   0 pidancier  (1000) pidancier  (1000)    25803 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/PKG-INFO
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      485 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/SOURCES.txt
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)        1 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/dependency_links.txt
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)        1 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/not-zip-safe
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       58 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/requires.txt
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       19 2024-03-26 19:27:41.000000 footprint_facility-1.0/footprint_facility.egg-info/top_level.txt
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      100 2024-03-25 21:12:39.000000 footprint_facility-1.0/pyproject.toml
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       57 2024-03-25 21:12:39.000000 footprint_facility-1.0/requirements.txt
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      824 2024-03-26 19:27:41.212756 footprint_facility-1.0/setup.cfg
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      134 2024-03-25 21:12:39.000000 footprint_facility-1.0/setup.py
--rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    81180 2024-03-25 21:12:39.000000 footprint_facility-1.0/versioneer.py
+drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-04-10 18:35:43.101927 footprint_facility-1.1/
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       61 2024-03-19 16:59:20.000000 footprint_facility-1.1/MANIFEST.in
+-rw-r--r--   0 pidancier  (1000) pidancier  (1000)    31946 2024-04-10 18:35:43.101927 footprint_facility-1.1/PKG-INFO
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    31434 2024-04-10 18:33:16.000000 footprint_facility-1.1/README.md
+drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-04-10 18:35:43.097927 footprint_facility-1.1/footprint_facility/
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      686 2024-04-10 18:33:16.000000 footprint_facility-1.1/footprint_facility/__init__.py
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      495 2024-04-10 18:35:43.105927 footprint_facility-1.1/footprint_facility/_version.py
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    19602 2024-04-10 18:33:16.000000 footprint_facility-1.1/footprint_facility/footprint_facility.py
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    33625 2024-04-10 18:33:16.000000 footprint_facility-1.1/footprint_facility/test_footprint_facility.py
+drwxrwxr-x   0 pidancier  (1000) pidancier  (1000)        0 2024-04-10 18:35:43.101927 footprint_facility-1.1/footprint_facility.egg-info/
+-rw-r--r--   0 pidancier  (1000) pidancier  (1000)    31946 2024-04-10 18:35:43.000000 footprint_facility-1.1/footprint_facility.egg-info/PKG-INFO
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      485 2024-04-10 18:35:43.000000 footprint_facility-1.1/footprint_facility.egg-info/SOURCES.txt
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)        1 2024-04-10 18:35:43.000000 footprint_facility-1.1/footprint_facility.egg-info/dependency_links.txt
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)        1 2024-04-10 18:35:42.000000 footprint_facility-1.1/footprint_facility.egg-info/not-zip-safe
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       58 2024-04-10 18:35:43.000000 footprint_facility-1.1/footprint_facility.egg-info/requires.txt
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       19 2024-04-10 18:35:43.000000 footprint_facility-1.1/footprint_facility.egg-info/top_level.txt
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      100 2024-03-19 16:59:20.000000 footprint_facility-1.1/pyproject.toml
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)       57 2024-04-10 17:21:38.000000 footprint_facility-1.1/requirements.txt
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      824 2024-04-10 18:35:43.105927 footprint_facility-1.1/setup.cfg
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)      134 2024-03-19 16:59:20.000000 footprint_facility-1.1/setup.py
+-rw-rw-r--   0 pidancier  (1000) pidancier  (1000)    81180 2024-03-19 16:59:20.000000 footprint_facility-1.1/versioneer.py
```

### Comparing `footprint_facility-1.0/PKG-INFO` & `footprint_facility-1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,36 @@
-Metadata-Version: 2.1
-Name: footprint_facility
-Version: 1.0
-Summary: Footprint Facility Library
-Author: GAEL Systems
-Author-email: dev@gael.fr
-License: LGPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: pyproj==3.6.1
-Requires-Dist: numpy==1.26.4
-Requires-Dist: shapely==2.0.3
-Requires-Dist: geojson==3.1.0
-
 # Footprint display facility
 
 This set of functions includes a set of facilities to manipulate the footprints to be displayed into leaflet, OpenLayer, MapBox and Cesium.
 
 It manages:
  - Split polygon to multi-polygon when crossing anti-meridian
  - Manage polar area including polar point inside the polygon boundary.
  - Manage long footprints with overlays
  - Manage thin footprints collapsing polygon in a single lineString
 
-# Preliminary installation
+# Preliminary information regrading dependencies
 We recommend the usage of a virtual environment to embed dependencies.
-The dependencies shall be installed before use:
+The dependencies are automatically installed during this module installation:
  - pyproj
  - numpy
  - shapely
  - geojson
 
 Details can be found in [requirements.txt](requirements.txt) file.
 
 ## Library usage
 The `shapely` library provides a set of feature that could be a solution to handle the footprints identified in this study. Unfortunately the library is also concerned by the display issue. For example the intersections operation in shapely fails when footprint contains antimeridian. This later library is mainly used to handle geometries types and formats conversions.  
 Numpy is used to manipulate the list of coordinates to fix the issues caused by lat/lon limits of the geometry.
 
 ## Installation
 ```python
-pip install -r requirements.txt
+pip install footprint-facility
 ```
-
+The module is retrieved from pypi.org service.
 # Available methods
 
 The ```rework_to_polygon_geometry(geometry: Geometry) -> Geometry``` method reworks the geometry parameter to manage polar and antimeridian singularities. This process implements the **Polar inclusive algorithm**. The objective of this algorithm is to add the North/South Pole into the list of coordinates of the polygon at the antimeridian cross.
 
 When the geometry contains the pole the single polygon geometry including the pole in its border point list is properly interpreted by displays systems. When the geometry does not contain the pole, the geometry is split among the antimeridian line.
 
 ```python
@@ -291,32 +274,108 @@
 returns
 
 ```python
 MULTIPOLYGON (
    ((-180 -69.61708714060345, -175.61055 -68.469902, -172.383392 -69.75074, -180 -71.81292858935237, -180 -69.61708714060345)),
    ((175.812988 -70.711365, 180 -69.61708714060345, 180 -71.81292858935237, 178.803558 -72.136864, 175.812988 -70.711365)))
 ```
+## Footprint simplification function
+Products such as "S3 Synergy" contains up to 290 points whereas they footprints are single rectangles. Others huge along track acquisition also contains greate number of coordinates. The footprint containing many points could be simplify improve indexing and display services.   
+This facility module decorates 2 identified algorithms to simplify these footprints:
+- Douglas–Peucker algorithm that is implemented into the shapely geometry library wrapped here as `footprint_facility.simplify`.
+- Convex hull algorithm can be used to reduce de number of points assembly footprint with many polygons. The algorithm is also already implemented in the shapely library.
+
+### The Douglas-Peucker algorithm
+The Douglas-Peucker algorithm is an algorithm that decimates a curve composed of line segments to a similar curve with fewer points. It was one of the earliest successful algorithms developed for cartographic generalization.  
+The purpose of the algorithm is, given a curve composed of line segments, to find a similar curve with fewer points. The algorithm defines 'dissimilar' based on the maximum distance between the original curve and the simplified curve. The simplified curve consists of a subset of the points that defined the original curve.  
+The shapely library used in the footprint_facility module implements this algorithm of simplification. The definition of the distance to be used for the simplification shall be carefully defined to minimize the surface change.
+Code simplification snippet  
+```python
+from footprint_facility import rework_to_polygon_geometry, to_geojson, simplify
+ 
+geometry = rework_to_polygon_geometry(origin_geometry)
+geojson = to_geojson(simplify(geometry, tolerance=0.4))
+ 
+print(geojson)
+```
+
+![img.png](img/img_25.png)
+We observe the algorithm is quite efficient and reduced the larger the number of points between tolerance set between 0.005 and 0.5:
+
+![img_1.png](img/img_26.png)
+The variation of the surface regarding reduction of the number of point is not significant.
+
+#### More Complex footprints
+
+When the footprint crosses antimeridian or pass other the poles, the polygon is not anymore properly supported by the algortihm. it is recommended to systematically manage rework of polygon before performing the simplification.
+
+Example of Footprints crossing antimeridian and pole. The Douglas-Peucker algorithm properly manages this use case when antimeridian case has been previously handled. The pole area (polar inclusion solution) is also well supported:
+
+![img_2.png](img/img_27.png)
+
+The Use case of single footprint crossing antimeridian managed as multi-polygon are also well supported:
+![img_3.png](img/img_28.png)
+
+Sentinel-3 Synergy Data sets identified in the footprint category can be simplified:
+![img_4.png](img/img_29.png)
+Here, the 295 points are well aligned and a distance 0 properly simplifies the polygon.
+
+### The Convex Hull algorithm 
+
+The convex hull is the smallest convex polygon that encloses all points of a geometry. The Sentinel-1 wave-mode images are organized in a list of polygons, and the previously analyzed "Douglas-Peucker" optimization cannot be considered efficient enough to simplify them. The following scheme shows the convex hull (in purple) simplifying the wave-mode images of the set of polygons (in yellow) into a single enclosed polygon.
+
+![img_5.png](img/img_30.png)
+The curvature of the Earth is visible using an algorithm that considers coordinates in a Euclidean reference frame. The algorithm will be improved to support spherical coordinates, but the 2D convex hull used here reduces the number of points by 90%. The convex hull created an envelope that contains all the points of the wave mode without fitting the entire huge envelope (green shape): This algorithm remains a good solution for reducing the number of points to optimize indexing systems.
+
+
+When using the convex hull algorithm with a footprint that crosses the antimeridian, it must be managed before applying the implementation. In the following scheme, the antimeridian is materialized in red and the footprint hull is spread on each side of the red line:
+
+![img_6.png](img/img_31.png)
+
+Code snippett to manage the footprint
+```python
+import shapely
+from footprint_facility import rework_to_polygon_geometry, to_geojson
+ 
+geometry = rework_to_polygon_geometry(origin_geometry)
+ 
+# split eastern/wester part of the polygon
+west_geometry = geometry.intersection(shapely.box(-180, -90, 0, 90))
+east_geometry = geometry.intersection(shapely.box(0, -90, 180, 90))
+ 
+convex_hull = shapely.MultiPolygon([east_geometry.convex_hull, west_geometry.convex_hull])
+print (to_geojson(convex_hull))
+```
+
+### Footprint simplification conclusion
+Reducing the number of points in the EO data footprint can have a positive effect by optimizing the display and faster indexing systems. However, it may introduce inaccuracies in these footprints. For example, using the convex hull algorithm on a Sentinel-1 wave mode can reduce the number of points to 90%, the counterpart is the footprint will cover a larger area than the data.  
+The use of the Douglas-Peucker algorithm is also very efficient and according to the tolerance parameter, the simplified result footprint surface may not shift more than 1%. For example, we demonstrate that S3 SYNERGY products can be completely simplified with 0 tolerance without any surface modification. Other products, in particular long footprints with many points along tracks, can also be simplified by controlling the deviations with the tolerance.
+
 ## Performance management
 The methods are completed with embedded performances metrics capabilities. To activate them, use the following `check_time` method:
 
 ```python
 import footprint_facility 
 footprint_facility.check_time(enable=True,
                               incremental=False,
                               summary_time=True)
 ```
 `enable` parameter to `False` fully deactivate the time management.  
 `incremental` parameter to `True` displays metrics during the execution.  
-`summary_time` parameter to `True` stores metrics for futur display with `footprint_facility.show_summary()`
+`summary_time` parameter to `True` stores metrics for future display with `footprint_facility.show_summary()`
 
 Sample Output:
  ```
-check_cross_antimeridian:	0.64 μs/point
-rework_to_polygon_geometry:	10.35 μs/point
-rework_to_linestring_geometry:	2.36 μs/point
+check_cross_antimeridian:	    0.69 μs/point
+rework_to_polygon_geometry:	    6.94 μs/point
+simplify:	                    1.00 μs/point
+rework_to_linestring_geometry:      2.99 μs/point
  ```
 
 # Known issues
-## footprint support
+## Footprint support
 Very long footprint crossing both the North and the South poles, crossing the antimeridian 3 times (Use-case Number 10) fails to be rendered.
-## polar detection
+## Polar detection
 Detection of the polar point inside the footprint is based on projection transformation within polar stereoscopic projection. Such a transformation cannot be performed on raw footprint that shall manage antimeridian discontinuity.
+## East/West swaths larger that 180
+When eastern distance between consecutive coordinates is longer than 180 and coordinates longitude sign is reverted (e.g. longitudes sequentially -175 then +175), the algorithm uses the smallest area and consider the polygon crossing the antimeridian. 
+To fix this issue, the algorithm shall be upgraded to take into account the clockwise orientation of the coordinates.
```

### Comparing `footprint_facility-1.0/footprint_facility/footprint_facility.py` & `footprint_facility-1.1/footprint_facility/footprint_facility.py`

 * *Files 16% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 
     # When the geometry does not contain pole: Cuts the geometry among the
     # antimeridian line.
     if not _check_contains_pole(reworked):
         reworked = _split_polygon_to_antimeridian(reworked)
     else:
         # Case of footprint crossing equator, antimeridian and polar zone
-        # Split at equator
+        # Split at the equator
         # Warn:
         if check_cross_equator(reworked):
             reworked = _split_polygon_to_equator(reworked)
         # When footprint contains overlapping, it happens at polar location.
         # Polygon containing overlapping are considered invalid in shapely
         # library. It includes validity check and correction methods.
         # The shapely correction method extrude the overlap areas and fails
@@ -391,35 +391,116 @@
             shapely.linestrings(right_antimeridian)])
     else:
         reworked = shapely.linestrings(boundaries)
 
     return reworked
 
 
-def simplify(geometry: Geometry, tolerence=1, preserve_topology=True):
+def _simplify_compute_statistics(geometry, tolerance=.1,
+                                 preserve_topology=True):
+    """
+    Computes the simplified variatiopns statitics:
+     - number of points change
+     - area change
+
+    :param geometry: the geometry to be computed
+    :param tolerance: the ify
+    :param preserve_topology:
+    :return:
+    """
+    origin_area = getattr(geometry, 'area', 0)
+    origin_points_number = len(shapely.get_coordinates(geometry))
+
+    reworked = simplify(geometry, tolerance=tolerance,
+                        preserve_topology=preserve_topology)
+
+    new_area = reworked.area
+    variation_area = (new_area - origin_area) / origin_area
+    new_points_number = len(shapely.get_coordinates(reworked))
+    variation_point = ((new_points_number - origin_points_number) /
+                       origin_points_number)
+
+    return {'tolerance': tolerance,
+            'geometry': reworked,
+            'Area': {"orig": origin_area, "new": new_area,
+                     "variation": variation_area},
+            'Points': {"orig": origin_points_number,
+                       "new": new_points_number,
+                       "variation": variation_point}}
+
+
+def find_best_tolerance_for(geometry,
+                            max_area_percentage_change=1,
+                            min_point_number_reduction_percentage=50):
+    """
+    The Douglas-Peucker based #simplify algorithm requires a tolerance shall
+    be parametrized. The best tolerance value depends on the geometry shape
+    complexity. This method aims to evaluate the best tolerance for a
+    geometry controlling its surface change wrt the reduction of the number of
+    points.
+
+    This method computes statistics by running #symplify method with various
+    tolerance values. It may be time-consuming when expected values greater
+    than 1% of area change and up to 80% of reduced points numbers.
+    :param geometry: the geometry to evaluate
+    :param max_area_percentage_change:  maximum accepted surface modification.
+    :param min_point_number_reduction_percentage: point reduction percentage
+       objective.
+    :return: the tolerance due to the given parameters if parameters cannot
+    be reached, 0 is returned.
+    """
+    min_tolerance = 0.0001
+    max_tolerance = 2.0
+    step = 0.0001
+
+    previous_tolerance = 0
+
+    for tolerance in (map(lambda x: x/10000.0,
+                          range(int(min_tolerance*10000),
+                                int(max_tolerance*10000),
+                                int(step*10000)))):
+        measurement = _simplify_compute_statistics(geometry, tolerance)
+
+        # Checks surface area modification by the algorithm
+        area_var = measurement['Area']['variation']
+        if area_var >= abs(max_area_percentage_change / 100):
+            return previous_tolerance
+
+        # Checks coord number modification by the algorithm
+        point_variation = abs(measurement['Points']['variation'])
+        if point_variation >= abs(min_point_number_reduction_percentage / 100):
+            return previous_tolerance
+
+        previous_tolerance = tolerance
+    return 0
+
+
+@timing
+def simplify(geometry: Geometry, tolerance=.1, preserve_topology=True):
     """
     Returns a simplified representation of the geometric object.
     This method wraps shapely library https://shapely.readthedocs.io/en/
        stable/reference/shapely.simplify.html#shapely.simplify
 
     All points in the simplified object will be within the tolerance distance
-    of the original geometry. By default a slower algorithm is used that
+    of the original geometry. default a slower algorithm is used that
     preserves topology. If preserve topology is set to False the much quicker
     Douglas-Peucker algorithm is used.
 
     :param geometry:
-    :param tolerence: The maximum allowed geometry displacement. The higher
+    :param tolerance: The maximum allowed geometry displacement. The higher
     this value, the smaller the number of vertices in the resulting geometry.
-    :param preserve_topology: By default (True), the operation will avoid
+    :param preserve_topology: default (True), the operation will avoid
     creating invalid geometries (checking for collapses, ring-intersections,
-    etc), but this is computationally more expensive.
+    etc.), but this is computationally more expensive.
     :return:
     """
-    shapely.simplify(shapely.buffer(geometry, 0.0),
-                     tolerence, preserve_topology)
+    return shapely.simplify(
+        shapely.buffer(geometry, 0.0), tolerance=tolerance,
+        preserve_topology=preserve_topology)
 
 
 #############################################################################
 # Utilities for Geometry manipulation
 # - convert to wkt
 # - convert to geojson
 # - build sample disk footprint from its center and radius.
@@ -433,16 +514,16 @@
     """
     return getattr(geometry, "wkt")
 
 
 # Create GeoJSON string from Geometry
 def to_geojson(geometry: Geometry, feature_id=None, properties=None):
     """
-    Convert the geometry to string GeoJSON format. The Id of the feature and
-    its properties can be provided by the caller.
+    Convert the geometry to string GeoJSON format. The identifier of the
+    feature can be provided by the caller as well as the property dictionary.
     :param geometry: the geometry to convert
     :param feature_id: a user defined feature identifier, the identifier will
     be automatically generated if not provided by the user.
     :param properties: a set of property to embed into the feature.
     :return: the GeoJSON string
     """
     if properties is None:
```

### Comparing `footprint_facility-1.0/setup.cfg` & `footprint_facility-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `footprint_facility-1.0/versioneer.py` & `footprint_facility-1.1/versioneer.py`

 * *Files identical despite different names*

