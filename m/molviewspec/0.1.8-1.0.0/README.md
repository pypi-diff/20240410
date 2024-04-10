# Comparing `tmp/molviewspec-0.1.8.tar.gz` & `tmp/molviewspec-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molviewspec-0.1.8.tar", last modified: Thu Feb  1 17:54:41 2024, max compression
+gzip compressed data, was "molviewspec-1.0.0.tar", last modified: Wed Apr 10 18:22:39 2024, max compression
```

## Comparing `molviewspec-0.1.8.tar` & `molviewspec-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:54:41.203282 molviewspec-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-01 17:54:30.000000 molviewspec-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-02-01 17:54:41.203282 molviewspec-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-02-01 17:54:30.000000 molviewspec-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:54:41.203282 molviewspec-0.1.8/molviewspec/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-01 17:54:30.000000 molviewspec-0.1.8/molviewspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-02-01 17:54:30.000000 molviewspec-0.1.8/molviewspec/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-02-01 17:54:30.000000 molviewspec-0.1.8/molviewspec/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-01 17:54:30.000000 molviewspec-0.1.8/molviewspec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 17:54:41.203282 molviewspec-0.1.8/molviewspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-02-01 17:54:41.000000 molviewspec-0.1.8/molviewspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-01 17:54:41.000000 molviewspec-0.1.8/molviewspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 17:54:41.000000 molviewspec-0.1.8/molviewspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-01 17:54:41.000000 molviewspec-0.1.8/molviewspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-01 17:54:41.000000 molviewspec-0.1.8/molviewspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-01 17:54:30.000000 molviewspec-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-01 17:54:41.203282 molviewspec-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-01 17:54:30.000000 molviewspec-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:22:39.808738 molviewspec-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-10 18:22:31.000000 molviewspec-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-10 18:22:39.808738 molviewspec-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-10 18:22:31.000000 molviewspec-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:22:39.808738 molviewspec-1.0.0/molviewspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 18:22:31.000000 molviewspec-1.0.0/molviewspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27035 2024-04-10 18:22:31.000000 molviewspec-1.0.0/molviewspec/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-04-10 18:22:31.000000 molviewspec-1.0.0/molviewspec/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-10 18:22:31.000000 molviewspec-1.0.0/molviewspec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:22:39.808738 molviewspec-1.0.0/molviewspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-10 18:22:39.000000 molviewspec-1.0.0/molviewspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 18:22:39.000000 molviewspec-1.0.0/molviewspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:22:39.000000 molviewspec-1.0.0/molviewspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 18:22:39.000000 molviewspec-1.0.0/molviewspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 18:22:39.000000 molviewspec-1.0.0/molviewspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 18:22:31.000000 molviewspec-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 18:22:39.808738 molviewspec-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-10 18:22:31.000000 molviewspec-1.0.0/setup.py
```

### Comparing `molviewspec-0.1.8/LICENSE.txt` & `molviewspec-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `molviewspec-0.1.8/PKG-INFO` & `molviewspec-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-Metadata-Version: 2.1
-Name: molviewspec
-Version: 0.1.8
-Summary: Generate Mol* views using this simple Python library, which allows you to compose complex scenes in a step-wise manner.
-Home-page: https://github.com/molstar/mol-view-spec
-Download-URL: https://github.com/molstar/mol-view-spec/archive/v0.1.8.tar.gz
-Author: Sebastian Bittrich, Adam Midlik, David Sehnal
-Author-email: sebastian.bittrich@rcsb.org, midlik@ebi.ac.uk, david.sehnal@gmail.com
-License: MIT
-Keywords: molecular graphics,scientific visualization,web graphics,view specification,scene building,Mol*
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Natural Language :: English
-Classifier: Typing :: Typed
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: pydantic<2
+MolViewSpec
+=============
 
-# MolViewSpec
+MolViewSpec (*.msvj) is a JSON-based file format that is used to describe visual scenes or views used in molecular 
+visualization.
+It adopts declarative data-driven approach to describe, load, render, and visually deliver molecular structures, along
+with 3D representations, coloring schemes, and associated structural, biological, or functional annotations.
+This Python toolkit allows for describing the information required for representing a molecular view state as data in a nested 
+tree format that can be consumed by visualization software tools such as 
+[Mol*](https://github.com/molstar/molstar/tree/master/src/extensions/mvs).
 
+
+## The Idea behind MolViewSpec
+
+In the long run, MolViewSpec aims to re-imagine how users define molecular scenes by detaching this process from any 
+concrete 3D viewer.
+
+MolViewSpec's workflow is:
+1. `define scene using MolViewSpec`
+2. `generic state description as .msvj`
+3. `open in any MolViewSpec-compatible 3D viewer`
+
+Opposed to the traditional workflow that locks users into using a specific 3D viewer, such as:
+1. `define scene in Mol*`
+2. `Mol*-specific state format`
+3. `open only in Mol*`
+
+
+## See the MolViewSpec in Action
+Colab Notebook: https://colab.research.google.com/drive/1O2TldXlS01s-YgkD9gy87vWsfCBTYuz9
+
+
+## Access Type Definitions
+All type definitions can be found here:
+- using a dedicated Server endpoint: http://localhost:9000/api/v1/utils/models/openapi.json
+- in Markdown: https://molstar.org/mol-view-spec-docs/tree-schema/
+
+
+## Description of the MolViewSpec State Tree
 MolViewSpec provides a generic description of typical visual scenes that may occur as part of molecular visualizations.
 A tree format allows the composition of complex scene descriptors by combining reoccurring nodes that serve as
 building blocks.
 
 Nodes can be nested to allow chaining of operations as child nodes will be applied to the result of the operation
 described by its parent node.
 
@@ -36,15 +49,15 @@
 {
   "root": {
     "kind": "root",
     "children": [
       {
         "kind": "download",
         "params": {
-          "url": "https://www.ebi.ac.uk/pdbe/entry-files/download/1cbs_updated.cif"
+          "url": "https://files.wwpdb.org/download/1cbs.cif"
         },
         "children": [
           {
             "kind": "parse",
             "params": {
               "format": "mmcif"
             },
@@ -82,73 +95,78 @@
     "timestamp": "2023-11-16T11:41:07.421220"
   }
 }
 ```
 
 Mol* is the reference implementation for reading MolViewSpec files.
 
