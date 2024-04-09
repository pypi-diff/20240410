# Comparing `tmp/pyqentangle-3.3.2.tar.gz` & `tmp/pyqentangle-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqentangle-3.3.2.tar", last modified: Sun Mar 31 02:08:06 2024, max compression
+gzip compressed data, was "pyqentangle-4.0.0.tar", last modified: Tue Apr  9 23:15:04 2024, max compression
```

## Comparing `pyqentangle-3.3.2.tar` & `pyqentangle-4.0.0.tar`

### file list

```diff
@@ -1,43 +1,38 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.863179 pyqentangle-3.3.2/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-10-13 13:49:27.000000 pyqentangle-3.3.2/LICENSE
--rw-r--r--   0 stephenhky   (501) staff       (20)      178 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)     5771 2024-03-31 02:08:06.862696 pyqentangle-3.3.2/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     4736 2023-10-20 02:14:38.000000 pyqentangle-3.3.2/README.md
--rw-r--r--   0 stephenhky   (501) staff       (20)       83 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/pyproject.toml
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.837529 pyqentangle-3.3.2/pyqentangle/
--rw-r--r--   0 stephenhky   (501) staff       (20)      366 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/pyqentangle/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     6506 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/pyqentangle/continuous.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.847896 pyqentangle-3.3.2/pyqentangle/cythonmodule/
--rw-r--r--   0 stephenhky   (501) staff       (20)       27 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/pyqentangle/cythonmodule/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      233 2021-09-04 16:42:55.000000 pyqentangle-3.3.2/pyqentangle/cythonmodule/interpolate.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   370709 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle/cythonmodule/interpolate_nocheck.c
--rw-r--r--   0 stephenhky   (501) staff       (20)      653 2023-10-13 13:31:28.000000 pyqentangle-3.3.2/pyqentangle/cythonmodule/interpolate_nocheck.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)     4484 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/pyqentangle/metrics.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.850341 pyqentangle-3.3.2/pyqentangle/quantumstates/
--rw-r--r--   0 stephenhky   (501) staff       (20)       49 2020-10-13 13:49:27.000000 pyqentangle-3.3.2/pyqentangle/quantumstates/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      138 2020-10-13 13:49:27.000000 pyqentangle-3.3.2/pyqentangle/quantumstates/bipartite.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2975 2021-09-04 16:42:55.000000 pyqentangle-3.3.2/pyqentangle/quantumstates/harmonics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3481 2021-09-04 16:42:55.000000 pyqentangle-3.3.2/pyqentangle/schmidt.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3618 2020-10-13 13:49:27.000000 pyqentangle-3.3.2/pyqentangle/tncompute.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      661 2020-10-13 13:49:27.000000 pyqentangle-3.3.2/pyqentangle/utils.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.844057 pyqentangle-3.3.2/pyqentangle.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)     5771 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)      980 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-16 17:47:10.000000 pyqentangle-3.3.2/pyqentangle.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)       63 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       12 2024-03-31 02:08:06.000000 pyqentangle-3.3.2/pyqentangle.egg-info/top_level.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       63 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       38 2024-03-31 02:08:06.863327 pyqentangle-3.3.2/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     2359 2024-03-31 02:06:58.000000 pyqentangle-3.3.2/setup.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-03-31 02:08:06.861460 pyqentangle-3.3.2/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)      318 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/testConcurrence.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1855 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/testContinuousEntanglement.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      803 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/testDiscreteEntanglement.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3795 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/testRedDenMat.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      747 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_continuous_complex.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      768 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_fullredden.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1318 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_harmonics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      809 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_interpolation.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1183 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_metrics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2896 2023-06-21 22:42:24.000000 pyqentangle-3.3.2/test/test_partialtranspose.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-04-09 23:15:04.855883 pyqentangle-4.0.0/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-10-13 13:49:27.000000 pyqentangle-4.0.0/LICENSE
+-rw-r--r--   0 stephenhky   (501) staff       (20)       66 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)     5690 2024-04-09 23:15:04.855272 pyqentangle-4.0.0/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4736 2023-10-20 02:14:38.000000 pyqentangle-4.0.0/README.md
+-rw-r--r--   0 stephenhky   (501) staff       (20)       67 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/pyproject.toml
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-04-09 23:15:04.833182 pyqentangle-4.0.0/pyqentangle/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      339 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/pyqentangle/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6860 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/pyqentangle/continuous.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4484 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/pyqentangle/metrics.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-04-09 23:15:04.841238 pyqentangle-4.0.0/pyqentangle/quantumstates/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       49 2020-10-13 13:49:27.000000 pyqentangle-4.0.0/pyqentangle/quantumstates/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      138 2020-10-13 13:49:27.000000 pyqentangle-4.0.0/pyqentangle/quantumstates/bipartite.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2975 2021-09-04 16:42:55.000000 pyqentangle-4.0.0/pyqentangle/quantumstates/harmonics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3481 2021-09-04 16:42:55.000000 pyqentangle-4.0.0/pyqentangle/schmidt.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3527 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/pyqentangle/tncompute.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      661 2020-10-13 13:49:27.000000 pyqentangle-4.0.0/pyqentangle/utils.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-04-09 23:15:04.838684 pyqentangle-4.0.0/pyqentangle.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     5690 2024-04-09 23:15:04.000000 pyqentangle-4.0.0/pyqentangle.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)      807 2024-04-09 23:15:04.000000 pyqentangle-4.0.0/pyqentangle.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2024-04-09 23:15:04.000000 pyqentangle-4.0.0/pyqentangle.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-16 17:47:10.000000 pyqentangle-4.0.0/pyqentangle.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)       48 2024-04-09 23:15:04.000000 pyqentangle-4.0.0/pyqentangle.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       12 2024-04-09 23:15:04.000000 pyqentangle-4.0.0/pyqentangle.egg-info/top_level.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       48 2024-04-09 23:07:59.000000 pyqentangle-4.0.0/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       38 2024-04-09 23:15:04.856033 pyqentangle-4.0.0/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1885 2024-04-09 23:09:07.000000 pyqentangle-4.0.0/setup.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2024-04-09 23:15:04.854198 pyqentangle-4.0.0/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      318 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/testConcurrence.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1855 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/testContinuousEntanglement.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      803 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/testDiscreteEntanglement.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3795 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/testRedDenMat.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      747 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_continuous_complex.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      768 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_fullredden.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1318 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_harmonics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      809 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_interpolation.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1183 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_metrics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2896 2023-06-21 22:42:24.000000 pyqentangle-4.0.0/test/test_partialtranspose.py
```

### Comparing `pyqentangle-3.3.2/LICENSE` & `pyqentangle-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/PKG-INFO` & `pyqentangle-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqentangle
-Version: 3.3.2
+Version: 4.0.0
 Summary: Quantum Entanglement in Python
 Home-page: https://github.com/stephenhky/pyqentangle
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Keywords: quantum physics Schmidt decompostion entanglement
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -12,16 +12,14 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quantum Entanglement in Python
```

### Comparing `pyqentangle-3.3.2/README.md` & `pyqentangle-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/pyqentangle/continuous.py` & `pyqentangle-4.0.0/pyqentangle/continuous.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 
 from itertools import product
 
 import numpy as np
 
