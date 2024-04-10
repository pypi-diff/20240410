# Comparing `tmp/seml-0.4.4.tar.gz` & `tmp/seml-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seml-0.4.4.tar", last modified: Tue Apr  9 14:50:20 2024, max compression
+gzip compressed data, was "seml-0.4.5.tar", last modified: Wed Apr 10 07:56:34 2024, max compression
```

## Comparing `seml-0.4.4.tar` & `seml-0.4.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.729006 seml-0.4.4/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1135 2023-09-19 07:51:23.000000 seml-0.4.4/LICENSE
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      183 2024-03-01 09:42:10.000000 seml-0.4.4/MANIFEST.in
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6930 2024-04-09 14:50:20.729006 seml-0.4.4/PKG-INFO
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4163 2024-04-09 14:39:51.000000 seml-0.4.4/README.md
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1468 2024-04-09 14:49:42.000000 seml-0.4.4/pyproject.toml
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)       38 2024-04-09 14:50:20.729006 seml-0.4.4/setup.cfg
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.673007 seml-0.4.4/src/
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.713007 seml-0.4.4/src/seml/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1201 2024-03-19 10:39:23.000000 seml-0.4.4/src/seml/__init__.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    34241 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/__main__.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    13861 2024-03-11 16:09:35.000000 seml-0.4.4/src/seml/add.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    30912 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/config.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2220 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/configure.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     3289 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/console.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    14313 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/database.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7370 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/description.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1030 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/errors.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2892 2024-03-19 10:39:24.000000 seml-0.4.4/src/seml/evaluation.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7975 2024-02-27 10:41:48.000000 seml-0.4.4/src/seml/experiment.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     9015 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/json.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    46239 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/manage.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    11371 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/mattermost_observer.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      635 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/module_hider.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1509 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/network.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6324 2024-02-12 17:39:39.000000 seml-0.4.4/src/seml/observers.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    10803 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/parameters.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4210 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/prepare_experiment.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6020 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/project.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     5786 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/settings.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     8014 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/sources.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    43616 2024-04-09 14:43:23.000000 seml-0.4.4/src/seml/start.py
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.673007 seml-0.4.4/src/seml/templates/
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.725006 seml-0.4.4/src/seml/templates/slurm/
--rwxr-xr-x   0 gaoni    (10028) tumuser  (20909)      647 2023-09-19 07:51:24.000000 seml-0.4.4/src/seml/templates/slurm/jupyter_template.sh
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2042 2024-02-13 07:29:32.000000 seml-0.4.4/src/seml/templates/slurm/slurm_template.sh
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      253 2024-01-26 21:46:29.000000 seml-0.4.4/src/seml/typer.py
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)    17301 2024-03-11 15:10:43.000000 seml-0.4.4/src/seml/utils.py
-drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-09 14:50:20.725006 seml-0.4.4/src/seml.egg-info/
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6930 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/PKG-INFO
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      859 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/SOURCES.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)        1 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/dependency_links.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)       44 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/entry_points.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)      279 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/requires.txt
--rw-r--r--   0 gaoni    (10028) tumuser  (20909)        5 2024-04-09 14:50:20.000000 seml-0.4.4/src/seml.egg-info/top_level.txt
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.529594 seml-0.4.5/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1135 2023-09-19 07:51:23.000000 seml-0.4.5/LICENSE
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      183 2024-03-01 09:42:10.000000 seml-0.4.5/MANIFEST.in
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6964 2024-04-10 07:56:34.525594 seml-0.4.5/PKG-INFO
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4163 2024-04-09 14:52:10.000000 seml-0.4.5/README.md
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1494 2024-04-10 07:50:03.000000 seml-0.4.5/pyproject.toml
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)       38 2024-04-10 07:56:34.529594 seml-0.4.5/setup.cfg
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.481594 seml-0.4.5/src/
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.513594 seml-0.4.5/src/seml/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1201 2024-03-19 10:39:23.000000 seml-0.4.5/src/seml/__init__.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    34619 2024-04-10 07:50:03.000000 seml-0.4.5/src/seml/__main__.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    13861 2024-03-11 16:09:35.000000 seml-0.4.5/src/seml/add.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    30915 2024-04-09 18:51:21.000000 seml-0.4.5/src/seml/config.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2220 2024-04-09 14:52:10.000000 seml-0.4.5/src/seml/configure.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     3289 2024-04-09 14:43:23.000000 seml-0.4.5/src/seml/console.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    14313 2024-04-09 14:52:10.000000 seml-0.4.5/src/seml/database.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7370 2024-04-09 14:43:23.000000 seml-0.4.5/src/seml/description.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1030 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/errors.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2892 2024-03-19 10:39:24.000000 seml-0.4.5/src/seml/evaluation.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     7975 2024-02-27 10:41:48.000000 seml-0.4.5/src/seml/experiment.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     9015 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/json.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    46239 2024-04-09 14:43:23.000000 seml-0.4.5/src/seml/manage.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    11371 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/mattermost_observer.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      635 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/module_hider.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     1509 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/network.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6324 2024-02-12 17:39:39.000000 seml-0.4.5/src/seml/observers.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    10803 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/parameters.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     4210 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/prepare_experiment.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6020 2024-04-09 14:43:23.000000 seml-0.4.5/src/seml/project.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     5786 2024-04-09 14:52:10.000000 seml-0.4.5/src/seml/settings.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     8014 2024-04-09 14:43:23.000000 seml-0.4.5/src/seml/sources.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    43669 2024-04-10 07:50:03.000000 seml-0.4.5/src/seml/start.py
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.481594 seml-0.4.5/src/seml/templates/
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.525594 seml-0.4.5/src/seml/templates/slurm/
+-rwxr-xr-x   0 gaoni    (10028) tumuser  (20909)      647 2023-09-19 07:51:24.000000 seml-0.4.5/src/seml/templates/slurm/jupyter_template.sh
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     2042 2024-02-13 07:29:32.000000 seml-0.4.5/src/seml/templates/slurm/slurm_template.sh
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      253 2024-01-26 21:46:29.000000 seml-0.4.5/src/seml/typer.py
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)    17301 2024-03-11 15:10:43.000000 seml-0.4.5/src/seml/utils.py
+drwxr-xr-x   0 gaoni    (10028) tumuser  (20909)        0 2024-04-10 07:56:34.525594 seml-0.4.5/src/seml.egg-info/
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)     6964 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/PKG-INFO
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      859 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/SOURCES.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)        1 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/dependency_links.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)       44 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/entry_points.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)      298 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/requires.txt
+-rw-r--r--   0 gaoni    (10028) tumuser  (20909)        5 2024-04-10 07:56:34.000000 seml-0.4.5/src/seml.egg-info/top_level.txt
```

### Comparing `seml-0.4.4/LICENSE` & `seml-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/PKG-INFO` & `seml-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seml
-Version: 0.4.4
+Version: 0.4.5
 Summary: Slurm Experiment Management Library
 Author: DAML Group @ TUM
 Author-email: Daniel Zügner <zuegnerd@in.tum.de>, Johannes Gsteiger <johannes.gasteiger@tum.de>, Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 Maintainer-email: Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Johannes Klicpera, Daniel Zügner, Nicholas Gao
