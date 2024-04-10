# Comparing `tmp/cai_causal_graph-0.4.7.tar.gz` & `tmp/cai_causal_graph-0.4.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cai_causal_graph-0.4.7.tar", max compression
+gzip compressed data, was "cai_causal_graph-0.4.7.dev0.tar", max compression
```

## Comparing `cai_causal_graph-0.4.7.tar` & `cai_causal_graph-0.4.7.dev0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/LICENSE
--rw-r--r--   0        0        0     1686 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/README.md
--rw-r--r--   0        0        0     1287 2024-04-10 09:30:58.498926 cai_causal_graph-0.4.7/cai_causal_graph/__init__.py
--rw-r--r--   0        0        0   101920 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/causal_graph.py
--rw-r--r--   0        0        0     2599 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/exceptions.py
--rw-r--r--   0        0        0    28767 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/graph_components.py
--rw-r--r--   0        0        0    21769 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/identify_utils.py
--rw-r--r--   0        0        0     1865 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/interfaces.py
--rw-r--r--   0        0        0    63360 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/time_series_causal_graph.py
--rw-r--r--   0        0        0     4427 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/type_definitions.py
--rw-r--r--   0        0        0     4914 2024-04-10 09:30:41.594889 cai_causal_graph-0.4.7/cai_causal_graph/utils.py
--rw-r--r--   0        0        0     2570 2024-04-10 09:30:58.498926 cai_causal_graph-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-27 16:40:54.196859 cai_causal_graph-0.4.7.dev0/LICENSE
+-rw-r--r--   0        0        0     1686 2024-03-27 16:40:54.196859 cai_causal_graph-0.4.7.dev0/README.md
+-rw-r--r--   0        0        0     1292 2024-03-27 16:41:09.184989 cai_causal_graph-0.4.7.dev0/cai_causal_graph/__init__.py
+-rw-r--r--   0        0        0   101529 2024-03-27 16:40:54.196859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/causal_graph.py
+-rw-r--r--   0        0        0     2599 2024-03-27 16:40:54.196859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/exceptions.py
+-rw-r--r--   0        0        0    28767 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/graph_components.py
+-rw-r--r--   0        0        0    19394 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/identify_utils.py
+-rw-r--r--   0        0        0     1865 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/interfaces.py
+-rw-r--r--   0        0        0    63360 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/time_series_causal_graph.py
+-rw-r--r--   0        0        0     4427 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/type_definitions.py
+-rw-r--r--   0        0        0     4914 2024-03-27 16:40:54.200859 cai_causal_graph-0.4.7.dev0/cai_causal_graph/utils.py
+-rw-r--r--   0        0        0     2263 2024-03-27 16:41:09.180989 cai_causal_graph-0.4.7.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 cai_causal_graph-0.4.7.dev0/PKG-INFO
```

### Comparing `cai_causal_graph-0.4.7/LICENSE` & `cai_causal_graph-0.4.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/README.md` & `cai_causal_graph-0.4.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/__init__.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'EDGE_T',  # Keep for backwards compatibility.
     'NODE_T',  # Keep for backwards compatibility.
     # Time series specific tags
     'TIME_LAG',
     'VARIABLE_NAME',
 ]
 