-from .cythonmodule.interpolate import numerical_continuous_interpolation_nocheck
 from . import schmidt_decomposition, OutOfRangeException, UnequalLengthException
 
 
+def interpolate(xarray, yarray, x):
+    left = 0
+    right = len(xarray) - 1
+    idx = right // 2
+    while (idx != 0 and idx != len(xarray) - 1) and (not (x >= xarray[idx] and x < xarray[idx + 1])):
+        if x >= xarray[idx + 1]:
+            left = idx + 1
+        elif x < xarray[idx]:
+            right = idx - 1
+        idx = (left + right) // 2
+
+    return yarray[idx] + (yarray[idx + 1] - yarray[idx]) / (xarray[idx + 1] - xarray[idx]) * (x - xarray[idx])
+
+
 def numerical_continuous_interpolation(xarray, yarray, x):
     """Evaluate the value of a function given a variable x using interpolation
 
     With a function approximated by given arrays of independent variable (`xarray`)
     and of dependent variable (`yarray`), the value of this function given `x` is
     calculated by interpolation.
 
@@ -32,15 +45,15 @@
     minx = np.min(xarray)
     maxx = np.max(xarray)
     if x == maxx:
         return yarray[-1]
     if not (x >= minx and x < maxx):
         raise OutOfRangeException(x)
 
-    return numerical_continuous_interpolation_nocheck(xarray, yarray, x)
+    return interpolate(xarray, yarray, x)
 
 
 def numerical_continuous_function(xarray, yarray):
     """Return a function with the given arrays of independent and dependent variables
 
     With a function approximated by given arrays of independent variable (`xarray`)
     and of dependent variable (`yarray`), it returns a lambda function that takes
```

### Comparing `pyqentangle-3.3.2/pyqentangle/metrics.py` & `pyqentangle-4.0.0/pyqentangle/metrics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/pyqentangle/quantumstates/harmonics.py` & `pyqentangle-4.0.0/pyqentangle/quantumstates/harmonics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/pyqentangle/schmidt.py` & `pyqentangle-4.0.0/pyqentangle/schmidt.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/pyqentangle/tncompute.py` & `pyqentangle-4.0.0/pyqentangle/tncompute.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,18 @@
 
     Given a discrete normalized quantum system, given in terms of 2-D numpy array ``bipartitepurestate_tensor``,
     each element of ``bipartitepurestate_tensor[i, j]`` is the coefficient of the ket :math:`|ij\\rangle`,
     calculate the reduced density matrix of the specified subsystem.
 
     :param bipartitepurestate_tensor: tensor describing the bi-partitite states, with each elements the coefficients for :math:`|ij\\rangle`
     :param kept: subsystem, 0 indicating the first subsystem; 1 the second
-    :param use_cython: use legacy Cython code (default: False)
     :return: reduced density matrix of the specified subsystem
     :type bipartitepurestate_tensor: numpy.ndarray
     :type kept: int
-    :type use_cython: bool
     :rtype: numpy.ndarray
