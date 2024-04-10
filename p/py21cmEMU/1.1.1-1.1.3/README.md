# Comparing `tmp/py21cmemu-1.1.1.tar.gz` & `tmp/py21cmemu-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py21cmemu-1.1.1.tar", max compression
+gzip compressed data, was "py21cmemu-1.1.3.tar", max compression
```

## Comparing `py21cmemu-1.1.1.tar` & `py21cmemu-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-10-25 13:10:56.576297 py21cmemu-1.1.1/LICENSE
--rw-r--r--   0        0        0     2481 2023-10-25 13:10:56.576297 py21cmemu-1.1.1/README.rst
--rw-r--r--   0        0        0     2387 2023-10-25 13:11:16.116414 py21cmemu-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      405 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/__init__.py
--rw-r--r--   0        0        0     3359 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/config.py
--rw-r--r--   0        0        0     3564 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/emulator.py
--rw-r--r--   0        0        0    16226 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/emulator_constants.npz
--rw-r--r--   0        0        0     2444 2023-10-25 13:11:16.116414 py21cmemu-1.1.1/src/py21cmemu/get_emulator.py
--rw-r--r--   0        0        0     5399 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/inputs.py
--rw-r--r--   0        0        0     7670 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/outputs.py
--rw-r--r--   0        0        0     2860 2023-10-25 13:10:56.604297 py21cmemu-1.1.1/src/py21cmemu/properties.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 py21cmemu-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-04-10 15:12:49.641367 py21cmemu-1.1.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1073 2024-04-10 15:12:49.641367 py21cmemu-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2481 2024-04-10 15:12:49.641367 py21cmemu-1.1.3/README.rst
+-rw-r--r--   0        0        0     2399 2024-04-10 15:13:01.685348 py21cmemu-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      405 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/__init__.py
+-rw-r--r--   0        0        0     3360 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/config.py
+-rw-r--r--   0        0        0     3565 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/emulator.py
+-rw-r--r--   0        0        0    16226 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/emulator_constants.npz
+-rw-r--r--   0        0        0     2445 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/get_emulator.py
+-rw-r--r--   0        0        0     5400 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/inputs.py
+-rw-r--r--   0        0        0     7671 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/outputs.py
+-rw-r--r--   0        0        0     2861 2024-04-10 15:12:49.661367 py21cmemu-1.1.3/src/py21cmemu/properties.py
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 py21cmemu-1.1.3/PKG-INFO
```

### Comparing `py21cmemu-1.1.1/LICENSE` & `py21cmemu-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.1.1/README.rst` & `py21cmemu-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.1.1/pyproject.toml` & `py21cmemu-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py21cmEMU"
-version = "1.1.1"
+version = "1.1.3"
 description = "Emulator of 21cmFAST summaries."
 authors = ["Daniela Breitman <daniela.breitman@sns.it>"]
 license = "MIT"
 readme = ["README.rst"]
 homepage = "https://github.com/21cmFAST/21cmEMU"
 repository = "https://github.com/21cmFAST/21cmEMU"
 documentation = "https://21cmEMU.readthedocs.io"
@@ -30,15 +30,15 @@
 Changelog = "https://github.com/21cmFAST/21cmEMU/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = ">=8.0.1"
 numpy = "^1.22.0"
 scipy = "^1.10.1"
-tensorflow = "^2.6.0"
+tensorflow = ">=2.4.0, <= 2.14.0"
 appdirs = "^1.4.4"
 toml = "^0.10.2"
 GitPython = "^3.1.31"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/config.py` & `py21cmemu-1.1.3/src/py21cmemu/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """User-facing configuration for py21cmEMU."""
+
 from __future__ import annotations
 
 import logging
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any
 from typing import Generator
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/emulator.py` & `py21cmemu-1.1.3/src/py21cmemu/emulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that interacts with the Emulator Tensorflow model."""
+
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 import tensorflow as tf
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/emulator_constants.npz` & `py21cmemu-1.1.3/src/py21cmemu/emulator_constants.npz`

 * *Files identical despite different names*

### Comparing `py21cmemu-1.1.1/src/py21cmemu/get_emulator.py` & `py21cmemu-1.1.3/src/py21cmemu/get_emulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Download and install the emulator data."""
+
 from __future__ import annotations
 
 import logging
 from warnings import warn
 
 import git
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/inputs.py` & `py21cmemu-1.1.3/src/py21cmemu/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing functionality for handling emulator inputs."""
+
 from __future__ import annotations
 
 from typing import Dict
 from typing import Sequence
 from typing import Union
 
 import numpy as np
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/outputs.py` & `py21cmemu-1.1.3/src/py21cmemu/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module whose functionality is to organise the emulator output."""
+
 from __future__ import annotations
 
 import dataclasses as dc
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Generator
```

### Comparing `py21cmemu-1.1.1/src/py21cmemu/properties.py` & `py21cmemu-1.1.3/src/py21cmemu/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A module definining the static properties of the Emulator."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 import numpy as np
```

### Comparing `py21cmemu-1.1.1/PKG-INFO` & `py21cmemu-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py21cmEMU
-Version: 1.1.1
+Version: 1.1.3
 Summary: Emulator of 21cmFAST summaries.
 Home-page: https://github.com/21cmFAST/21cmEMU
 License: MIT
 Keywords: Epoch of Reionization,Cosmology
 Author: Daniela Breitman
 Author-email: daniela.breitman@sns.it
 Requires-Python: >=3.8,<3.12
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: tensorflow (>=2.6.0,<3.0.0)
+Requires-Dist: tensorflow (>=2.4.0,<=2.14.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Changelog, https://github.com/21cmFAST/21cmEMU/releases
 Project-URL: Documentation, https://21cmEMU.readthedocs.io
 Project-URL: Repository, https://github.com/21cmFAST/21cmEMU
 Description-Content-Type: text/x-rst
 
 =======
```

