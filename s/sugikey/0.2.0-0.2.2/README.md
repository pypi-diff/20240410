# Comparing `tmp/sugikey-0.2.0.tar.gz` & `tmp/sugikey-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugikey-0.2.0.tar", max compression
+gzip compressed data, was "sugikey-0.2.2.tar", max compression
```

## Comparing `sugikey-0.2.0.tar` & `sugikey-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      910 2024-03-01 20:22:10.570979 sugikey-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3126 2023-08-29 19:40:45.319741 sugikey-0.2.0/README.md
--rw-r--r--   0        0        0      172 2021-04-15 07:09:46.000000 sugikey-0.2.0/sugikey/__init__.py
--rw-r--r--   0        0        0     3141 2023-07-13 19:57:04.760825 sugikey-0.2.0/sugikey/bokeh_sk.py
--rw-r--r--   0        0        0    20668 2023-08-20 11:38:31.794114 sugikey-0.2.0/sugikey/draw.py
--rw-r--r--   0        0        0     7236 2023-07-13 19:44:00.825331 sugikey-0.2.0/sugikey/examples.py
--rw-r--r--   0        0        0    10203 2023-07-13 19:41:23.681319 sugikey-0.2.0/sugikey/optim.py
--rw-r--r--   0        0        0    18095 2023-08-20 11:38:34.805070 sugikey-0.2.0/sugikey/processing.py
--rw-r--r--   0        0        0     1535 2023-08-20 11:38:32.675659 sugikey-0.2.0/sugikey/sankey.py
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 sugikey-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      956 2024-04-10 19:37:22.553857 sugikey-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3291 2024-04-10 19:28:22.091382 sugikey-0.2.2/README.md
+-rw-r--r--   0        0        0      172 2021-04-15 07:09:46.000000 sugikey-0.2.2/sugikey/__init__.py
+-rw-r--r--   0        0        0     3141 2023-07-13 19:57:04.760825 sugikey-0.2.2/sugikey/bokeh_sk.py
+-rw-r--r--   0        0        0    20929 2024-04-10 19:34:03.816895 sugikey-0.2.2/sugikey/draw.py
+-rw-r--r--   0        0        0     7298 2024-04-10 18:57:37.820150 sugikey-0.2.2/sugikey/examples.py
+-rw-r--r--   0        0        0    10203 2023-07-13 19:41:23.681319 sugikey-0.2.2/sugikey/optim.py
+-rw-r--r--   0        0        0    18174 2024-04-10 19:06:09.154797 sugikey-0.2.2/sugikey/processing.py
+-rw-r--r--   0        0        0     1626 2024-04-10 18:46:21.826484 sugikey-0.2.2/sugikey/sankey.py
+-rw-r--r--   0        0        0     3923 1970-01-01 00:00:00.000000 sugikey-0.2.2/PKG-INFO
```

### Comparing `sugikey-0.2.0/pyproject.toml` & `sugikey-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "sugikey"
-version = "0.2.0"
+version = "0.2.2"
 description = "Drawing Sankey diagrams in Python"
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^1.5.3"
-matplotlib = "^3.7.1"
+python = "^3.9"
+pandas = "^2.2.1"
+matplotlib = "^3.8.4"
 networkx = "^3.0"
-pulp = "^2.7.0"
+pulp = "^2.8.0"
 openpyxl = "^3.1.2"
-bokeh = "^3.1.0"
+bokeh = "^3.4.0"
 sphinx-material = "^0.0.36"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 jupyterlab = "^3.6.3"
 black = "^23.3.0"
@@ -32,8 +32,11 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 branch = "main"
 upload_to_repository = true
 hvcs = "gitlab"
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `sugikey-0.2.0/README.md` & `sugikey-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 Have a look at the [documentation](https://gitabab.gitlab.io/sugikey/) for more information.
 
 ## More on Sankey diagrams
 
 * [Why Sankey diagrams are so great for understanding energy data](https://medium.com/@spectalizer/why-sankey-diagrams-are-so-great-for-understanding-energy-data-b14649d40890)
 
+* [Sankey diagrams now have the package they deserve](https://medium.com/@spectalizer/sankey-diagrams-now-have-the-new-python-package-they-deserved-68754a0830d3)
+
 ## Support
 
 Write an issue if there is an issue.
 
 
 ## Authors and acknowledgment
 Zlatan B.
```

