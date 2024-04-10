# Comparing `tmp/extremitypathfinder-2.7.1.tar.gz` & `tmp/extremitypathfinder-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extremitypathfinder-2.7.1.tar", max compression
+gzip compressed data, was "extremitypathfinder-2.7.2.tar", max compression
```

## Comparing `extremitypathfinder-2.7.1.tar` & `extremitypathfinder-2.7.2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0      200 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/.editorconfig
--rw-r--r--   0        0        0     2043 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     5082 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/CHANGELOG.rst
--rw-r--r--   0        0        0     3091 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1056 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/LICENSE
--rw-r--r--   0        0        0      772 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/Makefile
--rw-r--r--   0        0        0     2532 2023-06-16 21:50:49.078368 extremitypathfinder-2.7.1/README.rst
--rw-r--r--   0        0        0      574 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/example.json
--rw-r--r--   0        0        0      132 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/command_line.py
--rw-r--r--   0        0        0      198 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/configs.py
--rw-r--r--   0        0        0    14841 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/extremitypathfinder.py
--rw-r--r--   0        0        0      833 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/numba_replacements.py
--rw-r--r--   0        0        0     6902 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/plotting.py
--rw-r--r--   0        0        0      379 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/types.py
--rw-r--r--   0        0        0    43344 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/utils.py
--rw-r--r--   0        0        0     8673 2023-06-16 21:50:49.090368 extremitypathfinder-2.7.1/extremitypathfinder/utils_numba.py
--rw-r--r--   0        0        0     2082 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/__init__.py
--rw-r--r--   0        0        0      580 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/cli_test.py
--rwxr-xr-x   0        0        0     7211 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/helper_fcts_test.py
--rwxr-xr-x   0        0        0      839 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/helpers.py
--rwxr-xr-x   0        0        0     7351 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/main_test.py
--rw-r--r--   0        0        0    10817 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/test_cases.py
--rw-r--r--   0        0        0    12624 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tests/test_find_visible.py
--rwxr-xr-x   0        0        0      499 2023-06-16 21:50:49.094368 extremitypathfinder-2.7.1/tox.ini
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 extremitypathfinder-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/.editorconfig
+-rw-r--r--   0        0        0     1901 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     5316 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     3091 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1056 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/LICENSE
+-rw-r--r--   0        0        0      944 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/Makefile
+-rw-r--r--   0        0        0     2532 2024-04-10 10:08:25.807036 extremitypathfinder-2.7.2/README.rst
+-rw-r--r--   0        0        0      574 2024-04-10 10:08:25.815037 extremitypathfinder-2.7.2/example.json
+-rw-r--r--   0        0        0      132 2024-04-10 10:08:25.815037 extremitypathfinder-2.7.2/extremitypathfinder/__init__.py
+-rw-r--r--   0        0        0     2234 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/command_line.py
+-rw-r--r--   0        0        0      198 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/configs.py
+-rw-r--r--   0        0        0    15153 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/extremitypathfinder.py
+-rw-r--r--   0        0        0      832 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/numba_replacements.py
+-rw-r--r--   0        0        0     6966 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/plotting.py
+-rw-r--r--   0        0        0      379 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/types.py
+-rw-r--r--   0        0        0    43882 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/utils.py
+-rw-r--r--   0        0        0     8679 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/extremitypathfinder/utils_numba.py
+-rw-r--r--   0        0        0     3158 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/__init__.py
+-rw-r--r--   0        0        0      580 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/cli_test.py
+-rwxr-xr-x   0        0        0     7239 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/helper_fcts_test.py
+-rwxr-xr-x   0        0        0      913 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/helpers.py
+-rwxr-xr-x   0        0        0     7459 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/main_test.py
+-rw-r--r--   0        0        0    10773 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/test_cases.py
+-rw-r--r--   0        0        0    12827 2024-04-10 10:08:25.819037 extremitypathfinder-2.7.2/tests/test_find_visible.py
+-rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 extremitypathfinder-2.7.2/PKG-INFO
```

### Comparing `extremitypathfinder-2.7.1/.pre-commit-config.yaml` & `extremitypathfinder-2.7.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-ast  # Is it valid Python?
       - id: debug-statements # no debbuging statements used
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
@@ -15,36 +15,30 @@
         args: [ "--autofix" ]
       - id: check-merge-conflict
       - id: check-docstring-first
       - id: requirements-txt-fixer
       #            -   id: detect-aws-credentials
       - id: detect-private-key
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5
     hooks:
-      - id: isort
-        args: [ "--profile", "black", "--filter-files" ]
-
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
-        language_version: python3
-        args:
-          - --line-length=120
+      # linter.
+      - id: ruff
+        args: [ --fix ]
+      - id: ruff-format
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [ black ]
 
   - repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
+    rev: 7.0.0
     hooks:
       - id: flake8
         exclude: ^(docs|scripts|tests)/
         # E203 whitespace before ':'
         args:
           - --max-line-length=120
           - --ignore=E203