@@ -45,14 +45,15 @@
 Requires-Dist: munch>=2.0.4
 Requires-Dist: debugpy>=1.2.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: typer<1.0,>=0.9
 Requires-Dist: rich<14.0,>=13.0
 Requires-Dist: omegaconf<3.0,>=2.3.0
 Requires-Dist: gitignore_parser>=0.1.11
+Requires-Dist: setuptools>=69.2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: ssh-forward
 Requires-Dist: sshtunnel>=0.4.0; extra == "ssh-forward"
 Requires-Dist: filelock>=3.13.3; extra == "ssh-forward"
```

### Comparing `seml-0.4.4/README.md` & `seml-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/pyproject.toml` & `seml-0.4.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "seml"
-version = "0.4.4"
+version = "0.4.5"
 description = "Slurm Experiment Management Library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Daniel Zügner", email = "zuegnerd@in.tum.de" },
     { name = "Johannes Gsteiger", email = "johannes.gasteiger@tum.de" },
@@ -28,14 +28,15 @@
     "munch>=2.0.4",
     "debugpy>=1.2.1",
     "requests>=2.28.1",
     "typer>=0.9, <1.0",
     "rich>=13.0, <14.0",
     "omegaconf>=2.3.0, <3.0",
     "gitignore_parser>=0.1.11",