### Comparing `sugikey-0.2.0/sugikey/bokeh_sk.py` & `sugikey-0.2.2/sugikey/bokeh_sk.py`

 * *Files identical despite different names*

### Comparing `sugikey-0.2.0/sugikey/draw.py` & `sugikey-0.2.2/sugikey/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Draw (Sankey diagram or node link diagrams)"""
 
-import copy
 from dataclasses import dataclass, field
 
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Any
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 
 
 def get_default_text_kwargs(label_category, library):
     """Get default keyword arguments.
 
     Args:
         label_category: The category of the label.
+            One of "node_label" or "edge_label".
         library: The library being used.
 
     Returns:
         A dictionary with the default keyword argument, e.g. {"fontsize": 10}.
     """
     if label_category == "node_label":
         font_size = 10
@@ -52,26 +52,28 @@
         dx_node: node half width
         dx_arrow
     """
 
     n_segments: int = 100
     link_geometry: str = "cubic_spline"
     write_node_names: bool = True
-    node_name_dy_frac: float = 0.1  # vertical distance between node center and node label, as a fraction of dy_node
+    node_name_dy_frac: float = (
+        0.1  # vertical distance between node center and node label, as a fraction of dy_node
+    )
     library: str = "Matplotlib"
-    node_label_kwargs: dict = None
+    node_label_kwargs: Optional[Dict[str, Any]] = None
     write_edge_values: bool = True
-    edge_label_kwargs: dict = None  # field(default_factory=lambda: {"fontsize": 8})
+    edge_label_kwargs: Optional[Dict[str, Any]] = None
     edge_label_format: str = "{}"
     dx_node: float = 0.2
     dx_arrow: float = 0.1
-    edge_edge_kw: Optional[dict] = None
-    node_edge_kw: Optional[dict] = None
-    edge_fill_kw: Optional[dict] = None
-    node_fill_kw: Optional[dict] = None
+    edge_edge_kw: Optional[Dict[str, Any]] = None
+    node_edge_kw: Optional[Dict[str, Any]] = None
+    edge_fill_kw: Optional[Dict[str, Any]] = None
+    node_fill_kw: Optional[Dict[str, Any]] = None
     debug_visuals: bool = False
     link_color_attribute: Optional[str] = None
 
     def __post_init__(self):
         """Default kwargs in post-init"""
         if self.edge_edge_kw is None:
             self.edge_edge_kw = {"color": "gray"}
@@ -112,15 +114,17 @@
         dy_node = dig.nodes[node]["max_value"]
         plt.plot(
             [x_node, x_node], [y_node - dy_node / 2, y_node + dy_node / 2], color="gray"
         )
 
 
 def cubic_spline_link(
-    x_from_to: np.array = None, y_from_to: np.array = None, n_segments: int = 100
+    x_from_to: Optional[np.ndarray] = None,
+    y_from_to: Optional[np.ndarray] = None,
+    n_segments: int = 100,
 ):
     """Draw a cubic spline with 0 slope from a point to another point
 
     Args:
         x_from_to: a numpy array with two x coordinates
         y_from_to: a numpy array with two x coordinates
         n_segments: number of straight segments with which to draw the spline
@@ -159,16 +163,16 @@
     return node_x, node_y, d_y
 
 
 @dataclass
 class Polyline:
     """A polyline or broken line"""
 
-    x_list: np.array
-    y_list: np.array
+    x_list: List[float]
+    y_list: List[float]
     name: str = ""
     color_attribute_value: Optional[str] = None
 
     @property
     def n_points(self):
         """Number of points"""
         n_x = len(self.x_list)
@@ -231,14 +235,15 @@
             candidate_pline = pline
         elif not pline.start_touches_end(candidate_pline):
             # disjoint polylines: add candidate_pline to list, make new one candidate
             new_plines.append(candidate_pline)
             candidate_pline = pline
         else:
             candidate_pline = pline.append_to(candidate_pline)
+    assert candidate_pline is not None
     new_plines.append(candidate_pline)
     return new_plines
 
 
 def get_polygon(polylines: List[Polyline]) -> Polyline:
     """Concatenate polylines even if their ends do not touch (for filling)"""
     polygon = polylines[0]