@@ -57,15 +51,15 @@
     rev: "0.49"
     hooks:
       - id: check-manifest
         args: [ "--no-build-isolation", "--ignore",  "*.png,docs/*,publish.py,readthedocs.yml,poetry.lock,setup.py,scripts/*" ]
         additional_dependencies: [ numpy, poetry>=1.4 ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
 
 # TODO enable for very detailed linting:
 #    -   repo: https://github.com/pycqa/pylint
 #        rev: pylint-2.6.0
 #        hooks:
```

### Comparing `extremitypathfinder-2.7.1/CHANGELOG.rst` & `extremitypathfinder-2.7.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changelog
 =========
 
+
+2.7.2 (2024-04-10)
+-------------------
+
+- added support for python 3.12
+
+internal:
+
+- added tests for python 3.12
+- use ruff pre-commit hooks
+- made dependency groups docs and plot optional
+- added tox tes for documentation build
+
+
+
 2.7.1 (2023-05-16)
 -------------------
 
 internal:
 
 - JIT compile more utility functions (including numpy.linalg.solve)
 - add scipy dependency for JIT compiling numpy.linalg.solve
```

### Comparing `extremitypathfinder-2.7.1/CONTRIBUTING.rst` & `extremitypathfinder-2.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/LICENSE` & `extremitypathfinder-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/Makefile` & `extremitypathfinder-2.7.2/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
+# NOTE: install the package itselt to make the CLI commands available (required for the tests)
 install:
 	@echo "installing the development dependencies..."
-	@poetry install --all-extras
+	@poetry install --all-extras --sync --with dev,docs,plot
 	@#poetry install --no-dev
 
 
 update:
 	@echo "updating the dependencies pinned in 'pyproject.toml':"
 	@poetry update -vvv
 	#poetry export -f requirements.txt --output docs/requirements.txt --without-hashes
 
 lock:
 	@echo "pinning the dependencies in 'pyproject.toml':"
 	@poetry lock -vvv
 
 
 test:
-	#pytest
-	@tox
+	poetry run pytest
+
+tox:
+	@poetry run tox
 
 hook:
 	@pre-commit install
 	@pre-commit run --all-files
 
-hook2:
+hookup:
 	@pre-commit autoupdate
+	@pre-commit install
 
 clean:
 	rm -rf .pytest_cache .coverage coverage.xml tests/__pycache__ .mypyp_cache/ .tox
 
 
 build:
 	poetry build
```

### Comparing `extremitypathfinder-2.7.1/README.rst` & `extremitypathfinder-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/example.json` & `extremitypathfinder-2.7.2/example.json`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/command_line.py` & `extremitypathfinder-2.7.2/extremitypathfinder/command_line.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/extremitypathfinder.py` & `extremitypathfinder-2.7.2/extremitypathfinder/extremitypathfinder.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 import networkx as nx
 import numpy as np
 
 from extremitypathfinder import configs
 from extremitypathfinder import types as t
 from extremitypathfinder import utils
 from extremitypathfinder.configs import DEFAULT_PICKLE_NAME
-from extremitypathfinder.types import InputCoord, InputCoordList, Length, ObstacleIterator, Path
+from extremitypathfinder.types import (
+    InputCoord,
+    InputCoordList,
+    Length,
+    ObstacleIterator,
+    Path,
+)
 
 
 class PolygonEnvironment:
     """Class allowing to use polygons to represent "2D environments" and use them for path finding.
 
     Keeps a "loaded" and prepared environment for consecutive path queries.
     Internally uses a visibility graph optimised for shortest path finding.
@@ -28,15 +34,17 @@
     nr_edges: int
     prepared: bool = False
     holes: List[np.ndarray]
     extremity_indices: np.ndarray
     reprs_n_distances: Dict[int, np.ndarray]
     graph: t.Graph
     # TODO
-    temp_graph: Optional[t.Graph] = None  # for storing and plotting the graph during a query
+    temp_graph: Optional[t.Graph] = (
+        None  # for storing and plotting the graph during a query
+    )
     boundary_polygon: np.ndarray
     coords: np.ndarray
     edge_vertex_idxs: np.ndarray
     extremity_mask: np.ndarray
     vertex_edge_idxs: np.ndarray
 
     @property
@@ -76,35 +84,42 @@
 
         :raises AssertionError: when validate=True and the input is invalid.
         """
         self.prepared = False
         # loading the map
         boundary_coordinates = np.array(boundary_coordinates, dtype=configs.DTYPE_FLOAT)
         list_of_hole_coordinates = [
-            np.array(hole_coords, dtype=configs.DTYPE_FLOAT) for hole_coords in list_of_hole_coordinates
+            np.array(hole_coords, dtype=configs.DTYPE_FLOAT)
+            for hole_coords in list_of_hole_coordinates
         ]
         if validate:
-            utils.check_data_requirements(boundary_coordinates, list_of_hole_coordinates)
+            utils.check_data_requirements(
+                boundary_coordinates, list_of_hole_coordinates
+            )
 
         # Note: independent copy!
         self.holes = list_of_hole_coordinates
         self.boundary_polygon = boundary_coordinates
 
         # TODO redundant data. refactor all functions to only use one format
         (
             self.coords,
             self.extremity_indices,
             self.extremity_mask,
             self.vertex_edge_idxs,
             self.edge_vertex_idxs,
-        ) = utils.compile_polygon_datastructs(boundary_coordinates, list_of_hole_coordinates)
+        ) = utils.compile_polygon_datastructs(
+            boundary_coordinates, list_of_hole_coordinates
+        )
 
         nr_total_pts = self.edge_vertex_idxs.shape[0]
         self.nr_vertices = nr_total_pts
-        self.reprs_n_distances = utils.cmp_reps_n_distance_dict(self.coords, self.extremity_indices)
+        self.reprs_n_distances = utils.cmp_reps_n_distance_dict(
+            self.coords, self.extremity_indices
+        )
 
         # start and goal points will be stored after all polygon coordinates
         self.idx_start = nr_total_pts
         self.idx_goal = nr_total_pts + 1
 
         self.prepare()
 
@@ -156,15 +171,17 @@
 
         .. note::
             Pre computing the shortest paths between all directly reachable extremities
             and storing them in the graph would not be an advantage, because then the graph is fully connected.
             A* would visit every node in the graph at least once (-> disadvantage!).
         """
         if self.prepared:  # idempotent
-            warnings.warn("called .prepare() on already prepared map. skipping...", stacklevel=1)
+            warnings.warn(
+                "called .prepare() on already prepared map. skipping...", stacklevel=1
+            )
             return
 
         self.graph = utils.compute_graph(
             self.nr_edges,
             self.extremity_indices,
             self.reprs_n_distances,
             self.coords,
@@ -251,15 +268,17 @@
         # the visibility of only the graph nodes has to be checked (not all extremities!)
         # IMPORTANT: also check if the start node is visible from the goal node!
         candidate_idxs: Set[int] = set(self.graph.nodes)
         candidate_idxs.add(start)
         repr_n_dists = utils.cmp_reps_n_distances(origin, coords)
         self.reprs_n_distances[origin] = repr_n_dists
         vert_idx2repr, vert_idx2dist = repr_n_dists
-        visibles_goal = self.get_visible_idxs(origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist)
+        visibles_goal = self.get_visible_idxs(
+            origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist
+        )
         if len(visibles_goal) == 0:
             # The goal node does not have any neighbours. Hence there is not possible path to the goal.
             return [], None
 
         # IMPORTANT geometrical property of this problem: it is always shortest to directly reach a node
         #   instead of visiting other nodes first (there is never an advantage through reduced edge weight)
         # -> when goal is directly reachable, there can be no other shorter path to it. Terminate
@@ -284,40 +303,51 @@
 
         origin = start
         # the visibility of only the graphs nodes have to be checked
         # the goal node does not have to be considered, because of the earlier check
         repr_n_dists = utils.cmp_reps_n_distances(origin, coords)
         self.reprs_n_distances[origin] = repr_n_dists
         vert_idx2repr, vert_idx2dist = repr_n_dists
-        visibles_start = self.get_visible_idxs(origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist)
+        visibles_start = self.get_visible_idxs(
+            origin, candidate_idxs, coords, vert_idx2repr, vert_idx2dist
+        )
 
         if len(visibles_start) == 0:
             # The start node does not have any neighbours. Hence there is no possible path to the goal.
             return [], None
 
         # add edges: start <-> extremity (i)
         for i in visibles_start:
             graph.add_edge(start, i, weight=vert_idx2dist[i])
 
         # apply mapping to start and goal index as well
-        start_mapped = utils.find_identical_single(start, graph.nodes, self.reprs_n_distances)
+        start_mapped = utils.find_identical_single(
+            start, graph.nodes, self.reprs_n_distances
+        )
         if start_mapped != start:
             nx.relabel_nodes(graph, {start: start_mapped}, copy=False)
 
-        goal_mapped = utils.find_identical_single(goal, graph.nodes, self.reprs_n_distances)
+        goal_mapped = utils.find_identical_single(
+            goal, graph.nodes, self.reprs_n_distances
+        )
         if goal_mapped != goal_mapped:
             nx.relabel_nodes(graph, {goal: goal_mapped}, copy=False)
 
-        self._idx_start_tmp, self._idx_goal_tmp = start_mapped, goal_mapped  # for plotting
+        self._idx_start_tmp, self._idx_goal_tmp = (
+            start_mapped,
+            goal_mapped,
+        )  # for plotting
 
         def l2_distance(n1, n2):
             return utils.get_distance(n1, n2, self.reprs_n_distances)
 
         try:
-            id_path = nx.astar_path(graph, start_mapped, goal_mapped, heuristic=l2_distance, weight="weight")
+            id_path = nx.astar_path(
+                graph, start_mapped, goal_mapped, heuristic=l2_distance, weight="weight"
+            )
         except nx.exception.NetworkXNoPath:
             return [], None
 
         # clean up
         # TODO re-use the same graph. need to keep track of all merged edges
         # if start_mapped == start:
         #     graph.remove_node(start)
```

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/numba_replacements.py` & `extremitypathfinder-2.7.2/extremitypathfinder/numba_replacements.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" 'transparent' numba functionality replacements
+"""'transparent' numba functionality replacements
 
 njit decorator
 data types
 
 dtype_2int_tuple = typeof((1, 1))
 @njit(b1(i4, i4, i4[:, :]), cache=True)
 @njit(dtype_2int_tuple(f8, f8), cache=True)
```

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/plotting.py` & `extremitypathfinder-2.7.2/extremitypathfinder/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 SHOW_PLOTS = False
 PLOTTING_DIR = "all_plots"
 PLOT_FILE_ENDING = ".svg"
 
 
 def get_plot_name(file_name="plot"):
-    return abspath(join(PLOTTING_DIR, file_name + "_" + str(time.time())[:-7] + PLOT_FILE_ENDING))
+    return abspath(
+        join(PLOTTING_DIR, file_name + "_" + str(time.time())[:-7] + PLOT_FILE_ENDING)
+    )
 
 
 def export_plot(fig, file_name):
     fig.set_size_inches(EXPORT_SIZE_X, EXPORT_SIZE_Y, forward=True)
     plt.savefig(get_plot_name(file_name), dpi=EXPORT_RESOLUTION)
     plt.close()
 
@@ -208,37 +210,40 @@
 
 class PlottingEnvironment(PolygonEnvironment):
     """Extends PolygonEnvironment. In addition to the base functionality it
     plots graphs of the polygons, the visibility graph and the computed path.
     Stores all graphs in the folder defined by plotting_dir parameter."""
 
     def __init__(self, plotting_dir=PLOTTING_DIR):
-        super().__init__()
         global PLOTTING_DIR
         PLOTTING_DIR = plotting_dir
         if not exists(plotting_dir):
             makedirs(plotting_dir)
+        super().__init__()
 
     def store(self, *args, **kwargs):
         """In addition to storing, also plots a graph of the input polygons."""
         super().store(*args, **kwargs)
         draw_loaded_map(self)
 
     def prepare(self):
         """Also draws a prepared map with the computed visibility graph."""
+        super().prepare()
         draw_prepared_map(self)
 
     def find_shortest_path(self, start_coordinates, goal_coordinates, *args, **kwargs):
         """Also draws the computed shortest path."""
         # important to not delete the temp graph! for plotting
         vertex_path, distance = super().find_shortest_path(
             start_coordinates, goal_coordinates, *args, free_space_after=False, **kwargs
         )
 
         draw_only_path(self, vertex_path, start_coordinates, goal_coordinates)
-        if self.temp_graph:  # in some cases (e.g. direct path possible) no graph is being created!
+        if (
+            self.temp_graph
+        ):  # in some cases (e.g. direct path possible) no graph is being created!
             draw_graph(self, self.temp_graph)
             draw_with_path(self, self.temp_graph, vertex_path)
             del self.temp_graph  # free the memory
 
         # extract the coordinates from the path
         return vertex_path, distance
```

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/utils.py` & `extremitypathfinder-2.7.2/extremitypathfinder/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 import networkx as nx
 import numpy as np
 import numpy.linalg
 
 from extremitypathfinder import configs
 from extremitypathfinder import types as t
-from extremitypathfinder.configs import BOUNDARY_JSON_KEY, DEFAULT_PICKLE_NAME, HOLES_JSON_KEY
+from extremitypathfinder.configs import (
+    BOUNDARY_JSON_KEY,
+    DEFAULT_PICKLE_NAME,
+    HOLES_JSON_KEY,
+)
 from extremitypathfinder.utils_numba import (
     _angle_rep_inverse,
     _compute_repr_n_dist,
     _fill_edge_vertex_idxs,
     _fill_extremity_mask,
     _has_clockwise_numbering,
     _inside_polygon,
@@ -22,26 +26,34 @@
     _no_identical_consequent_vertices,
 )
 
 
 def cmp_reps_n_distances(orig_idx: int, coords: np.ndarray) -> np.ndarray:
     coords_orig = coords[orig_idx]
     coords_translated = coords - coords_orig
-    repr_n_dists = np.apply_along_axis(_compute_repr_n_dist, axis=1, arr=coords_translated)
+    repr_n_dists = np.apply_along_axis(
+        _compute_repr_n_dist, axis=1, arr=coords_translated
+    )
     return repr_n_dists.T
 
 
-def cmp_reps_n_distance_dict(coords: np.ndarray, extremity_indices: np.ndarray) -> Dict[int, np.ndarray]:
+def cmp_reps_n_distance_dict(
+    coords: np.ndarray, extremity_indices: np.ndarray
+) -> Dict[int, np.ndarray]:
     # Note: distance and angle representation relation are symmetric,
     # but exploiting this has been found to be slower than using the numpy functionality with slight overhead
-    reps_n_distance_dict = {i: cmp_reps_n_distances(i, coords) for i in extremity_indices}
+    reps_n_distance_dict = {
+        i: cmp_reps_n_distances(i, coords) for i in extremity_indices
+    }
     return reps_n_distance_dict
 
 
-def is_within_map(p: np.ndarray, boundary: np.ndarray, holes: Iterable[np.ndarray]) -> bool:
+def is_within_map(
+    p: np.ndarray, boundary: np.ndarray, holes: Iterable[np.ndarray]
+) -> bool:
     if not _inside_polygon(p, boundary, border_value=True):
         return False
     for hole in holes:
         if _inside_polygon(p, hole, border_value=False):
             return False
     return True
 
@@ -113,28 +125,32 @@
         raise TypeError("Each point of a polygon must consist of two values (x,y).")
     if not _no_identical_consequent_vertices(polygon):
         raise ValueError("Consequent vertices of a polynomial must not be identical.")
     if not _no_self_intersection(polygon):
         raise ValueError("The given polygon has self intersections")
 
 
-def check_data_requirements(boundary_coords: np.ndarray, list_hole_coords: List[np.ndarray]):
+def check_data_requirements(
+    boundary_coords: np.ndarray, list_hole_coords: List[np.ndarray]
+):
     """ensures that all the following conditions on the polygons are fulfilled:
         - basic polygon requirements (s. above)
         - edge numbering has to follow this convention (for easier computations):
             * outer boundary polygon: counter clockwise
             * holes: clockwise
 
     :param boundary_coords:
     :param list_hole_coords:
     :return:
     """
     _check_polygon(boundary_coords)
     if _has_clockwise_numbering(boundary_coords):
-        raise ValueError("Vertex numbering of the boundary polygon must be counter clockwise.")
+        raise ValueError(
+            "Vertex numbering of the boundary polygon must be counter clockwise."
+        )
     for hole_coords in list_hole_coords:
         _check_polygon(hole_coords)
         if not _has_clockwise_numbering(hole_coords):
             raise ValueError("Vertex numbering of hole polygon must be clockwise.")
 
 
 def _find_within_range(
@@ -198,15 +214,17 @@
             res = not res
         return res
 
     idxs_within = {i for i in candidate_idxs if within_filter_func(representations[i])}
     return idxs_within
 
 
-def get_neighbour_idxs(i: int, vertex_edge_idxs: np.ndarray, edge_vertex_idxs: np.ndarray) -> Tuple[int, int]:
+def get_neighbour_idxs(
+    i: int, vertex_edge_idxs: np.ndarray, edge_vertex_idxs: np.ndarray
+) -> Tuple[int, int]:
     edge_idx1, edge_idx2 = vertex_edge_idxs[i]
     neigh_idx1 = edge_vertex_idxs[edge_idx1, 0]
     neigh_idx2 = edge_vertex_idxs[edge_idx2, 1]
     return neigh_idx1, neigh_idx2
 
 
 def find_visible(
@@ -257,15 +275,20 @@
         edges_is_crossing,
         edges_max_dist,
         edges_max_rep,
         edges_min_rep,
         non_crossing_edges,
         edge_vertex_idxs,
     ) = _compile_visibility_datastructs(
-        distances, edge_vertex_idxs, edges_to_check, extremity_mask, representations, vertex_edge_idxs
+        distances,
+        edge_vertex_idxs,
+        edges_to_check,
+        extremity_mask,
+        representations,
+        vertex_edge_idxs,
     )
 
     # check non-crossing edges
     # TODO skipped edges. argsort
     # sort after the minimum representation
     edge_idxs_sorted = sorted(non_crossing_edges, key=lambda e: edges_min_rep[e])
     # edge_ptr_iter = iter(ptr for ptr in edge_ptrs if not edges_is_crossing[ptr])
@@ -284,15 +307,19 @@
 
     # when there are no origin-crossing edges, we are done
     if len(crossing_edges) == 0:
         return set(candidates_sorted)
 
     # check origin-crossing edges
     candidates_sorted, edges_max_rep, edges_min_rep, representations = rotate_crossing(
-        candidates_sorted, edges_is_crossing, edges_max_rep, edges_min_rep, representations
+        candidates_sorted,
+        edges_is_crossing,
+        edges_max_rep,
+        edges_min_rep,
+        representations,
     )
 
     # start with checking the first candidate again
     edge_idxs_sorted = sorted(crossing_edges, key=lambda e: edges_min_rep[e])
     _check_candidates(
         candidates_sorted,
         edge_idxs_sorted,
@@ -306,17 +333,21 @@
         edges_max_dist,
     )
     # TODO avoid conversion?
     candidates_ = set(candidates_sorted)
     return candidates_
 
 
-def _eliminate_eq_candidates(candidates: List[int], distances: np.ndarray, representations: np.ndarray) -> List[int]:
+def _eliminate_eq_candidates(
+    candidates: List[int], distances: np.ndarray, representations: np.ndarray
+) -> List[int]:
     # sort after angle representation, then after distance ascending
-    candidates_sorted = sorted(candidates, key=lambda i: (representations[i], distances[i]))
+    candidates_sorted = sorted(
+        candidates, key=lambda i: (representations[i], distances[i])
+    )
     rep_prev = representations[candidates_sorted[0]]
     i = 1
     while i < len(candidates_sorted):
         candidate = candidates_sorted[i]
         rep = representations[candidate]
         if np.isnan(rep) or rep == rep_prev:
             # the candidate is equal to the origin OR
@@ -327,15 +358,20 @@
             rep_prev = rep
             i += 1
 
     return candidates_sorted
 
 
 def _compile_visibility_datastructs(
-    distances, edge_vertex_idxs, edges_to_check, extremity_mask, representations, vertex_edge_idxs
+    distances,
+    edge_vertex_idxs,
+    edges_to_check,
+    extremity_mask,
+    representations,
+    vertex_edge_idxs,
 ):
     edges = list(edges_to_check)
     nr_edges_total = len(edge_vertex_idxs)
     edges_min_rep = np.zeros(nr_edges_total, dtype=float)
     edges_max_rep = np.zeros(nr_edges_total, dtype=float)
     edges_max_dist = np.zeros(nr_edges_total, dtype=float)
     edges_is_crossing = np.zeros(nr_edges_total, dtype=bool)
@@ -361,15 +397,17 @@
         if identical_node is not None:
             # one of the edge vertices is identical to origin
             # no points lie truly "behind" this edge as there is no "direction of sight" defined
             # <-> angle representation/range undefined for just this single edge
             # however if one considers the point neighbouring in the other direction (<-> two edges)
             # these two neighbouring edges define an invisible angle range
             # -> simply move the pointer
-            i1, i2 = get_neighbour_idxs(identical_node, vertex_edge_idxs, edge_vertex_idxs)
+            i1, i2 = get_neighbour_idxs(
+                identical_node, vertex_edge_idxs, edge_vertex_idxs
+            )
             r1, r2 = representations[i1], representations[i2]
             min_rep = min(r1, r2)
             max_rep = max(r1, r2)
 
             # Note: the second edge should not be considered twice
             e1, e2 = vertex_edge_idxs[identical_node]
             if e1 != e:
@@ -443,15 +481,17 @@
         edges_max_rep,
         edges_min_rep,
         non_crossing_edges,
         edge_vertex_idxs,
     )
 
 
-def rotate_crossing(candidate_idxs, edges_is_crossing, edges_max_rep, edges_min_rep, representations):
+def rotate_crossing(
+    candidate_idxs, edges_is_crossing, edges_max_rep, edges_min_rep, representations
+):
     if not np.all(edges_min_rep >= 0.0):
         raise ValueError
 
     # TODO refactor
     if not np.any(edges_is_crossing):
         return set(candidate_idxs)
 
@@ -459,24 +499,28 @@
     # trick: rotate coordinate system to avoid dealing with origin crossings
     # -> implementation for regular edges can be reused!
     # bring the minimum maximal angle representation ("supremum") of all crossing edges to 0
     supremum_cross_edge_rep = np.min(edges_max_rep[edges_is_crossing])
     infimum_to_0 = 4.0 - supremum_cross_edge_rep
     # Note: adding an angle < 180deg to the minimum edge_idx representations (quadrant 1 & 2) cannot lead to "overflow"
     edges_min_rep[edges_is_crossing] = edges_min_rep[edges_is_crossing] + infimum_to_0
-    edges_max_rep[edges_is_crossing] = (edges_max_rep[edges_is_crossing] + infimum_to_0) % 4.0
+    edges_max_rep[edges_is_crossing] = (
+        edges_max_rep[edges_is_crossing] + infimum_to_0
+    ) % 4.0
     # Note: all maximum representations were moved to 1. or 2. quadrant
     # -> became the smaller that the previously min rep! -> swap
     tmp = edges_min_rep
     edges_min_rep = edges_max_rep
     edges_max_rep = tmp
     # apply same transformation also to candidate representations
     # TODO avoid large copy. use dict
     representations = representations.copy()  # IMPORTANT: work on independent copy
-    representations[candidate_idxs] = (representations[candidate_idxs] + infimum_to_0) % 4.0
+    representations[candidate_idxs] = (
+        representations[candidate_idxs] + infimum_to_0
+    ) % 4.0
     # Note: new sorting is required
     candidate_idxs = sorted(candidate_idxs, key=lambda i: representations[i])
     # TODO move to tests
     # non_nan_reps = representations[np.logical_not(np.isnan(representations))]
     # assert np.all(non_nan_reps >= 0.0)
     # assert np.all(non_nan_reps <= 4.0)
     # if not np.all(edges_min_rep >= 0.0):
@@ -551,15 +595,17 @@
             visibility_is_blocked = dist_to_candidate > edge_max_dist
         else:
             # optimisation: if a candidate is farther away from the query point than both vertices of the edge,
             #   it surely lies behind the edge
             # ATTENTION: even if a candidate is closer to the query point than both vertices of the edge,
             #   it still needs to be checked!
             further_away = dist_to_candidate > edge_max_dist
-            visibility_is_blocked = further_away or _lies_behind(p1, p2, candidate_idx, origin, coords)
+            visibility_is_blocked = further_away or _lies_behind(
+                p1, p2, candidate_idx, origin, coords
+            )
 
         if visibility_is_blocked:
             candidate_indices.pop(candidate_ptr_curr)
             # Note: keep ptr at the same position (list shrank)
         else:
             # move pointer to the next candidate
             candidate_ptr_curr += 1
@@ -702,28 +748,32 @@
         n1 = n2
         n2 = tmp
     _, dists = reprs_n_distances[n1]
     distance = dists[n2]
     return distance
 
 
-def _find_identical(candidates: Iterable[int], reprs_n_distances: Dict[int, np.ndarray]) -> Dict[int, int]:
+def _find_identical(
+    candidates: Iterable[int], reprs_n_distances: Dict[int, np.ndarray]
+) -> Dict[int, int]:
     # for shortest path computations all graph nodes should be unique
     # join all nodes with the same coordinates
     merging_mapping = {}
     # symmetric relation -> only consider one direction
     for n1, n2 in itertools.combinations(candidates, 2):
         dist = get_distance(n1, n2, reprs_n_distances)
         if dist == 0.0:  # same coordinates
             merging_mapping[n2] = n1
 
     return merging_mapping
 
 
-def find_identical_single(i: int, candidates: Iterable[int], reprs_n_distances: Dict[int, np.ndarray]) -> int:
+def find_identical_single(
+    i: int, candidates: Iterable[int], reprs_n_distances: Dict[int, np.ndarray]
+) -> int:
     # for shortest path computations all graph nodes should be unique
     # join all nodes with the same coordinates
     # symmetric relation -> only consider one direction
     for n in candidates:
         if i == n:
             continue
         dist = get_distance(i, n, reprs_n_distances)
@@ -814,15 +864,17 @@
     boundary_data = _try_extraction(json_loaded, BOUNDARY_JSON_KEY)
     holes_data = _try_extraction(json_loaded, HOLES_JSON_KEY)
     boundary_coordinates = _convert2polygon(boundary_data)
     list_of_holes = [_convert2polygon(hole_data) for hole_data in holes_data]
     return boundary_coordinates, list_of_holes
 
 
-def convert_gridworld(size_x: int, size_y: int, obstacle_iter: iter, simplify: bool = True) -> (list, list):
+def convert_gridworld(
+    size_x: int, size_y: int, obstacle_iter: iter, simplify: bool = True
+) -> (list, list):
     """
     prerequisites: grid world must not have non-obstacle cells which are surrounded by obstacles
     ("single white cell in black surrounding" = useless for path planning)
     :param size_x: the horizontal grid world size
     :param size_y: the vertical grid world size
     :param obstacle_iter: an iterable of coordinate pairs (x,y) representing blocked grid cells (obstacles)
     :param simplify: whether the polygons should be simplified or not. reduces edge amount, allow diagonal edges
@@ -832,15 +884,18 @@
         the origin of the polygon coordinate system is (-0.5,-0.5) in the grid cell system (= corners of the grid world)
     """
 
     assert size_x > 0 and size_y > 0
 
     if len(obstacle_iter) == 0:
         # there are no obstacles. return just the simple boundary rectangle
-        return [np.array(x, y) for x, y in [(0, 0), (size_x, 0), (size_x, size_y), (0, size_y)]], []
+        return [
+            np.array(x, y)
+            for x, y in [(0, 0), (size_x, 0), (size_x, size_y), (0, size_y)]
+        ], []
 
     # convert (x,y) into np.arrays
     # obstacle_iter = [np.array(o) for o in obstacle_iter]
     obstacle_iter = np.array(obstacle_iter)
 
     def within_grid(pos):
         return 0 <= pos[0] < size_x and 0 <= pos[1] < size_y
@@ -891,15 +946,17 @@
 
         # follow the border between obstacles and free cells ("wall") until one
         # reaches the start position again
         while True:
             # left has to be checked first
             # do not check if just turned left or right (-> the left is blocked for sure)
             # left_pos = current_pos + left_vect
-            if not (just_turned or boundary_detect_fct(current_pos + directions[left_index])):
+            if not (
+                just_turned or boundary_detect_fct(current_pos + directions[left_index])
+            ):
                 # print('< turn left')
                 forward_index = left_index
                 left_index = (forward_index - 1) % 4
                 forward_vect = directions[forward_index]
                 just_turned = True
 
                 # add a new node at the correct position
@@ -936,44 +993,54 @@
         return np.array(edge_list, dtype=float)
 
     # build the boundary polygon
     # start at the lowest and leftmost unblocked grid cell
     start_pos = find_start(start_pos=(0, 0), boundary_detect_fct=is_unblocked)
     # print(start_pos+directions[3])
     # raise ValueError
-    boundary_edges = construct_polygon(start_pos, boundary_detect_fct=is_blocked, cntr_clockwise_wanted=True)
+    boundary_edges = construct_polygon(
+        start_pos, boundary_detect_fct=is_blocked, cntr_clockwise_wanted=True
+    )
 
     if simplify:
         # TODO
         raise NotImplementedError()
 
     # detect which of the obstacles have to be converted into holes
     # just the obstacles inside the boundary polygon are part of holes
     # shift coordinates by +(0.5,0.5) for correct detection
     # the border value does not matter here
 
-    def get_unchecked_obstacles(obstacles: Iterable, poly: np.ndarray, required_val: bool = True) -> List:
+    def get_unchecked_obstacles(
+        obstacles: Iterable, poly: np.ndarray, required_val: bool = True
+    ) -> List:
         unchecked_obstacles = []
         for o in obstacles:
             p = o + 0.5
             if _inside_polygon(p, poly, border_value=True) == required_val:
                 unchecked_obstacles.append(o)
 
         return unchecked_obstacles
 
     unchecked_obstacles = get_unchecked_obstacles(obstacle_iter, boundary_edges)
 
     hole_list = []
     while len(unchecked_obstacles) > 0:
-        start_pos = find_start(start_pos=(0, 0), boundary_detect_fct=pos_in_iter, iter=unchecked_obstacles)
-        hole = construct_polygon(start_pos, boundary_detect_fct=is_unblocked, cntr_clockwise_wanted=False)
+        start_pos = find_start(
+            start_pos=(0, 0), boundary_detect_fct=pos_in_iter, iter=unchecked_obstacles
+        )
+        hole = construct_polygon(
+            start_pos, boundary_detect_fct=is_unblocked, cntr_clockwise_wanted=False
+        )
 
         # detect which of the obstacles still do not belong to any hole:
         # delete the obstacles which are included in the just constructed hole
-        unchecked_obstacles = get_unchecked_obstacles(unchecked_obstacles, hole, required_val=False)
+        unchecked_obstacles = get_unchecked_obstacles(
+            unchecked_obstacles, hole, required_val=False
+        )
 
         if simplify:
             # TODO
             pass
 
         hole_list.append(hole)
 
@@ -999,21 +1066,27 @@
     :return:
     """
     extremity_mask = np.full(len(coordinates), False, dtype=bool)
     _fill_extremity_mask(coordinates, extremity_mask)
     return extremity_mask
 
 
-def _cmp_extremities(list_of_polygons, coords, boundary_coordinates, list_of_hole_coordinates):
-    extremity_masks = [_cmp_extremity_mask(coords_poly) for coords_poly in list_of_polygons]
+def _cmp_extremities(
+    list_of_polygons, coords, boundary_coordinates, list_of_hole_coordinates
+):
+    extremity_masks = [
+        _cmp_extremity_mask(coords_poly) for coords_poly in list_of_polygons
+    ]
     extremity_mask = np.concatenate(extremity_masks, axis=0, dtype=bool)
     # Attention: since polygons are allowed to overlap, only consider extremities that are actually within the map
     for extremity_idx in np.where(extremity_mask)[0]:
         extrimity_coords = coords[extremity_idx]
-        if not is_within_map(extrimity_coords, boundary_coordinates, list_of_hole_coordinates):
+        if not is_within_map(
+            extrimity_coords, boundary_coordinates, list_of_hole_coordinates
+        ):
             extremity_mask[extremity_idx] = False
     extremity_indices = np.where(extremity_mask)[0]
     return extremity_indices, extremity_mask
 
 
 def _cmp_edge_vertex_idxs(coordinates: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     nr_coords = len(coordinates)
@@ -1021,27 +1094,31 @@
     vertex_edge_idxs = np.empty((nr_coords, 2), dtype=int)
     _fill_edge_vertex_idxs(edge_vertex_idxs, vertex_edge_idxs)
     return edge_vertex_idxs, vertex_edge_idxs
 
 
 def _cmp_edge_and_vertex_idxs(list_of_polygons):
     # compute edge and vertex indices from polygon data structure
-    edge_and_vertex_indices = [_cmp_edge_vertex_idxs(coords_poly) for coords_poly in list_of_polygons]
+    edge_and_vertex_indices = [
+        _cmp_edge_vertex_idxs(coords_poly) for coords_poly in list_of_polygons
+    ]
     offset = 0
     for edge_vertex_idxs, vertex_edge_idxs in edge_and_vertex_indices:
         edge_vertex_idxs += offset
         vertex_edge_idxs += offset
         offset += len(edge_vertex_idxs)
     edge_vertex_idxs, vertex_edge_idxs = zip(*edge_and_vertex_indices)
     edge_vertex_idxs = np.concatenate(edge_vertex_idxs, axis=0)
     vertex_edge_idxs = np.concatenate(vertex_edge_idxs, axis=0)
     return edge_vertex_idxs, vertex_edge_idxs
 
 
-def compile_polygon_datastructs(boundary_coordinates: np.ndarray, list_of_hole_coordinates: List[np.ndarray]):
+def compile_polygon_datastructs(
+    boundary_coordinates: np.ndarray, list_of_hole_coordinates: List[np.ndarray]
+):
     list_of_polygons = [boundary_coordinates] + list_of_hole_coordinates
     coords = np.concatenate(list_of_polygons, axis=0, dtype=configs.DTYPE_FLOAT)
     edge_vertex_idxs, vertex_edge_idxs = _cmp_edge_and_vertex_idxs(list_of_polygons)
     extremity_indices, extremity_mask = _cmp_extremities(
         list_of_polygons, coords, boundary_coordinates, list_of_hole_coordinates
     )
     return coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs
```

### Comparing `extremitypathfinder-2.7.1/extremitypathfinder/utils_numba.py` & `extremitypathfinder-2.7.2/extremitypathfinder/utils_numba.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,13 +238,15 @@
     # assert np.allclose(np.dot(A, x), b)
 
     # vertices on the edge are possibly visible! ( < not <=)
     return x[1] < 1.0
 
 
 @njit(b1(i8, i8, i8, i8, f8[:, :]), cache=True)
-def _lies_behind(idx_p1: int, idx_p2: int, idx_v: int, idx_orig: int, coords: np.ndarray) -> bool:
+def _lies_behind(
+    idx_p1: int, idx_p2: int, idx_v: int, idx_orig: int, coords: np.ndarray
+) -> bool:
     coords_origin = coords[idx_orig]
     coords_p1_rel = coords[idx_p1] - coords_origin
     coords_p2_rel = coords[idx_p2] - coords_origin
     coords_v_rel = coords[idx_v] - coords_origin
     return _lies_behind_inner(coords_p1_rel, coords_p2_rel, coords_v_rel)
```

### Comparing `extremitypathfinder-2.7.1/pyproject.toml` & `extremitypathfinder-2.7.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extremitypathfinder"
-version = "2.7.1"
+version = "2.7.2"
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/jannikmi/extremitypathfinder"
 homepage = "https://extremitypathfinder.readthedocs.io/en/latest/"
 documentation = "https://extremitypathfinder.readthedocs.io/en/latest/"
 keywords = ["path-planning", "path-finding", "shortest-path", "visibility", "graph", "polygon", "grid", "map", "robotics", "navigation", "offline"]
 classifiers = [
@@ -35,37 +35,82 @@
 ]
 #exclude = ["my_package/excluded.py"]
 
 [tool.poetry.scripts]
 extremitypathfinder = "extremitypathfinder.command_line:main"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-numpy = "^1.22"
+python = ">=3.8,<4"
 networkx = "^3"
-numba = {version = "^0.56.0", optional = true}
+numpy = [
+    { version = ">=1.21,<2", python = "<3.9" },
+    { version = ">=1.23,<2", python = ">=3.9" }
+]
+numba = [
+    { version = ">=0.56,<1", python = "<3.12", optional = true },
+    { version = ">=0.59,<1", python = ">=3.12", optional = true }
+]
 # required for jit of np.linalg.solve with numba
-scipy = {version = "^1.10.1", optional = true}
+scipy = [
+    { version = ">=1.9,<2", python = "<3.12", optional = true },
+    { version = ">=1.10,<2", python = ">=3.12", optional = true }
+]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
+pytest = "*"
+tox = "*"
 
 [tool.poetry.group.plot.dependencies]
+# also required for runnin the tests
 matplotlib = "*"
 
-[tool.poetry.group.test.dependencies]
-pytest = "*"
-tox = "*"
-
 [tool.poetry.group.docs.dependencies]
 Sphinx = "*"
 sphinx-rtd-theme = "*"
 
+[tool.poetry.group.plot]
+optional = true
+
+[tool.poetry.group.docs]
+optional = true
+
+
 [tool.poetry.extras]
 numba = ["numba", "scipy"]
-plot = ["matplotlib"]
-test = ["pytest", "tox"]
-docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [build-system]
 requires = ["poetry-core>=1.5", "poetry>=1.4"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = true
+envlist =
+    docs,py{38,39,310,311,312}{,-numba}
+
+[gh-actions]
+python =
+    3.8: py38{,-numba}
+    3.9: py39{,-numba}
+    3.10: py310{,-numba}
+    3.11: py311{,-numba}
+    3.12: py312{,-numba}
+
+
+[testenv:docs]
+description = build documentation
+basepython = python3.12
+allowlist_externals = poetry,sphinx-build
+commands =
+  poetry install -v --with docs
+  sphinx-build -d "{envtmpdir}{/}doctree" docs "{toxworkdir}{/}docs_out" --color -b html
+  python -c 'print(r"documentation available under file://{toxworkdir}{/}docs_out{/}index.html")'
+
+[testenv]
+allowlist_externals = poetry
+commands =
+    !numba: poetry install -v --with dev,plot
+    numba:  poetry install -v --with dev,plot --extras numba
+    poetry run pytest {posargs}
+"""
```

### Comparing `extremitypathfinder-2.7.1/tests/cli_test.py` & `extremitypathfinder-2.7.2/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.7.1/tests/helper_fcts_test.py` & `extremitypathfinder-2.7.2/tests/helper_fcts_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 TODO test find_visible(), ...
 TODO test if relation is really bidirectional (y in find_visible(x,y) <=> x in find_visible(y,x))
 TODO test input data validation
 """
+
 from os.path import abspath, join, pardir
 from typing import Dict, Set
 
 import numpy as np
 import pytest
 
 from extremitypathfinder import PolygonEnvironment, configs
@@ -18,15 +19,17 @@
     read_json,
 )
 from tests.helpers import proto_test_case
 from tests.test_find_visible import _clean_visibles
 
 
 def test_inside_polygon():
-    polygon_test_case = np.array([(-1.0, -1.0), (1.0, -1.0), (1.0, 1.0), (-1.0, 1.0)], dtype=configs.DTYPE_FLOAT)
+    polygon_test_case = np.array(
+        [(-1.0, -1.0), (1.0, -1.0), (1.0, 1.0), (-1.0, 1.0)], dtype=configs.DTYPE_FLOAT
+    )
 
     for border_value in [True, False]:
 
         def test_fct(input):
             p = np.array(input, dtype=configs.DTYPE_FLOAT)
             return _inside_polygon(p, polygon_test_case, border_value)
 
@@ -103,15 +106,18 @@
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 0.0, 1: 1.0}, {0}),
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 0.0, 1: 1.1}, {0}),
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 1.0, 1: 0.0}, {1}),
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 1.1, 1: 0.0}, {1}),
     ],
 )
 def test_clean_visible_idxs(
-    visible_idxs: Set[int], cand_idx2repr: Dict[int, float], vert_idx2dist: Dict[int, float], expected: Set[int]
+    visible_idxs: Set[int],
+    cand_idx2repr: Dict[int, float],
+    vert_idx2dist: Dict[int, float],
+    expected: Set[int],
 ):
     res = _clean_visibles(visible_idxs, cand_idx2repr, vert_idx2dist)
     assert res == expected
 
 
 @pytest.mark.parametrize(
     "coords, expected",
```

### Comparing `extremitypathfinder-2.7.1/tests/helpers.py` & `extremitypathfinder-2.7.2/tests/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 
 def proto_test_case(data, fct):
     for input, expected_output in data:
         # print(input, expected_output, fct(input))
         actual_output = fct(input)
         if actual_output != expected_output:
-            print("input: {} expected: {} got: {}".format(input, expected_output, actual_output))
+            print(
+                "input: {} expected: {} got: {}".format(
+                    input, expected_output, actual_output
+                )
+            )
         assert actual_output == expected_output
 
 
-def other_edge_intersects(n1: int, n2: int, edge_vertex_idxs: np.ndarray, coords: np.ndarray) -> bool:
+def other_edge_intersects(
+    n1: int, n2: int, edge_vertex_idxs: np.ndarray, coords: np.ndarray
+) -> bool:
     p1 = coords[n1]
     p2 = coords[n2]
     for i1, i2 in edge_vertex_idxs:
         if i1 == n1 or i2 == n2:
             # no not check the same edge
             continue
         q1 = coords[i1]
```

### Comparing `extremitypathfinder-2.7.1/tests/main_test.py` & `extremitypathfinder-2.7.2/tests/main_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,26 @@
 
 
 # TODO pytest parameterize
 
 
 def try_test_cases(environment, test_cases):
     def validate(start_coordinates, goal_coordinates, expected_output):
-        output = environment.find_shortest_path(start_coordinates, goal_coordinates, verify=True)
+        output = environment.find_shortest_path(
+            start_coordinates, goal_coordinates, verify=True
+        )
         path, length = output
-        assert type(path) is list
+        assert isinstance(path, list), "path should be a list"
         expected_path, expected_length = expected_output
         if expected_length is None:
             correct_result = length is None and path == expected_path
         else:
-            correct_result = path == expected_path and length == pytest.approx(expected_length)
+            correct_result = path == expected_path and length == pytest.approx(
+                expected_length
+            )
         if correct_result:
             status_str = "OK"
         else:
             status_str = "XX"
         print(f"{status_str} input: {(start_coordinates, goal_coordinates)} ")
         assert correct_result, f"unexpected result (path, length): got {output} instead of {expected_output} "
 
@@ -76,29 +80,28 @@
 
     print("testing grid environment")
     try_test_cases(grid_env, TEST_DATA_GRID_ENV)
 
     # when the deep copy mechanism works correctly
     # even after many queries the internal graph should have the same structure as before
     # otherwise the temporarily added vertices during a query stay stored
-    nr_graph_nodes = len(grid_env.graph.nodes)
+    # nr_graph_nodes = len(grid_env.graph.nodes)
     # TODO
     # assert nr_graph_nodes == 16, "the graph should stay unchanged by shortest path queries!"
-
-    nr_nodes_env1_old = len(grid_env.graph.nodes)
+    # nr_nodes_env1_old = len(grid_env.graph.nodes)
 
 
 def test_poly_env():
     poly_env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
     poly_env.store(*POLY_ENV_PARAMS, validate=True)
     nr_exp_extremities = 4
     assert (
         len(list(poly_env.all_extremities)) == nr_exp_extremities
     ), f"the environment should detect all {nr_exp_extremities} extremities!"
-    nr_nodes_env2 = len(poly_env.graph.nodes)
+    # nr_nodes_env2 = len(poly_env.graph.nodes)
     # TODO
     # assert nr_nodes_env2 == nr_exp_extremities, (
     #     f"the visibility graph should store all {nr_exp_extremities} extremities {list(poly_env.all_extremities)}!"
     #     f"\n found: {poly_env.graph.nodes}"
     # )
 
     # nr_nodes_env1_new = len(grid_env.graph.nodes)
@@ -150,15 +153,17 @@
     graph = env.graph
     extremities = env.extremity_indices
     edge_vertex_idxs = env.edge_vertex_idxs
 
     def connection_as_expected(i1: int, i2: int):
         if i2 not in extremities:
             return
-        should_be_connected = not other_edge_intersects(i1, i2, edge_vertex_idxs, coords)
+        should_be_connected = not other_edge_intersects(
+            i1, i2, edge_vertex_idxs, coords
+        )
         graph_neighbors_e = set(graph.neighbors(i1))
         are_connected = i2 in graph_neighbors_e
         assert should_be_connected == are_connected
 
     for e in extremities:
         n1, n2 = utils.get_neighbour_idxs(e, env.vertex_edge_idxs, edge_vertex_idxs)
         connection_as_expected(e, n1)
```

### Comparing `extremitypathfinder-2.7.1/tests/test_cases.py` & `extremitypathfinder-2.7.2/tests/test_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # size_x, size_y, obstacle_iter
 from math import sqrt
 
-import numpy as np
-
-from extremitypathfinder import utils
 
 GRID_ENV_PARAMS = (
     19,
     10,
     [
         # (x,y),
         # obstacles changing boundary
@@ -334,15 +331,17 @@
             88.55556650808049,
         ),
     ),
 ]
 
 SEPARATED_ENV = (
     [(5, 5), (-5, 5), (-5, -5), (5, -5)],
-    [[(-5.1, 1), (-5.1, 2), (5.1, 2), (5.1, 1)]],  # intersecting polygons -> no path possible
+    [
+        [(-5.1, 1), (-5.1, 2), (5.1, 2), (5.1, 1)]
+    ],  # intersecting polygons -> no path possible
     # [[(-5, 1), (-5, 2), (5, 2), (5, 1)]], # hole lies on the edges -> path possible
 )
 
 TEST_DATA_SEPARATE_ENV = [
     # ((start,goal),(path,distance))
     (((0, 0), (0, 4)), ([], None)),  # unreachable
 ]
