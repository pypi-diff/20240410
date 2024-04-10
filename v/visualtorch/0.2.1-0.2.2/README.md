# Comparing `tmp/visualtorch-0.2.1.tar.gz` & `tmp/visualtorch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualtorch-0.2.1.tar", last modified: Sat Mar  2 09:35:14 2024, max compression
+gzip compressed data, was "visualtorch-0.2.2.tar", last modified: Wed Apr 10 15:15:25 2024, max compression
```

## Comparing `visualtorch-0.2.1.tar` & `visualtorch-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 09:35:14.030317 visualtorch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-02 09:35:07.000000 visualtorch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-03-02 09:35:14.030317 visualtorch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-02 09:35:07.000000 visualtorch-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 09:35:14.030317 visualtorch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-02 09:35:07.000000 visualtorch-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 09:35:14.030317 visualtorch-0.2.1/visualtorch/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-02 09:35:07.000000 visualtorch-0.2.1/visualtorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-03-02 09:35:07.000000 visualtorch-0.2.1/visualtorch/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-03-02 09:35:07.000000 visualtorch-0.2.1/visualtorch/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-03-02 09:35:07.000000 visualtorch-0.2.1/visualtorch/layered.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-02 09:35:07.000000 visualtorch-0.2.1/visualtorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 09:35:14.030317 visualtorch-0.2.1/visualtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-03-02 09:35:13.000000 visualtorch-0.2.1/visualtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-02 09:35:13.000000 visualtorch-0.2.1/visualtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 09:35:13.000000 visualtorch-0.2.1/visualtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-02 09:35:13.000000 visualtorch-0.2.1/visualtorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-02 09:35:13.000000 visualtorch-0.2.1/visualtorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:15:25.125809 visualtorch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 15:15:17.000000 visualtorch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-10 15:15:25.125809 visualtorch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-10 15:15:17.000000 visualtorch-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-10 15:15:17.000000 visualtorch-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:15:25.125809 visualtorch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-10 15:15:17.000000 visualtorch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:15:25.125809 visualtorch-0.2.2/visualtorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/layered.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/lenet_style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:15:25.125809 visualtorch-0.2.2/visualtorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-10 15:15:17.000000 visualtorch-0.2.2/visualtorch/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:15:25.125809 visualtorch-0.2.2/visualtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-10 15:15:25.000000 visualtorch-0.2.2/visualtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 15:15:25.000000 visualtorch-0.2.2/visualtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:15:25.000000 visualtorch-0.2.2/visualtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 15:15:25.000000 visualtorch-0.2.2/visualtorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 15:15:25.000000 visualtorch-0.2.2/visualtorch.egg-info/top_level.txt
```

### Comparing `visualtorch-0.2.1/LICENSE` & `visualtorch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `visualtorch-0.2.1/PKG-INFO` & `visualtorch-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Architecture visualization of Torch models
 Home-page: https://github.com/willyfh/visualtorch
 Author: Willy Fitra Hendria
 Author-email: willyfitrahendria@gmail.com
 License: MIT
 Keywords: visualize architecture,torch visualization,visualtorch
 Classifier: Programming Language :: Python :: 3.10
@@ -19,21 +19,21 @@
 <div align="center">
  <h1>🔥 VisualTorch 🔥</h1>
 
 [![python](https://img.shields.io/badge/python-3.10%2B-blue)]() [![pytorch](https://img.shields.io/badge/pytorch-2.0%2B-orange)]() [![Downloads](https://static.pepy.tech/personalized-badge/visualtorch?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/visualtorch) [![Run Tests](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml/badge.svg)](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/visualtorch/badge/?version=latest)](https://visualtorch.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style and graph-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
+**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style, graph-style, and LeNet-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
 
 **Note:** VisualTorch may not yet support complex models, but contributions are welcome!
 
 <div align="center">
 
-![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/7e2c35ea-d34d-4b92-b414-285bccb8576a)
+![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/398c3356-4de0-446b-a30b-d8ebe532d2c2)
 
 </div>
 
 ## Documentation
 
 Online documentation is available at [visualtorch.readthedocs.io](https://visualtorch.readthedocs.io/en/latest/).
```