-
     """
     if not (kept in [0, 1]):
         raise ValueError('kept can only be 0 or 1!')
 
     ketnode = tn.Node(bipartitepurestate_tensor)
     branode = tn.Node(np.conj(bipartitepurestate_tensor))
```

### Comparing `pyqentangle-3.3.2/pyqentangle/utils.py` & `pyqentangle-4.0.0/pyqentangle/utils.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/pyqentangle.egg-info/PKG-INFO` & `pyqentangle-4.0.0/pyqentangle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqentangle
-Version: 3.3.2
+Version: 4.0.0
 Summary: Quantum Entanglement in Python
 Home-page: https://github.com/stephenhky/pyqentangle
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Keywords: quantum physics Schmidt decompostion entanglement
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -12,16 +12,14 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Quantum Entanglement in Python
```

### Comparing `pyqentangle-3.3.2/pyqentangle.egg-info/SOURCES.txt` & `pyqentangle-4.0.0/pyqentangle.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 pyqentangle/utils.py
 pyqentangle.egg-info/PKG-INFO
 pyqentangle.egg-info/SOURCES.txt
 pyqentangle.egg-info/dependency_links.txt
 pyqentangle.egg-info/not-zip-safe
 pyqentangle.egg-info/requires.txt
 pyqentangle.egg-info/top_level.txt
-pyqentangle/cythonmodule/__init__.py
-pyqentangle/cythonmodule/interpolate.py
-pyqentangle/cythonmodule/interpolate_nocheck.c
-pyqentangle/cythonmodule/interpolate_nocheck.pyx
 pyqentangle/quantumstates/__init__.py
 pyqentangle/quantumstates/bipartite.py
 pyqentangle/quantumstates/harmonics.py
 test/testConcurrence.py
 test/testContinuousEntanglement.py
 test/testDiscreteEntanglement.py
 test/testRedDenMat.py
```

### Comparing `pyqentangle-3.3.2/setup.py` & `pyqentangle-4.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 
 from setuptools import setup
 import numpy as np
 
-try:
-    from Cython.Build import cythonize
-    ext_modules = cythonize(['pyqentangle/cythonmodule/interpolate_nocheck.pyx'])
-except ImportError:
-    from setuptools import Extension
-    ext_modules = [
-        Extension('pyqentangle.cythonmodule.interpolate_nocheck', ['pyqentangle/cythonmodule/interpolate_nocheck.c'])
-    ]
-
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 def package_description():
@@ -24,44 +15,41 @@
 
 
 def install_requirements():
     return [package_string.strip() for package_string in open('requirements.txt', 'r')]
 
 
 setup(name='pyqentangle',
-      version="3.3.2",
+      version="4.0.0",
       description="Quantum Entanglement in Python",
       long_description=package_description(),
       long_description_content_type='text/markdown',
       classifiers=[
           "Topic :: Scientific/Engineering :: Physics",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Chemistry",
           "License :: OSI Approved :: MIT License",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
-          "Programming Language :: Cython",
-          "Programming Language :: C",
           "Intended Audience :: Science/Research",
           "Intended Audience :: Developers",
           "Intended Audience :: Education"
       ],
       keywords="quantum physics Schmidt decompostion entanglement",
       url="https://github.com/stephenhky/pyqentangle",
       author="Kwan-Yuet Ho",
       author_email="stephenhky@yahoo.com.hk",
       license='MIT',
-      packages=['pyqentangle', 'pyqentangle.quantumstates', 'pyqentangle.cythonmodule'],
+      packages=['pyqentangle', 'pyqentangle.quantumstates'],
       package_dir={'pyqentangle': 'pyqentangle'},
-      package_data={
-          'pyqentangle': ['cythonmodule/*.c', 'cythonmodule/*.pyx']
-      },
+      # package_data={
+      #     'pyqentangle': ['cythonmodule/*.c', 'cythonmodule/*.pyx']
+      # },
       include_dirs=[np.get_include()],
-      setup_requires=['Cython', 'numpy', ],
+      setup_requires=['numpy', ],
       install_requires=install_requirements(),
-      ext_modules=ext_modules,
       test_suite="test",
       include_package_data=True,
       zip_safe=False)
```

### Comparing `pyqentangle-3.3.2/test/testContinuousEntanglement.py` & `pyqentangle-4.0.0/test/testContinuousEntanglement.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/testDiscreteEntanglement.py` & `pyqentangle-4.0.0/test/testDiscreteEntanglement.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/testRedDenMat.py` & `pyqentangle-4.0.0/test/testRedDenMat.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_continuous_complex.py` & `pyqentangle-4.0.0/test/test_continuous_complex.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_fullredden.py` & `pyqentangle-4.0.0/test/test_fullredden.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_harmonics.py` & `pyqentangle-4.0.0/test/test_harmonics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_interpolation.py` & `pyqentangle-4.0.0/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_metrics.py` & `pyqentangle-4.0.0/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pyqentangle-3.3.2/test/test_partialtranspose.py` & `pyqentangle-4.0.0/test/test_partialtranspose.py`

 * *Files identical despite different names*