```

### Comparing `extremitypathfinder-2.7.1/tests/test_find_visible.py` & `extremitypathfinder-2.7.2/tests/test_find_visible.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,29 @@
 import itertools
 from typing import Set, Tuple
 
 import numpy as np
 import pytest
 
 from extremitypathfinder import PolygonEnvironment, configs, utils
-from extremitypathfinder.utils import _find_within_range, _lies_behind, get_neighbour_idxs
+from extremitypathfinder.utils import (
+    _find_within_range,
+    _lies_behind,
+    get_neighbour_idxs,
+)
 from tests.test_cases import GRID_ENV_PARAMS, POLYGON_ENVS
 
 
 def find_candidates_behind(
-    origin: int, v1: int, v2: int, candidates: Set[int], distances: np.ndarray, coords: np.ndarray
+    origin: int,
+    v1: int,
+    v2: int,
+    candidates: Set[int],
+    distances: np.ndarray,
+    coords: np.ndarray,
 ) -> Set[int]:
     dist_v1 = distances[v1]
     dist_v2 = distances[v2]
     max_distance = max(dist_v1, dist_v2)
     idxs_behind = set()
     # for all remaining vertices v it has to be tested if the line segment from query point (=origin) to v
     #    has an intersection with the current edge p1---p2
@@ -36,15 +45,17 @@
         further_away = dist2orig > max_distance
         if further_away or _lies_behind(v1, v2, idx, origin, coords):
             idxs_behind.add(idx)
         # vertex lies in front of this edge
     return idxs_behind
 
 