-## The Tree Root
 
-Every tree starts with a single `root` node, which contains all nodes in a structure fashion, and a `metadata` node, 
+### The Tree Root
+
+Every tree starts with a single `root` node, which contains all nodes in a structure fashion, and a `metadata` node,
 which can hold additional information such as a `version` tag as well as the `timestamp` when a view was created.
 
 ```json
 {
   "root": {},
   "metadata": {
     "version": "0.1",
     "timestamp": "2023-11-16T11:41:07.421220"
   }
 }
 ```
 
-## The `root` Node
+
+### The `root` Node
 
 All nodes of the tree must define their `kind` and may have 0 or more child nodes (`children`).
 The `root` is a special node with a `kind` of `root` that contains a collection of `children`.
 
 ```json
 {
   "kind": "root",
   "children": []
 }
 ```
 
-## The `download` Node
+
+### The `download` Node
 
 Node types other than the `root` may contain an optional `params` property. A common action is loading of 3D structure
 data. This is done using a node of `kind` `download`. In this context, `params` can for example provide the `url` from
 which data will be loaded from.
 
 ```json
 {
   "kind": "download",
   "children": [],
   "params": {
-    "url": "https://www.ebi.ac.uk/pdbe/entry-files/download/1cbs_updated.cif"
+    "url": "https://files.wwpdb.org/download/1cbs.cif"
   }
 }
 ```
 
-## The `parse` Node
+
+### The `parse` Node
 
 The previous `download` operation merely obtains the resources from the specified URL. To make it available to the
 viewer, the data must be parsed. This operation expects that the `format` is defined (in this case mmCIF is parsed).
 
 ```json
 {
   "kind": "parse",
   "children": [],
   "params": {
     "format": "mmcif"
   }
 }
 ```
 