### Comparing `visualtorch-0.2.1/README.md` & `visualtorch-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <div align="center">
  <h1>🔥 VisualTorch 🔥</h1>
 
 [![python](https://img.shields.io/badge/python-3.10%2B-blue)]() [![pytorch](https://img.shields.io/badge/pytorch-2.0%2B-orange)]() [![Downloads](https://static.pepy.tech/personalized-badge/visualtorch?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/visualtorch) [![Run Tests](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml/badge.svg)](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/visualtorch/badge/?version=latest)](https://visualtorch.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style and graph-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
+**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style, graph-style, and LeNet-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
 
 **Note:** VisualTorch may not yet support complex models, but contributions are welcome!
 
 <div align="center">
 
-![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/7e2c35ea-d34d-4b92-b414-285bccb8576a)
+![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/398c3356-4de0-446b-a30b-d8ebe532d2c2)
 
 </div>
 
 ## Documentation
 
 Online documentation is available at [visualtorch.readthedocs.io](https://visualtorch.readthedocs.io/en/latest/).
```

### Comparing `visualtorch-0.2.1/setup.py` & `visualtorch-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Setup file for visualtorch."""
 
 # Copyright (C) 2024 Willy Fitra Hendria
 # SPDX-License-Identifier: MIT
 
+from pathlib import Path
+
 import setuptools
 
-with open("README.md", "r") as fh:
+file_path = Path("README.md")
+with file_path.open("r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="visualtorch",
-    version="0.2.1",
+    version="0.2.2",
     author="Willy Fitra Hendria",
     author_email="willyfitrahendria@gmail.com",
     description="Architecture visualization of Torch models",
     keywords=["visualize architecture", "torch visualization", "visualtorch"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/willyfh/visualtorch",
```

### Comparing `visualtorch-0.2.1/visualtorch/graph.py` & `visualtorch-0.2.2/visualtorch/graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,206 +1,246 @@
 """Graph View module for pytorch model visualization."""
 
 # Copyright (C) 2024 Willy Fitra Hendria
 # SPDX-License-Identifier: MIT
 
-import aggdraw
-from PIL import Image
+from collections import defaultdict
 from math import ceil
-from .layer_utils import model_to_adj_matrix, add_input_dummy_layer, TARGET_OPS
-from .utils import Circle, Ellipses, get_keys_by_value, Box
+from typing import Any
+
+import aggdraw
 import numpy as np
-from typing import Optional, Dict, Any, Tuple, List
 import torch
+from PIL import Image
+
+from .utils.layer_utils import TARGET_OPS, add_input_dummy_layer, model_to_adj_matrix
+from .utils.utils import Box, Circle, Ellipses, get_keys_by_value
 
 
 def graph_view(
     model: torch.nn.Module,
-    input_shape: Tuple[int, ...],
-    to_file: Optional[str] = None,
-    color_map: Optional[Dict[Any, Any]] = None,
+    input_shape: tuple[int, ...],
+    to_file: str | None = None,
+    color_map: dict[Any, Any] | None = None,
     node_size: int = 50,
-    background_fill: Any = "white",
+    background_fill: str | tuple[int, ...] = "white",
     padding: int = 10,
     layer_spacing: int = 250,
     node_spacing: int = 10,
-    connector_fill: Any = "gray",
+    connector_fill: str | tuple[int, ...] = "gray",
     connector_width: int = 1,
     ellipsize_after: int = 10,
-    inout_as_tensor: bool = True,
     show_neurons: bool = True,
+    opacity: int = 255,
 ) -> Image.Image:
-    """
-    Generates an architecture visualization for a given linear PyTorch model (i.e., one input and output tensor for each
-    layer) in a graph style.
+    """Generates an architecture visualization for a given linear PyTorch model in a graph style.
 
     Args:
         model (torch.nn.Module): A PyTorch model that will be visualized.
         input_shape (tuple): The shape of the input tensor.
         to_file (str, optional): Path to the file to write the created image to. If the image does not exist yet,
             it will be created, else overwritten. Image type is inferred from the file ending. Providing None
             will disable writing.
-        color_map (dict, optional): Dict defining fill and outline for each layer by class type. Will fallback to default
-            values for not specified classes.
+        color_map (dict, optional): Dict defining fill and outline for each layer by class type. Will fallback
+            to default values for not specified classes.
         node_size (int, optional): Size in pixels each node will have.
         background_fill (Any, optional): Color for the image background. Can be str or (R,G,B,A).
         padding (int, optional): Distance in pixels before the first and after the last layer.
         layer_spacing (int, optional): Spacing in pixels between two layers.
         node_spacing (int, optional): Spacing in pixels between nodes.
         connector_fill (Any, optional): Color for the connectors. Can be str or (R,G,B,A).
         connector_width (int, optional): Line-width of the connectors in pixels.
         ellipsize_after (int, optional): Maximum number of neurons per layer to draw. If a layer is exceeding this,
             the remaining neurons will be drawn as ellipses.
-        inout_as_tensor (bool, optional): If True there will be one input and output node for each tensor, else the
-            tensor will be flattened and one node for each scalar will be created (e.g., a (10, 10) shape will be
-            represented by 100 nodes).
         show_neurons (bool, optional): If True a node for each neuron in supported layers is created (constrained by
             ellipsize_after), else each layer is represented by a node.
+        opacity (int, optional): Transparency of the color (0 ~ 255).
 
     Returns:
         Image.Image: Generated architecture image.
     """
-
-    if color_map is None:
-        color_map = dict()
+    _color_map: dict = {}
+    if color_map is not None:
+        _color_map = defaultdict(dict, color_map)
 
     # Iterate over the model to compute bounds and generate boxes
 
-    layers: List[Any] = list()
-    layer_y = list()
-
     # Attach helper layers
 
     id_to_num_mapping, adj_matrix, model_layers = model_to_adj_matrix(
-        model, input_shape
+        model,
+        input_shape,
     )
 
     # Add fake input layers
 
     id_to_num_mapping, adj_matrix, model_layers = add_input_dummy_layer(
-        input_shape, id_to_num_mapping, adj_matrix, model_layers
+        input_shape,
+        id_to_num_mapping,
+        adj_matrix,
+        model_layers,
     )
 
     # Create architecture
 
     current_x = padding  # + input_label_size[0] + text_padding
 
-    id_to_node_list_map = dict()
-
-    for index, layer_list in enumerate(model_layers):
-        current_y = 0
-        nodes = []
-        layer: Any
-        for layer in layer_list:
-            is_box = True
-            units = 1
-
-            if show_neurons:
-                if hasattr(layer, "_saved_bias_sym_sizes_opt"):
-                    is_box = False
-                    units = layer._saved_bias_sym_sizes_opt[0]
-                elif hasattr(layer, "_saved_mat2_sym_sizes"):
-                    is_box = False
-                    units = layer._saved_mat2_sym_sizes[1]
-                elif hasattr(layer, "units"):  # for dummy input layer
-                    is_box = False
-                    units = layer.units
-
-            n = min(units, ellipsize_after)
-            layer_nodes = list()
-
-            for i in range(n):
-                scale = 1
-                c: Box | Circle | Ellipses
-                if not is_box:
-                    if i != ellipsize_after - 2:
-                        c = Circle()
-                    else:
-                        c = Ellipses()
-                else:
-                    c = Box()
-                    scale = 3
-
-                c.x1 = current_x
-                c.y1 = current_y
-                c.x2 = c.x1 + node_size
-                c.y2 = c.y1 + node_size * scale
-
-                current_y = c.y2 + node_spacing
-
-                c.fill = color_map.get(TARGET_OPS[layer.name()], {}).get(
-                    "fill", "#ADD8E6"
-                )
-                c.outline = color_map.get(TARGET_OPS[layer.name()], {}).get(
-                    "outline", "black"
-                )
-
-                layer_nodes.append(c)
-
-            id_to_node_list_map[str(id(layer))] = layer_nodes
-            nodes.extend(layer_nodes)
-            current_y += 2 * node_size
-
-        layer_y.append(current_y - node_spacing - 2 * node_size)
-        layers.append(nodes)
-        current_x += node_size + layer_spacing
+    layers, layer_y, id_to_node_list_map = _create_architecture(
+        model_layers,
+        current_x,
+        show_neurons,
+        ellipsize_after,
+        node_size,
+        node_spacing,
+        _color_map,
+        opacity,
+        layer_spacing,
+    )
 
     # Generate image
 
-    img_width = (
-        len(layers) * node_size + (len(layers) - 1) * layer_spacing + 2 * padding
-    )
+    img_width = len(layers) * node_size + (len(layers) - 1) * layer_spacing + 2 * padding
     img_height = max(*layer_y) + 2 * padding
     img = Image.new(
-        "RGBA", (int(ceil(img_width)), int(ceil(img_height))), background_fill
+        "RGBA",
+        (int(ceil(img_width)), int(ceil(img_height))),
+        background_fill,
     )
 
     draw = aggdraw.Draw(img)
 
     # y correction (centering)
     for i, layer in enumerate(layers):
         y_off = (img.height - layer_y[i]) / 2
         node: Any
         for node in layer:
             node.y1 += y_off
             node.y2 += y_off
 
-    for start_idx, end_idx in zip(*np.where(adj_matrix > 0)):
+    for start_idx, end_idx in zip(*np.where(adj_matrix > 0), strict=False):
         start_id = next(get_keys_by_value(id_to_num_mapping, start_idx))
         end_id = next(get_keys_by_value(id_to_num_mapping, end_idx))
 
         start_layer_list = id_to_node_list_map[start_id]
         end_layer_list = id_to_node_list_map[end_id]
 
         # draw connectors
-        for start_node_idx, start_node in enumerate(start_layer_list):
+        for start_node in start_layer_list:
             for end_node in end_layer_list:
                 if not isinstance(start_node, Ellipses) and not isinstance(
-                    end_node, Ellipses
+                    end_node,
+                    Ellipses,
                 ):
                     _draw_connector(
                         draw,
                         start_node,
                         end_node,
                         color=connector_fill,
                         width=connector_width,
                     )
 
-    for i, layer in enumerate(layers):
-        for node_index, node in enumerate(layer):
+    for layer in layers:
+        for node in layer:
             node.draw(draw)
 
     draw.flush()
 
     if to_file is not None:
         img.save(to_file)
 
     return img
 
 
-def _draw_connector(draw, start_node, end_node, color, width):
+def _draw_connector(
+    draw: aggdraw.Draw,
+    start_node: Box | Circle | Ellipses,
+    end_node: Box | Circle | Ellipses,
+    color: str | tuple[int, ...],
+    width: int,
+) -> None:
+    """Draw the line connector between nodes."""
     pen = aggdraw.Pen(color, width)
     x1 = start_node.x2
     y1 = start_node.y1 + (start_node.y2 - start_node.y1) / 2
     x2 = end_node.x1
     y2 = end_node.y1 + (end_node.y2 - end_node.y1) / 2
     draw.line([x1, y1, x2, y2], pen)
+
+
+def _retrieve_isbox_units(layer: torch.autograd.Function, show_neurons: bool) -> tuple[bool, int]:
+    """Return the number of units and the flag whether to visualize using a box or not."""
+    print("test: ", type(layer))
+    is_box = True
+    units = 1
+    if show_neurons:
+        if hasattr(layer, "_saved_bias_sym_sizes_opt"):
+            is_box = False
+            units = layer._saved_bias_sym_sizes_opt[0]  # noqa: SLF001
+        elif hasattr(layer, "_saved_mat2_sym_sizes"):
+            is_box = False
+            units = layer._saved_mat2_sym_sizes[1]  # noqa: SLF001
+        elif hasattr(layer, "units"):  # for dummy input layer
+            is_box = False
+            units = layer.units
+    return is_box, units
+
+
+def _create_architecture(
+    model_layers: list[list],
+    current_x: int,
+    show_neurons: bool,
+    ellipsize_after: int,
+    node_size: int,
+    node_spacing: int,
+    color_map: dict[Any, Any],
+    opacity: int,
+    layer_spacing: int,
+) -> tuple[list, list, dict]:
+    """Create nodes of architecture for each layers."""
+    id_to_node_list_map = {}
+    layers = []
+    layer_y = []
+    for layer_list in model_layers:
+        current_y = 0
+        nodes = []
+        layer: Any
+        for layer in layer_list:
+            is_box, units = _retrieve_isbox_units(layer, show_neurons)
+
+            n = min(units, ellipsize_after)
+            layer_nodes = []
+
+            for i in range(n):
+                scale = 1
+                c: Box | Circle | Ellipses
+                if not is_box:
+                    c = Circle() if i != ellipsize_after - 2 else Ellipses()
+                else:
+                    c = Box()
+                    scale = 3
+
+                c.x1 = current_x
+                c.y1 = current_y
+                c.x2 = c.x1 + node_size
+                c.y2 = c.y1 + node_size * scale
+
+                current_y = c.y2 + node_spacing
+
+                c.set_fill(
+                    color_map.get(TARGET_OPS[layer.name()], {}).get("fill", "#ADD8E6"),
+                    opacity,
+                )
+                c.outline = color_map.get(TARGET_OPS[layer.name()], {}).get(
+                    "outline",
+                    "black",
+                )
+
+                layer_nodes.append(c)
+
+            id_to_node_list_map[str(id(layer))] = layer_nodes
+            nodes.extend(layer_nodes)
+            current_y += 2 * node_size
+
+        layer_y.append(current_y - node_spacing - 2 * node_size)
+        layers.append(nodes)
+        current_x += node_size + layer_spacing
+    return layers, layer_y, id_to_node_list_map
```

### Comparing `visualtorch-0.2.1/visualtorch/layer_utils.py` & `visualtorch-0.2.2/visualtorch/utils/layer_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,88 @@
 """Layer Utils module for pytorch model visualization."""
 
 # Copyright (C) 2024 Willy Fitra Hendria
 # SPDX-License-Identifier: MIT
 
-import numpy as np
+from collections import OrderedDict, defaultdict
+from typing import Any
 
+import numpy as np
 import torch
-import torch.nn as nn
+from torch import nn
 
 from .utils import get_keys_by_value
 
-from typing import Tuple, Dict, List, Any
-
-from collections import defaultdict
-
 # WARNING: currently, graph visualization relying on following operations,
 # thereby only linear and convolutional layers are supported.
-# TODO: implement a more dynamic/better approach to support all layers
+# We need to implement a more dynamic/better approach to support all layers
 TARGET_OPS = defaultdict(
-    lambda: None, {"AddmmBackward0": nn.Linear, "ConvolutionBackward0": nn.Conv2d}
+    lambda: None,
+    {"AddmmBackward0": nn.Linear, "ConvolutionBackward0": nn.Conv2d},
 )
 
 
 class SpacingDummyLayer(nn.Module):
-    def __init__(self, spacing: int = 50):
+    """A dummy layer to add spacing."""
+
+    def __init__(self, spacing: int = 50) -> None:
         super().__init__()
         self.spacing = spacing
 
 
 class InputDummyLayer:
-    def __init__(self, name, units=None):
+    """A dummy layer for input."""
+
+    def __init__(self, name: str, units: int | None = None) -> None:
         if units:
             self.units = units
         self._name = name
 
-    def name(self):
+    def name(self) -> str:
+        """Return layer name"""
         return self._name
 
 
 def model_to_adj_matrix(
-    model, input_shape
-) -> Tuple[Dict[str, int], np.ndarray, List[List[torch.nn.Module]]]:
-    """
-    Extract adjacency matrix representation from a pytorch model.
+    model: nn.Module | nn.Sequential,
+    input_shape: tuple[int, ...],
+) -> tuple[dict[str, int], np.ndarray, list[list[torch.nn.Module]]]:
+    """Extract adjacency matrix representation from a pytorch model.
 
     Args:
         model: PyTorch model.
         input_shape (tuple): The shape of the input tensor expected by the model, including batch dim.
 
     Returns:
         tuple: A tuple containing:
-            - id_to_index_adj_mapping (dict): Mapping from node IDs to their corresponding index in the adjacency matrix.
-            - adjacency_matrix (numpy.ndarray): The adjacency matrix representing connections between model operations/layers.
+            - id_to_index_adj_mapping (dict): Mapping from node IDs to their corresponding index in
+                the adjacency matrix.
+            - adjacency_matrix (numpy.ndarray): The adjacency matrix representing connections between
+                model operations/layers.
             - model_layers (list): List of model layers organized by their hierarchy.
     """
     dummy_input = torch.rand(input_shape)
     output_var = model(dummy_input)
 
-    nodes = []
-    edges = []
-    id_to_ops = {}
+    nodes: list = []
+    edges: list = []
+    id_to_ops: dict = {}
 
     max_level = [0]
     max_level_id = [""]
 
-    def add_nodes(fn, source=None, level=0):
-        assert not torch.is_tensor(fn)
-
-        if str(type(fn).__name__) in TARGET_OPS.keys():
-            node_id = str(id(fn))
-            id_to_ops[node_id] = fn
-            if node_id not in nodes:
-                nodes.append(node_id)
-            level += 1
-            if level > max_level[0]:
-                max_level[0] = level
-                max_level_id[0] = node_id
-
-            edges.append((node_id, source))
-            source = node_id
-
-        # recurse
-        if hasattr(fn, "next_functions"):
-            for u in fn.next_functions:
-                if u[0] is not None:
-                    add_nodes(u[0], source, level)
-
-    def add_base_tensor(var):
-        if var.grad_fn:
-            add_nodes(var.grad_fn)
-
-        if var._is_view():
-            add_base_tensor(var._base)
-
     # Extract nodes and edges for the target ops
     # Currently only the ones in the TARGET_OPS are supported.
 
     # handle multiple outputs
     if isinstance(output_var, tuple):
         for v in output_var:
-            add_base_tensor(v)
+            _add_base_tensor(v, id_to_ops, nodes, edges, max_level, max_level_id)
     else:
-        add_base_tensor(output_var)
+        _add_base_tensor(output_var, id_to_ops, nodes, edges, max_level, max_level_id)
 
     # Create adjacency matrix
     adjacency_matrix = np.zeros((len(nodes), len(nodes)))
     id_to_index_adj_mapping = {node: idx for idx, node in enumerate(nodes)}
 
     for src_id, trg_id in edges:
         if trg_id is not None:
@@ -126,50 +103,138 @@
                 trg_id = next(get_keys_by_value(id_to_index_adj_mapping, trg_idx))
                 new_layer.append(trg_id)
 
         temp_model_layers.append(list(new_layer))
 
     # Filter duplicate layers
     seen = set()
-    model_layers: List[List] = []
+    model_layers: list[list] = []
     for i in range(len(temp_model_layers) - 1, -1, -1):
         new_layers = []
         for layer_id in temp_model_layers[i]:
             if layer_id in seen:
                 continue
             seen.add(layer_id)
             new_layers.append(id_to_ops[layer_id])
         model_layers.insert(0, list(new_layers))
 
     return id_to_index_adj_mapping, adjacency_matrix, model_layers
 
 
 def add_input_dummy_layer(
-    input_shape: Tuple[int, ...],
-    id_to_num_mapping: Dict[str, int],
+    input_shape: tuple[int, ...],
+    id_to_num_mapping: dict[str, int],
     adj_matrix: np.ndarray,
-    model_layers: List[List[Any]],
-) -> Tuple[Dict[str, int], np.ndarray, List[List[str]]]:
-    """
-    Add an input dummy layer to the model layers and update the adjacency matrix accordingly.
+    model_layers: list[list[Any]],
+) -> tuple[dict[str, int], np.ndarray, list[list[str]]]:
+    """Add an input dummy layer to the model layers and update the adjacency matrix accordingly.
 
     Args:
         input_shape (tuple): The shape of the input tensor.
         id_to_num_mapping (dict): Mapping from node IDs to their corresponding index in the adjacency matrix.
         adj_matrix (numpy.ndarray): The adjacency matrix representing connections between model operations.
         model_layers (list): List of model layers organized by their dependencies.
 
     Returns:
         tuple: A tuple containing:
-            - id_to_num_mapping (dict): Updated mapping from node IDs to their corresponding index in the adjacency matrix.
+            - id_to_num_mapping (dict): Updated mapping from node IDs to their corresponding index in
+                the adjacency matrix.
             - adj_matrix (numpy.ndarray): Updated adjacency matrix.
             - model_layers (list): Updated list of model layers with the input dummy layer.
     """
     first_hidden_layer = model_layers[0][0]
     input_dummy_layer = InputDummyLayer("input", input_shape[1])
     model_layers.insert(0, [input_dummy_layer])
     id_to_num_mapping[str(id(input_dummy_layer))] = len(id_to_num_mapping.keys())
     adj_matrix = np.pad(
-        adj_matrix, ((0, 1), (0, 1)), mode="constant", constant_values=0
+        adj_matrix,
+        ((0, 1), (0, 1)),
+        mode="constant",
+        constant_values=0,
     )
     adj_matrix[-1, id_to_num_mapping[str(id(first_hidden_layer))]] += 1
     return id_to_num_mapping, adj_matrix, model_layers
+
+
+def register_hook(
+    model: nn.Module,
+    module: nn.Module,
+    hooks: list,
+    layers: OrderedDict,
+) -> None:
+    """Registers a forward hook on the specified module and collects the module and the output shapes.
+
+    Args:
+        model (nn.Module): The parent model.
+        module (nn.Module): The module to register the hook on.
+        hooks (List): A list to store the registered hooks.
+        layers (OrderedDict): An OrderedDict to store information about the registered modules and output shapes.
+
+    Returns:
+        None
+    """
+
+    def hook(
+        module: nn.Module,
+        _: tuple[torch.Tensor],
+        out: torch.Tensor,
+    ) -> None:
+        class_name = str(module.__class__).split(".")[-1].split("'")[0]
+        module_idx = len(layers)
+
+        m_key = "%s-%i" % (class_name, module_idx + 1)
+        layers[m_key] = OrderedDict()
+        layers[m_key]["module"] = module
+        if isinstance(out, list | tuple):
+            layers[m_key]["output_shape"] = tuple((-1,) + o.size()[1:] for o in out)
+        else:
+            layers[m_key]["output_shape"] = out.size()
+
+    if not isinstance(module, nn.Sequential) and not isinstance(module, nn.ModuleList) and module is not model:
+        hooks.append(module.register_forward_hook(hook))
+
+
+def _add_nodes(
+    fn: torch.autograd.function,
+    id_to_ops: dict,
+    nodes: list,
+    edges: list,
+    max_level: list[int],
+    max_level_id: list[str],
+    source: str | None = None,
+    level: int = 0,
+) -> None:
+    assert not torch.is_tensor(fn)
+
+    if str(type(fn).__name__) in TARGET_OPS:
+        node_id = str(id(fn))
+        id_to_ops[node_id] = fn
+        if node_id not in nodes:
+            nodes.append(node_id)
+        level += 1
+        if level > max_level[0]:
+            max_level[0] = level
+            max_level_id[0] = node_id
+
+        edges.append((node_id, source))
+        source = node_id
+
+    # recurse
+    if hasattr(fn, "next_functions"):
+        for u in fn.next_functions:
+            if u[0] is not None:
+                _add_nodes(u[0], id_to_ops, nodes, edges, max_level, max_level_id, source, level)
+
+
+def _add_base_tensor(
+    var: torch.Tensor,
+    id_to_ops: dict,
+    nodes: list,
+    edges: list,
+    max_level: list[int],
+    max_level_id: list[str],
+) -> None:
+    if var.grad_fn:
+        _add_nodes(var.grad_fn, id_to_ops, nodes, edges, max_level, max_level_id)
+
+    if var._is_view():  # noqa: SLF001
+        _add_base_tensor(var._base, id_to_ops, nodes, edges, max_level, max_level_id)  # noqa: SLF001
```

### Comparing `visualtorch-0.2.1/visualtorch/layered.py` & `visualtorch-0.2.2/visualtorch/layered.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,114 @@
 """Layered View module for pytorch model visualization."""
 
 # Copyright (C) 2024 Willy Fitra Hendria
 # SPDX-License-Identifier: MIT
 
-from PIL import ImageFont
+from collections import OrderedDict, defaultdict
 from math import ceil
-from typing import Any, List
-from .utils import (
-    self_multiply,
-    linear_layout,
-    vertical_image_concat,
-    ColorWheel,
-    Box,
-    get_rgba_tuple,
-    ImageDraw,
-    register_hook,
-)
-from .layer_utils import SpacingDummyLayer
+from typing import Any
 
 import aggdraw
 import PIL
 import torch
-import torch.nn as nn
-from PIL import Image
+from PIL import Image, ImageFont
+from torch import nn
 
-from collections import OrderedDict
+from .utils.layer_utils import SpacingDummyLayer, register_hook
+from .utils.utils import (
+    Box,
+    ColorWheel,
+    ImageDraw,
+    get_rgba_tuple,
+    linear_layout,
+    self_multiply,
+    vertical_image_concat,
+)
 
 
 def layered_view(
-    model,
-    input_shape,
+    model: nn.Module | nn.Sequential | nn.ModuleList,
+    input_shape: tuple[int, ...],
     to_file: str | None = None,
     min_z: int = 10,
     min_xy: int = 10,
     max_z: int = 400,
     max_xy: int = 2000,
     scale_z: float = 0.1,
     scale_xy: float = 1,
     type_ignore: list | None = None,
     index_ignore: list | None = None,
     color_map: dict | None = None,
     one_dim_orientation: str = "z",
-    background_fill: Any = "white",
+    background_fill: str | tuple[int, ...] = "white",
     draw_volume: bool = True,
     padding: int = 10,
     spacing: int = 10,
     draw_funnel: bool = True,
-    shade_step=10,
+    shade_step: int = 10,
     legend: bool = False,
     font: ImageFont = None,
-    font_color: Any = "black",
+    font_color: str | tuple[int, ...] = "black",
+    opacity: int = 255,
 ) -> PIL.Image:
-    """
-    Generate a layered architecture visualization for a given linear torch model (i.e., one input and output tensor for each
-    layer), suitable for Convolutional Neural Networks (CNNs).
+    """Generate a layered architecture visualization for a given torch model.
 
     Args:
         model (torch.nn.Module): A torch model that will be visualized.
         input_shape (tuple): The shape of the input tensor (default: (1, 3, 224, 224)).
-        to_file (str, optional): Path to the file to write the created image. If the image exists, it will be overwritten.
+        to_file (str, optional): Path to the file to write the created image. Overwrite if exist.
             Image type is inferred from the file extension. Providing None will disable writing.
         min_z (int, optional): Minimum size in pixels that a layer will have along the z-axis.
         min_xy (int, optional): Minimum size in pixels that a layer will have along the x and y axes.
         max_z (int, optional): Maximum size in pixels that a layer will have along the z-axis.
         max_xy (int, optional): Maximum size in pixels that a layer will have along the x and y axes.
         scale_z (float, optional): Scalar multiplier for the size of each layer along the z-axis.
         scale_xy (float, optional): Scalar multiplier for the size of each layer along the x and y axes.
         type_ignore (list, optional): List of layer types in the torch model to ignore during drawing.
         index_ignore (list, optional): List of layer indexes in the torch model to ignore during drawing.
         color_map (dict, optional): Dictionary defining fill and outline colors for each layer by class type.
             Will fallback to default values for unspecified classes.
-        one_dim_orientation (str, optional): Axis on which one-dimensional layers should be drawn. Can be 'x', 'y', or 'z'.
-        background_fill (str or tuple, optional): Background color for the image. Can be a string or a tuple (R, G, B, A).
+        one_dim_orientation (str, optional): Axis on which one-dim layers should be drawn. E.g., 'x', 'y', or 'z'.
+        background_fill (str or tuple, optional): Background color for the image. A string or a tuple (R, G, B, A).
         draw_volume (bool, optional): Flag to switch between 3D volumetric view and 2D box view.
         padding (int, optional): Distance in pixels before the first and after the last layer.
         spacing (int, optional): Spacing in pixels between two layers.
         draw_funnel (bool, optional): If True, a funnel will be drawn between consecutive layers.
         shade_step (int, optional): Deviation in lightness for drawing shades (only in volumetric view).
         legend (bool, optional): Add a legend of the layers to the image.
-        font (PIL.ImageFont, optional): Font that will be used for the legend. Leaving this as None will use the default font.
+        font (PIL.ImageFont, optional): Font that will be used for the legend. If None, default font will be used.
         font_color (str or tuple, optional): Color for the font if used. Can be a string or a tuple (R, G, B, A).
+        opacity (int): Transparency of the color (0 ~ 255).
 
     Returns:
         PIL.Image: An Image object representing the generated architecture visualization.
     """
-
     # Iterate over the model to compute bounds and generate boxes
 
-    boxes = list()
-    layer_y = list()
-    color_wheel = ColorWheel()
-    current_z = padding
     x_off = -1
 
-    layer_types = list()
-
     img_height = 0
     max_right = 0
 
     if type_ignore is None:
-        type_ignore = list()
+        type_ignore = []
 
     if index_ignore is None:
-        index_ignore = list()
+        index_ignore = []
 
-    if color_map is None:
-        color_map = dict()
+    _color_map: dict = {}
+    if color_map is not None:
+        _color_map = defaultdict(dict, color_map)
 
     dummy_input = torch.rand(*input_shape)
 
     # Get the list of layers
-    # all_layers = get_layers(model)
 
     layers: OrderedDict[str, Any] = OrderedDict()
-    hooks: List[Any] = []
+    hooks: list[Any] = []
 
     model.apply(lambda module: register_hook(model, module, hooks, layers))
 
     with torch.no_grad():
         if isinstance(model, nn.ModuleList):
             output = dummy_input
             for layer in model:
@@ -125,90 +116,42 @@
         else:
             output = model(dummy_input)
 
     # remove these hooks
     for h in hooks:
         h.remove()
 
-    for index, key in enumerate(layers):
-        layer = layers[key]["module"]
-        shape = layers[key]["output_shape"]
-        # Do no render the SpacingDummyLayer, just increase the pointer
-        if type(layer) == SpacingDummyLayer:
-            current_z += layer.spacing
-            continue
-
-        # Ignore layers that the use has opted out to
-        if type(layer) in type_ignore or index in index_ignore:
-            continue
-
-        layer_type = type(layer)
-
-        if layer_type not in layer_types:
-            layer_types.append(layer_type)
-
-        x = min_xy
-        y = min_xy
-        z = min_z
-
-        shape = shape[1:]  # drop batch size
-
-        if len(shape) == 1:
-            if one_dim_orientation in ["x", "y", "z"]:
-                shape = (1,) * "cxyz".index(one_dim_orientation) + shape
-            else:
-                raise ValueError(f"unsupported orientation: {one_dim_orientation}")
-
-        shape = shape + (1,) * (4 - len(shape))  # expand 4D.
-
-        x = min(max(shape[1] * scale_xy, x), max_xy)
-        y = min(max(shape[2] * scale_xy, y), max_xy)
-        z = min(max(int(self_multiply(shape[0:1] + shape[3:]) * scale_z), z), max_z)
-
-        box = Box()
-
-        box.de = 0
-        if draw_volume:
-            box.de = int(x / 3)
-
-        if x_off == -1:
-            x_off = int(box.de / 2)
-
-        # top left coordinate
-        box.x1 = current_z - int(box.de / 2)
-        box.y1 = box.de
-
-        # bottom right coordinate
-        box.x2 = box.x1 + z
-        box.y2 = box.y1 + y
-
-        box.fill = color_map.get(layer_type, {}).get(
-            "fill", color_wheel.get_color(layer_type)
-        )
-        box.outline = color_map.get(layer_type, {}).get("outline", "black")
-        color_map[layer_type] = {"fill": box.fill, "outline": box.outline}
-
-        box.shade = shade_step
-        boxes.append(box)
-        layer_y.append(box.y2 - (box.y1 - box.de))
-
-        # Update image bounds
-        hh = box.y2 - (box.y1 - box.de)
-        if hh > img_height:
-            img_height = hh
-
-        if box.x2 + box.de > max_right:
-            max_right = box.x2 + box.de
-
-        current_z += z + spacing
+    layer_y, layer_types, boxes, x_off, img_height, max_right = _create_architecture(
+        layers,
+        x_off,
+        img_height,
+        max_right,
+        type_ignore,
+        index_ignore,
+        min_xy,
+        min_z,
+        one_dim_orientation,
+        scale_xy,
+        max_xy,
+        scale_z,
+        max_z,
+        draw_volume,
+        shade_step,
+        spacing,
+        _color_map,
+        opacity,
+        padding,
+    )
 
     # Generate image
     img_width = max_right + x_off + padding
     img = Image.new(
-        "RGBA", (int(ceil(img_width)), int(ceil(img_height))), background_fill
+        "RGBA",
+        (int(ceil(img_width)), int(ceil(img_height))),
+        background_fill,
     )
     draw = aggdraw.Draw(img)
 
     # x, y correction (centering)
     for i, node in enumerate(boxes):
         y_off = (img.height - layer_y[i]) / 2
         node.y1 += y_off
@@ -263,15 +206,15 @@
         text_height = font.getbbox("Ag")[3]
         cube_size = text_height
 
         de = 0
         if draw_volume:
             de = cube_size // 2
 
-        patches = list()
+        patches = []
 
         for layer_type in layer_types:
             label = layer_type.__name__
             text_size = font.getbbox(label)
             label_patch_size = (cube_size + de + spacing + text_size[2], cube_size + de)
             # this only works if cube_size is bigger than text height
 
@@ -283,22 +226,20 @@
             box = Box()
             box.x1 = 0
             box.x2 = box.x1 + cube_size
             box.y1 = de
             box.y2 = box.y1 + cube_size
             box.de = de
             box.shade = shade_step
-            box.fill = color_map.get(layer_type, {}).get("fill", "#000000")
-            box.outline = color_map.get(layer_type, {}).get("outline", "#000000")
+            box.set_fill(_color_map.get(layer_type, {}).get("fill", "#000000"), opacity)
+            box.outline = _color_map.get(layer_type, {}).get("outline", "#000000")
             box.draw(draw_box)
 
             text_x = box.x2 + box.de + spacing
-            text_y = (
-                label_patch_size[1] - text_height
-            ) / 2  # 2D center; use text_height and not the current label!
+            text_y = (label_patch_size[1] - text_height) / 2  # 2D center; use text_height and not the current label!
             draw_text.text((text_x, text_y), label, font=font, fill=font_color)
 
             draw_box.flush()
             img_box.paste(img_text, mask=img_text)
             patches.append(img_box)
 
         legend_image = linear_layout(
@@ -312,7 +253,114 @@
         )
         img = vertical_image_concat(img, legend_image, background_fill=background_fill)
 
     if to_file is not None:
         img.save(to_file)
 
     return img
+
+
+def _create_architecture(
+    layers: OrderedDict[str, Any],
+    x_off: int,
+    img_height: int,
+    max_right: int,
+    type_ignore: list,
+    index_ignore: list,
+    min_xy: int,
+    min_z: int,
+    one_dim_orientation: str,
+    scale_xy: float,
+    max_xy: int,
+    scale_z: float,
+    max_z: int,
+    draw_volume: bool,
+    shade_step: int,
+    spacing: int,
+    color_map: dict,
+    opacity: int,
+    padding: int,
+) -> tuple:
+    boxes = []
+    layer_types = []
+    layer_y = []
+    color_wheel = ColorWheel()
+    current_z = padding
+
+    for index, key in enumerate(layers):
+        layer = layers[key]["module"]
+        shape = layers[key]["output_shape"]
+        # Do no render the SpacingDummyLayer, just increase the pointer
+        if type(layer) == SpacingDummyLayer:
+            current_z += layer.spacing
+            continue
+
+        # Ignore layers that the use has opted out to
+        if type(layer) in type_ignore or index in index_ignore:
+            continue
+
+        layer_type = type(layer)
+
+        if layer_type not in layer_types:
+            layer_types.append(layer_type)
+
+        x = min_xy
+        y = min_xy
+        z = min_z
+
+        shape = shape[1:]  # drop batch size
+
+        if len(shape) == 1:
+            if one_dim_orientation in ["x", "y", "z"]:
+                shape = (1,) * "cxyz".index(one_dim_orientation) + shape
+            else:
+                error_msg = f"unsupported orientation: {one_dim_orientation}"
+                raise ValueError(error_msg)
+
+        shape = shape + (1,) * (4 - len(shape))  # expand 4D.
+
+        x = min(max(shape[1] * scale_xy, x), max_xy)
+        y = min(max(shape[2] * scale_xy, y), max_xy)
+        z = min(max(int(self_multiply(shape[0:1] + shape[3:]) * scale_z), z), max_z)
+
+        box = Box()
+
+        box.de = 0
+        if draw_volume:
+            box.de = int(x / 3)
+
+        if x_off == -1:
+            x_off = int(box.de / 2)
+
+        # top left coordinate
+        box.x1 = current_z - int(box.de / 2)
+        box.y1 = box.de
+
+        # bottom right coordinate
+        box.x2 = box.x1 + z
+        box.y2 = box.y1 + y
+
+        box.set_fill(
+            color_map.get(layer_type, {}).get(
+                "fill",
+                color_wheel.get_color(layer_type),
+            ),
+            opacity,
+        )
+        box.outline = color_map.get(layer_type, {}).get("outline", "black")
+        color_map[layer_type] = {"fill": box.fill, "outline": box.outline}
+
+        box.shade = shade_step
+        boxes.append(box)
+        layer_y.append(box.y2 - (box.y1 - box.de))
+
+        # Update image bounds
+        hh = box.y2 - (box.y1 - box.de)
+        if hh > img_height:
+            img_height = hh
+
+        if box.x2 + box.de > max_right:
+            max_right = box.x2 + box.de
+
+        current_z += z + spacing
+
+    return layer_y, layer_types, boxes, x_off, img_height, max_right
```

### Comparing `visualtorch-0.2.1/visualtorch/utils.py` & `visualtorch-0.2.2/visualtorch/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,114 @@
 """Utils module for pytorch model visualization."""
 
 # Copyright (C) 2024 Willy Fitra Hendria
 # SPDX-License-Identifier: MIT
 
-from typing import Any, Dict
-from PIL import ImageColor, ImageDraw, Image
+from collections.abc import Generator
+from typing import Any
+
 import aggdraw
 import PIL
-import torch
-import torch.nn as nn
-from collections import OrderedDict
-from typing import List, Tuple
+from PIL import Image, ImageColor, ImageDraw
+
 
+class Shape:
+    """Base class for shapes"""
 
-class RectShape:
-    def __init__(self):
+    def __init__(self) -> None:
         self.x1 = 0
         self.x2 = 0
         self.y1 = 0
         self.y2 = 0
-        self._fill = None
-        self._outline = None
+        self._fill = ()
+        self._outline = ()
 
     @property
-    def fill(self):
+    def fill(self) -> tuple:
+        """Return the fill color."""
         return self._fill
 
-    @fill.setter
-    def fill(self, v):
-        self._fill = get_rgba_tuple(v)
+    def set_fill(self, color: str | tuple, opacity: int) -> None:
+        """Set color and opacity.
+
+        Args:
+            color (Any): The color representation, i.e., rbg, hex, or color name.
+            opacity (int): The transparency of the color (0 ~ 255).
+
+        Returns:
+            None
+        """
+        self._fill = get_rgba_tuple(color, opacity)
 
     @property
-    def outline(self):
+    def outline(self) -> tuple:
+        """Return the outline/border color."""
         return self._outline
 
     @outline.setter
-    def outline(self, v):
+    def outline(self, v: str | tuple) -> None:
         self._outline = get_rgba_tuple(v)
 
-    def _get_pen_brush(self):
+    def _get_pen_brush(self) -> tuple:
+        """Get aggdraw pen and brush"""
         pen = aggdraw.Pen(self._outline)
         brush = aggdraw.Brush(self._fill)
         return pen, brush
 
 
-class Box(RectShape):
+class StackedBox(Shape):
+    """Stacked Box shape class."""
+
     de: int
     shade: int
+    offset_z: int
+    label: str
+    output_shape: tuple
 
-    def draw(self, draw: ImageDraw):
+    def draw(self, draw: ImageDraw) -> None:
+        """Draw box shape."""
         pen, brush = self._get_pen_brush()
 
         if hasattr(self, "de") and self.de > 0:
-            brush_s1 = aggdraw.Brush(fade_color(self.fill, self.shade))
-            brush_s2 = aggdraw.Brush(fade_color(self.fill, 2 * self.shade))
+            brush_s2 = aggdraw.Brush(_fade_color(self.fill, 4 * self.shade))
+
+            # Calculate initial offset
+            offset = -self.offset_z * self.de // 2
+
+            # Define initial brush
+            brush_choice = brush_s2 if self.de % 2 == 0 else brush
+
+            # Loop through each iteration
+            for _ in range(self.de):
+                draw.rectangle(
+                    [self.x1 + offset, self.y1 + offset, self.x2 + offset, self.y2 + offset],
+                    pen,
+                    brush_choice,
+                )
+                offset += self.offset_z
+                # Switch brush
+                brush_choice = brush_s2 if brush_choice is brush else brush
+
+        else:
+            draw.rectangle([self.x1, self.y1, self.x2, self.y2], pen, brush)
+
+
+class Box(Shape):
+    """Box shape class."""
+
+    de: int
+    shade: int
+
+    def draw(self, draw: ImageDraw) -> None:
+        """Draw box shape."""
+        pen, brush = self._get_pen_brush()
+
+        if hasattr(self, "de") and self.de > 0:
+            brush_s1 = aggdraw.Brush(_fade_color(self.fill, self.shade))
+            brush_s2 = aggdraw.Brush(_fade_color(self.fill, 2 * self.shade))
 
             draw.line(
                 [
                     self.x1 + self.de,
                     self.y1 - self.de,
                     self.x1 + self.de,
                     self.y2 - self.de,
@@ -104,22 +155,28 @@
                 pen,
                 brush_s2,
             )
 
         draw.rectangle([self.x1, self.y1, self.x2, self.y2], pen, brush)
 
 
-class Circle(RectShape):
-    def draw(self, draw: ImageDraw):
+class Circle(Shape):
+    """Circle shape class."""
+
+    def draw(self, draw: ImageDraw) -> None:
+        """Draw circle shape."""
         pen, brush = self._get_pen_brush()
         draw.ellipse([self.x1, self.y1, self.x2, self.y2], pen, brush)
 
 
-class Ellipses(RectShape):
-    def draw(self, draw: ImageDraw):
+class Ellipses(Shape):
+    """Ellipses shape class."""
+
+    def draw(self, draw: ImageDraw) -> None:
+        """Draw ellipses shape."""
         pen, brush = self._get_pen_brush()
         w = self.x2 - self.x1
         d = int(w / 7)
         draw.ellipse(
             [
                 self.x1 + (w - d) / 2,
                 self.y1 + 1 * d,
@@ -148,67 +205,67 @@
             ],
             pen,
             brush,
         )
 
 
 class ColorWheel:
-    def __init__(self, colors: list | None = None):
-        self._cache: Dict[type, Any] = dict()
-        self.colors = (
-            colors
-            if colors is not None
-            else ["#FFE4B5", "#ADD8E6", "#98FB98", "#FFA07A", "#D8BFD8"]
-        )
+    """Default colors for the shapes."""
 
-    def get_color(self, class_type: type):
-        if class_type not in self._cache.keys():
+    def __init__(self, colors: list | None = None) -> None:
+        self._cache: dict[type, Any] = {}
+        self.colors = colors if colors is not None else ["#FFE4B5", "#ADD8E6", "#98FB98", "#FFA07A", "#D8BFD8"]
+
+    def get_color(self, class_type: type) -> tuple | None:
+        """Return color from cache if exist, if not, get from the list and store it to the cache."""
+        if class_type not in self._cache:
             index = len(self._cache.keys()) % len(self.colors)
             self._cache[class_type] = self.colors[index]
         return self._cache.get(class_type)
 
 
-def fade_color(color: tuple, fade_amount: int) -> tuple:
+def _fade_color(color: tuple, fade_amount: int) -> tuple:
+    """To create shadow effect."""
     r = max(0, color[0] - fade_amount)
     g = max(0, color[1] - fade_amount)
     b = max(0, color[2] - fade_amount)
     return r, g, b, color[3]
 
 
-def get_rgba_tuple(color: Any) -> tuple:
-    """
-    Converts a color representation to an RGBA tuple.
+def get_rgba_tuple(color: str | int | tuple, opacity: int = 255) -> tuple:
+    """Converts a color representation to an RGBA tuple.
 
     Args:
         color (Any): The color representation to be converted.
+        opacity (int): The transparency of the color (0 ~ 255).
 
     Returns:
-        tuple: A tuple representing the color in RGBA format, with values for red (R), green (G), blue (B), and alpha (A).
+        tuple: A tuple representing the color in RGBA format, with values for R, G, B, and A.
     """
     if isinstance(color, tuple):
         rgba = color
     elif isinstance(color, int):
         rgba = (color >> 16 & 0xFF, color >> 8 & 0xFF, color & 0xFF, color >> 24 & 0xFF)
     else:
         rgba = ImageColor.getrgb(color)
 
     if len(rgba) == 3:
-        rgba = (rgba[0], rgba[1], rgba[2], 255)
+        rgba = (rgba[0], rgba[1], rgba[2], opacity)
     return rgba
 
 
-def get_keys_by_value(d, v):
-    for key in d.keys():  # reverse search the dict for the value
+def get_keys_by_value(d: dict, v: int) -> Generator:
+    """Get keys from dictionary given the value."""
+    for key in d:  # reverse search the dict for the value
         if d[key] == v:
             yield key
 
 
 def self_multiply(tensor_tuple: tuple) -> int | float:
-    """
-    Multiplies all elements in the tuple together.
+    """Multiplies all elements in the tuple together.
 
     Args:
         tensor_tuple (tuple): A tuple containing tensors.
 
     Returns:
         int or float: The result of multiplying all elements together.
     """
@@ -220,61 +277,64 @@
     s = tensor_list[0]
     for i in range(1, len(tensor_list)):
         s *= tensor_list[i]
     return s
 
 
 def vertical_image_concat(
-    im1: Image, im2: Image, background_fill: Any = "white"
+    im1: Image,
+    im2: Image,
+    background_fill: str | tuple = "white",
 ) -> PIL.Image:
-    """
-    Concatenates two PIL images vertically.
+    """Concatenates two PIL images vertically.
 
     Args:
         im1 (PIL.Image): The top image.
         im2 (PIL.Image): The bottom image.
-        background_fill (str or tuple, optional): Color for the image background. Can be a string or a tuple (R, G, B, A).
+        background_fill (str or tuple, optional): Color for the background. A string or a tuple (R, G, B, A).
 
     Returns:
         PIL.Image: A new image resulting from the vertical concatenation of the two input images.
     """
     dst = Image.new(
-        "RGBA", (max(im1.width, im2.width), im1.height + im2.height), background_fill
+        "RGBA",
+        (max(im1.width, im2.width), im1.height + im2.height),
+        background_fill,
     )
     dst.paste(im1, (0, 0))
     dst.paste(im2, (0, im1.height))
     return dst
 
 
 def linear_layout(
     images: list,
     max_width: int = -1,
     max_height: int = -1,
     horizontal: bool = True,
     padding: int = 0,
     spacing: int = 0,
-    background_fill: Any = "white",
+    background_fill: str | tuple = "white",
 ) -> PIL.Image:
-    """
-    Creates a linear layout of a passed list of images in horizontal or vertical orientation. The layout will wrap in x
-    or y dimension if a maximum value is exceeded.
+    """Creates a linear layout of a passed list of images in horizontal or vertical orientation.
+
+    The layout will wrap in x or y dimension if a maximum value is exceeded.
 
     Args:
         images (list): List of PIL images.
         max_width (int, optional): Maximum width of the image. Only enforced in horizontal orientation.
         max_height (int, optional): Maximum height of the image. Only enforced in vertical orientation.
         horizontal (bool, optional): If True, will draw images horizontally, else vertically.
         padding (int, optional): Top, bottom, left, right border distance in pixels.
         spacing (int, optional): Spacing in pixels between elements.
-        background_fill (str or tuple, optional): Color for the image background. Can be a string or a tuple (R, G, B, A).
+        background_fill (str or tuple, optional): Color for the background. A string or a tuple (R, G, B, A).
 
     Returns:
         PIL.Image: An Image object representing the linear layout of the passed list of images.
     """
-    coords = list()
+    coords = []
     width = 0
     height = 0
 
     x, y = padding, padding
 
     for img in images:
         if horizontal:
@@ -297,49 +357,11 @@
 
             width = max(x + img.width + padding, width)
             height = max(y + img.height + padding, height)
 
             y += img.height + spacing
 
     layout = Image.new("RGBA", (width, height), background_fill)
-    for img, coord in zip(images, coords):
+    for img, coord in zip(images, coords, strict=False):
         layout.paste(img, coord)
 
     return layout
-
-
-def register_hook(
-    model: nn.Module, module: nn.Module, hooks: List, layers: OrderedDict
-) -> None:
-    """
-    Registers a forward hook on the specified module and collects the module and the output shapes.
-
-    Args:
-        model (nn.Module): The parent model.
-        module (nn.Module): The module to register the hook on.
-        hooks (List): A list to store the registered hooks.
-        layers (OrderedDict): An OrderedDict to store information about the registered modules and output shapes.
-
-    Returns:
-        None
-    """
-
-    def hook(
-        module: nn.Module, input: Tuple[torch.Tensor], output: torch.Tensor
-    ) -> None:
-        class_name = str(module.__class__).split(".")[-1].split("'")[0]
-        module_idx = len(layers)
-
-        m_key = "%s-%i" % (class_name, module_idx + 1)
-        layers[m_key] = OrderedDict()
-        layers[m_key]["module"] = module
-        if isinstance(output, (list, tuple)):
-            layers[m_key]["output_shape"] = tuple((-1,) + o.size()[1:] for o in output)
-        else:
-            layers[m_key]["output_shape"] = output.size()
-
-    if (
-        not isinstance(module, nn.Sequential)
-        and not isinstance(module, nn.ModuleList)
-        and module is not model
-    ):
-        hooks.append(module.register_forward_hook(hook))
```

### Comparing `visualtorch-0.2.1/visualtorch.egg-info/PKG-INFO` & `visualtorch-0.2.2/visualtorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Architecture visualization of Torch models
 Home-page: https://github.com/willyfh/visualtorch
 Author: Willy Fitra Hendria
 Author-email: willyfitrahendria@gmail.com
 License: MIT
 Keywords: visualize architecture,torch visualization,visualtorch
 Classifier: Programming Language :: Python :: 3.10
@@ -19,21 +19,21 @@
 <div align="center">
  <h1>🔥 VisualTorch 🔥</h1>
 
 [![python](https://img.shields.io/badge/python-3.10%2B-blue)]() [![pytorch](https://img.shields.io/badge/pytorch-2.0%2B-orange)]() [![Downloads](https://static.pepy.tech/personalized-badge/visualtorch?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/visualtorch) [![Run Tests](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml/badge.svg)](https://github.com/willyfh/visualtorch/actions/workflows/pytest.yml) [![Documentation Status](https://readthedocs.org/projects/visualtorch/badge/?version=latest)](https://visualtorch.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
-**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style and graph-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
+**VisualTorch** aims to help visualize Torch-based neural network architectures. It currently supports generating layered-style, graph-style, and LeNet-style architectures for PyTorch Sequential and Custom models. This tool is adapted from [visualkeras](https://github.com/paulgavrikov/visualkeras), [pytorchviz](https://github.com/szagoruyko/pytorchviz), and [pytorch-summary](https://github.com/sksq96/pytorch-summary).
 
 **Note:** VisualTorch may not yet support complex models, but contributions are welcome!
 
 <div align="center">
 
-![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/7e2c35ea-d34d-4b92-b414-285bccb8576a)
+![VisualTorch Examples](https://github.com/willyfh/visualtorch/assets/5786636/398c3356-4de0-446b-a30b-d8ebe532d2c2)
 
 </div>
 
 ## Documentation
 
 Online documentation is available at [visualtorch.readthedocs.io](https://visualtorch.readthedocs.io/en/latest/).
```

