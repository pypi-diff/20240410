# Comparing `tmp/chetoolbox-0.0.8.tar.gz` & `tmp/chetoolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chetoolbox-0.0.8.tar", last modified: Fri Feb 16 19:11:24 2024, max compression
+gzip compressed data, was "chetoolbox-0.0.9.tar", last modified: Fri Feb 23 18:21:06 2024, max compression
```

## Comparing `chetoolbox-0.0.8.tar` & `chetoolbox-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 19:11:24.575411 chetoolbox-0.0.8/
--rw-rw-rw-   0        0        0    35821 2024-01-30 16:09:10.000000 chetoolbox-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      665 2024-02-16 19:11:24.567806 chetoolbox-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1367 2024-01-30 16:09:10.000000 chetoolbox-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 19:11:24.525492 chetoolbox-0.0.8/chetoolbox/
--rw-rw-rw-   0        0        0        0 2024-01-30 16:09:10.000000 chetoolbox-0.0.8/chetoolbox/__init__.py
--rw-rw-rw-   0        0        0     5161 2024-02-16 16:35:49.000000 chetoolbox-0.0.8/chetoolbox/common.py
--rw-rw-rw-   0        0        0     3331 2024-01-30 16:09:10.000000 chetoolbox-0.0.8/chetoolbox/display.py
--rw-rw-rw-   0        0        0     1374 2024-01-30 16:09:10.000000 chetoolbox-0.0.8/chetoolbox/fluids.py
--rw-rw-rw-   0        0        0    21781 2024-02-16 19:10:55.000000 chetoolbox-0.0.8/chetoolbox/props.py
--rw-rw-rw-   0        0        0    17920 2024-02-16 15:20:37.000000 chetoolbox-0.0.8/chetoolbox/separations.py
-drwxrwxrwx   0        0        0        0 2024-02-16 19:11:24.567806 chetoolbox-0.0.8/chetoolbox.egg-info/
--rw-rw-rw-   0        0        0      665 2024-02-16 19:11:24.000000 chetoolbox-0.0.8/chetoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-02-16 19:11:24.000000 chetoolbox-0.0.8/chetoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 19:11:24.000000 chetoolbox-0.0.8/chetoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-02-16 19:11:24.000000 chetoolbox-0.0.8/chetoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-16 19:11:24.000000 chetoolbox-0.0.8/chetoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-02-16 19:11:24.576517 chetoolbox-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1070 2024-02-16 19:10:55.000000 chetoolbox-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-23 18:21:06.399199 chetoolbox-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2024-01-30 16:09:10.000000 chetoolbox-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      665 2024-02-23 18:21:06.399199 chetoolbox-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1275 2024-02-21 18:39:41.000000 chetoolbox-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-23 18:21:06.370952 chetoolbox-0.0.9/chetoolbox/
+-rw-rw-rw-   0        0        0        0 2024-01-30 16:09:10.000000 chetoolbox-0.0.9/chetoolbox/__init__.py
+-rw-rw-rw-   0        0        0    11387 2024-02-23 16:25:49.000000 chetoolbox-0.0.9/chetoolbox/common.py
+-rw-rw-rw-   0        0        0     3331 2024-01-30 16:09:10.000000 chetoolbox-0.0.9/chetoolbox/display.py
+-rw-rw-rw-   0        0        0     1374 2024-01-30 16:09:10.000000 chetoolbox-0.0.9/chetoolbox/fluids.py
+-rw-rw-rw-   0        0        0    22666 2024-02-22 18:59:57.000000 chetoolbox-0.0.9/chetoolbox/props.py
+-rw-rw-rw-   0        0        0    28206 2024-02-23 16:25:49.000000 chetoolbox-0.0.9/chetoolbox/separations.py
+drwxrwxrwx   0        0        0        0 2024-02-23 18:21:06.398198 chetoolbox-0.0.9/chetoolbox.egg-info/
+-rw-rw-rw-   0        0        0      665 2024-02-23 18:21:06.000000 chetoolbox-0.0.9/chetoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-02-23 18:21:06.000000 chetoolbox-0.0.9/chetoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-23 18:21:06.000000 chetoolbox-0.0.9/chetoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-02-23 18:21:06.000000 chetoolbox-0.0.9/chetoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-02-23 18:21:06.000000 chetoolbox-0.0.9/chetoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-02-23 18:21:06.406199 chetoolbox-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2024-02-23 17:19:39.000000 chetoolbox-0.0.9/setup.py
```

### Comparing `chetoolbox-0.0.8/LICENSE.txt` & `chetoolbox-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chetoolbox-0.0.8/PKG-INFO` & `chetoolbox-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chetoolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library of common chemical engineering calculations
 Author: Quan Phan & Ethan Molnar
 Author-email: Phanqv@mail.uc.edu
 Keywords: python,chemical engineering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `chetoolbox-0.0.8/README.md` & `chetoolbox-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # CheToolbox
 Co-Written by Quan Phan & Ethan Molnar
 ## About
-CheToolbox or Chemical Engineering Toolbox is a python package designed to formalize the calculations I have learned through university and professional experience in code. Funcitons are written to be clear, conscise, easy to use, and save time compared to starting from scratch. This code is written in a semi-functional programming style, with a focus on internal consistency.
+CheToolbox or Chemical Engineering Toolbox is a python package designed to formalize calculations learned throughout university and professional experience in code. Funcitons are written to be clear, conscise, easy to use, and save time compared to starting from scratch. This code is written in a semi-functional programming style, with a focus on internal consistency.
 ## License
 CheToolbox is distributed under GPL Liscense version 3 (GPLv3)
 ## Dependencies
 The following dependencies will be necessary for CheToolbox to build properly,
 - Python >= 2.7: http://www.python.org/ (also install development files)
-- PIP >= 7.0: https://pip.pypa.io/ (not required in some scenarios, but never bad to have)
 - SciPy >= 0.11.0: http://www.scipy.org/
 - NumPy >= 1.16.0: http://www.numpy.org/
 - pandas
 ## Usage
 ```py
 import numpy as np
 from chetoolbox import separations
 ```
 ```py