-## The `structure` Node
+
+### The `structure` Node
 
 There are different ways to load the content of a mmCIF file. Common actions are loading the 1st biological assembly or
 loading the deposited coordinates (also called "asymmetric unit" or "model coordinates").
 The action is defined as `kind`. In this example, the `model` coordinates are loaded.
 
 ```json
 {
@@ -156,15 +174,16 @@
   "children": [],
   "params": {
     "kind": "model"
   }
 }
 ```
 
-## The `component` Node
+
+### The `component` Node
 
 At this point, the loaded file is available in the viewer but nothing is visualized yet. Several selection (called
 "components") can be created. The example creates a component that includes everything using a `selector` set to `all`.
 Other options could be a selection for protein chains, nucleic acids, ligands etc.
 Components are reusable groups of atoms, residues, or chains, which can be interacted with programmatically.
 
 ```json
@@ -173,40 +192,74 @@
   "children": [],
   "params": {
     "selector": "all"
   }
 }
 ```
 
-## The `representation` Node
+
+### The `representation` Node
 
 The `representation` nodes applies to previously created components, which is provided by the parent node of a
 `representation` node. Representations are dedicated visuals that constitute a component. In this example, the selection
 from above -- which selects the entire structure -- and depicts it as cartoon by specifying `cartoon` as `type`.
 
 ```json
 {
     "kind": "representation",
     "params": {
       "type": "cartoon"
     }
 }
 ```
 
-## Expanding the Tree
+
+### Expanding the Tree
 Nodes can have 0 or more nodes as children. It is, for example, possible to create multiple `component` nodes based on a
 particular `structure` node to create different representations for different types of molecules.
 
-# Development
 
-## Lint
+### Development
+
+### Install from PyPI
+```shell
+pip install molviewspec
+```
+
+Find the package at: https://pypi.org/project/molviewspec/
+
+### Setting up the environment
+
+```
+mamba env create -f ./environment.yaml
+conda activate mol-view-spec-dev
+```
+
+### Running the server
+
+```
+cd molviewspec
+python serve.py # or make serve
+```
+
+will run the server on `localhost:9000` with reload mode on.
+
+- API Docs: `http://localhost:9000/docs`
+- Example: `http://localhost:9000/api/v1/examples/load?id=1tqn`
+
+### Formatting the Project
 
 ```
 make format
 make mypy
 ```
 