+    "setuptools>=69.2.0",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "ruff", "pre-commit"]
 ssh_forward = ["sshtunnel>=0.4.0", "filelock>=3.13.3"]
 
 [tool.ruff.format]
```

### Comparing `seml-0.4.4/src/seml/__init__.py` & `seml-0.4.5/src/seml/__init__.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/__main__.py` & `seml-0.4.5/src/seml/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import functools
 import json
 import logging
 import os
 import sys
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Set, Tuple, TypeVar
+from typing import Callable, Dict, List, Optional, Sequence, Set, Tuple, TypeVar
 
 from typing_extensions import Annotated, ParamSpec
 
 import seml.typer as typer
 from seml.add import add_config_files
 from seml.configure import configure
 from seml.database import (
@@ -48,15 +48,15 @@
 
 
 def restrict_collection(require: bool = True):
     """Decorator to require a collection name."""
 
     def decorator(fun: Callable[P, R]) -> Callable[P, R]:
         @functools.wraps(fun)
-        def wrapper(ctx: typer.Context, *args, **kwargs):
+        def wrapper(ctx: typer.Context, *args: P.args, **kwargs: P.kwargs):
             if require and not ctx.obj['collection']:
                 raise typer.BadParameter('Please specify a collection name.', ctx=ctx)
             elif not require and ctx.obj['collection']:
                 raise typer.BadParameter(
                     'Please do not specify a collection name.', ctx=ctx
                 )
             return fun(ctx, *args, **kwargs)
@@ -86,75 +86,81 @@
         '-y',
         '--yes',
         help='Automatically confirm all dialogues with yes.',
         is_flag=True,
     ),
 ]
 SacredIdAnnotation = Annotated[
-    int,
+    Optional[int],
     typer.Option(
         '-id',
         '--sacred-id',
         help='Sacred ID (_id in the database collection) of the experiment. '
         'Takes precedence over other filters.',
     ),
 ]
 FilterDictAnnotation = Annotated[
-    Dict,
+    Optional[Dict],
     typer.Option(
         '-f',
         '--filter-dict',
         help='Dictionary (passed as a string, e.g. \'{"config.dataset": "cora_ml"}\') to filter '
         'the experiments by.',
         metavar='JSON',
         parser=json.loads,
     ),
 ]
+BatchIdAnnotation = Annotated[
+    Optional[int],
+    typer.Option(
+        '-b',
+        '--batch-id',
+        help='Batch ID (batch_id in the database collection) of the experiments. '
+        'Experiments that were staged together have the same batch_id.',
+    ),
+]
+
+
+def parse_optional_str_list(values: Optional[Sequence[str]]) -> List[str]:
+    if values is None:
+        return []
+    return [
+        __x.strip()
+        for _x in values
+        for __x in _x.replace(',', ' ').split()
+        if __x.strip()
+    ]
+
+
 ProjectionAnnotation = Annotated[
     List[str],
     typer.Option(
         '-p',
         '--projection',
         help='List of configuration keys, e.g., `config.model`, to additionally print.',
-        parser=lambda s: s.strip(),
-        callback=lambda values: [
-            __x.strip() for _x in values for __x in _x.replace(',', ' ').split() if __x
-        ],
+        parser=str.strip,
+        callback=parse_optional_str_list,
         metavar='KEY',
     ),
 ]