-def _clean_visibles(visible_idxs: Set[int], cand_idx2repr: np.ndarray, vert_idx2dist: np.ndarray) -> Set[int]:
+def _clean_visibles(
+    visible_idxs: Set[int], cand_idx2repr: np.ndarray, vert_idx2dist: np.ndarray
+) -> Set[int]:
     # in case some vertices have the same representation, only return (link) the closest vertex
     if len(visible_idxs) <= 1:
         return visible_idxs
 
     cleaned = set()
     visible_idxs_sorted = sorted(visible_idxs, key=lambda i: cand_idx2repr[i])
     min_dist = np.inf
@@ -158,15 +169,17 @@
             # angle range blocked by a single edge is always <180 degree
             angle_range = 4 - angle_range
 
         edge_angle_range[edge] = angle_range
         samples[edge] = (v1, v2, repr1, repr2, lies_on_edge, range_less_180)
 
     # edges with the highest angle range first
-    edges_prioritised = sorted(edge_angle_range.keys(), reverse=True, key=lambda e: edge_angle_range[e])
+    edges_prioritised = sorted(
+        edge_angle_range.keys(), reverse=True, key=lambda e: edge_angle_range[e]
+    )
 
     visibles = set()
     # goal: eliminating all vertices lying behind any edge ("blocking the view")
     for edge in edges_prioritised:
         if len(candidates) == 0:
             break
 