-## Publish the Python Library
+### Publishing the Python Library
 
 - Set version (in https://github.com/molstar/mol-view-spec/blob/master/molviewspec/molviewspec/__init__.py)
 - Create a GitHub release
 - Tag will automatically publish to PyPI
+
+
+## Mol* Extension 
+
+MolViewSpec is supported in Mol* via an [official extension](https://github.com/molstar/molstar/tree/master/src/extensions/mvs).
```

### Comparing `molviewspec-0.1.8/molviewspec/nodes.py` & `molviewspec-1.0.0/molviewspec/nodes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Definitions of all 'nodes' used by the MolViewSpec format specification and its builder implementation.
+"""
+
 from __future__ import annotations
 
 from typing import Any, Literal, Mapping, Optional, Union
 
 from pydantic import BaseModel, Field
 
 KindT = Literal[
@@ -29,51 +33,75 @@
     "tooltip_from_source",
     "tooltip_from_uri",
     "transform",
 ]
 
 
 class Node(BaseModel):
+    """
+    Base impl of all state tree nodes.
+    """
+
     kind: KindT = Field(description="The type of this node.")
     params: Optional[Mapping[str, Any]] = Field(description="Optional params that are needed for this node.")
     children: Optional[list[Node]] = Field(description="Optional collection of nested child nodes.")
 
 
 DescriptionFormatT = Literal["markdown", "plaintext"]
 
 
 class Metadata(BaseModel):
+    """
+    Global metadata, which describes the purpose and creation date of a state tree.
+    """
+
     version: str = Field(description="Version of the spec used to write this tree.")
     title: Optional[str] = Field(description="Name of this view.")
     description: Optional[str] = Field(description="Detailed description of this view.")
     description_format: Optional[DescriptionFormatT] = Field(description="Format of the description.")
     timestamp: str = Field(description="Timestamp when this view was exported.")
 
 
 class State(BaseModel):
+    """
+    Root node of all state trees.
+    """
+
     root: Node = Field(description="Root of the node tree.")
     metadata: Metadata = Field(description="Associated metadata.")
 
 
 class DownloadParams(BaseModel):
+    """
+    Download node, describing where structure data should be fetched from.
+    """
+
     url: str = Field(description="URL from which to pull structure data.")
 
 
 ParseFormatT = Literal["mmcif", "bcif", "pdb"]
 
 
 class ParseParams(BaseModel):
+    """
+    Parse node, describing how to parse downloaded data.
+    """
+
     format: ParseFormatT = Field(description="The format of the structure data.")
 
 
 StructureTypeT = Literal["model", "assembly", "symmetry", "symmetry_mates"]
 
 
 class StructureParams(BaseModel):
-    type: StructureTypeT
+    """
+    Structure node, describing which type (assembly 1, deposited coordinates, etc.) of the parsed data to create.
+    """
+
+    type: StructureTypeT = Field(description="How to interpret the loaded data")
     assembly_id: Optional[str] = Field(description="Use the name to specify which assembly to load")
     assembly_index: Optional[int] = Field(description="0-based assembly index, use this to load the 1st assembly")
     model_index: Optional[int] = Field(description="0-based model index in case multiple NMR frames are present")
     block_index: Optional[int] = Field(
         description="0-based block index in case multiple mmCIF or SDF data blocks are " "present"
     )
     block_header: Optional[str] = Field(description="Reference a specific mmCIF or SDF data block by its block header")
@@ -81,21 +109,31 @@
     ijk_min: Optional[tuple[int, int, int]] = Field(description="Bottom-left Miller indices")
     ijk_max: Optional[tuple[int, int, int]] = Field(description="Top-right Miller indices")
 
 
 ComponentSelectorT = Literal["all", "polymer", "protein", "nucleic", "branched", "ligand", "ion", "water"]
 
 
-class ComponentExpression(BaseModel):  # Feel free to rename (this used to be InlineSchemaParams)
-    label_entity_id: Optional[str]
-    label_asym_id: Optional[str]
-    auth_asym_id: Optional[str]
-    label_seq_id: Optional[int]
-    auth_seq_id: Optional[int]
-    pdbx_PDB_ins_code: Optional[str]
+class ComponentExpression(BaseModel):
+    """
+    Component expressions are used to make selections.
+    """
+
+    label_entity_id: Optional[str] = Field(description="Select an entity by its identifier")
+    label_asym_id: Optional[str] = Field(
+        description="Select a chain using its standard, programmatically-assigned identifier"
+    )
+    auth_asym_id: Optional[str] = Field(description="Select a chain using its legacy, author-assigned identifier")
+    label_seq_id: Optional[int] = Field(
+        description="Select a residue by its standard, programmatically-assigned sequence position"
+    )
+    auth_seq_id: Optional[int] = Field(description="Select a residue by its legacy, author-assigned sequence position")
+    pdbx_PDB_ins_code: Optional[str] = Field(
+        description="Optional legacy insertion code, only relevant for `auth_seq_id`"
+    )
     beg_label_seq_id: Optional[int] = Field(
         description="Defines a consecutive range of residues when combined with `end_label_seq_id`."
     )
     end_label_seq_id: Optional[int] = Field(
         description="Defines a consecutive range of residues when combined with `beg_label_seq_id`. End indices are inclusive."
     )
     beg_auth_seq_id: Optional[int] = Field(
@@ -264,15 +302,19 @@
     "yellow",
     "yellowgreen",
 ]
 ColorT = Union[ColorNamesT, str]  # str represents hex colors for now
 
 
 class RepresentationParams(BaseModel):
-    type: RepresentationTypeT
+    """
+    Representation node, describing how to represent a component.
+    """
+
+    type: RepresentationTypeT = Field(description="Representation type, i.e. cartoon, ball-and-stick, etc.")
 
 
 SchemaT = Literal[
     "whole_structure",
     "entity",
     "chain",
     "auth_chain",
@@ -284,143 +326,211 @@
     "auth_atom",
     "all_atomic",
 ]
 SchemaFormatT = Literal["cif", "bcif", "json"]
 
 
 class _DataFromUriParams(BaseModel):
-    uri: str
-    format: SchemaFormatT
-    category_name: Optional[str] = Field(description="Only applies when format is 'cif' or 'bcif'")
+    """
+    Abstract node that's shared by all resource-based selections.
+    """
+
+    uri: str = Field(description="Location of the resource")
+    format: SchemaFormatT = Field(description="Format of the resource, i.e. 'cif', 'bcif', or 'json'")
+    category_name: Optional[str] = Field(
+        description="Category wherein selection is located. Only applies when format is 'cif' or 'bcif'."
+    )
     field_name: Optional[str] = Field(
         description="Name of the column in CIF or field name (key) in JSON that "
         "contains the desired value (color/label/tooltip/component...); the "
         "default value is 'color'/'label'/'tooltip'/'component' depending "
         "on the node kind",
     )
-    block_header: Optional[str] = Field(description="Only applies when format is 'cif' or 'bcif'")
-    block_index: Optional[int] = Field(description="Only applies when format is 'cif' or 'bcif'")
-    schema_: SchemaT = Field(alias="schema")  # must be aliased to not shadow BaseModel attribute
+    block_header: Optional[str] = Field(
+        description="Block name wherein selection is located. Only applies when format is 'cif' or 'bcif'."
+    )
+    block_index: Optional[int] = Field(
+        description="Block index wherein selection is located. Only applies when format is 'cif' or 'bcif'."
+    )
+    # must be aliased to not shadow BaseModel attribute
+    schema_: SchemaT = Field(alias="schema", description="granularity/type of the selection")
 
 
 class _DataFromSourceParams(BaseModel):
-    category_name: str
+    """
+    Abstract node that's shared by all selections based on the source file.
+    """
+
+    category_name: str = Field(description="Category wherein selection is located.")
     field_name: Optional[str] = Field(
         description="Name of the column in CIF that contains the desired value ("
         "color/label/tooltip/component...); the default value is "
         "'color'/'label'/'tooltip'/'component' depending on the node kind",
     )
-    block_header: Optional[str]
-    block_index: Optional[int]
-    schema_: SchemaT = Field(alias="schema")  # must be aliased to not shadow BaseModel attribute
+    block_header: Optional[str] = Field(description="Block name wherein selection is located.")
+    block_index: Optional[int] = Field(description="Block index wherein selection is located.")
+    # must be aliased to not shadow BaseModel attribute
+    schema_: SchemaT = Field(alias="schema", description="granularity/type of the selection")
 
 
 class ComponentInlineParams(BaseModel):
+    """
+    Selection based on function arguments.
+    """
+
     selector: Union[ComponentSelectorT, ComponentExpression, list[ComponentExpression]] = Field(
         description="Describes one or more selections or one of the enumerated selectors."
     )
 
 
 class ComponentFromUriParams(_DataFromUriParams):
+    """
+    Selection based on another resource.
+    """
+
     field_values: Optional[list[str]] = Field(
         description="Create the component from rows that have any of these "
         "values in the field specified by `field_name`. If not "
         "provided, create the component from all rows."
     )
 
 
 class ComponentFromSourceParams(_DataFromSourceParams):
+    """
+    Selection based on a category in the source file.
+    """
+
     field_values: Optional[list[str]] = Field(
         description="Create the component from rows that have any of these "
         "values in the field specified by `field_name`. If not "
         "provided, create the component from all rows."
     )
 
 
 class ColorInlineParams(ComponentInlineParams):
-    color: ColorT
+    """
+    Color based on function arguments.
+    """
+
+    color: ColorT = Field(description="Color using SVG color names or RGB hex code")
 
 
 class ColorFromUriParams(_DataFromUriParams):
-    pass
+    """
+    Color based on another resource.
+    """
 
 
 class ColorFromSourceParams(_DataFromSourceParams):
-    pass
+    """
+    Color based on a category in the source file.
+    """
 
 
 class LabelInlineParams(BaseModel):
-    text: str
+    """
+    Label based on function arguments.
+    """
+
+    text: str = Field(description="Text to show as label")
     # schema and other stuff not needed here, the label will be applied on the whole parent Structure or Component
 
 
 class LabelFromUriParams(_DataFromUriParams):
-    pass
+    """
+    Label based on another resource.
+    """
 
 
 class LabelFromSourceParams(_DataFromSourceParams):
-    pass
+    """
+    Label based on a category in the source file.
+    """
 
 
 class TooltipInlineParams(BaseModel):
-    text: str
+    text: str = Field(description="Text to show as tooltip upon hover")
     # schema and other stuff not needed here, the tooltip will be applied on the whole parent Structure or Component
 
 
 class TooltipFromUriParams(_DataFromUriParams):
     pass
 
 
 class TooltipFromSourceParams(_DataFromSourceParams):
     pass
 
 
 class FocusInlineParams(BaseModel):
+    """
+    Define the camera focus based on function arguments.
+    """
+
     direction: Optional[tuple[float, float, float]] = Field(
         description="Direction of the view (vector position -> target)"
     )
     up: Optional[tuple[float, float, float]] = Field(
         description="Controls the rotation around the vector between target and position"
     )
 
 
 class TransformParams(BaseModel):
+    """
+    Define a transformation.
+    """
+
     rotation: Optional[tuple[float, ...]] = Field(
-        description="In a column major (j * 3 + i indexing) format, this is equivalent to Fortran-order in numpy, to be multiplied from the left",
+        description="9d vector describing the rotation, in a column major (j * 3 + i indexing) format, this is equivalent to Fortran-order in numpy, to be multiplied from the left",
     )
-    translation: Optional[tuple[float, float, float]] = Field()
+    translation: Optional[tuple[float, float, float]] = Field(description="3d vector describing the translation")
 
 
 class CameraParams(BaseModel):
+    """
+    Controls the global camera position.
+    """
+
     target: tuple[float, float, float] = Field(description="What to look at")
     position: tuple[float, float, float] = Field(description="The position of the camera")
     up: tuple[float, float, float] = Field(
         description="Controls the rotation around the vector between target and position", required=True
     )
 
 
 class CanvasParams(BaseModel):
-    background_color: ColorT
+    """
+    Controls global canvas properties.
+    """
+
+    background_color: ColorT = Field(description="Background color using SVG color names or RGB hex code")
 
 
 class SphereParams(BaseModel):
-    position: tuple[float, float, float]
-    radius: float
-    color: ColorT
-    label: Optional[str]
-    tooltip: Optional[str]
+    """
+    Experimental: Defines a sphere primitive.
+    """
+
+    position: tuple[float, float, float] = Field(description="Position of the primitive")
+    radius: float = Field(description="Radius of the sphere")
+    color: ColorT = Field(description="Color of the sphere")
+    label: Optional[str] = Field(description="Optional text label")
+    tooltip: Optional[str] = Field(description="Optional tooltip label, shown upon hover")
 
 
 class LineParams(BaseModel):
-    position1: tuple[float, float, float]
-    position2: tuple[float, float, float]
-    radius: float
-    color: ColorT
-    label: Optional[str]
-    tooltip: Optional[str]
+    """
+    Experimental: Defines a line primitive.
+    """
+
+    position1: tuple[float, float, float] = Field(description="Start position of the primitive")
+    position2: tuple[float, float, float] = Field(description="End position of the primitive")
+    radius: float = Field(description="Radius of the line")
+    color: ColorT = Field(description="Color of the line")
+    label: Optional[str] = Field(description="Optional text label")
+    tooltip: Optional[str] = Field(description="Optional tooltip label, shown upon hover")
 
 
 def validate_state_tree(json: str) -> None:
     """
     Validates a JSON string and checks whether it's a valid state representation.
     :param json: payload to validate
     :raises ValidationError if JSON is malformed or state tree type definitions are violated
```

### Comparing `molviewspec-0.1.8/molviewspec/utils.py` & `molviewspec-1.0.0/molviewspec/utils.py`

 * *Files identical despite different names*

### Comparing `molviewspec-0.1.8/setup.py` & `molviewspec-1.0.0/setup.py`

 * *Files identical despite different names*

