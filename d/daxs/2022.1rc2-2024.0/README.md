# Comparing `tmp/daxs-2022.1rc2.tar.gz` & `tmp/daxs-2024.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daxs-2022.1rc2.tar", last modified: Tue Sep 27 08:31:00 2022, max compression
+gzip compressed data, was "daxs-2024.0.tar", last modified: Wed Apr 10 14:39:06 2024, max compression
```

## Comparing `daxs-2022.1rc2.tar` & `daxs-2024.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2022-09-27 08:31:00.817058 daxs-2022.1rc2/
--rw-r--r--   0 marius     (501) staff       (20)     1101 2022-04-22 13:01:47.000000 daxs-2022.1rc2/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)     2889 2022-09-27 08:31:00.817222 daxs-2022.1rc2/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     2139 2022-09-02 13:43:13.000000 daxs-2022.1rc2/README.md
--rw-r--r--   0 marius     (501) staff       (20)       90 2022-09-02 13:43:27.000000 daxs-2022.1rc2/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)     1557 2022-09-27 08:31:00.818013 daxs-2022.1rc2/setup.cfg
--rw-r--r--   0 marius     (501) staff       (20)       69 2021-10-27 09:45:33.000000 daxs-2022.1rc2/setup.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2022-09-27 08:31:00.795962 daxs-2022.1rc2/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2022-09-27 08:31:00.805551 daxs-2022.1rc2/src/daxs/
--rw-r--r--   0 marius     (501) staff       (20)      103 2022-09-27 08:27:13.000000 daxs-2022.1rc2/src/daxs/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3463 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/filters.py
--rw-r--r--   0 marius     (501) staff       (20)     1884 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/interpolators.py
--rw-r--r--   0 marius     (501) staff       (20)    20592 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/measurements.py
--rw-r--r--   0 marius     (501) staff       (20)     9522 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/scans.py
--rw-r--r--   0 marius     (501) staff       (20)     7762 2022-09-27 08:23:59.000000 daxs-2022.1rc2/src/daxs/sources.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2022-09-27 08:31:00.809806 daxs-2022.1rc2/src/daxs/tests/
--rw-r--r--   0 marius     (501) staff       (20)        0 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     1046 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/conftest.py
--rw-r--r--   0 marius     (501) staff       (20)      926 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_filters.py
--rw-r--r--   0 marius     (501) staff       (20)       74 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_import.py
--rw-r--r--   0 marius     (501) staff       (20)     6993 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_measurements.py
--rw-r--r--   0 marius     (501) staff       (20)     3881 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_scans.py
--rw-r--r--   0 marius     (501) staff       (20)     2033 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_sources.py
--rw-r--r--   0 marius     (501) staff       (20)      626 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/tests/test_utils.py
--rw-r--r--   0 marius     (501) staff       (20)     3034 2022-09-02 13:43:27.000000 daxs-2022.1rc2/src/daxs/utils.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2022-09-27 08:31:00.807464 daxs-2022.1rc2/src/daxs.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)     2889 2022-09-27 08:31:00.000000 daxs-2022.1rc2/src/daxs.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)      598 2022-09-27 08:31:00.000000 daxs-2022.1rc2/src/daxs.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2022-09-27 08:31:00.000000 daxs-2022.1rc2/src/daxs.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)      197 2022-09-27 08:31:00.000000 daxs-2022.1rc2/src/daxs.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        5 2022-09-27 08:31:00.000000 daxs-2022.1rc2/src/daxs.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.721764 daxs-2024.0/
+-rw-r--r--   0 marius     (501) staff       (20)     1101 2024-04-10 14:14:43.000000 daxs-2024.0/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)     4235 2024-04-10 14:39:06.721422 daxs-2024.0/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     2822 2023-10-19 13:31:45.000000 daxs-2024.0/README.md
+-rw-r--r--   0 marius     (501) staff       (20)     2904 2024-04-10 14:11:23.000000 daxs-2024.0/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)       38 2024-04-10 14:39:06.721844 daxs-2024.0/setup.cfg
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.713101 daxs-2024.0/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.715972 daxs-2024.0/src/daxs/
+-rw-r--r--   0 marius     (501) staff       (20)       99 2024-04-10 14:12:28.000000 daxs-2024.0/src/daxs/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      804 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/config.py
+-rw-r--r--   0 marius     (501) staff       (20)     3488 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/filters.py
+-rw-r--r--   0 marius     (501) staff       (20)     2018 2023-11-07 13:45:30.000000 daxs-2024.0/src/daxs/interpolators.py
+-rw-r--r--   0 marius     (501) staff       (20)    21715 2023-11-07 13:45:30.000000 daxs-2024.0/src/daxs/measurements.py
+-rw-r--r--   0 marius     (501) staff       (20)    10459 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/scans.py
+-rw-r--r--   0 marius     (501) staff       (20)     7521 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/sources.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.718928 daxs-2024.0/src/daxs/tests/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/tests/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     1173 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/tests/conftest.py
+-rw-r--r--   0 marius     (501) staff       (20)      911 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/tests/test_filters.py
+-rw-r--r--   0 marius     (501) staff       (20)       74 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/tests/test_import.py
+-rw-r--r--   0 marius     (501) staff       (20)     6816 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/tests/test_measurements.py
+-rw-r--r--   0 marius     (501) staff       (20)     3906 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/tests/test_scans.py
+-rw-r--r--   0 marius     (501) staff       (20)     2349 2024-04-10 14:11:23.000000 daxs-2024.0/src/daxs/tests/test_sources.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.720146 daxs-2024.0/src/daxs/utils/
+-rw-r--r--   0 marius     (501) staff       (20)      209 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/utils/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      460 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/utils/arrays.py
+-rw-r--r--   0 marius     (501) staff       (20)     1323 2023-11-07 13:14:58.000000 daxs-2024.0/src/daxs/utils/bragg.py
+-rw-r--r--   0 marius     (501) staff       (20)     3347 2023-11-07 13:45:30.000000 daxs-2024.0/src/daxs/utils/material.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-04-10 14:39:06.720385 daxs-2024.0/src/daxs.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     4235 2024-04-10 14:39:06.000000 daxs-2024.0/src/daxs.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      654 2024-04-10 14:39:06.000000 daxs-2024.0/src/daxs.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2024-04-10 14:39:06.000000 daxs-2024.0/src/daxs.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)      186 2024-04-10 14:39:06.000000 daxs-2024.0/src/daxs.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        5 2024-04-10 14:39:06.000000 daxs-2024.0/src/daxs.egg-info/top_level.txt
```

### Comparing `daxs-2022.1rc2/LICENSE` & `daxs-2024.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2022 European Synchrotron Radiation Facility
+Copyright (c) 2020-2024 European Synchrotron Radiation Facility
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `daxs-2022.1rc2/README.md` & `daxs-2024.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 # Data Analysis for X-ray Spectroscopy
 
-## Installation
+## Usage at the ESRF
 
-You can install the development version using:
-`python3 -m pip install [--ignore-installed] https://gitlab.esrf.fr/spectroscopy/daxs/-/archive/main/daxs-main.tar`
+### In scripts
 
-The `--ignore-installed` argument **is required** if you want to upgrade an
-existing installation.
+If you want to use the library in scripts you execute on the ESRF computing cluster, follow the steps below.
 