@@ -201,19 +214,28 @@
             # use discard() instead of remove() to not raise an error (they might not be candidates)
             idxs_behind.discard(v1)
             idxs_behind.discard(v2)
             #  candidates with the same representation as v1 or v2 should be considered.
             #   they may be visible, but must be ruled out if they lie behind any edge!
             equal_repr_allowed = True
 
-        idxs_behind = _find_within_range(repr1, repr2, idxs_behind, range_less_180, equal_repr_allowed, representations)
+        idxs_behind = _find_within_range(
+            repr1,
+            repr2,
+            idxs_behind,
+            range_less_180,
+            equal_repr_allowed,
+            representations,
+        )
         if not lies_on_edge:
             # Note: when the origin lies on the edge, all candidates within the angle range lie behind the edge
             # -> actual "behind/in front" checks can be skipped!
-            idxs_behind = find_candidates_behind(origin, v1, v2, idxs_behind, distances, coords)
+            idxs_behind = find_candidates_behind(
+                origin, v1, v2, idxs_behind, distances, coords
+            )
 
         # vertices behind any edge are not visible and should not be considered any further
         candidates.difference_update(idxs_behind)
 
     # all edges have been checked
     # all remaining vertices were not concealed behind any edge and hence are visible
     visibles.update(candidates)
