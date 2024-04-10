# Comparing `tmp/icon_uxarray-0.1.6.tar.gz` & `tmp/icon_uxarray-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icon_uxarray-0.1.6.tar", last modified: Tue Apr  9 15:36:01 2024, max compression
+gzip compressed data, was "icon_uxarray-0.1.7.tar", last modified: Wed Apr 10 06:25:44 2024, max compression
```

## Comparing `icon_uxarray-0.1.6.tar` & `icon_uxarray-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.915298 icon_uxarray-0.1.6/icon_uxarray/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/icon_uxarray/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/icon_uxarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:36:01.000000 icon_uxarray-0.1.6/icon_uxarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:36:01.919298 icon_uxarray-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/Torus_Triangles_100m_x_100m_res5m.nc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 15:35:53.000000 icon_uxarray-0.1.6/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:25:44.318743 icon_uxarray-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-10 06:25:44.318743 icon_uxarray-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:25:44.314743 icon_uxarray-0.1.7/icon_uxarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/icon_uxarray/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/icon_uxarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/icon_uxarray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/icon_uxarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/icon_uxarray/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:25:44.318743 icon_uxarray-0.1.7/icon_uxarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 06:25:44.000000 icon_uxarray-0.1.7/icon_uxarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 06:25:44.318743 icon_uxarray-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 06:25:44.318743 icon_uxarray-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   414674 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/tests/Torus_Triangles_100m_x_100m_res5m.nc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-10 06:25:31.000000 icon_uxarray-0.1.7/tests/test_base.py
```

### Comparing `icon_uxarray-0.1.6/HISTORY.md` & `icon_uxarray-0.1.7/HISTORY.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Lines too long in conftest. [Jacopo]
+- Stop testing on winzoz, xarray does not seem to close files properly.
+  [Jacopo]
+- Double quotes. [Jacopo]
+- Configure tests in vscode. [Jacopo]
+- I did not understand how to reset properly. [Jacopo]
+- Add environment variable to disable HDF5 file locking to try and fix
+  winzoz issues. [Jacopo]
+- Forgot to delete one line. [Jacopo]
+- Try context manager and copy. [Jacopo]
+- Try closing xarray dataset and cleaning up after tests. [Jacopo]
+- Add test for file overwriting in test_icon_grid_2_ugrid() [Jacopo]
+
+
+0.1.6 (2024-04-09)
+------------------
+- Release: version 0.1.6 🚀 [Jacopo]
 - Add base module to top level. [Jacopo]
 - Fix package name in installation command. [Jacopo]
 
 
 0.1.5 (2024-04-09)
 ------------------
 - Release: version 0.1.5 🚀 [Jacopo]
```

### Comparing `icon_uxarray-0.1.6/LICENSE` & `icon_uxarray-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.6/PKG-INFO` & `icon_uxarray-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.6
+Version: 0.1.7
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.6/README.md` & `icon_uxarray-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.6/icon_uxarray/base.py` & `icon_uxarray-0.1.7/icon_uxarray/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     ugrid_fname = os.path.join(
         os.path.dirname(icon_grid_fname),
         "ux_" + os.path.basename(icon_grid_fname),
     )
     if os.path.isfile(ugrid_fname):
         os.remove(ugrid_fname)
     xr_grid.to_netcdf(ugrid_fname, mode="w", format="NETCDF4")
+    xr_grid.close()
 
     return ugrid_fname
 
 
 # ==============================================================================
 def is_boundary_triangle(grid: ux.Grid, itri: int, lims: list[float]) -> bool:
     """
```

### Comparing `icon_uxarray-0.1.6/icon_uxarray/cli.py` & `icon_uxarray-0.1.7/icon_uxarray/cli.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.6/icon_uxarray.egg-info/PKG-INFO` & `icon_uxarray-0.1.7/icon_uxarray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icon_uxarray
-Version: 0.1.6
+Version: 0.1.7
 Summary: Awesome icon_uxarray created by jcanton
 Home-page: https://github.com/jcanton/icon_uxarray/
 Author: jcanton
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `icon_uxarray-0.1.6/setup.py` & `icon_uxarray-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.6/tests/Torus_Triangles_100m_x_100m_res5m.nc` & `icon_uxarray-0.1.7/tests/Torus_Triangles_100m_x_100m_res5m.nc`

 * *Files identical despite different names*

### Comparing `icon_uxarray-0.1.6/tests/test_base.py` & `icon_uxarray-0.1.7/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,20 @@
     assert ugrid.mesh.face_coordinates == "clon clat"
     assert ugrid.mesh.face_node_connectivity == "vertex_of_cell"
     assert ugrid.mesh.edge_node_connectivity == "edge_vertices"
     assert ugrid.mesh.face_edge_connectivity == "edge_of_cell"
     assert ugrid.mesh.face_face_connectivity == "neighbor_cell_index"
     assert ugrid.mesh.edge_face_connectivity == "adjacent_cell_of_edge"
 
-    # # Clean up the temporary files
-    # os.remove(ugrid_fname)
+    # test file overwriting
+    ugrid_fname = icon_grid_2_ugrid(ICON_GRID_FNAME)
+    assert os.path.isfile(ugrid_fname)
+
+    # Clean up the temporary files
+    os.remove(ugrid_fname)
 
 
 def test_is_boundary_triangle():
     """
     Test case for the is_boundary_triangle function.
 
     This function tests the behavior of the is_boundary_triangle function by
@@ -92,16 +96,16 @@
         218, 219, 220, 222, 223, 245, 246, 247, 248, 254, 255, 273, 274, 275,
         276, 286, 287, 301, 302, 303, 304, 318, 319, 329, 330, 331, 332, 350,
         351, 357, 358, 359, 360, 382, 383, 384, 385, 386, 387, 388, 414, 415
         ]
 
     assert face_ids == expected
 
-    # # Clean up the temporary files
-    # os.remove(ugrid_fname)
+    # Clean up the temporary files
+    os.remove(ugrid_fname)
 
 
 def test_remove_torus_boundaries():
     """
     Test function for removing torus boundary triangles from a UX grid or
     dataset.
     """
@@ -138,7 +142,10 @@
     assert float(result.temperature.min()) == 0.0
     assert float(result.temperature.max()) == 413
 
     # Test with invalid grid
     invalid_grid = None
     with pytest.raises(Exception) as e_info:
         remove_torus_boundaries(invalid_grid)
+
+    # Clean up the temporary files
+    os.remove(ugrid_fname)
```

