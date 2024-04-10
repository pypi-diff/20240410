# Comparing `tmp/pentapy-1.2.0.tar.gz` & `tmp/pentapy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pentapy-1.2.0.tar", last modified: Sat Apr 15 18:17:43 2023, max compression
+gzip compressed data, was "pentapy-1.3.0.tar", last modified: Wed Apr 10 21:43:17 2024, max compression
```

## Comparing `pentapy-1.2.0.tar` & `pentapy-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-15 18:17:02.000000 pentapy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-15 18:17:43.604335 pentapy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-15 18:17:02.000000 pentapy-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-15 18:17:02.000000 pentapy-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:17:43.604335 pentapy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:17:02.000000 pentapy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.600335 pentapy-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/src/pentapy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 18:17:43.000000 pentapy-1.2.0/src/pentapy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/solver.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/solver.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-15 18:17:02.000000 pentapy-1.2.0/src/pentapy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/src/pentapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-15 18:17:43.000000 pentapy-1.2.0/src/pentapy.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:17:43.604335 pentapy-1.2.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-15 18:17:02.000000 pentapy-1.2.0/tests/test_pentapy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:43:17.896190 pentapy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-10 21:42:44.000000 pentapy-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-10 21:43:17.896190 pentapy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-10 21:42:44.000000 pentapy-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 21:42:44.000000 pentapy-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:43:17.896190 pentapy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-10 21:42:44.000000 pentapy-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:43:17.888190 pentapy-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:43:17.892190 pentapy-1.3.0/src/pentapy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 21:43:17.000000 pentapy-1.3.0/src/pentapy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/solver.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/solver.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-10 21:42:44.000000 pentapy-1.3.0/src/pentapy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:43:17.892190 pentapy-1.3.0/src/pentapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 21:43:17.000000 pentapy-1.3.0/src/pentapy.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:43:17.892190 pentapy-1.3.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4747 2024-04-10 21:42:44.000000 pentapy-1.3.0/tests/test_pentapy.py
```

### Comparing `pentapy-1.2.0/LICENSE` & `pentapy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pentapy-1.2.0/PKG-INFO` & `pentapy-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pentapy
-Version: 1.2.0
+Version: 1.3.0
 Summary: pentapy: A toolbox for pentadiagonal matrizes.
 Author-email: Sebastian Müller <info@geostat-framework.org>
 License: MIT
 Project-URL: Homepage, https://github.com/GeoStat-Framework/pentapy
 Project-URL: Documentation, https://pentapy.readthedocs.io
 Project-URL: Source, https://github.com/GeoStat-Framework/pentapy
 Project-URL: Tracker, https://github.com/GeoStat-Framework/pentapy/issues
@@ -15,30 +15,49 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.20.0
 Provides-Extra: scipy
+Requires-Dist: scipy; extra == "scipy"
 Provides-Extra: umfpack
+Requires-Dist: scikit-umfpack; extra == "umfpack"
 Provides-Extra: all
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: scikit-umfpack; extra == "all"
 Provides-Extra: doc
+Requires-Dist: m2r2>=0.2.8; extra == "doc"
+Requires-Dist: scipy>=1.1.0; extra == "doc"
+Requires-Dist: matplotlib>=3; extra == "doc"
+Requires-Dist: perfplot<0.9; extra == "doc"
+Requires-Dist: numpydoc>=1.1; extra == "doc"
+Requires-Dist: sphinx>=7; extra == "doc"
+Requires-Dist: sphinx-gallery>=0.8; extra == "doc"
+Requires-Dist: sphinx-rtd-theme>=2; extra == "doc"
 Provides-Extra: test
+Requires-Dist: pytest-cov>=3; extra == "test"
 Provides-Extra: check