@@ -225,15 +247,17 @@
     boundary = np.array(boundary, dtype=configs.DTYPE_FLOAT)
     holes = [np.array(hole, dtype=configs.DTYPE_FLOAT) for hole in holes]
     # (coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs)
     return utils.compile_polygon_datastructs(boundary, holes)
 
 
 def _yield_input_args(boundary_data):
-    coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs = boundary_data
+    coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs = (
+        boundary_data
+    )
     candidates = set(np.where(extremity_mask)[0])
     nr_edges = len(edge_vertex_idxs)
     edges_to_check = set(range(nr_edges))
     for origin in range(len(coords)):  # all possible vertices as origins
         reps_n_distances = utils.cmp_reps_n_distances(origin, coords)
         representations, distances = reps_n_distances
 
@@ -324,8 +348,10 @@
         coords,
         representations,
         distances,
         edge_vertex_idxs,
         vertex_edge_idxs,
         extremity_mask,
     )
-    assert visibles_found == visibles_expected, f"expected {visibles_expected} but got {visibles_found}"
+    assert (
+        visibles_found == visibles_expected
+    ), f"expected {visibles_expected} but got {visibles_found}"
```

### Comparing `extremitypathfinder-2.7.1/PKG-INFO` & `extremitypathfinder-2.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: extremitypathfinder
-Version: 2.7.1
+Version: 2.7.2
 Summary: python package for fast shortest path computation on 2D polygon or grid maps
 Home-page: https://extremitypathfinder.readthedocs.io/en/latest/
 License: MIT
 Keywords: path-planning,path-finding,shortest-path,visibility,graph,polygon,grid,map,robotics,navigation,offline
 Author: jannikmi
 Author-email: github@michelfe.it
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Provides-Extra: docs
 Provides-Extra: numba
-Provides-Extra: plot
-Provides-Extra: test
 Requires-Dist: networkx (>=3,<4)
-Requires-Dist: numba (>=0.56.0,<0.57.0) ; extra == "numba"
-Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0) ; extra == "numba"
+Requires-Dist: numba (>=0.56,<1) ; (python_version < "3.12") and (extra == "numba")
+Requires-Dist: numba (>=0.59,<1) ; (python_version >= "3.12") and (extra == "numba")
+Requires-Dist: numpy (>=1.21,<2) ; python_version < "3.9"
+Requires-Dist: numpy (>=1.23,<2) ; python_version >= "3.9"
+Requires-Dist: scipy (>=1.10,<2) ; (python_version >= "3.12") and (extra == "numba")
+Requires-Dist: scipy (>=1.9,<2) ; (python_version < "3.12") and (extra == "numba")
 Project-URL: Documentation, https://extremitypathfinder.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jannikmi/extremitypathfinder
 Description-Content-Type: text/x-rst
 
 ===================
 extremitypathfinder
 ===================
```