@@ -327,15 +332,15 @@
 
 
 @dataclass
 class NodeRepresentation:
     """Geometric representation of a node"""
 
     polylines: List[Polyline]  # edges
-    polygon: Polyline  # filled
+    polygon: Optional[Polyline]  # filled
     label: Optional[Label]
     color_attribute_value: Optional[str] = None
 
     def __post_init__(self):
         col_attr_val = self.color_attribute_value
         if self.polygon is not None and col_attr_val is not None:
             for poly in self.polylines:
@@ -448,17 +453,20 @@
             x_from_to, y_from_to, n_segments=draw_config.n_segments
         )
         y_above = y_below + edge_val
 
     x_fill = np.concatenate([x_below, x_below[::-1]])
     y_fill = np.concatenate([y_below, y_above[::-1]])
 
-    edge_plines = [Polyline(x_below, y_below), Polyline(x_below, y_above)]
+    edge_plines = [
+        Polyline(x_below.tolist(), y_below.tolist()),
+        Polyline(x_below.tolist(), y_above.tolist()),
+    ]
     edge_name = f"{node} -> {next_node}"
-    edge_poly = Polyline(x_fill, y_fill, name=edge_name)
+    edge_poly = Polyline(x_fill.tolist(), y_fill.tolist(), name=edge_name)
 
     dig.nodes[next_node]["y_in"] += edge_val
 
     if draw_config.write_edge_values:
         label_str = draw_config.edge_label_format.format(edge_val)
         edge_label = Label(np.mean(x_fill), np.mean(y_fill), label_str, "edge_label")
     else:
```

### Comparing `sugikey-0.2.0/sugikey/examples.py` & `sugikey-0.2.2/sugikey/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Example data to test and showcase the package"""
 
 import copy
+from typing import Dict
 
 import networkx as nx
 import pandas as pd
 
 
 def balanced_tree(branching_factor: int = 2, height: int = 3):
     """Balanced tree"""
@@ -145,15 +146,15 @@
     iea_df = iea_df_full[iea_df_full["Country"]==country]
     flow_df = translate_iea_energy_balance(iea_df, year)
 
     Args:
         iea_df: a dataframe from the world energy balance highlights dataset
         year: year to visualize
     """