-BatchIdAnnotation = Annotated[
-    int,
-    typer.Option(
-        '-b',
-        '--batch-id',
-        help='Batch ID (batch_id in the database collection) of the experiments. '
-        'Experiments that were staged together have the same batch_id.',
-    ),
-]
 
 _STATE_LIST = [s for states in States.values() for s in states]
 FilterStatesAnnotation = Annotated[
     List[str],
     typer.Option(
         '-s',
         '--filter-states',
         help='List of states to filter the experiments by. If empty (""), all states are considered.',
         metavar=f'[{"|".join(_STATE_LIST)}]',
         parser=lambda s: s.strip().upper(),
-        callback=lambda values: [
-            __x.strip().upper()
-            for _x in values
-            for __x in _x.replace(',', ' ').split()
-            if __x
-        ],
+        callback=parse_optional_str_list,
     ),
 ]
 SBatchOptionsAnnotation = Annotated[
-    Dict,
+    Optional[Dict],
     typer.Option(
         '-sb',
         '--sbatch-options',
         help='Dictionary (passed as a string, e.g. \'{"gres": "gpu:2"}\') to request two GPUs.',
         metavar='JSON',
         parser=json.loads,
     ),
@@ -201,31 +207,31 @@
         '-pm',
         '--post-mortem',
         help='Activate post-mortem debugging with pdb.',
         is_flag=True,
     ),
 ]
 WorkerGPUsAnnotation = Annotated[
-    str,
+    Optional[str],
     typer.Option(
         '-wg',
         '--worker-gpus',
         help='The IDs of the GPUs used by the local worker. Will be directly passed to CUDA_VISIBLE_DEVICES.',
     ),
 ]
 WorkerCPUsAnnotation = Annotated[
-    int,
+    Optional[int],
     typer.Option(
         '-wc',
         '--worker-cpus',
         help='The number of CPUs used by the local worker. Will be directly passed to OMP_NUM_THREADS.',
     ),
 ]
 WorkerEnvAnnotation = Annotated[
-    Dict,
+    Optional[Dict],
     typer.Option(
         '-we',
         '--worker-env',
         help='Further environment variables to be set for the local worker.',
         metavar='JSON',
         parser=json.loads,
     ),
@@ -253,14 +259,35 @@
     bool,
     typer.Option(
         '--no-resolve-descriptions',
         help='Whether to prevent using omegaconf to resolve experiment descriptions',
         is_flag=True,
     ),
 ]
+DebugAnnotation = Annotated[
+    bool,
+    typer.Option(
+        '-d',
+        '--debug',
+        help='Run a single interactive experiment without Sacred observers and with post-mortem debugging. '
+        'Implies `--verbose --num-exps 1 --post-mortem --output-to-console`.',
+        is_flag=True,
+    ),
+]
+
+DebugServerAnnotation = Annotated[
+    bool,
+    typer.Option(
+        '-ds',
+        '--debug-server',
+        help='Run the experiment with a debug server, to which you can remotely connect with e.g. VS Code. '
+        'Implies `--debug`.',
+        is_flag=True,
+    ),
+]
 
 
 def version_callback(value: bool):
     if value:
         from seml import __version__
 
         print(__version__)
@@ -299,15 +326,15 @@
 ):
     """SEML - Slurm Experiment Management Library."""
     from rich.logging import RichHandler
 
     from seml.console import console
 
     if len(logging.root.handlers) == 0:
-        logging_level = logging.VERBOSE if verbose else logging.INFO
+        logging_level = logging.NOTSET if verbose else logging.INFO
         handler = RichHandler(
             logging_level,
             console=console,
             show_path=False,
             show_level=True,
             show_time=False,
         )
@@ -381,15 +408,15 @@
         typer.Option(
             '-l',
             '--lab',
             help='Start a jupyter-lab instance instead of jupyter notebook.',
         ),
     ] = False,
     conda_env: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-c',
             '--conda-env',
             help='Start the Jupyter instance in a Conda environment.',
         ),
     ] = None,
     sbatch_options: SBatchOptionsAnnotation = None,
@@ -493,25 +520,25 @@
             '-f',
             '--force',
             help='Force adding the experiment even if it already exists in the database.',
             is_flag=True,
         ),
     ] = False,
     overwrite_params: Annotated[
-        Dict,
+        Optional[Dict],
         typer.Option(
             '-o',
             '--overwrite-params',
             help='Dictionary (passed as a string, e.g. \'{"epochs": 100}\') to overwrite parameters in the config.',
             metavar='JSON',
             parser=json.loads,
         ),
     ] = None,
     description: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-d',
             '--description',
             help='A description for the experiment.',
         ),
     ] = None,
     no_resolve_descriptions: NoResolveDescriptionAnnotation = False,