-It is best if you install the library in a virtual environment to avoid messing
-up other Python packages. See [the official
-documentation](https://docs.python.org/3/tutorial/venv.html) on how to create
-and use virtual environments.
+1. Use a terminal to log in on one of the computing cluster front ends: `ssh -Y account@slurm-nice-devel`. The `account` can be your personal SMIS account or the user experiment number. Enter the associated password when prompted.
+2. Ask for resources: `srun --x11 --pty bash -l`. This will give you an interactive shell from which you can also start code editors like `Spyder`. In addition, you can add `--time=hh:mm:ss` to specify the maximum time the resources will be available; by default, it will be 1 hour.
+3. Load the spectroscopy environment module: `module load spectroscopy`. The command loads an environment that contains the development version of the `daxs` library.
+4. Print the version of the library to test that everything went smoothly: `python -c "import daxs; print(daxs.__version__)"`.
 
-## Usage at the ESRF
+If all goes well with the previous command and you don't get an error, you should be able to use the library in your scripts.
+
+### In Jupyter notebooks
 
-### Scripts and command line
+You can also use the library in Jupyter notebooks.
 
-To use the library on the computing cluster, follow the steps below.
+1. Connect to <https://jupyter-slurm.esrf.fr>.
+2. Select the `Spectroscopy (latest)` in the `Jupyter environment` drop-down menu.
+3. Change the `Job duration` in case you need to run your notebook for a longer time, than the default 1 hour.
+4. Press `Start` at the bottom of the page.
 
-1. Login on the front-end: `ssh -Y slurm-nice-devel`
-2. Ask for resources: `srun --pty bash`
-3. Load the spectroscopy module: `module load conda; module load spectroscopy`.
-  The command loads a Python virtual environment that contains the latest version
-  of the library.
-4. Print the version of the library to test that everything went smoothly:
-  `python -c "import daxs; print(daxs.__version__)"`
+![image](https://gitlab.esrf.fr/spectroscopy/daxs/-/raw/main/doc/images/jupyter-slurm.png){width=35%}
 
-If all went well, you should be able to use the library in your scripts.
+You can find more information about Jupyter at ESRF [here](https://confluence.esrf.fr/display/DAUWK/Jupyter+@+ESRF).
 
-### JupyterHub
+While this simplifies the usage, you will not be able to add Python packages to the virtual environment. If you want to use additional packages not present in the environment, either open an issue [here](https://gitlab.esrf.fr/apptainer/spectroscopy/-/issues) or install the library in your home directory, in a virtual environment (see below).
 
-You can also use the library in a Jupyter Notebook. Follow steps 1-3
-from above. Next, install the kernel by running `kernel-install`.
+## Local installation on your computer
 
-After, connect to <https://jupyter-slurm.esrf.fr> and start a server on
-the Intel partition. On the right-hand side, press *New*. The Python
-environment should be in the list, as shown in the image below. Select
-it to create a new Jupyter Notebook.
+You can install the latest release of the library using:
 
-![image](https://gitlab.esrf.fr/spectroscopy/daxs/-/raw/main/doc/images/jupyter.png)
+`python3 -m pip install daxs`
 
-Run `kernel-remove` to remove the kernel. Alternatively, you can use the
-`jupyter kernelspec` command to manage the kernels.
+If you want to use the latest development version, you can install it directly with:
+
+`python3 -m pip install [--ignore-installed] https://gitlab.esrf.fr/spectroscopy/daxs/-/archive/main/daxs-main.tar`
+
+The `--ignore-installed` argument **is required** if you want to upgrade an
+existing installation.
 
-While this simplifies the usage, you will not be able to add Python packages to
-the virtual environment. If you want to use additional packages not present in
-the environment, the best approach is to install the library in your home
-directory, in a virtual environment.
+It is best if you install the library in a virtual environment to avoid messing up other Python packages. See [the official documentation](https://docs.python.org/3/tutorial/venv.html) on how to create and use virtual environments.
 
 ## Documentation
 
-The documentation can be found at
-<https://spectroscopy.gitlab-pages.esrf.fr/daxs>.
+The documentation can be found at <https://spectroscopy.gitlab-pages.esrf.fr/daxs>.
```

### Comparing `daxs-2022.1rc2/src/daxs/filters.py` & `daxs-2024.0/src/daxs/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# coding: utf-8
 """The module provides functions for filtering data."""
+from __future__ import annotations
+
 import logging
 
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 
 def hampel(data, window_size=None, threshold=3.5, axis=0):
-    """Outliers detection using the Hampel filter.
+    """
+    Outliers detection using the Hampel filter.
 
     More details about the filter can be found here:
 
     - https://fr.mathworks.com/help/dsp/ref/hampelfilter.html
     - https://dsp.stackexchange.com/questions/26552
     - https://stackoverflow.com/questions/22354094
```

### Comparing `daxs-2022.1rc2/src/daxs/interpolators.py` & `daxs-2024.0/src/daxs/interpolators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# coding: utf-8
 """The module provides interpolators."""
+from __future__ import annotations
+
 import logging
 
 import numpy as np
 from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
 
 logger = logging.getLogger(__name__)
 
 
 class Interpolator2D:
     """Two-dimensional interpolator."""
 
-    def __init__(self, x, y, z, kind="linear", fill_value=np.nan):
-
+    def __init__(self, x, y, z, kind="linear", fill_value=np.nan):  # noqa: PLR0913
         """
 
         Parameters
         ----------
         x : numpy.array
             X-axis values (1-D array)
         y : numpy.array
@@ -24,14 +24,15 @@
         z : numpy.array
             Data values (1-D array)
         kind : {'nearest', 'linear'}
             The kind of interpolation to use.
         fill_value : float
             Value used to fill in for requested points outside of the convex hull
             of the input points.
+
         """
         self.x = x
         self.y = y
         self.z = z
 
         self.kind = kind
         self.fill_value = fill_value
@@ -42,14 +43,16 @@
     def interpolator(self):
         """The actual interpolator."""
         if self._interpolator is None:
             if self.kind == "nearest":
                 interp = NearestNDInterpolator((self.x, self.y), self.z)
             elif self.kind == "linear":
                 interp = LinearNDInterpolator((self.x, self.y), self.z, self.fill_value)
+            else:
+                raise ValueError(f"Unknown interpolation method: {self.kind}")
             self._interpolator = interp
         return self._interpolator
 
     def update(self, parameters=None):
         """Update the interpolator parameters."""
         if parameters is None or not parameters:
             return
```

### Comparing `daxs-2022.1rc2/src/daxs/measurements.py` & `daxs-2024.0/src/daxs/measurements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-# coding: utf-8
 """The module provides classes to deal with different types of measurements."""
+from __future__ import annotations
 
 import copy
 import logging
-from typing import Any, Dict, List, Union
 
 import numpy as np
 
 from daxs.interpolators import Interpolator2D
 from daxs.scans import Scan
 from daxs.sources import Hdf5Source, Source
 
 logger = logging.getLogger(__name__)
 
 
 class Measurement:
     """Base class for measurements."""
 
-    def __init__(self, sources: Union[Source, List[Source]] = None):
+    def __init__(self, sources: Source | list[Source]):
         """
         Parameters
         ----------
         sources :
             Sources of scans.
-        """
-        assert sources is not None, "The sources argument is required."
 
+        """
         if isinstance(sources, Source):
             sources = [sources]
         self.sources = sources
 
-        self._scans: Any = None
+        self._scans = None
         self._x, self._signal, self._monitor = None, None, None
 
     @property
-    def scans(self) -> List[Scan]:
+    def scans(self) -> list[Scan]:
         """The scans of the measurement."""
         if self._scans is None:
-            scans: List[Scan] = []
+            scans: list[Scan] = []
             for source in self.sources:
                 scans.extend(source.scans)
 
             if len(scans) == 0:
                 raise ValueError("The measurement has no scans.")
 
             # Sanity check the scans.
@@ -64,69 +62,74 @@
 
                 reference = scan
 
             self._scans = scans
         return self._scans
 
     def get_scans_common_axis(
-        self, axis: str = "x", mode: str = "intersection", sort: bool = False
+        self, label: str = "x", mode: str = "intersection", sort: bool = False
     ) -> np.ndarray:
-        """The common axis of the scans in the measurement."""
         # If there is a single scan, use its axis as the common axis.
         if len(self.scans) == 1:
             [scan] = self.scans
-            return getattr(scan, axis)
+            return getattr(scan, label)
 
-        start, stop, size = None, None, None
+        axis, start, stop, size, step = None, None, None, None, None
         for scan in self.scans:
-            a = getattr(scan, axis)
+            axis = getattr(scan, label)
+
+            step = np.abs((axis[0] - axis[-1]) / (axis.size - 1))
 
-            step = np.abs((a[0] - a[-1]) / (a.size - 1))
             message = (
-                f"{axis.upper()}-axis parameters for scan {scan.label}: "
-                f"start = {a[0]:.8f}, stop = {a[-1]:.8f}, step = {step:.8f} "
-                f"number of points = {a.size:d}."
+                f"{label.upper()}-axis parameters for scan {scan.label}: "
+                f"start = {axis[0]:.8f}, stop = {axis[-1]:.8f}, step = {step:.8f} "
+                f"number of points = {axis.size:d}."
             )
             logger.debug(message)
 
             if None in [start, stop, size]:
-                start, stop, size = a[0], a[-1], a.size
+                start, stop, size = axis[0], axis[-1], axis.size
                 continue
 
             if sort:
-                a = np.sort(a, kind="stable")
+                axis = np.sort(axis, kind="stable")
 
             if mode == "intersection":
-                start = max(start, a[0])
-                stop = min(stop, a[-1])
+                start = max(start, axis[0])
+                stop = min(stop, axis[-1])
             elif mode == "union":
-                start = min(start, a[0])
-                stop = max(stop, a[-1])
+                start = min(start, axis[0])
+                stop = max(stop, axis[-1])
             else:
                 raise ValueError(f"Unknown mode: {mode}.")
 
-            size = np.max([a.size, size])
+            size = np.max([axis.size, size])
 
-            a, step = np.linspace(start, stop, size, retstep=True)
+            axis, step = np.linspace(start, stop, size, retstep=True)
+
+        if axis is None or step is None:
+            raise ValueError("The common axis could not be determined.")
 
         message = (
             f"Common axis parameters using {mode} mode: "
-            f"min = {a.min():.8f}, max = {a.max():.8f}, step = {step:.8f}, "
-            f"number of points = {a.size:d}."
+            f"min = {axis.min():.8f}, max = {axis.max():.8f}, step = {step:.8f}, "
+            f"number of points = {axis.size:d}."
         )
         logger.info(message)
-        return a
+        return axis
 
-    def remove_scans(self, indices: Union[int, List[int]] = None) -> None:
-        """Remove scans from the measurement.
+    def remove_scans(self, indices: int | list[int] | None = None) -> None:
+        """
+        Remove scans from the measurement.
 
         Parameters
         ----------
         indices :
             Indices of the scans to be removed.
+
         """
         assert indices is not None, "The indices argument is required."
 
         if isinstance(indices, int):
             indices = [indices]
 
         for index in indices:
@@ -166,54 +169,61 @@
     @property
     def monitor(self):
         if self._monitor is None:
             self.process()
         return self._monitor
 
     def find_outliers(self, method="hampel", **kwargs):
-        """Find outliers in the data.
+        """
+        Find outliers in the data.
 
         See the docstring of :meth:`.scans.Scan.find_outliers`.
         """
-        for _, scan in enumerate(self.scans):
+        for scan in self.scans:
             scan.find_outliers(method=method, **kwargs)
 
     def remove_outliers(self, method="hampel", **kwargs):
-        """Remove outliers from the signal.
+        """
+        Remove outliers from the signal.
 
         See the docstring of :meth:`.scans.Scan.remove_outliers`.
         """
         logger.info("Removing outliers.")
         for scan in self.scans:
             scan.remove_outliers(method=method, **kwargs)
         self._signal = None
 
     def process(self, aggregation="fraction of sums", normalization=None):
-        """Process the scans data.
+        """
+        Process the scans data.
 
         The processing includes aggregating the data of the selected scans
         and normalizing the signal.
         """
         self.aggregate(mode=aggregation)
         if normalization is not None:
             self.normalize(mode=normalization)
 
     def aggregate(self, mode="fraction of sums"):
         # pylint: disable=too-many-branches
-        """Aggregate the scans signal using the selected mode. When present, the
-        aggregated monitor is always a sum of the monitors from the individual scans.
+        """
+        Aggregate the scans signal using the selected mode.
+
+        When present, the aggregated monitor is always a sum of the monitors from
+        the individual scans.
 
         Parameters
         ----------
         mode : str
             Defines how the signal is aggregated.
 
                 - "sum" : Sum of the signals from all scans.
                 - "fraction of sums" : Fraction of the signals sum and monitors sum.
                 - "sum of fractions" : Sum of the signal and monitor fractions.
+
         """
         for scan in self.scans:
             if scan.monitor is None:
                 logger.info(
                     "No monitor data for scan %s. Setting aggregation mode to sum.",
                     scan.label,
                 )
@@ -228,54 +238,57 @@
                 self._signal += scan.signal
             elif mode == "sum of fractions":
                 self._signal += scan.signal / scan.monitor
             elif mode == "fraction of sums":
                 self._signal += scan.signal
             else:
                 raise ValueError(f"Unknown aggregation mode {mode}.")
-            if mode != "sum":
+            if mode != "sum" and self._monitor is not None:
                 self._monitor += scan.monitor
 
         if mode == "fraction of sums":
             self._signal = self._signal / self._monitor
 
         logger.info("The scans data was aggregated using the %s mode.", mode)
 
     def normalize(self, mode: str = "area") -> None:
-        """Normalize the signal.
+        """
+        Normalize the signal.
 
         Parameters
         ----------
         mode :
             Defines how the signal is normalized.
 
               - "area": Normalize using the absolute signal area calculated using the
                 trapezoidal rule.
               - "maximum": Normalize using the absolute maximum intensity of the signal.
 
         Notes
         -----
         This will overwrite the original signal with the normalized one.
+
         """
         assert mode is not None, "The mode has to be defined."
 
         if self._signal is None:
             self.aggregate()
 
-        if mode == "area":
+        if mode == "area" and self._signal is not None:
             self._signal = self._signal / np.abs(np.trapz(self._signal, self.x))
-        elif mode == "maximum":
+        elif mode == "maximum" and self._signal is not None:
             self._signal = self._signal / np.abs(np.max(self._signal))
         else:
             raise ValueError(f"Unknown normalization mode {mode}.")
 
         logger.info("The signal was normalized using the %s.", mode)
 
     def dead_time_correction(self, tau=None, detection_time=None):
-        """Perform a dead time correction using a non-paralyzable model.
+        """
+        Perform a dead time correction using a non-paralyzable model.
 
         See the docstring of :meth:`.scans.Scan.dead_time_correction`.
         """
         assert tau is not None, "The detector dead time (tau) must be set."
         for scan in self.scans:
             scan.dead_time_correction(tau, detection_time)
 
@@ -283,60 +296,65 @@
         """Reset the measurement."""
         self._x, self._signal, self._monitor = None, None, None
         if scans:
             for scan in self.scans:
                 scan.reset()
 
     def save(self, filename=None, delimiter=","):
-        """Save the current x and signal to file.
+        """
+        Save the current x and signal to file.
 
         Parameters
         ----------
         filename : str
             Name of the output file.
         delimiter : str
             Column delimiter in the output file.
+
         """
         assert filename is not None, "The filename argument is required."
+        assert self.signal is not None, "The signal is not defined."
         with open(filename, "w", encoding="utf-8") as fp:
             fp.write("# x signal\n")
             data = np.array(list(zip(self.x, self.signal)))
             np.savetxt(fp, data, delimiter=delimiter, fmt="%.6e %.6e")
             logger.info("The data was saved to %s.", filename)
 
 
 class Xas(Measurement1D):
     """Class to represent a X-ray absorption measurement."""
 
 
 class Xes(Measurement1D):
     """Class to represent a X-ray emission measurement."""
 
-    def concentration_correction(
+    def concentration_correction(  # noqa: C901
         self,
-        indices: Union[int, List[int]] = None,
-        data_mappings: Dict[str, Any] = None,
-        scans: Union[Scan, List[Scan]] = None,
+        indices: int | list[int] | None = None,
+        data_mappings=None,
+        scans: Scan | list[Scan] | None = None,
     ) -> None:
-        """Apply the concentration correction using data from the specified scans.
+        """
+        Apply the concentration correction using data from the specified scans.
 
         Parameters
         ----------
         indices :
             Indices of the scans used for concentration correction.
         data_mappings :
             Mappings used to retrieve the data of the concentration correction scans.
         scans :
             Scans used for concentration corrections.
+
         """
         assert (
             indices is not None or scans is not None
         ), "Either the indices or scans must be specified."
 
-        conc_corr_scans: List[Scan] = []
+        conc_corr_scans: list[Scan] = []
 
         if indices is not None:
             if isinstance(indices, int):
                 indices = [indices]
 
             if len(self.sources) != 1:
                 raise ValueError(
@@ -376,15 +394,15 @@
             )
 
         for scan, conc_corr_scan in zip(self.scans, conc_corr_scans):
             # Signal data in the concentration correction scan must be sorted using
             # the same order as the one from the scan that is being corrected. The
             # assignment does that.
             conc_corr_scan.indices = copy.deepcopy(scan.indices)
-            scan = scan / conc_corr_scan
+            scan = scan / conc_corr_scan  # noqa: PLW2901
 
         # Force signal and monitor reevaluation.
         self._signal, self._monitor = None, None
 
 
 class Measurement2D(Measurement):
     """Base class for 2D measurements."""
@@ -422,21 +440,22 @@
         """The interpolator of the current plane."""
         if self._interpolator is None:
             self._interpolator = Interpolator2D(self.x, self.y, self.signal)
         return self._interpolator
 
     @property
     def acquisition_mode(self):
-        """There are two ways to measure a RIXS plane:
+        """
+        There are two ways to measure a RIXS plane:
 
         1. Step through a range of emission energies and scan the incoming
            (monochromator) energy for each step.
         2. Step through incoming (monochromator) energy and scan the emission energy.
         """
-        if all(isinstance(scan.y, (int, float)) for scan in self.scans):
+        if all(scan.y is not None and scan.y.size == 1 for scan in self.scans):
             mode = "absorption"
         else:
             mode = "emission"
         logger.debug("The RIXS plane was acquired in %s mode.", mode)
         return mode
 
     def reset(self, scans=True):
@@ -444,35 +463,56 @@
         self._x, self._y, self._signal, self._monitor = None, None, None, None
         self._interpolator = None
         self.cuts = {}
         if scans:
             for scan in self.scans:
                 scan.reset()
 
+    def find_outliers(self, method="hampel", **kwargs):
+        """
+        Find outliers in the data.
+
+        See the docstring of :meth:`.scans.Scan.find_outliers`.
+        """
+        for scan in self.scans:
+            scan.find_outliers(method=method, **kwargs)
+
+    def remove_outliers(self, method="hampel", **kwargs):
+        """
+        Remove outliers from the signal.
+
+        See the docstring of :meth:`.scans.Scan.remove_outliers`.
+        """
+        logger.info("Removing outliers.")
+        for scan in self.scans:
+            scan.remove_outliers(method=method, **kwargs)
+        self._signal = None
+
     def concentration_correction(
         self,
-        index: int = None,
-        data_mappings: Dict[str, Any] = None,
-        scan: Scan = None,
+        index: int | None = None,
+        data_mappings: str | None = None,
+        scan: Scan | None = None,
     ) -> None:
-        """Apply the concentration correction.
+        """
+        Apply the concentration correction.
 
         A point in the concentration correction scan is used to correct a scan
         of the plane.
 
         Parameters
         ----------
         index :
             Index of the scan used for concentration correction.
         data_mappings:
             Mappings used to retrieve the data of the concentration correction scan.
         scan:
             Scan used for concentration corrections.
-        """
 
+        """
         assert (
             index is not None or scan is not None
         ), "Either the index or scan must be specified."
 
         conc_corr_scan: Scan = None
 
         if index is not None:
@@ -508,15 +548,15 @@
 
         assert len(self.scans) == len(conc_corr_scan.signal), (
             "The number of points in the concentration correction ",
             "scan is not equal to the number of scans in the measurement.",
         )
 
         for i, scan in enumerate(self.scans):  # pylint: disable=all
-            scan = scan / (conc_corr_scan.signal[i], conc_corr_scan.monitor[i])
+            scan = scan / (conc_corr_scan.signal[i], conc_corr_scan.monitor[i])  # noqa
 
         self.reset(scans=False)
 
     def process(self):
         """Read and store the scans data."""
         acquisition_mode = self.acquisition_mode
 
@@ -541,22 +581,24 @@
 
             # Convert to energy transfer.
             y = x - y
 
         self._x, self._y, self._signal = x, y, signal
 
     def interpolate(self, xi=None, yi=None):
-        """Interpolate the plane using new axes.
+        """
+        Interpolate the plane using new axes.
 
         Parameters
         ----------
         xi : numpy.array
             The new X-axis.
         yi : numpy.array
             The new Y-axis.
+
         """
         if xi is None or yi is None:
             logger.info("Please specify both function arguments.")
             return
 
         xi, yi = np.meshgrid(xi, yi)
         signal = self.interpolator(xi, yi)
@@ -575,15 +617,16 @@
         # Assign the values.
         self._x, self._y, self._signal = x, y, signal
 
         # Update the interpolator.
         self.interpolator.update({"x": x, "y": y, "z": signal})
 
     def cut(self, mode="CEE", energies=None, npoints=1024):
-        """Calculate the cuts specified by the mode and energies.
+        """
+        Calculate the cuts specified by the mode and energies.
 
         Parameters
         ----------
         mode : str
             Defines the way to cut the plane:
 
             - "CEE" - constant emission energy
@@ -591,16 +634,19 @@
             - "CET" - constant energy transfer
 
         energies : list(float)
             Energies of the cuts.
 
         npoints : int
             Number of points for the cuts.
+
         """
         assert energies is not None, "The energies parameter must be defined."
+        assert isinstance(self.x, np.ndarray), "The x-axis is not defined."
+        assert isinstance(self.y, np.ndarray), "The y-axis is not defined."
 
         mode = mode.upper()
 
         # Update the xc and yc arrays depending on the type of cut.
         for energy in energies:
             xc = np.linspace(self.x.min(), self.x.max(), npoints)
             yc = np.linspace(self.y.min(), self.y.max(), npoints)
```

### Comparing `daxs-2022.1rc2/src/daxs/scans.py` & `daxs-2024.0/src/daxs/scans.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-# coding: utf-8
 """The module provides classes for the representation of scans in measurements."""
 
+from __future__ import annotations
+
 import copy
 import logging
-from typing import Optional
+from typing import Iterable
 
 import numpy as np
 
 from daxs.filters import hampel
-from daxs.utils import arrays_intersect
+from daxs.utils.arrays import intersect
 
 logger = logging.getLogger(__name__)
 
 
 class Scan:
     def __init__(
         self,
-        x: np.ndarray,
-        signal: np.ndarray,
-        data: dict = None,
+        x: np.ndarray | None = None,
+        signal: np.ndarray | None = None,
+        data: dict | None = None,
     ) -> None:
-
         """
-        Base class for the representation of scans in measurements.
+        Define the base representation of scans in measurements.
 
         Parameters
         ----------
         x :
             X-axis values (1D array).
         signal :
             Signal values (1D or 2D array). For a 2D array, the components must be
             stored as rows. A 1D array will be converted to a 2D array.
         data :
             Storage for the raw scan data and metadata.
+
         """
         assert x is not None, "The X-axis values must be set."
         assert signal is not None, "The signal values must be set."
 
         # Convert the signal to a 2D array.
         if signal.ndim == 1:
             signal = signal[np.newaxis, :]
 
         assert signal.ndim in (1, 2), "The signal must be a 1D or a 2D array."
 
         self._x = x
         self._y = None
         self._signal = signal
         self._monitor = None
-        self._data = {} if data is None else data
 
         # Array of indices used to reindex the data.
-        self._indices: Optional[np.ndarray] = None
+        self._indices: np.ndarray | None = None
 
-        # Copy the X-axis and signal values.
+        # Copy the X-axis and signal values to an internal data dictionary.
+        self._data = {} if data is None else data
         for attr in ("x", "signal"):
             self._data[attr] = copy.deepcopy(getattr(self, f"_{attr}"))
 
         self.outliers, self.medians = None, None
 
         self.reindex()
 
@@ -71,36 +72,38 @@
         a = np.sort(a, kind="stable")
 
         # Do nothing when receiving identical values.
         if np.array_equal(self._x, a):
             logger.debug("The new X-axis values are the same as the current ones.")
             return
 
-        if not arrays_intersect(a, self._x):
+        if not intersect(a, self._x):
             if self._x.shape == a.shape:
                 # If the new values are not within the current values, but the two
                 # arrays have the same shape, we simply assign the new values to the
                 # X-axis. This is useful when the X-axis changes to different units,
-                # e.g. angle to energy
+                # e.g. angle to energy.
                 logger.debug("Assigning the new X-axis values.")
                 self._x = np.copy(a)
                 self._indices = None
                 return
             raise ValueError(
                 "Incompatible values for the new X-axis; outside the current ones "
                 "and of different shape."
             )
         self.interpolate(a)
 
     @property
     def y(self):
-        try:
-            return self._data["y"]
-        except KeyError:
-            return None
+        if self._y is None:
+            try:
+                self._y = self._data["y"]
+            except KeyError:
+                self._y = None
+        return self._y
 
     @property
     def signal(self):
         if self._signal is None:
             self._signal = self._data["signal"]
         return self._signal.mean(axis=0)
 
@@ -122,22 +125,22 @@
         assert (
             a.shape == self._x.shape
         ), "The shape of the indices and X-axis arrays must be the same."
         self._indices = a
         self.reset()
 
     @property
-    def filename(self) -> Optional[str]:
+    def filename(self) -> str | None:
         try:
             return self.data["filename"]
         except KeyError:
             return None
 
     @property
-    def index(self) -> Optional[int]:
+    def index(self) -> int | None:
         try:
             return self.data["index"]
         except KeyError:
             return None
 
     @property
     def label(self) -> str:
@@ -149,73 +152,90 @@
 
     def reset(self):
         """Reset the scan data to the values read from file."""
         self._x = self._data["x"]
         self._y = None
         self._signal = self.data["signal"]
         self._monitor = None
+        self._indices = None
         self.outliers, self.medians = None, None
         self.reindex()
 
     def reindex(self):
         if self._indices is None:
             self._indices = np.argsort(self._x, kind="stable")
         self._x = self._x[self._indices]
         self._signal = self._signal[:, self._indices]
-        if self.monitor is not None:
+        # The test for self.monitor not being None, is necessary because it
+        # is not always present, and all the checks in setting a value are in
+        # the setter. The test for self._monitor not being None, is necessary to
+        # avoid a Pylance warning.
+        if self.monitor is not None and self._monitor is not None:
             self._monitor = self._monitor[self._indices]
 
     def find_outliers(self, method="hampel", **kwargs):
-        """Find outliers in the signal.
+        """
+        Find outliers in the signal.
 
         See the docstring in the :mod:`daxs.filters`.
         """
         if method == "hampel":
             self.outliers, self.medians = hampel(self._signal, axis=1, **kwargs)
         else:
             raise ValueError(f"Unknown method: {method}.")
 
     def remove_outliers(self, method="hampel", **kwargs):
-        """Remove outliers from the signal.
+        """
+        Remove outliers from the signal.
 
         See the docstring of :meth:`daxs.scans.Scan.find_outliers`.
         """
         if self.outliers is None or self.medians is None:
             self.find_outliers(method=method, **kwargs)
-        self._signal = np.where(self.outliers, self.medians, self._signal)
+
+        if self.outliers is not None and self.medians is not None:
+            self._signal = np.where(self.outliers, self.medians, self._signal)
+        else:
+            logger.info("No outliers found for scan %s.", self.label)
 
     def plot(self, ax=None, shift=None):
-        """Plot the scan data and outliers if available.
+        """
+        Plot the scan data and outliers if available.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes
             The axes to plot the scan data on.
         shift : float
             Shift the signal by the given value.
+
         """
         assert ax is not None, "The axes must be provided."
         if shift is None:
             shift = np.mean(self._signal)
         for i, _ in enumerate(self._signal):
             ax.plot(self.x, self._signal[i, :] + i * shift, label=f"{i}")
             if self.outliers is not None:
                 indices = self.outliers[i, :]
                 ax.plot(self.x[indices], self._signal[i, :][indices] + i * shift, "k.")
             ax.legend()
 
-    def dead_time_correction(self, tau=None, detection_time=None):
-        """Perform a dead time correction using a non-paralyzable model.
+    def dead_time_correction(
+        self, tau: Iterable | None = None, detection_time: float | None = None
+    ):
+        """
+        Perform a dead time correction using a non-paralyzable model.
 
         Parameters
         ----------
-        tau : Iterable
+        tau
             The detector dead time in seconds.
-        detection_time : float
+        detection_time
             The time spent on a point of the scan in seconds.
+
         """
         assert tau is not None, "The detector dead time (tau) must be set."
 
         if detection_time is None:
             if "detection_time" not in self.data:
                 raise ValueError(
                     "Either the detection time parameter or data path must be set."
@@ -236,20 +256,22 @@
         norm = 1 - ((self._signal / detection_time).T * tau).T
         if np.any(norm == 0):
             raise ValueError("The normalization has zero values.")
 
         self._signal = self._signal / norm
 
     def interpolate(self, a):
-        """Interpolate the data.
+        """
+        Interpolate the data.
 
         Parameters
         ----------
         a : numpy.array
             Array used to interpolate the signal and monitor.
+
         """
         if self._signal is None:
             raise ValueError
 
         logger.debug(
             "Interpolating the signal and monitor data for scan %s.", self.label
         )
@@ -268,26 +290,32 @@
             self._monitor = np.interp(a, self._x, self._monitor)
 
         self._x = a
         self._signal = signal
         self._indices = None
 
     def __truediv__(self, other):
-        """Divide the scan by a scalar, a list/tuple/ndarray, or another scan."""
+        """Divide the scan by a scalar, a list/tuple, a Numpy array, or another scan."""
         if isinstance(other, (int, float)):
             signal_div, monitor_div = other, None
-        elif isinstance(other, (list, tuple, np.ndarray)):
-            if len(other) == 2:
+        elif isinstance(other, (list, tuple)):
+            try:
                 signal_div, monitor_div = other
-            else:
-                signal_div, monitor_div = other, None
+            except ValueError as e:
+                raise type(e)(
+                    f"The sequence must contain only two elements not {len(other)}."
+                ) from e
+        elif isinstance(other, np.ndarray):
+            signal_div, monitor_div = other, None
         elif isinstance(other, Scan):
             signal_div, monitor_div = other._signal, other._monitor
         else:
-            raise ValueError("Unsupported type encounter in division.")
+            raise TypeError(
+                f"Unsupported divisor type {type(other)} encountered in division."
+            )
 
         try:
             self._signal /= signal_div
             if self._monitor is not None and monitor_div is not None:
                 self._monitor /= monitor_div
         except (TypeError, ValueError) as e:
             raise type(e)("Cannot divide by the given type.") from e
```

### Comparing `daxs-2022.1rc2/src/daxs/sources.py` & `daxs-2024.0/src/daxs/sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-# coding: utf-8
 """The module provides classes to deal with different types of data sources."""
 
+from __future__ import annotations
+
+import contextlib
 import copy
 import logging
 import re
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import silx.io.h5py_utils
 
 from daxs.scans import Scan
 
 logger = logging.getLogger(__name__)
 
 
 class Selection:
-    def __init__(
-        self,
-        items: Union[int, str, List[int], List[str], List[Union[int, str]]] = None,
-    ):
+    def __init__(self, items):
         assert not isinstance(
             items, dict
         ), "The selection items cannot be a dictionary."
 
-        self.items: Optional[Any] = items
+        self.items = items
         self.normalize()
 
     def normalize(self):
-        """Convert the items to proper formatting.
+        """
+        Convert the items to proper formatting.
 
         Examples
         --------
-        A few examples on how different selection are normalized:
+        Here are a few examples of how different selections are normalized:
 
         - 1 to [1,]
         - "1" to [1,]
         - [1, "fscan"] to [1, "fscan"]
         - ["1-3", "fscan"] to [1, 2, 3, "fscan"]
+
         """
         if self.items is None:
             self.items = []
         elif isinstance(self.items, (int, str)):
             self.items = [self.items]
+        elif isinstance(self.items, np.ndarray):
+            self.items = self.items.tolist()
 
         items = []
         for item in self.items:
             if isinstance(item, int):
                 items.append(item)
             elif isinstance(item, str):
                 if re.search(r"^\d+$", item):
@@ -64,78 +66,75 @@
 
 
 class Source(ABC):
     """Base class for sources of scans."""
 
     @property
     @abstractmethod
-    def filename(self) -> str:
+    def filename(self) -> str | None:
         """The filename of the source."""
 
     @property
     @abstractmethod
-    def scans(self) -> List[Scan]:
+    def scans(self) -> list[Scan]:
         """Return all source scans."""
 
 
 class Hdf5Source(Source):
     def __init__(
         self,
-        filename: str = None,
-        included_scans: Any = None,
-        excluded_scans: Any = None,
-        data_mappings: dict = None,
+        filename: str,
+        included_scans=None,
+        excluded_scans=None,
+        data_mappings: dict | None = None,
     ):
-
-        """Class for a HDF5 source of scans
+        """
+        Class for a HDF5 source of scans
 
         Parameters
         ----------
         filename :
             Name of the HDF5 file.
         included_scans :
             Selection of included scans.
         excluded_scans :
             Selection of excluded scans.
         data_mappings :
             Mappings between scan attributes (x, signal, monitor, etc.) and paths in
             the HDF5 file.
-        """
 
+        """
         self._filename = filename
         self.included_scans = Selection(included_scans)
         self.excluded_scans = Selection(excluded_scans)
         self.data_mappings = data_mappings
 
-        self._scans: List[Scan] = None
-        self._selected_scans: List[int] = None
+        self._scans: list[Scan] | None = None
+        self._selected_scans: list[int] | None = None
 
     @property
-    def filename(self) -> str:
+    def filename(self) -> str | None:
         return self._filename
 
     @property
-    def selected_scans(self) -> List[int]:
+    def selected_scans(self) -> list[int]:
         """The selected scans considering the inclusions and exclusions selections."""
         if self._selected_scans is not None:
             return self._selected_scans
 
         included_scans, excluded_scans, selected_scans = [], [], []
 
         with silx.io.h5py_utils.File(self.filename) as fp:
-
             indices = []
 
             for group in fp.values():
                 title = group["title"][()]
 
-                try:
+                with contextlib.suppress(AttributeError):
                     title = title.decode("utf-8")
-                except AttributeError:
-                    pass
 
                 # The group.name is of the form /1.1, /1.2, /2.1, etc.
                 # The title contains the command executed by the user, e.g.
                 # fscan 3.16 3.22 60 0.0002.
                 index = int(group.name[1:-2])
                 if index in indices:
                     continue
@@ -168,77 +167,71 @@
     @property
     def scans(self):
         """Return the scans."""
         if self._scans is None:
             self._scans = [self.read_scan(index) for index in self.selected_scans]
         return self._scans
 
-    def read_data(self, index: int, data_path: str) -> np.ndarray:
-        """Read the data given the scan index and path."""
-
-        data_path = f"{index}{data_path}"
+    def read_data(self, index: int, data_paths: str | list[str]) -> np.ndarray:
+        """Read the data given the scan index and data paths."""
+        if isinstance(data_paths, str):
+            data_paths = [data_paths]
 
+        data: list = []
         with silx.io.h5py_utils.File(self.filename) as fp:
-            try:
-                data = fp[data_path][()]
-            except KeyError as e:
-                raise KeyError(f"Unable to access {data_path}.") from e
-            except TypeError as e:
-                raise TypeError(f"Unable to read data from {data_path}.") from e
-
-            if data.size == 0:
-                raise ValueError(f"Data from {data_path} is empty.")
+            for data_path in data_paths:
+                full_data_path = f"{index}{data_path}"
+                try:
+                    data_at_path = fp[full_data_path][()]  # type: ignore
+                except KeyError as e:
+                    raise KeyError(f"Unable to access {full_data_path}.") from e
+                except TypeError as e:
+                    raise TypeError(
+                        f"Unable to read data from {full_data_path}."
+                    ) from e
+
+                if isinstance(data_at_path, np.ndarray) and data_at_path.size == 0:
+                    raise ValueError(f"Data from {full_data_path} is empty.")
+
+                data.append(data_at_path)
+
+        # Return the element of the array if it has only one element.
+        if len(data) == 1:
+            [data] = data
 
-        return data
+        return np.array(data)
 
     def read_scan(self, index: int) -> Scan:
         """Return a scan object at the index."""
         assert isinstance(index, int), "The index must be an integer."
         assert (
             self.data_mappings is not None
         ), "The data_mappings attribute must be set."
         assert (
             "x" in self.data_mappings
         ), "The data_mappings attribute must contain an entry for the X-axis values."
         assert (
             "signal" in self.data_mappings
         ), "The data_mappings attribute must contain an entry for the signal values."
 
-        # If needed, convert the signal data paths to a list.
-        if isinstance(self.data_mappings["signal"], str):
-            self.data_mappings["signal"] = [self.data_mappings["signal"]]
-
-        data: Dict[str, Any] = {}
+        data = {}
 
         x = self.read_data(index, self.data_mappings["x"])
-
-        # Read data from the paths associated with the signal into a 2D
-        # array. Each data path is stored into a row. We assume that the
-        # signal from each path has the same length.
-        n = len(self.data_mappings["signal"])
-        signal = np.zeros((n, x.size))
-        for i, data_path in enumerate(self.data_mappings["signal"]):
-            signal[i, :] = self.read_data(index, data_path)
+        signal = self.read_data(index, self.data_mappings["signal"])
 
         # Read additional data paths.
-        for key, data_path in self.data_mappings.items():
+        for key, data_paths in self.data_mappings.items():
             if key in ("x", "signal"):
                 continue
             # These are not critical, so we do not raise an error if they are
             # not found.
-            value = None
             try:
-                value = self.read_data(index, data_path)
+                values = self.read_data(index, data_paths)
             except (KeyError, TypeError):
-                logger.error(
-                    "Could not read data from %s. Setting %s value to None",
-                    data_path,
-                    key,
-                )
-            else:
-                data[key] = copy.deepcopy(value)
+                values = None
+            data[key] = copy.deepcopy(values)
 
-        # Finally, store some metadata.
+        # Finally, copy some metadata.
         data["filename"] = self.filename
         data["index"] = index
 
         return Scan(x, signal, data)
```

### Comparing `daxs-2022.1rc2/src/daxs/tests/conftest.py` & `daxs-2024.0/src/daxs/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# coding: utf-8
 # pylint: disable=redefined-outer-name
 
 import os
 
 import h5py
 import numpy as np
 import pytest
 
 
-@pytest.fixture()
-def hdf5_mock_filename(tmp_path_factory):
+@pytest.fixture(scope="session")
+def hdf5_mock_path(tmp_path_factory):
+    """Mock HDF5 file."""
     path = os.path.join(tmp_path_factory.mktemp("files"), "test.h5")
+    rng = np.random.default_rng()
     with h5py.File(path, driver="core", mode="w") as h5:
         for scan_id in range(1, 6):
-            h5.create_dataset(f"{scan_id}.1/title", data="fscan".encode("utf-8"))
+            h5.create_dataset(f"{scan_id}.1/title", data=b"fscan")
+            h5.create_dataset(f"{scan_id}.1/instrument/name", data="detector")
             for counter in ["x", "signal", "monitor"]:
                 if scan_id not in (1, 2):
                     h5.create_dataset(
-                        f"{scan_id}.1/measurement/{counter}", data=np.random.rand(10)
+                        f"{scan_id}.1/measurement/{counter}", data=rng.random(10)
                     )
-        h5.create_dataset("2.1/measurement/x", data=np.random.rand(15))
-        h5.create_dataset("2.1/measurement/signal", data=np.random.rand(15))
-        h5.create_dataset("5.1/measurement/sec", data=np.random.rand(10))
+        h5.create_dataset("2.1/measurement/x", data=rng.random(15))
+        h5.create_dataset("2.1/measurement/signal", data=rng.random(15))
+        h5.create_dataset("5.1/measurement/sec", data=rng.random(10))
+        h5.create_dataset("5.1/measurement/counter1", data=rng.random(10))
+        h5.create_dataset("5.1/measurement/counter2", data=rng.random(10))
     yield path
     os.remove(path)
-
-
-@pytest.fixture()
-def hdf5_mock_file(hdf5_mock_filename):
-    return h5py.File(hdf5_mock_filename, driver="core", mode="r")
```

### Comparing `daxs-2022.1rc2/src/daxs/tests/test_filters.py` & `daxs-2024.0/src/daxs/tests/test_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# coding: utf-8
 # pylint: disable=redefined-outer-name
+
 import numpy as np
 import pytest
 
 from daxs.filters import hampel
 from daxs.sources import Hdf5Source
 from daxs.utils import resources
 
 
 @pytest.fixture
 def scans():
-    filename = resources.getfile("pd_foil_la_xanes.h5")
+    filename = resources.getfile("Pd_foil_La_XANES.h5")
     data_mappings = {
         "x": ".1/measurement/hdh_angle",
         "signal": [".1/measurement/g09", ".1/measurement/g14"],
     }
     source = Hdf5Source(filename, included_scans=5, data_mappings=data_mappings)
     yield from source.scans
```

### Comparing `daxs-2022.1rc2/src/daxs/tests/test_measurements.py` & `daxs-2024.0/src/daxs/tests/test_measurements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,60 @@
-# coding: utf-8
 # pylint: disable=redefined-outer-name
 
 import os
 
 import numpy as np
 import pytest
 
 from daxs.measurements import Measurement, Measurement1D, Xes
 from daxs.sources import Hdf5Source
 from daxs.utils import resources
 
 
-def test_measurement_init(hdf5_mock_filename):
-    with pytest.raises(AssertionError):
-        measurement = Measurement(None)
-        assert measurement
-
+def test_measurement_init(hdf5_mock_path):
     data_mappings = {"x": ".1/measurement/x", "signal": ".1/measurement/signal"}
-    source = Hdf5Source(hdf5_mock_filename, None, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, None, None, data_mappings)
 
     with pytest.raises(ValueError):
         measurement = Measurement(source)
         _ = measurement.scans
 
-    source = Hdf5Source(hdf5_mock_filename, 3, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 3, None, data_mappings)
     measurement = Measurement(source)
 
-    source = Hdf5Source(hdf5_mock_filename, [2, 3], None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, [2, 3], None, data_mappings)
     measurement = Measurement(source)
 
 
-def test_measurement_remove_scans(hdf5_mock_filename):
+def test_measurement_remove_scans(hdf5_mock_path):
     data_mappings = {"x": ".1/measurement/x", "signal": ".1/measurement/signal"}
-    source = Hdf5Source(hdf5_mock_filename, [3, 4, 5], None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, [3, 4, 5], None, data_mappings)
     measurement = Measurement(source)
 
     with pytest.raises(AssertionError):
         measurement.remove_scans()
 
-    indices = [f"{source.filename}/{i}" for i in (3, 4, 5)]
+    indices = [3, 4, 5]
     measurement.remove_scans(indices)
 
 
 @pytest.fixture()
 def hdf5_filename():
-    return resources.getfile("pd_foil_la_xanes.h5")
+    return resources.getfile("Pd_foil_La_XANES.h5")
 
 
 @pytest.fixture()
 def data_mappings():
     return {
         "x": ".1/measurement/hdh_angle",
         "signal": [".1/measurement/g09", ".1/measurement/g14"],
     }
 
 
 def test_measurement_get_scans_common_axis(hdf5_filename, data_mappings):
-
     source = Hdf5Source(hdf5_filename, included_scans=[3], data_mappings=data_mappings)
     measurement = Measurement(source)
     values = measurement.get_scans_common_axis("x")
     assert np.all(values == getattr(measurement.scans[0], "x"))
 
     source = Hdf5Source(hdf5_filename, [3, 4, 7, 8, 9], data_mappings=data_mappings)
     measurement = Measurement(source)
@@ -193,8 +187,8 @@
 
 
 @pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_xes_concentration_correction(hdf5_filename, data_mappings):
     source = Hdf5Source(hdf5_filename, included_scans=3, data_mappings=data_mappings)
     measurement = Xes(source)
     measurement.concentration_correction(5)
-    assert measurement.signal[0:2] == pytest.approx([1.11283322, 1.18376119])
+    assert measurement.signal[-2:] == pytest.approx([9.98247848e-03, 6.88869365e-03])
```

### Comparing `daxs-2022.1rc2/src/daxs/tests/test_scans.py` & `daxs-2024.0/src/daxs/tests/test_scans.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-# coding: utf-8
 # pylint: disable=redefined-outer-name
+
 import copy
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 from daxs.scans import Scan
 
 
 def test_scan_init():
-    x = np.random.rand(10)
-    signal = np.random.rand(10)
+    rng = np.random.default_rng()
+    x = rng.random(10)
+    signal = rng.random(10)
 
     with pytest.raises(AssertionError):
-        Scan(None, signal)
-    with pytest.raises(AssertionError):
-        Scan(x, None)
-    with pytest.raises(AssertionError):
         Scan(x, signal[np.newaxis, :, np.newaxis])
 
     Scan(x, signal)
 
 
 @pytest.fixture
 def scan():
@@ -66,15 +63,16 @@
     assert scan.signal == pytest.approx([4.0, 5.0, 1.5, 5.5, 2.0, 2.0])
 
 
 def test_scan_interpolate(scan):
     # pylint: disable=protected-access
     scan._signal = None
     with pytest.raises(ValueError):
-        scan.interpolate(a=np.random.rand(10))
+        rng = np.random.default_rng()
+        scan.interpolate(a=rng.random(10))
 
 
 def test_scan_outliers_removal(scan):
     scan.remove_outliers(method="hampel")
     assert scan.signal == pytest.approx([4.0, 5.0, 1.5, 2.5, 2.0])
 
 
@@ -108,30 +106,36 @@
 
 def test_scan_plot(scan):
     _, ax = plt.subplots()
     scan.remove_outliers(method="hampel")
     scan.plot(ax)
 
 
-@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_scan_true_div(scan):
     with pytest.raises(TypeError):
         scan1 = scan / (1.0, "b")
 
+    with pytest.raises(TypeError):
+        scan1 = scan / "just wrong"
+
     scan1 = copy.deepcopy(scan)
+
     scan1 = scan1 / 0.5
     assert scan1.signal == pytest.approx(scan.signal / 0.5)
 
+    with pytest.raises(ValueError):
+        scan1 = scan1 / (0.4, 0.2, 0.1)
+
     scan1.reset()
     scan1 = scan1 / (0.4, 0.3)
     assert scan1.signal == pytest.approx(scan.signal / 0.4)
     assert scan1.monitor == pytest.approx(scan.monitor / 0.3)
 
     scan1.reset()
-    scan1 = scan1 / np.array([1, 1, 1, 1, 1])
+    scan1 = scan1 / np.array([1, 1, 1, 1, 1], dtype=float)
     assert scan1.signal == pytest.approx(scan.signal)
 
     scan1.reset()
     scan2 = copy.deepcopy(scan)
     scan2 = scan2 / scan1
     assert scan2.signal[0:2] == pytest.approx([1.0, 1.0])
```

### Comparing `daxs-2022.1rc2/src/daxs/tests/test_sources.py` & `daxs-2024.0/src/daxs/tests/test_sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# coding: utf-8
 # pylint: disable=redefined-outer-name
 
+import numpy as np
 import pytest
 
-from daxs.sources import Selection, Hdf5Source
+from daxs.sources import Hdf5Source, Selection
 
 
 @pytest.mark.parametrize(
     "selection, normalized_selection",
     (
         (None, []),
         (1, [1]),
@@ -23,45 +23,52 @@
 
 
 @pytest.mark.parametrize(
     "included_scans, excluded_scans, selected_scans",
     (
         ("1-4", None, [1, 2, 3, 4]),
         ([1, 2, 3, 4], "fscan", []),
+        (np.array([1, 2, 3], dtype=np.int64), None, [1, 2, 3]),
         (".*", [1, 2, 3], [4, 5]),
     ),
 )
 def test_hdf5_source_selected_scans(
-    hdf5_mock_filename, included_scans, excluded_scans, selected_scans
+    hdf5_mock_path, included_scans, excluded_scans, selected_scans
 ):
-    source = Hdf5Source(hdf5_mock_filename, included_scans, excluded_scans)
+    source = Hdf5Source(hdf5_mock_path, included_scans, excluded_scans)
     assert source.selected_scans == selected_scans
     # The second test is for the cached values.
     assert source.selected_scans == selected_scans
 
 
-def test_hdf5_source_scans(hdf5_mock_filename):
+def test_hdf5_source_scans(hdf5_mock_path):
     data_mappings = {}
-    source = Hdf5Source(hdf5_mock_filename, 1, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 1, None, data_mappings)
     with pytest.raises(AssertionError):
         assert source.scans
 
     data_mappings["x"] = ".1/measurement/x"
     data_mappings["signal"] = ".1/measurement/signal"
-    source = Hdf5Source(hdf5_mock_filename, 1, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 1, None, data_mappings)
     with pytest.raises(KeyError):
         assert source.scans
 
     data_mappings["monitor"] = ".1/measurement/monitor"
-    source = Hdf5Source(hdf5_mock_filename, 3, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 3, None, data_mappings)
     assert source.scans
 
+    data_mappings["name"] = ".1/instrument/name"
+    source = Hdf5Source(hdf5_mock_path, 2, None, data_mappings)
+    assert source.scans[0].data["name"] == b"detector"
+    data_mappings.pop("name")
+
     data_mappings["detection_time"] = ".1/measurement/detection_time"
-    source = Hdf5Source(hdf5_mock_filename, 3, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 3, None, data_mappings)
     assert source.scans
 
     data_mappings["detection_time"] = ".1/measurement/sec"
-    source = Hdf5Source(hdf5_mock_filename, 3, None, data_mappings)
+    source = Hdf5Source(hdf5_mock_path, 3, None, data_mappings)
     assert source.scans
 
-    source = Hdf5Source(hdf5_mock_filename, 5, None, data_mappings)
+    data_mappings["not_set"] = [".1/measurement/counter1", ".1/measurement/counter2"]
+    source = Hdf5Source(hdf5_mock_path, 5, None, data_mappings)
     assert source.scans
```

### Comparing `daxs-2022.1rc2/src/daxs.egg-info/SOURCES.txt` & `daxs-2024.0/src/daxs.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 src/daxs/__init__.py
+src/daxs/config.py
 src/daxs/filters.py
 src/daxs/interpolators.py
 src/daxs/measurements.py
 src/daxs/scans.py
 src/daxs/sources.py
-src/daxs/utils.py
 src/daxs.egg-info/PKG-INFO
 src/daxs.egg-info/SOURCES.txt
 src/daxs.egg-info/dependency_links.txt
 src/daxs.egg-info/requires.txt
 src/daxs.egg-info/top_level.txt
 src/daxs/tests/__init__.py
 src/daxs/tests/conftest.py
 src/daxs/tests/test_filters.py
 src/daxs/tests/test_import.py
 src/daxs/tests/test_measurements.py
 src/daxs/tests/test_scans.py
 src/daxs/tests/test_sources.py
-src/daxs/tests/test_utils.py
+src/daxs/utils/__init__.py
+src/daxs/utils/arrays.py
+src/daxs/utils/bragg.py
+src/daxs/utils/material.py
```