-    flow_dict = {}
+    flow_dict = {}  # type: Dict[str, Dict[str, float]]
     for product, flow, value in zip(iea_df["Product"], iea_df["Flow"], iea_df[year]):
         translate_iea_balance_item(product, flow, value, flow_dict)
 
     flow_df = pd.DataFrame(flow_dict).transpose()
 
     for carrier in [
         "Electricity",
```

### Comparing `sugikey-0.2.0/sugikey/optim.py` & `sugikey-0.2.2/sugikey/optim.py`

 * *Files identical despite different names*

### Comparing `sugikey-0.2.0/sugikey/processing.py` & `sugikey-0.2.2/sugikey/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             dig.edges[(src, target)][col_name] = col_val
 
     calculate_node_values(dig)
 
     return dig
 
 
-def get_df_from_graph(dig) -> pd.DataFrame:
+def get_df_from_graph(dig: nx.DiGraph) -> pd.DataFrame:
     """Return a dataframe from a directed graph
 
     Args:
         dig: a directed graph with edge attribute "value"
 
     Returns:
         a dataframe with columns "source", "target" and "value", one row per flow
@@ -132,15 +132,15 @@
         imbalance = abs(in_value - out_value) / max_value
         if in_value * out_value > 0 and imbalance > 0.05:
             print(
                 f"Imbalanced node {node}: inflow {in_value:.2f} / outflow {out_value:.2f}"
             )
 
 
-def assign_layers(dig: nx.DiGraph, method: LayoutConfig = None):
+def assign_layers(dig: nx.DiGraph, method: Optional[LayoutConfig] = None):
     """Assign nodes to layers by length of longest directed path from each node
 
     This is done recursively.
     Align right: Leaves are in layer 0, parents of leaves are in layer -1 etc.
     Align left: Nodes with no parent are in layer 0, their children are in layer 1 etc.
     Align right justify:
 
@@ -212,15 +212,18 @@
         lay: a string, name of layer
         key_name: an optional string to sort the nodes
 
     Returns:
         a list of strings, names of nodes
     """
     if key_name is None:
-        key_fun = str
+
+        def key_fun(node):
+            return str(node)
+
     else:
 
         def key_fun(nod):
             return dig.nodes[nod][key_name]
 
     layer_nodes = sorted(
         [node for node in dig.nodes if dig.nodes[node]["layer"] == lay],
@@ -506,15 +509,17 @@
                 node_y = dig.nodes[node]["max_value"] / 2
             else:
                 prev_n = layer_nodes[i_ln - 1]
                 node_y += dig.nodes[prev_n]["max_value"] + dig.nodes[node]["max_value"]
             dig.nodes[node]["y"] = node_y
 
 
-def process_directed_graph(dig: nx.DiGraph, layout_config: LayoutConfig = None):
+def process_directed_graph(
+    dig: nx.DiGraph, layout_config: Optional[LayoutConfig] = None
+):
     """Process directed graph to prepare Sankey diagram
 
     Args:
         dig: a directed graph where each node has a "max_value" attribute
         layout_method
     """
```

### Comparing `sugikey-0.2.0/sugikey/sankey.py` & `sugikey-0.2.2/sugikey/sankey.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """High-level functions for Sankey diagrams in one or few lines of code"""
 
+from typing import Optional
+
 import matplotlib
 import networkx as nx
 import pandas as pd
 
 from . import processing
 from . import draw
 
 
 def sankey_from_dig(
     dig: nx.DiGraph,
-    layout_config: processing.LayoutConfig = None,
-    ax: matplotlib.axes.Axes = None,
-    draw_config: draw.DrawConfig = None,
+    layout_config: Optional[processing.LayoutConfig] = None,
+    ax: Optional[matplotlib.axes.Axes] = None,
+    draw_config: Optional[draw.DrawConfig] = None,
 ):
     """Plot Sankey diagram from directed graph
 
     Args:
         dig: a directed graph with edge attribute "value"
         layout_config: layout configuration
         ax: matplotlib axes
@@ -27,17 +29,17 @@
     processing.calculate_node_values(dig)
     processing.process_directed_graph(dig, layout_config)
     draw.draw_sankey(dig, ax, draw_config)
 
 
 def sankey_from_df(
     flow_df: pd.DataFrame,
-    layout_config: processing.LayoutConfig = None,
-    ax: matplotlib.axes.Axes = None,
-    draw_config: draw.DrawConfig = None,
+    layout_config: Optional[processing.LayoutConfig] = None,
+    ax: Optional[matplotlib.axes.Axes] = None,
+    draw_config: Optional[draw.DrawConfig] = None,
 ):
     """Plot Sankey diagram from dataframe
 
     Args:
         flow_df: a dataframe with columns "source", "target" and "value", one row per flow
         layout_config: layout configuration
         ax: matplotlib axes
```

### Comparing `sugikey-0.2.0/PKG-INFO` & `sugikey-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: sugikey
-Version: 0.2.0
+Version: 0.2.2
 Summary: Drawing Sankey diagrams in Python
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bokeh (>=3.1.0,<4.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: bokeh (>=3.4.0,<4.0.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pulp (>=2.7.0,<3.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pulp (>=2.8.0,<3.0.0)
 Requires-Dist: sphinx-material (>=0.0.36,<0.0.37)
 Description-Content-Type: text/markdown
 
 # Sugikey
 
 
 ## Description
@@ -66,14 +65,16 @@
 
 Have a look at the [documentation](https://gitabab.gitlab.io/sugikey/) for more information.
 
 ## More on Sankey diagrams
 
 * [Why Sankey diagrams are so great for understanding energy data](https://medium.com/@spectalizer/why-sankey-diagrams-are-so-great-for-understanding-energy-data-b14649d40890)
 
+* [Sankey diagrams now have the package they deserve](https://medium.com/@spectalizer/sankey-diagrams-now-have-the-new-python-package-they-deserved-68754a0830d3)
+
 ## Support
 
 Write an issue if there is an issue.
 
 
 ## Authors and acknowledgment
 Zlatan B.
```