-License-File: LICENSE
+Requires-Dist: black<25,>=24; extra == "check"
+Requires-Dist: isort[colors]; extra == "check"
+Requires-Dist: pylint; extra == "check"
+Requires-Dist: cython-lint; extra == "check"
 
 # Welcome to pentapy
 
 [![status](https://joss.theoj.org/papers/57c3bbdd7b7f3068dd1e669ccbcf107c/status.svg)](https://joss.theoj.org/papers/57c3bbdd7b7f3068dd1e669ccbcf107c)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2587158.svg)](https://doi.org/10.5281/zenodo.2587158)
 [![PyPI version](https://badge.fury.io/py/pentapy.svg)](https://badge.fury.io/py/pentapy)
 [![Build Status](https://github.com/GeoStat-Framework/pentapy/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/GeoStat-Framework/pentapy/actions)
```

### Comparing `pentapy-1.2.0/README.md` & `pentapy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pentapy-1.2.0/pyproject.toml` & `pentapy-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [
     "setuptools>=64",
-    "wheel",
     "setuptools_scm>=7",
-    "oldest-supported-numpy",
-    "Cython>=0.29.32,<3.0",
+    "numpy>=2.0.0rc1,<2.3; python_version >= '3.9'",
+    "oldest-supported-numpy; python_version < '3.9'",
+    "Cython>=3.0.10,<3.1.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 name = "pentapy"
 authors = [{name = "Sebastian Müller", email = "info@geostat-framework.org"}]
 readme = "README.md"
 license = {text = "MIT"}
 dynamic = ["version"]
 description = "pentapy: A toolbox for pentadiagonal matrizes."
 classifiers = [
@@ -22,46 +22,48 @@
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: Unix",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
-dependencies = ["numpy>=1.14.5"]
+dependencies = ["numpy>=1.20.0"]
 
 [project.optional-dependencies]
 scipy = ["scipy"]
 umfpack = ["scikit-umfpack"]
 all = [
     "scipy",
     "scikit-umfpack",
 ]
 doc = [
     "m2r2>=0.2.8",
     "scipy>=1.1.0",
     "matplotlib>=3",
     "perfplot<0.9",
     "numpydoc>=1.1",
-    "sphinx>=4",
+    "sphinx>=7",
     "sphinx-gallery>=0.8",
-    "sphinx-rtd-theme>=1,<1.1",
+    "sphinx-rtd-theme>=2",
 ]
 test = ["pytest-cov>=3"]
 check = [
-  "black>=23,<24",
-  "isort[colors]<6",
-  "pylint<3",
+  "black>=24,<25",
+  "isort[colors]",
+  "pylint",
+  "cython-lint",
 ]
 
 [project.urls]
 Homepage = "https://github.com/GeoStat-Framework/pentapy"
 Documentation = "https://pentapy.readthedocs.io"
 Source = "https://github.com/GeoStat-Framework/pentapy"
 Tracker = "https://github.com/GeoStat-Framework/pentapy/issues"
@@ -76,19 +78,26 @@
 write_to_template = "__version__ = '{version}'"
 local_scheme = "no-local-version"
 fallback_version = "0.0.0.dev0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
-line_length = 79
 
 [tool.black]
-line-length = 79
-target-version = ["py37"]
+target-version = [
+    "py38",
+    "py39",
+    "py310",
+    "py311",
+    "py312",
+]
+
+[tool.cython-lint]
+max-line-length = 120
 
 [tool.coverage]
     [tool.coverage.run]
     source = ["pentapy"]
     omit = [
         "*docs*",
         "*examples*",
@@ -126,16 +135,14 @@
     max-statements = 80
     max-attributes = 25
     max-public-methods = 75
 
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
-# Disable building PyPy wheels on all platforms, 32bit for py3.10/11 and musllinux builds, py3.6
-skip = ["cp36-*", "pp*", "cp31*-win32", "cp31*-manylinux_i686", "*-musllinux_*"]
+# Disable building PyPy wheels on all platforms, 32bit builds, py3.6, py3.7
+skip = ["cp36-*", "cp37-*", "pp*", "*-win32", "*-manylinux_i686", "*-musllinux_*"]
 # Run the package tests using `pytest`
 test-extras = "test"
 test-command = "pytest -v {package}/tests"
 # Skip trying to test arm64 builds on Intel Macs
 test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
-# no wheels for linux-32bit anymore for numpy>=1.22
-environment = "PIP_PREFER_BINARY=1"
```

### Comparing `pentapy-1.2.0/setup.py` & `pentapy-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pentapy: A toolbox for pentadiagonal matrizes."""
+
 import os
 
 import numpy as np
 from Cython.Build import cythonize
 from setuptools import Extension, setup
 
 # cython extensions
```

### Comparing `pentapy-1.2.0/src/pentapy/__init__.py` & `pentapy-1.3.0/src/pentapy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,21 +34,17 @@
 
 .. autosummary::
    diag_indices
    shift_banded
    create_banded
    create_full
 """
+
 from pentapy.core import solve
-from pentapy.tools import (
-    create_banded,
-    create_full,
-    diag_indices,
-    shift_banded,
-)
+from pentapy.tools import create_banded, create_full, diag_indices, shift_banded
 
 try:
     from pentapy._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
     __version__ = "0.0.0.dev0"
```

### Comparing `pentapy-1.2.0/src/pentapy/core.py` & `pentapy-1.3.0/src/pentapy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The core module of pentapy."""
+
 # pylint: disable=C0103, C0415, R0911, E0611
 import warnings
 
 import numpy as np
 
 from pentapy.solver import penta_solver1, penta_solver2
 from pentapy.tools import _check_penta, create_banded, shift_banded
@@ -97,35 +98,32 @@
         except ZeroDivisionError:
             warnings.warn("pentapy: PTRANS-II not suitable for input-matrix.")
             return np.full_like(rhs, np.nan)
     elif solver in [3, "3", "lapack", "solve_banded"]:  # pragma: no cover
         try:
             from scipy.linalg import solve_banded
         except ImportError as imp_err:  # pragma: no cover
-            raise ValueError(
-                "pentapy.solve: "
-                "scipy.linalg.solve_banded could not be imported"
-            ) from imp_err
+            msg = "pentapy.solve: scipy.linalg.solve_banded could not be imported"
+            raise ValueError(msg) from imp_err
         if is_flat and index_row_wise:
             mat_flat = np.array(mat)
             _check_penta(mat_flat)
             shift_banded(mat_flat, col_to_row=False, copy=False)
         elif is_flat:
             mat_flat = np.asarray(mat)
         else:
             mat_flat = create_banded(mat)
         return solve_banded((2, 2), mat_flat, rhs)
     elif solver in [4, "4", "spsolve"]:  # pragma: no cover
         try:
             from scipy import sparse as sps
             from scipy.sparse.linalg import spsolve
         except ImportError as imp_err:
-            raise ValueError(
-                "pentapy.solve: scipy.sparse could not be imported"
-            ) from imp_err
+            msg = "pentapy.solve: scipy.sparse could not be imported"
+            raise ValueError(msg) from imp_err
         if is_flat and index_row_wise:
             mat_flat = np.array(mat)
             _check_penta(mat_flat)
             shift_banded(mat_flat, col_to_row=False, copy=False)
         elif is_flat:
             mat_flat = np.asarray(mat)
         else:
@@ -140,23 +138,23 @@
         "umf",
         "umf_pack",
     ]:  # pragma: no cover
         try:
             from scipy import sparse as sps
             from scipy.sparse.linalg import spsolve
         except ImportError as imp_err:
-            raise ValueError(
-                "pentapy.solve: scipy.sparse could not be imported"
-            ) from imp_err
+            msg = "pentapy.solve: scipy.sparse could not be imported"
+            raise ValueError(msg) from imp_err
         if is_flat and index_row_wise:
             mat_flat = np.array(mat)
             _check_penta(mat_flat)
             shift_banded(mat_flat, col_to_row=False, copy=False)
         elif is_flat:
             mat_flat = np.asarray(mat)
         else:
             mat_flat = create_banded(mat)
         size = mat_flat.shape[1]
         M = sps.spdiags(mat_flat, [2, 1, 0, -1, -2], size, size, format="csc")
         return spsolve(M, rhs, use_umfpack=True)
     else:  # pragma: no cover
-        raise ValueError("pentapy.solve: unknown solver (" + str(solver) + ")")
+        msg = f"pentapy.solve: unknown solver ({solver})"
+        raise ValueError(msg)
```

### Comparing `pentapy-1.2.0/src/pentapy/solver.pyx` & `pentapy-1.3.0/src/pentapy/solver.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-#cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
+# cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
 """
 This is a solver linear equation systems with a penta-diagonal matrix,
 implemented in cython.
 """
 import numpy as np
 
-cimport cython
 cimport numpy as np
 
 
-def penta_solver1(double[:,:] mat_flat, double[:] rhs):
+def penta_solver1(double[:, :] mat_flat, double[:] rhs):
     return np.asarray(c_penta_solver1(mat_flat, rhs))
 
 
-def penta_solver2(double[:,:] mat_flat, double[:] rhs):
+def penta_solver2(double[:, :] mat_flat, double[:] rhs):
     return np.asarray(c_penta_solver2(mat_flat, rhs))
 
 
-cdef double[:] c_penta_solver1(double[:,:] mat_flat, double[:] rhs):
+cdef double[:] c_penta_solver1(double[:, :] mat_flat, double[:] rhs):
 
     cdef int mat_j = mat_flat.shape[1]
 
     cdef double[:] result = np.zeros(mat_j)
 
     cdef double[:] al = np.zeros(mat_j)
     cdef double[:] be = np.zeros(mat_j)
@@ -65,15 +64,15 @@
 
     for i in range(mat_j-3, -1, -1):
         result[i] = ze[i] - al[i] * result[i+1] - be[i] * result[i+2]
 
     return result
 
 
-cdef double[:] c_penta_solver2(double[:,:] mat_flat, double[:] rhs):
+cdef double[:] c_penta_solver2(double[:, :] mat_flat, double[:] rhs):
 
     cdef int mat_j = mat_flat.shape[1]
 
     cdef double[:] result = np.zeros(mat_j)
 
     cdef double[:] ps = np.zeros(mat_j)  # psi
     cdef double[:] si = np.zeros(mat_j)  # sigma
```

### Comparing `pentapy-1.2.0/src/pentapy/tools.py` & `pentapy-1.3.0/src/pentapy/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
    :toctree:
 
    diag_indices
    shift_banded
    create_banded
    create_full
 """
+
 # pylint: disable=C0103
 import numpy as np
 
 
 def diag_indices(n, offset=0):
     """
     Get indices for the main or minor diagonals of a matrix.
@@ -167,17 +168,19 @@
     Returns
     -------
     :class:`numpy.ndarray`
         Bandend matrix
     """
     mat = np.asanyarray(mat)
     if mat.ndim != 2:
-        raise ValueError("create_banded: matrix has to be 2D")
+        msg = "create_banded: matrix has to be 2D"
+        raise ValueError(msg)
     if mat.shape[0] != mat.shape[1]:
-        raise ValueError("create_banded: matrix has to be n x n")
+        msg = "create_banded: matrix has to be n x n"
+        raise ValueError(msg)
 
     size = mat.shape[0]
     mat_flat = np.zeros((5, size), dtype=dtype)
     mat_flat[up, :] = mat.diagonal()
 
     if col_wise:
         for i in range(up):
@@ -239,36 +242,40 @@
     Returns
     -------
     :class:`numpy.ndarray`
         Full matrix.
     """
     mat = np.asanyarray(mat)
     if mat.ndim != 2:
-        raise ValueError("create_full: matrix has to be 2D")
+        msg = "create_full: matrix has to be 2D"
+        raise ValueError(msg)
     if mat.shape[0] != up + low + 1:
-        raise ValueError("create_full: matrix has wrong count of bands")
+        msg = "create_full: matrix has wrong count of bands"
+        raise ValueError(msg)
     if mat.shape[1] < max(up, low) + 1:
-        raise ValueError("create_full: matrix has to few information")
+        msg = "create_full: matrix has to few information"
+        raise ValueError(msg)
     size = mat.shape[1]
     mat_full = np.diag(mat[up])
     if col_wise:
         for i in range(up):
             mat_full[diag_indices(size, up - i)] = mat[i, (up - i) :]
         for i in range(low):
-            mat_full[diag_indices(size, -(low - i))] = mat[
-                -i - 1, : -(low - i)
-            ]
+            mat_full[diag_indices(size, -(low - i))] = mat[-i - 1, : -(low - i)]
     else:
         for i in range(up):
             mat_full[diag_indices(size, up - i)] = mat[i, : -(up - i)]
         for i in range(low):
             mat_full[diag_indices(size, -(low - i))] = mat[-i - 1, (low - i) :]
     return mat_full
 
 
 def _check_penta(mat):
     if mat.ndim != 2:
-        raise ValueError("pentapy: matrix has to be 2D")
+        msg = "pentapy: matrix has to be 2D"
+        raise ValueError(msg)
     if mat.shape[0] != 5:
-        raise ValueError("pentapy: matrix needs 5 bands")
+        msg = "pentapy: matrix needs 5 bands"
+        raise ValueError(msg)
     if mat.shape[1] < 3:
-        raise ValueError("pentapy: matrix needs at least 3 rows")
+        msg = "pentapy: matrix needs at least 3 rows"
+        raise ValueError(msg)
```

### Comparing `pentapy-1.2.0/tests/test_pentapy.py` & `pentapy-1.3.0/tests/test_pentapy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This is the unittest for pentapy.
 """
+
 import unittest
 
 # import platform
 import warnings
 
 import numpy as np
 
@@ -20,29 +21,19 @@
         self.rand = np.random.RandomState(self.seed)
         self.mat = (self.rand.rand(5, self.size) - 0.5) * 1e-5
         self.rhs = self.rand.rand(self.size) * 1e5
 
     def test_tools(self):
         self.mat_int = np.zeros((100, 100), dtype=int)
         # fill bands of pentadiagonal matrix
-        self.mat_int[pp.diag_indices(100, 0)] = self.rand.randint(
-            1, 1000, size=100
-        )
-        self.mat_int[pp.diag_indices(100, 1)] = self.rand.randint(
-            1, 1000, size=99
-        )
-        self.mat_int[pp.diag_indices(100, 2)] = self.rand.randint(
-            1, 1000, size=98
-        )
-        self.mat_int[pp.diag_indices(100, -1)] = self.rand.randint(
-            1, 1000, size=99
-        )
-        self.mat_int[pp.diag_indices(100, -2)] = self.rand.randint(
-            1, 1000, size=98
-        )
+        self.mat_int[pp.diag_indices(100, 0)] = self.rand.randint(1, 1000, size=100)
+        self.mat_int[pp.diag_indices(100, 1)] = self.rand.randint(1, 1000, size=99)
+        self.mat_int[pp.diag_indices(100, 2)] = self.rand.randint(1, 1000, size=98)
+        self.mat_int[pp.diag_indices(100, -1)] = self.rand.randint(1, 1000, size=99)
+        self.mat_int[pp.diag_indices(100, -2)] = self.rand.randint(1, 1000, size=98)
         # create banded
         self.mat_int_col = pp.create_banded(self.mat_int)
         self.mat_int_row = pp.create_banded(self.mat_int, col_wise=False)
         # create full
         self.mat_int_col_ful = pp.create_full(self.mat_int_col, col_wise=True)
         self.mat_int_row_ful = pp.create_full(self.mat_int_row, col_wise=False)
         # shifting
@@ -76,17 +67,15 @@
         )
         sol_ful = pp.solve(self.mat_ful, self.rhs, solver=1)
 
         diff_row = np.max(np.abs(np.dot(self.mat_ful, sol_row) - self.rhs))
         diff_col = np.max(np.abs(np.dot(self.mat_ful, sol_col) - self.rhs))
         diff_ful = np.max(np.abs(np.dot(self.mat_ful, sol_ful) - self.rhs))
 
-        diff_row_col = np.max(
-            np.abs(self.mat_ful - pp.create_full(self.mat_col))
-        )
+        diff_row_col = np.max(np.abs(self.mat_ful - pp.create_full(self.mat_col)))
         self.assertAlmostEqual(diff_row * 1e-5, 0.0)
         self.assertAlmostEqual(diff_col * 1e-5, 0.0)
         self.assertAlmostEqual(diff_ful * 1e-5, 0.0)
         self.assertAlmostEqual(diff_row_col * 1e5, 0.0)
 
     def test_solve2(self):
         self.mat_col = pp.shift_banded(self.mat, col_to_row=False)
@@ -102,17 +91,15 @@
         )
         sol_ful = pp.solve(self.mat_ful, self.rhs, solver=2)
 
         diff_row = np.max(np.abs(np.dot(self.mat_ful, sol_row) - self.rhs))
         diff_col = np.max(np.abs(np.dot(self.mat_ful, sol_col) - self.rhs))
         diff_ful = np.max(np.abs(np.dot(self.mat_ful, sol_ful) - self.rhs))
 
-        diff_row_col = np.max(
-            np.abs(self.mat_ful - pp.create_full(self.mat_col))
-        )
+        diff_row_col = np.max(np.abs(self.mat_ful - pp.create_full(self.mat_col)))
         self.assertAlmostEqual(diff_row * 1e-5, 0.0)
         self.assertAlmostEqual(diff_col * 1e-5, 0.0)
         self.assertAlmostEqual(diff_ful * 1e-5, 0.0)
         self.assertAlmostEqual(diff_row_col * 1e5, 0.0)
 
     def test_error(self):
         self.err_mat = np.array(
```