@@ -535,34 +562,16 @@
 @app.command('start')
 @restrict_collection()
 def start_command(
     ctx: typer.Context,
     sacred_id: SacredIdAnnotation = None,
     filter_dict: FilterDictAnnotation = None,
     batch_id: BatchIdAnnotation = None,
-    debug: Annotated[
-        bool,
-        typer.Option(
-            '-d',
-            '--debug',
-            help='Run a single interactive experiment without Sacred observers and with post-mortem debugging. '
-            'Implies `--verbose --num-exps 1 --post-mortem --output-to-console`.',
-            is_flag=True,
-        ),
-    ] = False,
-    debug_server: Annotated[
-        bool,
-        typer.Option(
-            '-ds',
-            '--debug-server',
-            help='Run the experiment with a debug server, to which you can remotely connect with e.g. VS Code. '
-            'Implies `--debug`.',
-            is_flag=True,
-        ),
-    ] = False,
+    debug: DebugAnnotation = False,
+    debug_server: DebugServerAnnotation = False,
     local: Annotated[
         bool,
         typer.Option(
             '-l',
             '--local',
             help='Run the experiment locally instead of on a Slurm cluster.',
             is_flag=True,
@@ -614,14 +623,16 @@
 @restrict_collection()
 def launch_worker_command(
     ctx: typer.Context,
     num_exps: NumExperimentsAnnotation = 0,
     no_file_output: NoFileOutputAnnotation = False,
     steal_slurm: StealSlurmAnnotation = False,
     post_mortem: PostMortemAnnotation = False,
+    debug: DebugAnnotation = False,
+    debug_server: DebugServerAnnotation = False,
     output_to_console: OutputToConsoleAnnotation = False,
     worker_gpus: WorkerGPUsAnnotation = None,
     worker_cpus: WorkerCPUsAnnotation = None,
     worker_env: WorkerEnvAnnotation = None,
     sacred_id: SacredIdAnnotation = None,
     filter_dict: FilterDictAnnotation = None,
     batch_id: BatchIdAnnotation = None,
@@ -633,14 +644,16 @@
         ctx.obj['collection'],
         local=True,
         sacred_id=sacred_id,
         batch_id=batch_id,
         filter_dict=filter_dict,
         num_exps=num_exps,
         post_mortem=post_mortem,
+        debug=debug,
+        debug_server=debug_server,
         output_to_console=output_to_console,
         no_file_output=no_file_output,
         steal_slurm=steal_slurm,
         no_worker=False,
         set_to_pending=False,
         worker_gpus=worker_gpus,
         worker_cpus=worker_cpus,
@@ -656,15 +669,15 @@
     filter_dict: FilterDictAnnotation = None,
     batch_id: BatchIdAnnotation = None,
     filter_states: FilterStatesAnnotation = [
         *States.FAILED,
         *States.KILLED,
         *States.INTERRUPTED,
     ],
-    projection: ProjectionAnnotation = None,
+    projection: ProjectionAnnotation = [],
 ):
     """
     Prints fail traces of all failed experiments.
     """
     print_fail_trace(
         ctx.obj['collection'],
         sacred_id=sacred_id,
@@ -685,15 +698,15 @@
             '-k',
             '-keep-old',
             help='Keep the old source files in the database.',
             is_flag=True,
         ),
     ] = False,
     batch_ids: Annotated[
-        List[int],
+        Optional[List[int]],
         typer.Option(
             '-b',
             '--batch-ids',
             help='Batch IDs (batch_id in the database collection) of the experiments. '
             'Experiments that were staged together have the same batch_id.',
         ),
     ] = None,
@@ -867,15 +880,15 @@
 
 
 @app.command('status')
 @restrict_collection()
 def status_command(
     ctx: typer.Context,
     update_status: UpdateStatusAnnotation = True,
-    projection: ProjectionAnnotation = None,
+    projection: ProjectionAnnotation = [],
 ):
     """
     Report status of experiments in the database collection.
     """
     print_status(
         ctx.obj['collection'], update_status=update_status, projection=projection
     )
@@ -920,15 +933,15 @@
     description: Annotated[
         str,
         typer.Argument(
             help='The description to set.',
         ),
     ],
     sacred_id: SacredIdAnnotation = None,
-    filter_states: FilterStatesAnnotation = None,
+    filter_states: FilterStatesAnnotation = [],
     filter_dict: FilterDictAnnotation = None,
     batch_id: BatchIdAnnotation = None,
     yes: YesAnnotation = False,
     no_resolve_description: NoResolveDescriptionAnnotation = False,
 ):
     """
     Sets the description of experiment(s).
@@ -946,15 +959,15 @@
 
 
 @app_description.command('delete')
 @restrict_collection()
 def description_delete_command(
     ctx: typer.Context,
     sacred_id: SacredIdAnnotation = None,
-    filter_states: FilterStatesAnnotation = None,
+    filter_states: FilterStatesAnnotation = [],
     filter_dict: FilterDictAnnotation = None,
     batch_id: BatchIdAnnotation = None,
     yes: YesAnnotation = False,
 ):
     """
     Deletes the description of experiment(s).
     """
@@ -1004,47 +1017,47 @@
         typer.Option(
             '-t',
             '--template',
             help='The template to use for the project. To view available templates use `seml project list-templates`.',
         ),
     ] = 'default',
     project_name: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-n',
             '--name',
             help='The name of the project. (By default inferred from the directory name.)',
         ),
     ] = None,
     user_name: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-u',
             '--username',
             help='The author name to use for the project. (By default inferred from $USER)',
         ),
     ] = None,
     user_mail: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-m',
             '--usermail',
             help='The author email to use for the project. (By default empty.)',
         ),
     ] = None,
     git_remote: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-r',
             '--git-remote',
             help='The git remote to use for the project. (By default SETTINGS.TEMPLATE_REMOTE.)',
         ),
     ] = None,
     git_commit: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-c',
             '--git-commit',
             help='The exact git commit to use. May also be a tag or branch (By default latest)',
         ),
     ] = None,
     yes: YesAnnotation = False,
@@ -1065,23 +1078,23 @@
 
 
 @app_project.command('list-templates')
 @restrict_collection(False)
 def list_templates_command(
     ctx: typer.Context,
     git_remote: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-r',
             '--git-remote',
             help='The git remote to use for the project. (By default SETTINGS.TEMPLATE_REMOTE.)',
         ),
     ] = None,
     git_commit: Annotated[
-        str,
+        Optional[str],
         typer.Option(
             '-c',
             '--git-commit',
             help='The exact git commit to use. May also be a tag or branch (By default latest)',
         ),
     ] = None,
 ):
```

### Comparing `seml-0.4.4/src/seml/add.py` & `seml-0.4.5/src/seml/add.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/config.py` & `seml-0.4.5/src/seml/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
     elif len(exps) > 1:
         raise ExecutableError(
             f"Found more than 1 Sacred experiment in '{executable}'. "
             f"Can't resolve configs."
         )
     exp = exps[0]
     if not isinstance(exp, Experiment):
-        logging.warn(
+        logging.warning(
             'The use of sacred.Experiment is deprecated. Please use seml.experiment.Experiment instead.\n'
             'seml.experiment.Experiment already includes typical MongoDB observer and logging setups.\n'
             'Please familiar yourself with the new API and adjust your code accordingly.\n'
             'See https://github.com/TUM-DAML/seml/blob/master/examples/example_experiment.py'
         )
     with working_directory(working_dir):
         return _sacred_create_configs(exp, configs, named_configs)
```

### Comparing `seml-0.4.4/src/seml/configure.py` & `seml-0.4.5/src/seml/configure.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/console.py` & `seml-0.4.5/src/seml/console.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/database.py` & `seml-0.4.5/src/seml/database.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/description.py` & `seml-0.4.5/src/seml/description.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/errors.py` & `seml-0.4.5/src/seml/errors.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/evaluation.py` & `seml-0.4.5/src/seml/evaluation.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/experiment.py` & `seml-0.4.5/src/seml/experiment.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/json.py` & `seml-0.4.5/src/seml/json.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/manage.py` & `seml-0.4.5/src/seml/manage.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/mattermost_observer.py` & `seml-0.4.5/src/seml/mattermost_observer.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/module_hider.py` & `seml-0.4.5/src/seml/module_hider.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/network.py` & `seml-0.4.5/src/seml/network.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/observers.py` & `seml-0.4.5/src/seml/observers.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/parameters.py` & `seml-0.4.5/src/seml/parameters.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/prepare_experiment.py` & `seml-0.4.5/src/seml/prepare_experiment.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/project.py` & `seml-0.4.5/src/seml/project.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/settings.py` & `seml-0.4.5/src/seml/settings.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/sources.py` & `seml-0.4.5/src/seml/sources.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/start.py` & `seml-0.4.5/src/seml/start.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,20 +945,20 @@
                 # tq.set_postfix(current_id=exp['_id'], failed=f"{num_exceptions}/{jobs_counter} experiments")
 
 
 def print_command(
     db_collection_name: str,
     sacred_id: Optional[int],
     batch_id: Optional[int],
-    filter_states: List,
-    filter_dict: Dict,
+    filter_states: List[str],
+    filter_dict: Optional[Dict],
     num_exps: int,
     worker_gpus: Optional[str] = None,
     worker_cpus: Optional[int] = None,
-    worker_environment_vars: Dict = None,
+    worker_environment_vars: Optional[Dict] = None,
     unresolved: bool = False,
     resolve_interpolations: bool = True,
 ):
     import rich
 
     from seml.console import Heading, console
 
@@ -967,15 +967,15 @@
     filter_dict = build_filter_dict(filter_states, batch_id, filter_dict, sacred_id)
 
     env_dict = get_environment_variables(
         worker_gpus, worker_cpus, worker_environment_vars
     )
 
     orig_level = logging.root.level
-    logging.root.setLevel(logging.VERBOSE)
+    logging.root.setLevel(logging.NOTSET)
 
     exps_list = list(collection.find(filter_dict, limit=num_exps))
     if len(exps_list) == 0:
         return
 
     exp = exps_list[0]
     _, exe, config = get_command_from_exp(
@@ -1155,15 +1155,17 @@
             cpus=worker_cpus,
             environment_variables=worker_environment_vars,
             debug_server=debug_server,
         )
 
 
 def start_jupyter_job(
-    sbatch_options: dict = None, conda_env: str = None, lab: bool = False
+    sbatch_options: Optional[dict] = None,
+    conda_env: Optional[str] = None,
+    lab: bool = False,
 ):
     sbatch_options = sbatch_options if sbatch_options is not None else {}
     sbatch_options_merged = SETTINGS.SLURM_DEFAULT['sbatch_options']
     sbatch_options_merged.update(SETTINGS.SBATCH_OPTIONS_TEMPLATES.JUPYTER)
     sbatch_options_merged.update(sbatch_options)
     # Construct sbatch options string
     sbatch_options_str = create_slurm_options_string(sbatch_options_merged)
```

### Comparing `seml-0.4.4/src/seml/templates/slurm/jupyter_template.sh` & `seml-0.4.5/src/seml/templates/slurm/jupyter_template.sh`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/templates/slurm/slurm_template.sh` & `seml-0.4.5/src/seml/templates/slurm/slurm_template.sh`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml/utils.py` & `seml-0.4.5/src/seml/utils.py`

 * *Files identical despite different names*

### Comparing `seml-0.4.4/src/seml.egg-info/PKG-INFO` & `seml-0.4.5/src/seml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seml
-Version: 0.4.4
+Version: 0.4.5
 Summary: Slurm Experiment Management Library
 Author: DAML Group @ TUM
 Author-email: Daniel Zügner <zuegnerd@in.tum.de>, Johannes Gsteiger <johannes.gasteiger@tum.de>, Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 Maintainer-email: Nicholas Gao <n.gao@tum.de>, Dominik Fuchsgruber <d.fuchsgruber@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Johannes Klicpera, Daniel Zügner, Nicholas Gao
@@ -45,14 +45,15 @@
 Requires-Dist: munch>=2.0.4
 Requires-Dist: debugpy>=1.2.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: typer<1.0,>=0.9
 Requires-Dist: rich<14.0,>=13.0
 Requires-Dist: omegaconf<3.0,>=2.3.0
 Requires-Dist: gitignore_parser>=0.1.11
+Requires-Dist: setuptools>=69.2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: ssh-forward
 Requires-Dist: sshtunnel>=0.4.0; extra == "ssh-forward"
 Requires-Dist: filelock>=3.13.3; extra == "ssh-forward"
```

### Comparing `seml-0.4.4/src/seml.egg-info/SOURCES.txt` & `seml-0.4.5/src/seml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