-x = np.array([0.1,0.2,0.3,0.4]) # mol fraction of incoming stream
-K = np.array([4.2,1.75,.74,.34]) # corresponding K values
+x = np.array([0.1, 0.2, 0.3, 0.4]) # mol fraction of incoming stream
+K = np.array([4.2, 1.75, .74, .34]) # corresponding K values
 psi_init = 0.5 # an initial guess for psi
 ```
 ```py
-separations.psi_solver(x,K,psi_init)
+separations.psi_solver(x, K, psi_init)
 ```
 ```py
 (0.12109169497141782,
  array([0.07207241, 0.18334851, 0.30975219, 0.43474505]),
  array([0.30270414, 0.3208599 , 0.22921662, 0.14781332]),
  0.000675806754791175,
  2)
```

### Comparing `chetoolbox-0.0.8/chetoolbox/display.py` & `chetoolbox-0.0.9/chetoolbox/display.py`

 * *Files identical despite different names*

### Comparing `chetoolbox-0.0.8/chetoolbox/fluids.py` & `chetoolbox-0.0.9/chetoolbox/fluids.py`

 * *Files identical despite different names*

### Comparing `chetoolbox-0.0.8/chetoolbox/props.py` & `chetoolbox-0.0.9/chetoolbox/props.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,35 @@
   Cp : float
     Estimated specific heat capacity of the compound in J/mol*K (Joules per mole Kelvin).
   '''
   return const[0] + const[1]*T + const[2]*T**2 + const[3] / T**2
 
 # TODO #13 function to solve for ABCD specific heat constants given multiple (T, Cp) pairs
 
-# TODO #6 do we want/need a way to calculate deltaH_0 and deltaS_0 ie Hess' Law?
+def hess(prod: npt.ArrayLike, reac: npt.ArrayLike):
+  '''
+  Estimates change in enthalpy, entropy, or Gibb's free energy based on formation values for delta H, delta S or delta G.
+
+  Parameters:
+  -----------
+  prod : ArrayLike
+    The product species' stoichiometric coefficient and delta H, S, or G for formation in J/mol (Joules per mole). Shape must be N x 2.
+      Ex) np.array([coeff1, A1], [coeff2, A2], [coeff3, A3])
+  reac : ArrayLike
+    The reactant species' stoichiometric coefficient and delta H, S, or G for formation in J/mol (Joules per mole). Shape must be N x 2.
+      Ex) np.array([coeff1, A1], [coeff2, A2], [coeff3, A3])
+  Returns:
+  -----------
+  delta : float
+    change in enthalpy, entropy, or Gibb's free energy for the reaction in J/mol (Joules per mole).
+  '''
+  prod = np.atleast_1d(prod).reshape(-1, 2)
+  reac = np.atleast_1d(reac).reshape(-1, 2)
+
+  return np.sum(prod[:,0]*prod[:,1]) - np.sum(reac[:,0]* reac[:,1])
 
 def deltaH_est(prod: npt.ArrayLike, reac: npt.ArrayLike, T: float, deltaH_0: float, T_0: float = 298.) -> float:
   '''
   Estimates enthalpy of a balanced chemical reaction. A negative value indicates a net energy release.
 
   Parameters:
   -----------
```

### Comparing `chetoolbox-0.0.8/chetoolbox.egg-info/PKG-INFO` & `chetoolbox-0.0.9/chetoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chetoolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library of common chemical engineering calculations
 Author: Quan Phan & Ethan Molnar
 Author-email: Phanqv@mail.uc.edu
 Keywords: python,chemical engineering
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `chetoolbox-0.0.8/setup.py` & `chetoolbox-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A library of common chemical engineering calculations'
 LONG_DESCRIPTION = 'A personal project cataloging common chemical engineering calculations employing numerical methods'
 
 setup(
     name = 'chetoolbox',
     version = VERSION,
     author = 'Quan Phan & Ethan Molnar',
```