-__version__ = '0.4.7'
+__version__ = '0.4.7.dev0'
 
 from cai_causal_graph.causal_graph import CausalGraph, Skeleton
 from cai_causal_graph.time_series_causal_graph import TimeSeriesCausalGraph
 from cai_causal_graph.type_definitions import (
     EDGE_T,
     NODE_T,
     TIME_LAG,
```

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/causal_graph.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/causal_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1793,20 +1793,14 @@
         assert self.is_dag(), 'This method only works for DAGs but the current graph is not a DAG.'
 
         source = self._NodeCls.identifier_from(source)
         destination = self._NodeCls.identifier_from(destination)
 
         assert all(node in self.get_node_names() for node in [source, destination])
 
-        # In networkx 3.3 this will return a path of length 1 with just that node in it. We don't want to consider this
-        # particularly as there is no self loop from that node to itself. One could make an edge from source to source
-        # but then it would no longer be a DAG as we confirm in the first step of this method.
-        if source == destination:
-            return []
-
         return list(networkx.all_simple_paths(self.to_networkx(), source, destination))
 
     def directed_path_exists(self, source: NodeLike, destination: NodeLike) -> bool:
         """
         Check whether there exists a directed path between the source and destination.
 
         Unlike the `CausalGraph.get_all_causal_paths` method, this works for mixed causal graphs as well (note that
```

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/exceptions.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/graph_components.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/graph_components.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/identify_utils.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/identify_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from itertools import combinations
 from typing import List, Optional, Set, Tuple, Union
 
 import networkx
 
 from cai_causal_graph import CausalGraph, Skeleton
 from cai_causal_graph.exceptions import CausalGraphErrors
 from cai_causal_graph.graph_components import Node
-from cai_causal_graph.type_definitions import EdgeType, NodeLike
+from cai_causal_graph.type_definitions import NodeLike
 
 
 def _verify_identify_inputs(
     graph: Union[CausalGraph, Skeleton], node_1: NodeLike, node_2: Optional[NodeLike] = None
 ) -> Tuple[str, str]:
     """
     Verify the inputs to the identify utilities.
@@ -384,58 +383,7 @@
             | {parent for child in child_set for parent in graph.get_parents(child) if parent != node_id}
         )
     else:
         # We already know it is Skeleton here so no need for elif.
         mb = graph.get_neighbors(node_id)
 
     return mb
-
-
-def identify_colliders(graph: CausalGraph, unshielded_only: bool = False) -> List[str]:
-    """
-    Identify all the collider nodes in the provided `graph`.
-
-    :param graph: The graph given by a `cai_causal_graph.causal_graph.CausalGraph` instance.
-    :param unshielded_only: If `True`, only unshielded colliders are returned. If `False`, all colliders are returned.
-        Default is `False`. A collider is unshielded if there is no edge between any of its parents.
-    :return: A list of all node identifiers for the collider nodes in the graph.
-    """
-    colliders = set()
-
-    bidirected_edges = [(edge.source.identifier, edge.destination.identifier) for edge in graph.get_bidirected_edges()]
-
-    # go through every node in the graph
-    for node in graph.get_node_names():
-        # the node z is collider if x <> z <> y, x -> z <- y, x <> z <- y, or x -> z <> y
-        neighbors = graph.get_neighbors(node)
-
-        potential_parents = set()
-
-        for neighbor_node in neighbors:
-            # we need to check if the directed edge (neigh_node, node) exists
-            directed_exists = (
-                graph.edge_exists(neighbor_node, node)
-                and graph.get_edge(neighbor_node, node).edge_type == EdgeType.DIRECTED_EDGE
-            )
-            # we need to check if the bi-directed edge (neigh_node, node) or (node, neigh_node) exists
-            bidirected_exists = (neighbor_node, node) in bidirected_edges or (node, neighbor_node) in bidirected_edges
-
-            condition = directed_exists or bidirected_exists
-
-            if condition:
-                potential_parents.add(neighbor_node)
-
-        if len(potential_parents) >= 2:
-            # check if the collider is unshielded. A collider is unshielded if there is no edge between any of its
-            # parents
-            is_unshielded = True
-            if unshielded_only:
-                # test all the possible combinations of the potential parents
-                for parent_1, parent_2 in combinations(potential_parents, 2):
-                    if graph.edge_exists(parent_1, parent_2) or graph.edge_exists(parent_2, parent_1):
-                        is_unshielded = False
-                        break
-
-            if not unshielded_only or is_unshielded:
-                colliders.add(node)
-
-    return list(colliders)
```

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/interfaces.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/interfaces.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/time_series_causal_graph.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/time_series_causal_graph.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/type_definitions.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/type_definitions.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/cai_causal_graph/utils.py` & `cai_causal_graph-0.4.7.dev0/cai_causal_graph/utils.py`

 * *Files identical despite different names*

### Comparing `cai_causal_graph-0.4.7/pyproject.toml` & `cai_causal_graph-0.4.7.dev0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -38,32 +38,27 @@
 check_untyped_defs = true
 ignore_missing_imports = true
 pretty = true
 cache_dir = '/dev/null'
 
 [tool.poetry]
 name = "cai-causal-graph"
-version = "0.4.7"
+version = "0.4.7.dev0"
 description = "A Causal AI package for causal graphs."
 license = "Apache-2.0"
 authors = ["causaLens <opensource@causalens.com>"]
 readme = "README.md"
 homepage = "https://causalgraph.causalens.com/"
 repository = "https://github.com/causalens/cai-causal-graph"
 documentation = "https://causalgraph.causalens.com/"
 packages = [{include = "cai_causal_graph"}]
 
 [tool.poetry.dependencies]
 mypy-extensions = "^1.0.0"
-# networkx 3.3 broke how get_all_simple_paths works so want to bound for now.
-# networkx 3.1 is the last one to support 3.8. We will drop 3.8 on next minor.
-networkx = [
-    {version = ">=3.0.0, <3.3.0", python = ">=3.9.0, <3.13.0"},
-    {version = ">=3.0.0, <3.2.0", python = ">=3.8.0, <3.9.0"}  # 3.1 is the last version to support 3.8.
-]
+networkx = ">=3.0.0, <4.0.0"
 # Newest numpy is >= 3.9 so need to have different deps while we still support 3.8 but will drop 3.8 on next minor.
 # 1.26 is the first version to support 3.12, but want to allow other versions to support earlier numpy.
 numpy = [
     {version = "^1.20.0", python = ">=3.9.0, <3.13.0"},
     {version = ">=1.20.0, <1.25.0", python = ">=3.8.0, <3.9.0"}  # 1.24 is the last version to support 3.8.
 ]
 pandas = ">=1.0.0, <3.0.0"
```

### Comparing `cai_causal_graph-0.4.7/PKG-INFO` & `cai_causal_graph-0.4.7.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cai-causal-graph
-Version: 0.4.7
+Version: 0.4.7.dev0
 Summary: A Causal AI package for causal graphs.
 Home-page: https://causalgraph.causalens.com/
 License: Apache-2.0
 Author: causaLens
 Author-email: opensource@causalens.com
 Requires-Python: >=3.8.0,<3.13.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mypy-extensions (>=1.0.0,<2.0.0)
-Requires-Dist: networkx (>=3.0.0,<3.2.0) ; python_full_version >= "3.8.0" and python_full_version < "3.9.0"
-Requires-Dist: networkx (>=3.0.0,<3.3.0) ; python_full_version >= "3.9.0" and python_full_version < "3.13.0"
+Requires-Dist: networkx (>=3.0.0,<4.0.0)
 Requires-Dist: numpy (>=1.20.0,<1.25.0) ; python_full_version >= "3.8.0" and python_full_version < "3.9.0"
 Requires-Dist: numpy (>=1.20.0,<2.0.0) ; python_full_version >= "3.9.0" and python_full_version < "3.13.0"
 Requires-Dist: pandas (>=1.0.0,<3.0.0)
 Project-URL: Documentation, https://causalgraph.causalens.com/
 Project-URL: Repository, https://github.com/causalens/cai-causal-graph
 Description-Content-Type: text/markdown
```

