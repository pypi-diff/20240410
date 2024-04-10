# Comparing `tmp/primpy-2.3.9.tar.gz` & `tmp/primpy-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primpy-2.3.9.tar", last modified: Fri Oct 28 06:46:29 2022, max compression
+gzip compressed data, was "primpy-2.7.8.tar", last modified: Wed Apr 10 08:35:08 2024, max compression
```

## Comparing `primpy-2.3.9.tar` & `primpy-2.7.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-28 06:46:21.000000 primpy-2.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-10-28 06:46:29.943846 primpy-2.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-10-28 06:46:21.000000 primpy-2.3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/primpy/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10744 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/bigbang.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/primpy/efolds/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/efolds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/efolds/inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/efolds/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/equations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     5769 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/exceptionhandling.py
--rw-r--r--   0 runner    (1001) docker     (121)    12795 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)    12690 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/initialconditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/oscode_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4893 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (121)    35421 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/potentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/primpy/time/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/time/inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/time/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-10-28 06:46:21.000000 primpy-2.3.9/primpy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/primpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4399 2022-10-28 06:46:29.000000 primpy-2.3.9/primpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-28 06:46:29.000000 primpy-2.3.9/primpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 06:46:29.000000 primpy-2.3.9/primpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-28 06:46:29.000000 primpy-2.3.9/primpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-28 06:46:29.000000 primpy-2.3.9/primpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-28 06:46:29.943846 primpy-2.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-10-28 06:46:21.000000 primpy-2.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 06:46:29.943846 primpy-2.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7810 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_bigbang.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_efolds_inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_equations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_exceptionhandling.py
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7030 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_initialconditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8919 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_perturbations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5914 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_potentials.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_time_inflation.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-10-28 06:46:21.000000 primpy-2.3.9/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.564746 primpy-2.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 08:35:02.000000 primpy-2.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 08:35:08.564746 primpy-2.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 08:35:02.000000 primpy-2.7.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.556746 primpy-2.7.8/primpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/bigbang.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/primpy/efolds/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/efolds/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/exceptionhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/initialconditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/oscode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/primpy/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/time/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 08:35:02.000000 primpy-2.7.8/primpy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.564746 primpy-2.7.8/primpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 08:35:08.000000 primpy-2.7.8/primpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:35:08.564746 primpy-2.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-10 08:35:02.000000 primpy-2.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:35:08.560746 primpy-2.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_bigbang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_efolds_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_exceptionhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_initialconditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_time_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-10 08:35:02.000000 primpy-2.7.8/tests/test_version.py
```

### Comparing `primpy-2.3.9/LICENSE` & `primpy-2.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/PKG-INFO` & `primpy-2.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primpy
-Version: 2.3.9
+Version: 2.7.8
 Summary: primpy: Calculations for the primordial Universe.
 Author: Lukas Hergt
 Author-email: lh561@mrao.cam.ac.uk
 License: MIT
 Keywords: PPS,cosmic inflation,initial conditions for inflation,kinetic dominance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -14,21 +14,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyoscode
 
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.3.9
+:Version: 2.7.8
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.3.9/README.rst` & `primpy-2.7.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.3.9
+:Version: 2.7.8
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.3.9/primpy/bigbang.py` & `primpy-2.7.8/primpy/bigbang.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/efolds/inflation.py` & `primpy-2.7.8/primpy/efolds/inflation.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/efolds/perturbations.py` & `primpy-2.7.8/primpy/efolds/perturbations.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,37 +44,37 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         comoving curvature perturbations `R` w.r.t. e-folds `N`, where the e.o.m. is
         written as `ddR + 2 * damping * dR + frequency**2 R = 0`.
 
         """
         K = self.background.K
-        a2 = np.exp(2 * self.background.N[:self.idx_end])
-        H = self.background.H[:self.idx_end]
-        dphidN = self.background.dphidN[:self.idx_end]
+        a2 = np.exp(2 * self.background.N[self.idx_beg:self.idx_end+1])
+        H = self.background.H[self.idx_beg:self.idx_end+1]
+        dphidN = self.background.dphidN[self.idx_beg:self.idx_end+1]
         H2 = H**2
-        dV = self.background.potential.dV(self.background.phi[:self.idx_end])
-        Omega_K = self.background.Omega_K[:self.idx_end]
+        dV = self.background.potential.dV(self.background.phi[self.idx_beg:self.idx_end+1])
+        Omega_K = self.background.Omega_K[self.idx_beg:self.idx_end+1]
 
         kappa2 = self.k**2 + self.k * K * (K + 1) - 3 * K
         epsilon = dphidN**2 / 2
         xi = Omega_K + epsilon - 3
 
         damping2 = 2 * kappa2 / (kappa2 + K * epsilon) * (xi - dV / (H2 * dphidN)) - xi
         frequency2 = kappa2 / (a2 * H2) + (damping2 + xi + 1) * Omega_K
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for scalar modes for RST vacuum w.r.t. e-folds `N`."""
-        a_i = np.exp(self.background.N[0])
-        H_i = self.background.H[0]
-        z_i = a_i * self.background.dphidN[0]
+        a_i = np.exp(self.background.N[self.idx_beg])
+        H_i = self.background.H[self.idx_beg]
+        z_i = a_i * self.background.dphidN[self.idx_beg]
         Rk_i = 1 / np.sqrt(2 * self.k) / z_i
         dRk_i = -1j * self.k / (a_i * H_i) * Rk_i
         return Rk_i, dRk_i
 
 
 class TensorModeN(TensorMode):
     """Template for tensor modes."""
@@ -92,24 +92,24 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         tensor perturbations `h` w.r.t. e-folds `N`, where the e.o.m. is
         written as `ddh + 2 * damping * dh + frequency**2 h = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[:self.idx_end]
-        H2 = self.background.H[:self.idx_end]**2
-        dphidN = self.background.dphidN[:self.idx_end]
+        N = self.background.N[self.idx_beg:self.idx_end+1]
+        H2 = self.background.H[self.idx_beg:self.idx_end+1]**2
+        dphidN = self.background.dphidN[self.idx_beg:self.idx_end+1]
         frequency2 = (self.k**2 + self.k * K * (K + 1) + 2 * K) * np.exp(-2 * N) / H2
         damping2 = 3 - dphidN**2 / 2 + K * np.exp(-2 * N) / H2
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for tensor modes for RST vacuum w.r.t. e-folds `N`."""
-        a_i = np.exp(self.background.N[0])
-        H_i = self.background.H[0]
+        a_i = np.exp(self.background.N[self.idx_beg])
+        H_i = self.background.H[self.idx_beg]
         hk_i = 2 / np.sqrt(2 * self.k) / a_i
         dhk_i = -1j * self.k / (a_i * H_i) * hk_i
         return hk_i, dhk_i
```

### Comparing `primpy-2.3.9/primpy/equations.py` & `primpy-2.7.8/primpy/equations.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/events.py` & `primpy-2.7.8/primpy/events.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/exceptionhandling.py` & `primpy-2.7.8/primpy/exceptionhandling.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/inflation.py` & `primpy-2.7.8/primpy/inflation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 """:mod:`primpy.inflation`: general setup for equations for cosmic inflation."""
 from warnings import warn
 from abc import ABC
 import numpy as np
-from scipy.interpolate import interp1d
-from scipy.misc import derivative
+from scipy.interpolate import interp1d, InterpolatedUnivariateSpline
 from primpy.exceptionhandling import CollapseWarning, InflationStartWarning, InflationEndWarning
-from primpy.units import pi, c, a_B, mp_kg, lp_m, Mpc_m
-from primpy.parameters import T_CMB, K_STAR
+from primpy.units import pi, c, lp_m, Mpc_m
+from primpy.parameters import K_STAR, rho_r0_mp_ilp3
 from primpy.equations import Equations
 
 
 class InflationEquations(Equations, ABC):
     """Base class for inflation equations."""
 
     def __init__(self, K, potential, verbose=False):
@@ -97,18 +96,16 @@
         if np.isfinite(sol.N_beg) and np.isfinite(sol.N_end):
             sol.inflation_mask = (sol.N_beg <= sol.N) & (sol.N <= sol.N_end)
 
         def derive_a0(Omega_K0, h, delta_reh=None, w_reh=None):
             """Derive the scale factor today `a_0` either from reheating or from `Omega_K0`."""
             # derive a0 and Omega_K0 from reheating:
             if Omega_K0 is None:
-                rho_r0_SI = a_B * T_CMB**4 / c**2  # TODO: fix rho_r0 = rho_photon0 + rho_nu0 ?
-                rho_r0 = rho_r0_SI / mp_kg * lp_m**3
                 # just from instant reheating:
-                N0 = sol.N_end + np.log(3 / 2) / 4 + np.log(sol.V_end / rho_r0) / 4
+                N0 = sol.N_end + np.log(3 / 2) / 4 + np.log(sol.V_end / rho_r0_mp_ilp3) / 4
                 # additional term from general reheating:
                 if delta_reh is not None and w_reh is not None:
                     N0 += (1 - 3 * w_reh) * delta_reh / 4
                 sol.a0_lp = np.exp(N0)
                 sol.a0_Mpc = sol.a0_lp * lp_m / Mpc_m
                 sol.Omega_K0 = - sol.K * c**2 / (sol.a0_Mpc * 100e3 * h)**2
             # for flat universes the scale factor can be freely rescaled
@@ -173,26 +170,27 @@
             """Calibrate wavenumber for flat universes, then derive approximate power spectra."""
             calibrate_a_flat_universe(N_star, logaH_star)
 
             sol.N_dagg = sol.N_tot - sol.N_star
             logaH = sol.logaH[sol.inflation_mask]
             sol.logk = np.log(K_STAR) + logaH - sol.logaH_star
             sol.k_iMpc = np.exp(sol.logk)
-            sol.k_comoving = sol.k_iMpc * sol.a0_Mpc
+            sol.k_comoving = np.exp(logaH)
 
             derive_approx_power(**interp1d_kwargs)
 
         def calibrate_wavenumber_curved(Omega_K0, h, delta_reh=None, w_reh=None,
                                         **interp1d_kwargs):
             """Calibrate wavenumber for curved universes, then derive approximate power spectra."""
             derive_a0(Omega_K0=Omega_K0, h=h, delta_reh=delta_reh, w_reh=w_reh)
 
             N = sol.N[sol.inflation_mask]
             logaH = sol.logaH[sol.inflation_mask]
             sol.logk = logaH - np.log(sol.a0_Mpc)
+            sol.logaH_star = np.log(K_STAR * sol.a0_Mpc)
             if np.log(K_STAR) < np.min(sol.logk) or np.log(K_STAR) > np.max(sol.logk):
                 sol.N_cross = np.nan
             else:
                 logk, indices = np.unique(sol.logk, return_index=True)
                 logk2N = interp1d(logk, N[indices])
                 sol.N_cross = logk2N(np.log(K_STAR))
             sol.N_dagg = sol.N_cross - sol.N_beg
@@ -207,67 +205,53 @@
                 dphidt = sol.dphidt[sol.inflation_mask]
             else:
                 dphidt = H * sol.dphidN[sol.inflation_mask]
             sol.P_scalar_approx = (H**2 / (2 * pi * dphidt))**2
             sol.P_tensor_approx = 2 * (H / pi)**2
 
             logk, indices = np.unique(sol.logk, return_index=True)
-
-            bounds_error = interp1d_kwargs.pop('bounds_error', False)
-            fill_value = interp1d_kwargs.pop('fill_value', 1e-30)
-            kind = interp1d_kwargs.pop('kind', 'cubic')
-            sol.logk2P_scalar = interp1d(logk, sol.P_scalar_approx[indices],
-                                         bounds_error=bounds_error,
-                                         fill_value=fill_value,
-                                         kind=kind)
-            sol.logk2P_tensor = interp1d(logk, sol.P_tensor_approx[indices],
-                                         bounds_error=bounds_error,
-                                         fill_value=fill_value,
-                                         kind=kind)
-            derive_approx_ns()
-            derive_approx_nrun()
-            derive_approx_r()
-            derive_approx_As()
-
-        def derive_approx_ns(x0=np.log(K_STAR), dx=np.log(K_STAR)/10, order=9):
-            """Derive the spectral index `n_s` from `P_s_approx`."""
-            def logP(logk):
-                """Return log of PPS `P` w.r.t. log of wavenumber `k`."""
-                return np.log(sol.P_s_approx(np.exp(logk)))
-
-            sol.n_s = 1 + derivative(func=logP, x0=x0, dx=dx, n=1, order=order)
-            return sol.n_s
-
-        def derive_approx_nrun(x0=np.log(K_STAR), dx=np.log(K_STAR)/10., order=9):
-            """Derive the running of the spectral index `n_run` from `P_s_approx`."""
-            def logP(logk):
-                """Return log of PPS `P` w.r.t. log of wavenumber `k`."""
-                return np.log(sol.P_s_approx(np.exp(logk)))
-
-            sol.n_run = derivative(func=logP, x0=x0, dx=dx, n=2, order=order)
-            return sol.n_run
-
-        def derive_approx_r(k_pivot=K_STAR):
-            """Derive the tensor-to-scalar ratio `r` from `P_s_approx`."""
-            sol.r = sol.P_t_approx(k_pivot) / sol.P_s_approx(k_pivot)
-
-        def derive_approx_As(k_pivot=K_STAR):
-            """Derive the amplitude `A_s` from `P_s_approx`."""
-            sol.A_s = sol.P_s_approx(k_pivot)
+            spline_order = interp1d_kwargs.pop('k', 3)
+            extrapolate = interp1d_kwargs.pop('ext', 'const')
+            sol.logk2logP_s = InterpolatedUnivariateSpline(logk,
+                                                           np.log(sol.P_scalar_approx[indices]),
+                                                           k=spline_order, ext=extrapolate,
+                                                           **interp1d_kwargs)
+            sol.logk2logP_t = InterpolatedUnivariateSpline(logk,
+                                                           np.log(sol.P_tensor_approx[indices]),
+                                                           k=spline_order, ext=extrapolate,
+                                                           **interp1d_kwargs)
+            if sol.logk[0] < np.log(K_STAR) < sol.logk[-1]:
+                dlogPdlogk_s = sol.logk2logP_s.derivatives(np.log(K_STAR))
+                dlogPdlogk_t = sol.logk2logP_t.derivatives(np.log(K_STAR))
+                sol.A_s = np.exp(dlogPdlogk_s[0])
+                sol.n_s = 1 + dlogPdlogk_s[1]
+                sol.n_run = dlogPdlogk_s[2]
+                sol.n_runrun = dlogPdlogk_s[3]
+                sol.A_t = np.exp(dlogPdlogk_t[0])
+                sol.n_t = dlogPdlogk_t[1]
+                sol.r = sol.A_t / sol.A_s
+            else:
+                sol.A_s = np.nan
+                sol.n_s = np.nan
+                sol.n_run = np.nan
+                sol.n_runrun = np.nan
+                sol.A_t = np.nan
+                sol.n_t = np.nan
+                sol.r = np.nan
 
         if self.K == 0:
             sol.derive_approx_power = calibrate_wavenumber_flat
         else:
             sol.derive_approx_power = calibrate_wavenumber_curved
 
         def P_s_approx(k):
             """Slow-roll approximation for the primordial power spectrum for scalar modes."""
-            return sol.logk2P_scalar(np.log(k))
+            return np.exp(sol.logk2logP_s(np.log(k)))
 
         def P_t_approx(k):
             """Slow-roll approximation for the primordial power spectrum for tensor modes."""
-            return sol.logk2P_tensor(np.log(k))
+            return np.exp(sol.logk2logP_t(np.log(k)))
 
         sol.P_s_approx = P_s_approx
         sol.P_t_approx = P_t_approx
 
         return sol
```

### Comparing `primpy-2.3.9/primpy/initialconditions.py` & `primpy-2.7.8/primpy/initialconditions.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,84 @@
 from primpy.efolds.inflation import InflationEquationsN
 from primpy.solver import solve
 from primpy.events import InflationEvent, CollapseEvent, UntilNEvent
 import primpy.bigbang as bb
 
 
 # noinspection PyPep8Naming
+class SlowRollIC(object):
+    """Slow-roll initial conditions given `phi_i` and either of `N_i` or `Omega_Ki`.
+
+    Class for setting up initial conditions during slow-roll inflation where
+    the potential energy dominates over the kinetic energy.
+    """
+
+    def __init__(self, equations, phi_i, t_i=None, eta_i=None, x_end=1e300, **kwargs):
+        self.equations = equations
+        self.phi_i = phi_i
+        self.t_i = t_i
+        self.eta_i = eta_i
+        self.x_end = x_end
+
+        self.V_i = equations.potential.V(self.phi_i)
+        self.dV_i = equations.potential.dV(self.phi_i)
+        if 'N_i' in kwargs and 'Omega_Ki' not in kwargs:
+            self.N_i = kwargs.pop('N_i')
+            self.ic_input_param = {'N_i': self.N_i}
+            self.aH2_i = self.V_i / 3 * np.exp(2 * self.N_i) - equations.K
+            if self.aH2_i < 0:
+                raise InflationStartError(
+                    "V_i / 3 * exp(2 N_i) - 1 = %s < 0 but needs to be > 0. Increase either N_i "
+                    "or phi_i." % self.aH2_i, geometry="closed")
+            self.aH_i = np.sqrt(self.V_i / 3 * np.exp(2 * self.N_i) - equations.K)
+            self.Omega_Ki = -equations.K / self.aH2_i
+        elif 'Omega_Ki' in kwargs and 'N_i' not in kwargs:
+            self.Omega_Ki = kwargs.pop('Omega_Ki')
+            self.ic_input_param = {'Omega_Ki': self.Omega_Ki}
+            if self.Omega_Ki >= 1:
+                raise InflationStartError(
+                    "Primordial curvature for open universes has to be Omega_Ki < 1, "
+                    "but Omega_Ki = %g was requested." % self.Omega_Ki, geometry="open")
+            self.N_i = np.log(3 * equations.K / self.V_i * (1 - 1 / self.Omega_Ki)) / 2
+            self.aH2_i = -equations.K / self.Omega_Ki
+            self.aH_i = np.sqrt(self.aH2_i)
+        else:
+            raise TypeError("Need to specify either N_i xor Omega_Ki.")
+        self.H_i = self.aH_i * np.exp(-self.N_i)
+        if isinstance(self.equations, InflationEquationsT):
+            self.x_ini = self.t_i
+            self.x_end = self.x_end
+            self.dphidt_i = -self.dV_i / (3 * self.H_i)
+        elif isinstance(self.equations, InflationEquationsN):
+            self.x_ini = self.N_i
+            self.x_end = self.x_end
+            self.dphidN_i = -self.dV_i / (3 * self.H_i**2)
+
+    def __call__(self, y0, **ivp_kwargs):
+        """Set background equations of inflation for `N`, `phi` and `dphi`."""
+        if isinstance(self.equations, InflationEquationsT):
+            y0[self.equations.idx['dphidt']] = self.dphidt_i
+            y0[self.equations.idx['N']] = self.N_i
+        elif isinstance(self.equations, InflationEquationsN):
+            y0[self.equations.idx['dphidN']] = self.dphidN_i
+            if self.equations.track_time:
+                assert self.t_i is not None, ("`track_time=%s`, but `t_i=%s`."
+                                              % (self.equations.track_time, self.t_i))
+                y0[self.equations.idx['t']] = self.t_i
+        else:
+            raise NotImplementedError("`equations` has to be either of type `InflationEquationsT`"
+                                      "or of type `InflationEquationsN`, but type `%s` was given."
+                                      % type(self.equations))
+        y0[self.equations.idx['phi']] = self.phi_i
+        if self.equations.track_eta:
+            assert self.eta_i is not None, ("`track_eta=%s`, but `eta_i=%s`."
+                                            % (self.equations.track_eta, self.eta_i))
+            y0[self.equations.idx['eta']] = self.eta_i
+
+
 class InflationStartIC(object):
     """Inflation start initial conditions given `phi_i` and either of `N_i` or `Omega_Ki`.
 
     Class for setting up initial conditions at the start of inflation, when
     the curvature density parameter was maximal after kinetic dominance.
     """
 
@@ -197,16 +267,15 @@
                       InflationEvent(self.equations, direction=-1, terminal=True),
                       UntilNEvent(self.equations, self.N0),
                       CollapseEvent(self.equations)]
             with warnings.catch_warnings():
                 warnings.filterwarnings(action=self.warn_action, category=InflationWarning)
                 sol = solve(ic, events=events, **kwargs)
             if np.isfinite(sol.N_tot) and sol.N_tot > self.N_star:
-                # Fixme: kind=linear
-                sol.derive_approx_power(Omega_K0=self.Omega_K0, h=self.h, kind='linear')
+                sol.derive_approx_power(Omega_K0=self.Omega_K0, h=self.h)
                 self.vprint("N_tot = %.15g, N_star = %.15g for phi_i = %.15g"
                             % (sol.N_tot, sol.N_star, phi_i))
                 return sol.N_star - self.N_star
             elif np.size(sol.N_events['UntilN']) > 0 or sol.N[-1] >= self.N0:
                 self.vprint("N_tot > %g for phi_i = %.15g" % (self.N0, phi_i))
                 return sol.N[-1]
             elif (np.size(sol.N_events['Collapse']) > 0 or sol.N_tot <= self.N_star or
```

### Comparing `primpy-2.3.9/primpy/oscode_solver.py` & `primpy-2.7.8/primpy/oscode_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from primpy.time.perturbations import PerturbationT
 from primpy.efolds.perturbations import PerturbationN
 
 
 def solve_oscode(background, k, **kwargs):
     """Run :func:`pyoscode.solve` and store information for post-processing.
 
-    This is a wrapper around :func:`pyoscode.solve` to calculate the solution to
-    the Mukhanov-Sasaki equation.
+    This is a wrapper around :func:`pyoscode.solve` to calculate the solution
+    to the Mukhanov-Sasaki equation.
 
     Parameters
     ----------
         background : Bunch object as returned by :func:`primpy.solver.solve`
             Solution to the inflationary background equations used to calculate
             the frequency and damping term passed to oscode.
         k : int, float, np.ndarray
@@ -28,18 +28,24 @@
             their derivatives for two independent solutions. The perturbations
             (y0_1, y0_2) are scaled with `k` and their derivatives with `k**2`
             in order to produce freeze-out values of about order(~1).
             default : determined by input inflationary potential
         rtol : float
             Tolerance passed to pyoscode.
             default : 5e-5
-        fac : int, float
-            Integration of the mode evolution stops when the considered scale k
-            exceeds the comoving Hubble horizon by a factor of `fac`, i.e. when
-            `aH / k > fac`.
+        fac_beg : int, float
+            Integration of the mode evolution starts when the considered
+            scale 1/k is within a factor of `fac_beg` of the comoving Hubble
+            horizon, i.e. when `1/k > 1/aH / fac_beg`.
+            `fac_beg=0` starts integration immediately.
+            default : 0
+        fac_end : int, float
+            Integration of the mode evolution stops when the considered
+            scale 1/k exceeds the comoving Hubble horizon by a factor of
+            `fac_end`, i.e. when `1/k > 1/aH * fac_end`.
             default : 100
         even_grid : bool
             Set this to True if the grid of the independent variable is
             equally spaced.
             default : False
         vacuum : tuple
             Set of vacuum initial conditions to be computed.
@@ -60,49 +66,56 @@
             Monkey-patched version of the Bunch type usually returned by
             :func:`scipy.integrate.solve_ivp`.
 
     """
     assert 'tol' not in kwargs
     y0 = kwargs.pop('y0', background.potential.perturbation_ic)
     rtol = kwargs.pop('rtol', 5e-5)
-    fac = kwargs.pop('fac', 100)
+    fac_beg = kwargs.pop('fac_beg', 0)
+    fac_end = kwargs.pop('fac_end', 100)
     even_grid = kwargs.pop('even_grid', False)
     vacuum = kwargs.get('vacuum', ('RST',))
     drop_closed_large_scales = kwargs.pop('drop_closed_large_scales', True)
     b = background
     if isinstance(k, int) or isinstance(k, float):
         k = np.atleast_1d(k)
         return_pps = False
     else:
         return_pps = True
     PPS = PrimordialPowerSpectrum(background=b, k=k, **kwargs)
     # stop integration sufficiently after mode has crossed the horizon (lazy for loop):
-    j = 2
     for i, ki in enumerate(k):
-        for j in range(j, b.x.size):
-            if b.logaH[j] - np.log(ki) > np.log(fac):
-                if b.independent_variable == 't':
-                    p = PerturbationT(background=b, k=ki, idx_end=j+1, **kwargs)
-                elif b.independent_variable == 'N':
-                    p = PerturbationN(background=b, k=ki, idx_end=j+1, **kwargs)
-                else:
-                    raise NotImplementedError()
-                oscode_sol = []
-                for mode in [p.scalar, p.tensor]:
-                    for num in range(2):
-                        oscode_sol.append(pyoscode.solve(ts=b.x[:j+1], ti=b.x[0], tf=b.x[j],
-                                                         ws=np.log(mode.ms_frequency), logw=True,
-                                                         gs=mode.ms_damping, logg=False,
-                                                         x0=y0[2 * num] * ki,
-                                                         dx0=y0[2 * num + 1] * ki**2,
-                                                         rtol=rtol, even_grid=even_grid))
-                p.oscode_postprocessing(oscode_sol=oscode_sol)
-                if ki < 1 and b.K == +1 and drop_closed_large_scales:
-                    p.scalar.P_s_RST = 1e-30
-                for vac in vacuum:
-                    getattr(PPS, 'P_s_%s' % vac)[i] = getattr(p.scalar, 'P_s_%s' % vac)
-                    getattr(PPS, 'P_t_%s' % vac)[i] = getattr(p.tensor, 'P_t_%s' % vac)
-                break
+        if fac_beg == 0:
+            idx_beg = 0
+        else:
+            idx_beg = np.argwhere(np.log(ki) - b.logaH > np.log(fac_beg)).ravel()
+            # set idx_beg to 0 if horizon starts out too small:
+            idx_beg = 0 if idx_beg.size == 0 else idx_beg[-1]
+        idx_end = np.argwhere(b.logaH - np.log(ki) > np.log(fac_end)).ravel()[0]
+        # set minimum for idx_end, needed e.g. in KD for superhorizon modes:
+        idx_end = idx_end if idx_end - idx_beg > b.logaH.size//20 else idx_beg + b.logaH.size//20
+        if b.independent_variable == 't':
+            p = PerturbationT(background=b, k=ki, idx_beg=idx_beg, idx_end=idx_end, **kwargs)
+        elif b.independent_variable == 'N':
+            p = PerturbationN(background=b, k=ki, idx_beg=idx_beg, idx_end=idx_end, **kwargs)
+        else:
+            raise NotImplementedError()
+        oscode_sol = []
+        for mode in [p.scalar, p.tensor]:
+            for num in range(2):
+                oscode_sol.append(pyoscode.solve(ts=b.x[idx_beg:idx_end+1],
+                                                 ti=b.x[idx_beg], tf=b.x[idx_end],
+                                                 ws=np.log(mode.ms_frequency), logw=True,
+                                                 gs=mode.ms_damping, logg=False,
+                                                 x0=y0[2*num]*ki,
+                                                 dx0=y0[2*num+1]*ki**2,
+                                                 rtol=rtol, even_grid=even_grid))
+        p.oscode_postprocessing(oscode_sol=oscode_sol)
+        if ki < 1 and b.K == +1 and drop_closed_large_scales:
+            p.scalar.P_s_RST = 1e-30
+        for vac in vacuum:
+            getattr(PPS, 'P_s_%s' % vac)[i] = getattr(p.scalar, 'P_s_%s' % vac)
+            getattr(PPS, 'P_t_%s' % vac)[i] = getattr(p.tensor, 'P_t_%s' % vac)
     if return_pps:
         return PPS
     else:
         return p
```

### Comparing `primpy-2.3.9/primpy/perturbations.py` & `primpy-2.7.8/primpy/perturbations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python
 """:mod:`primpy.time.perturbations`: comoving curvature perturbations w.r.t. time `t`."""
 from abc import ABC, abstractmethod
 import numpy as np
 from scipy.integrate import solve_ivp
 from primpy.units import pi
+from primpy.parameters import K_STAR
 from primpy.equations import Equations
 
 
 class PrimordialPowerSpectrum(object):
     """Primordial Power spectrum of curvature perturbations."""
 
     def __init__(self, background, k, **kwargs):
         self.background = background
         self.k = k
-        self.k_iMpc = k / background.a0_Mpc
+        self.k_iMpc = k * K_STAR / np.exp(background.logaH_star)
         vacuum = kwargs.pop('vacuum', ('RST',))
         for vac in vacuum:
             setattr(self, 'P_s_%s' % vac, np.full_like(k, np.nan, dtype=float))
             setattr(self, 'P_t_%s' % vac, np.full_like(k, np.nan, dtype=float))
 
 
 class Perturbation(ABC):
@@ -76,14 +77,15 @@
 
 
 class Mode(Equations, ABC):
     """Template for scalar or tensor modes."""
 
     def __init__(self, background, k, **kwargs):
         super(Mode, self).__init__()
+        self.idx_beg = kwargs.get('idx_beg', 0)
         self.idx_end = kwargs.get('idx_end', background.x.size)
         self.background = background
         self.k = k
         f, d = self.mukhanov_sasaki_frequency_damping()
         self.ms_frequency = f
         self.ms_damping = d
         self.one = solve_ivp(lambda x, y: y, (0, 0), y0=np.zeros(2))
```

### Comparing `primpy-2.3.9/primpy/potentials.py` & `primpy-2.7.8/primpy/potentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     tag = 'mnp'
     name = 'MonomialPotential'
     tex = r'$\phi^p$'
     perturbation_ic = (1e-1, 0, 0, 1e-6)
 
     def __init__(self, **pot_kwargs):
         self.p = pot_kwargs.pop('p')
-        super(MonomialPotential, self).__init__(**pot_kwargs)
+        super().__init__(**pot_kwargs)
 
     def V(self, phi):
         """`V(phi) = Lambda**4 * phi**p`."""
         return self.Lambda**4 * np.abs(phi)**self.p
 
     def dV(self, phi):
         """`V(phi) = Lambda**4 * phi**(p-1) * p`."""
@@ -175,14 +175,38 @@
         return self.Lambda**4 * np.abs(phi)**(self.p - 3.) * self.p * (self.p - 1) * (self.p - 2)
 
     def inv_V(self, V):
         """`phi(V) = (V / Lambda**4)**(1/p)`."""
         return (V / self.Lambda**4)**(1/self.p)
 
     @staticmethod
+    def sr_Nstar2ns(N_star, **pot_kwargs):
+        """Slow-roll approximation for inferring `n_s` from `N_star`."""
+        p = pot_kwargs.pop('p')
+        return 1 - p / (2 * N_star) - 1 / N_star
+
+    @staticmethod
+    def sr_ns2Nstar(n_s, **pot_kwargs):
+        """Slow-roll approximation for inferring `N_star` from `n_s`."""
+        p = pot_kwargs.pop('p')
+        return (2 + p) / (2 * (1 - n_s))
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_kwargs):
+        """Slow-roll approximation for inferring `r` from `N_star`."""
+        p = pot_kwargs.pop('p')
+        return 16 * p / (4 * N_star + p)
+
+    @staticmethod
+    def sr_r2Nstar(r, **pot_kwargs):
+        """Slow-roll approximation for inferring `N_star` from `r`."""
+        p = pot_kwargs.pop('p')
+        return p * (16 - r) / (4 * r)
+
+    @staticmethod
     def sr_As2Lambda(A_s, phi_star, N_star, **pot_kwargs):
         """Get potential amplitude `Lambda` from PPS amplitude `A_s`.
 
         Find the inflaton amplitude `Lambda` (4th root of potential amplitude)
         that produces the desired amplitude `A_s` of the primordial power
         spectrum using the slow-roll approximation.
 
@@ -224,18 +248,34 @@
 
     tag = 'mn1'
     name = 'LinearPotential'
     tex = r'$\phi^1$'
     perturbation_ic = (1, 0, 0, 1)
 
     def __init__(self, **pot_kwargs):
-        super(LinearPotential, self).__init__(p=1, **pot_kwargs)
+        super().__init__(p=1, **pot_kwargs)
 
-    @classmethod
-    def sr_As2Lambda(cls, A_s, phi_star, N_star, **pot_kwargs):
+    @staticmethod
+    def sr_Nstar2ns(N_star, **pot_params):  # noqa: D102
+        return MonomialPotential.sr_Nstar2ns(N_star=N_star, p=1)
+
+    @staticmethod
+    def sr_ns2Nstar(n_s, **pot_params):  # noqa: D102
+        return MonomialPotential.sr_ns2Nstar(n_s=n_s, p=1)
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_params):  # noqa: D102
+        return MonomialPotential.sr_Nstar2r(N_star=N_star, p=1)
+
+    @staticmethod
+    def sr_r2Nstar(r, **pot_params):  # noqa: D102
+        return MonomialPotential.sr_r2Nstar(r=r, p=1)
+
+    @staticmethod
+    def sr_As2Lambda(A_s, phi_star, N_star, **pot_kwargs):
         """Get potential amplitude `Lambda` from PPS amplitude `A_s`.
 
         Find the inflaton amplitude `Lambda` (4th root of potential amplitude)
         that produces the desired amplitude `A_s` of the primordial power
         spectrum using the slow-roll approximation.
 
         Parameters
@@ -255,52 +295,65 @@
             phi_star : float
                 Inflaton value at horizon crossing of the pivot scale.
             N_star: float
                 Number of observable e-folds of inflation `N_star`
                 from horizon crossing till the end of inflation.
 
         """
-        return super(LinearPotential, cls).sr_As2Lambda(A_s, phi_star, N_star, p=1)
+        return MonomialPotential.sr_As2Lambda(A_s, phi_star, N_star, p=1)
 
 
-class QuadraticPotential(InflationaryPotential):
-    """Quadratic potential: `V(phi) = 0.5 * m**2 * phi**2`."""
+class QuadraticPotential(MonomialPotential):
+    """Quadratic potential: `V(phi) = Lambda**4 * phi**2`."""
 
     tag = 'mn2'
     name = 'QuadraticPotential'
     tex = r'$\phi^2$'
     perturbation_ic = (1e-1, 0, 0, 1e-5)
 
     def __init__(self, **pot_kwargs):
         if 'mass' in pot_kwargs:
-            if 'Lambda' in pot_kwargs:
-                raise Exception("'mass' and 'Lambda' must not be specified simultaneously.")
-            pot_kwargs['Lambda'] = np.sqrt(pot_kwargs.pop('mass'))
-        super(QuadraticPotential, self).__init__(**pot_kwargs)
-        self.mass = self.Lambda**2
+            raise ValueError("'mass' was dropped use 'Lambda' instead: Lambda**4=mass**2")
+        super().__init__(p=2, **pot_kwargs)
 
     def V(self, phi):
-        """`V(phi) = 0.5 * m**2 * phi**2`."""
-        return self.mass**2 * phi**2 / 2
+        """`V(phi) = Lambda**4 * phi**2`."""
+        return self.Lambda**4 * phi**2
 
     def dV(self, phi):
-        """`V'(phi) = m**2 phi`."""
-        return self.mass**2 * phi
+        """`V'(phi) = 2 * Lambda**4 * phi`."""
+        return 2 * self.Lambda**4 * phi
 
     def d2V(self, phi):
-        """`V''(phi) = m**2`."""
-        return self.mass**2
+        """`V''(phi) = 2 * Lambda**4`."""
+        return 2 * self.Lambda**4
 
     def d3V(self, phi):
         """`V'''(phi) = 0`."""
         return 0
 
     def inv_V(self, V):
-        """`phi(V) = sqrt(2 * V) / m`."""
-        return np.sqrt(2 * V) / self.mass
+        """`phi(V) = sqrt(V) / Lambda**2`."""
+        return np.sqrt(V) / self.Lambda**2
+
+    @staticmethod
+    def sr_Nstar2ns(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2ns(N_star=N_star, p=2)
+
+    @staticmethod
+    def sr_ns2Nstar(n_s, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_ns2Nstar(n_s=n_s, p=2)
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2r(N_star=N_star, p=2)
+
+    @staticmethod
+    def sr_r2Nstar(r, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_r2Nstar(r=r, p=2)
 
     @staticmethod
     def sr_As2Lambda(A_s, phi_star, N_star, **pot_kwargs):
         """Get potential amplitude `Lambda` from PPS amplitude `A_s`.
 
         Find the inflaton mass `m` (i.e. essentially the potential amplitude)
         that produces the desired amplitude `A_s` of the primordial power
@@ -343,18 +396,34 @@
 
     tag = 'mn3'
     name = 'CubicPotential'
     tex = r'$\phi^3$'
     perturbation_ic = (1, 0, 0, 1)
 
     def __init__(self, **pot_kwargs):
-        super(CubicPotential, self).__init__(p=3, **pot_kwargs)
+        super().__init__(p=3, **pot_kwargs)
 
-    @classmethod
-    def sr_As2Lambda(cls, A_s, phi_star, N_star, **pot_kwargs):
+    @staticmethod
+    def sr_Nstar2ns(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2ns(N_star=N_star, p=3)
+
+    @staticmethod
+    def sr_ns2Nstar(n_s, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_ns2Nstar(n_s=n_s, p=3)
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2r(N_star=N_star, p=3)
+
+    @staticmethod
+    def sr_r2Nstar(r, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_r2Nstar(r=r, p=3)
+
+    @staticmethod
+    def sr_As2Lambda(A_s, phi_star, N_star, **pot_kwargs):
         """Get potential amplitude `Lambda` from PPS amplitude `A_s`.
 
         Find the inflaton amplitude `Lambda` (4th root of potential amplitude)
         that produces the desired amplitude `A_s` of the primordial power
         spectrum using the slow-roll approximation.
 
         Parameters
@@ -374,30 +443,46 @@
             phi_star : float
                 Inflaton value at horizon crossing of the pivot scale.
             N_star: float
                 Number of observable e-folds of inflation `N_star`
                 from horizon crossing till the end of inflation.
 
         """
-        return super(CubicPotential, cls).sr_As2Lambda(A_s, phi_star, N_star, p=3)
+        return MonomialPotential.sr_As2Lambda(A_s, phi_star, N_star, p=3)
 
 
 class QuarticPotential(MonomialPotential):
     """Linear potential: `V(phi) = Lambda**4 * phi`."""
 
     tag = 'mn4'
     name = 'QuarticPotential'
     tex = r'$\phi^4$'
     perturbation_ic = (1, 0, 0, 1)
 
     def __init__(self, **pot_kwargs):
-        super(QuarticPotential, self).__init__(p=4, **pot_kwargs)
+        super().__init__(p=4, **pot_kwargs)
 
-    @classmethod
-    def sr_As2Lambda(cls, A_s, phi_star, N_star, **pot_kwargs):
+    @staticmethod
+    def sr_Nstar2ns(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2ns(N_star=N_star, p=4)
+
+    @staticmethod
+    def sr_ns2Nstar(n_s, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_ns2Nstar(n_s=n_s, p=4)
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_Nstar2r(N_star=N_star, p=4)
+
+    @staticmethod
+    def sr_r2Nstar(r, **pot_kwargs):  # noqa: D102
+        return MonomialPotential.sr_r2Nstar(r=r, p=4)
+
+    @staticmethod
+    def sr_As2Lambda(A_s, phi_star, N_star, **pot_kwargs):
         """Get potential amplitude `Lambda` from PPS amplitude `A_s`.
 
         Find the inflaton amplitude `Lambda` (4th root of potential amplitude)
         that produces the desired amplitude `A_s` of the primordial power
         spectrum using the slow-roll approximation.
 
         Parameters
@@ -417,28 +502,28 @@
             phi_star : float
                 Inflaton value at horizon crossing of the pivot scale.
             N_star: float
                 Number of observable e-folds of inflation `N_star`
                 from horizon crossing till the end of inflation.
 
         """
-        return super(QuarticPotential, cls).sr_As2Lambda(A_s, phi_star, N_star, p=4)
+        return MonomialPotential.sr_As2Lambda(A_s, phi_star, N_star, p=4)
 
 
 class StarobinskyPotential(InflationaryPotential):
     """Starobinsky potential: `V(phi) = Lambda**4 * (1 - exp(-sqrt(2/3) * phi))**2`."""
 
     tag = 'stb'
     name = 'StarobinskyPotential'
     tex = r'Starobinsky'
     gamma = np.sqrt(2 / 3)
     perturbation_ic = (1-2, 0, 0, 1e-8)
 
     def __init__(self, **pot_kwargs):
-        super(StarobinskyPotential, self).__init__(**pot_kwargs)
+        super().__init__(**pot_kwargs)
 
     def V(self, phi):
         """`V(phi) = Lambda**4 * (1 - exp(-sqrt(2/3) * phi))**2`."""
         return self.Lambda**4 * (1 - np.exp(-StarobinskyPotential.gamma * phi))**2
 
     def dV(self, phi):
         """`V'(phi) = Lambda**4 * 2 * gamma * exp(-2 * gamma * phi) * (-1 + exp(gamma * phi))`."""
@@ -456,14 +541,42 @@
         return self.Lambda**4 * 2 * gamma**3 * np.exp(-2 * gamma * phi) * (np.exp(gamma * phi) - 4)
 
     def inv_V(self, V):
         """`phi(V) = -np.log(1 - np.sqrt(V) / Lambda**2) / gamma`."""
         return -np.log(1 - np.sqrt(V) / self.Lambda**2) / StarobinskyPotential.gamma
 
     @staticmethod
+    def sr_Nstar2ns(N_star):
+        """Slow-roll approximation for inferring `n_s` from `N_star`."""
+        gamma = StarobinskyPotential.gamma
+        num = 2 * N_star * gamma**2 + np.sqrt(2) * gamma + 2
+        den = N_star * gamma * (N_star * gamma + np.sqrt(2))
+        return 1 - num / den
+
+    @staticmethod
+    def sr_ns2Nstar(n_s):
+        """Slow-roll approximation for inferring `N_star` from `n_s`."""
+        gamma = StarobinskyPotential.gamma
+        num = 2*gamma - np.sqrt(2) * (1-n_s) + np.sqrt(2*(1-n_s)**2 + 8*(1-n_s) + 4*gamma**2)
+        den = 2 * gamma * (1-n_s)
+        return num / den
+
+    @staticmethod
+    def sr_Nstar2r(N_star):
+        """Slow-roll approximation for inferring `r` from `N_star`."""
+        gamma = StarobinskyPotential.gamma
+        return 32 / (2*N_star*gamma + np.sqrt(2))**2
+
+    @staticmethod
+    def sr_r2Nstar(r):
+        """Slow-roll approximation for inferring `N_star` from `r`."""
+        gamma = StarobinskyPotential.gamma
+        return np.sqrt(2) * (4 - np.sqrt(r)) / (2 * gamma * np.sqrt(r))
+
+    @staticmethod
     def phi2efolds(phi):
         """Get e-folds `N` from inflaton `phi`.
 
         Find the number of e-folds `N` till end of inflation from inflaton `phi`
         using the slow-roll approximation.
 
         Parameters
@@ -538,15 +651,15 @@
     tag = 'nat'
     name = 'NaturalPotential'
     tex = r'Natural'
     perturbation_ic = (1e-1, 0, 0, 1e-5)
 
     def __init__(self, **pot_kwargs):
         self.phi0 = pot_kwargs.pop('phi0')
-        super(NaturalPotential, self).__init__(**pot_kwargs)
+        super().__init__(**pot_kwargs)
 
     def V(self, phi):
         """`V(phi) = Lambda**4 * (1 - cos(pi*phi/phi0))`."""
         return self.Lambda**4 / 2 * (1 - np.cos(pi * phi / self.phi0))
 
     def dV(self, phi):
         """`V(phi) = Lambda**4 * sin(pi*phi/phi0) * pi / phi0`."""
@@ -561,31 +674,45 @@
         return -self.Lambda**4 / 2 * np.sin(pi * phi / self.phi0) * (pi / self.phi0)**3
 
     def inv_V(self, V):
         """`phi(V) = arccos(1 - V / Lambda**4) * phi0 / pi`."""
         return np.arccos(1 - 2 * V / self.Lambda**4) * self.phi0 / pi
 
     @staticmethod
-    def sr_n_s(N_star, **pot_kwargs):
+    def sr_Nstar2ns(N_star, **pot_kwargs):
         """Slow-roll approximation for the spectral index `n_s`."""
         phi0 = pot_kwargs.pop('phi0')
         f = phi0 / pi
-        numerator = 1 + 4 * f**2
-        denominator = (-1 + np.exp(N_star / f**2)) * (1 + 2 * f**2)
-        return 1 - 1 / f**2 * (1 + numerator / denominator)
+        num = (2 * f**2 + (2 * f**2 + 1) * np.exp(N_star / f**2))
+        den = (f**2 * (2 * f**2 + 1) * (np.exp(N_star / f**2) - 1))
+        return 1 - num / den
 
     @staticmethod
-    def sr_r(N_star, **pot_kwargs):
+    def sr_ns2Nstar(n_s, **pot_kwargs):
+        """Slow-roll approximation for inferring `N_star` from `n_s`."""
+        phi0 = pot_kwargs.pop('phi0')
+        f = phi0 / pi
+        return f**2 * np.log(f**2 * (2*f**2*(1-n_s)+(1-n_s)+2) / ((2*f**2+1) * (f**2*(1-n_s)-1)))
+
+    @staticmethod
+    def sr_Nstar2r(N_star, **pot_kwargs):
         """Slow-roll approximation for the tensor-to-scalar ratio `r`."""
         phi0 = pot_kwargs.pop('phi0')
         f = phi0 / pi
-        return 16 / (-2 * f**2 + np.exp(N_star / f**2) * (1 + 2 * f**2))
+        return 16 / (-2 * f**2 + (2 * f**2 + 1) * np.exp(N_star / f**2))
 
-    @classmethod
-    def phi2efolds(cls, phi, phi0):
+    @staticmethod
+    def sr_r2Nstar(r, **pot_kwargs):
+        """Slow-roll approximation for inferring `N_star` from `r`."""
+        phi0 = pot_kwargs.pop('phi0')
+        f = phi0 / pi
+        return f**2 * np.log((2 * f**2 * r + 16) / (r * (2 * f**2 + 1)))
+
+    @staticmethod
+    def phi2efolds(phi, phi0):
         """Get e-folds `N` from inflaton `phi`.
 
         Find the number of e-folds `N` till end of inflation from inflaton `phi`
         using the slow-roll approximation.
 
         Parameters
         ----------
@@ -663,15 +790,15 @@
     name = 'DoubleWellPotential'
     tex = r'Double-Well (p)'
     perturbation_ic = (1e-1, 0, 0, 1e-5)
 
     def __init__(self, **pot_kwargs):
         self.phi0 = pot_kwargs.pop('phi0')
         self.p = pot_kwargs.pop('p')
-        super(DoubleWellPotential, self).__init__(**pot_kwargs)
+        super().__init__(**pot_kwargs)
         self.prefactor = 2 * self.p * self.Lambda**4
 
     def V(self, phi):
         """`V(phi) = Lambda**4 * (1 - (phi/phi0)**p)**2`.
 
         Double-Well shifted such that left minimum is at zero: phi -> phi-phi0
         """
@@ -728,15 +855,15 @@
 
     tag = 'dw2'
     name = 'DoubleWell2Potential'
     tex = r'Double-Well (quadratic)'
     perturbation_ic = (1e-1, 0, 0, 1e-5)
 
     def __init__(self, **pot_kwargs):
-        super(DoubleWell2Potential, self).__init__(p=2, **pot_kwargs)
+        super().__init__(p=2, **pot_kwargs)
 
     @staticmethod
     def phi2efolds(phi_shifted, phi0):
         """Get e-folds `N` from inflaton `phi`.
 
         Find the number of e-folds `N` till end of inflation from inflaton `phi`
         using the slow-roll approximation.
@@ -819,15 +946,15 @@
 
     tag = 'dw4'
     name = 'DoubleWell4Potential'
     tex = r'Double-Well (quartic)'
     perturbation_ic = (1e-1, 0, 0, 1e-5)
 
     def __init__(self, **pot_kwargs):
-        super(DoubleWell4Potential, self).__init__(p=4, **pot_kwargs)
+        super().__init__(p=4, **pot_kwargs)
 
     @staticmethod
     def phi_end_squared(phi0):
         """Get inflaton at end of inflation using slow-roll.
 
         Parameters
         ----------
```

### Comparing `primpy-2.3.9/primpy/solver.py` & `primpy-2.7.8/primpy/solver.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/time/inflation.py` & `primpy-2.7.8/primpy/time/inflation.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/primpy/time/perturbations.py` & `primpy-2.7.8/primpy/time/perturbations.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,35 +43,35 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         comoving curvature perturbations `R` w.r.t. time `t`, where the e.o.m. is
         written as `ddR + 2 * damping * dR + frequency**2 R = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[:self.idx_end]
-        dphidt = self.background.dphidt[:self.idx_end]
-        H = self.background.H[:self.idx_end]
-        dV = self.background.potential.dV(self.background.phi[:self.idx_end])
+        N = self.background.N[self.idx_beg:self.idx_end+1]
+        dphidt = self.background.dphidt[self.idx_beg:self.idx_end+1]
+        H = self.background.H[self.idx_beg:self.idx_end+1]
+        dV = self.background.potential.dV(self.background.phi[self.idx_beg:self.idx_end+1])
 
         kappa2 = self.k**2 + self.k * K * (K + 1) - 3 * K
         shared = 2 * kappa2 / (kappa2 + K * dphidt**2 / (2 * H**2))
         terms = dphidt**2 / (2 * H**2) - 3 - dV / (H * dphidt) - K * np.exp(-2 * N) / H**2
 
         frequency2 = kappa2 * np.exp(-2 * N) - K * np.exp(-2 * N) * (1 + shared * terms)
         damping = (3 * H + shared * terms * H) / 2
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping
         else:
             return np.sqrt(frequency2 + 0j), damping
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for scalar modes for RST vacuum w.r.t. cosmic time `t`."""
-        a_i = np.exp(self.background.N[0])
-        dphidt_i = self.background.dphidt[0]
-        H_i = self.background.H[0]
+        a_i = np.exp(self.background.N[self.idx_beg])
+        dphidt_i = self.background.dphidt[self.idx_beg]
+        H_i = self.background.H[self.idx_beg]
         z_i = a_i * dphidt_i / H_i
         Rk_i = 1 / np.sqrt(2 * self.k) / z_i
         dRk_i = -1j * self.k / a_i * Rk_i
         return Rk_i, dRk_i
 
 
 class TensorModeT(TensorMode):
@@ -90,21 +90,21 @@
 
         Frequency and damping term of the Mukhanov-Sasaki equations for the
         tensor perturbations `h` w.r.t. time `t`, where the e.o.m. is
         written as `ddh + 2 * damping * dh + frequency**2 h = 0`.
 
         """
         K = self.background.K
-        N = self.background.N[: self.idx_end]
+        N = self.background.N[self.idx_beg:self.idx_end+1]
         frequency2 = (self.k**2 + self.k * K * (K + 1) + 2 * K) * np.exp(-2 * N)
-        damping2 = 3 * self.background.H[: self.idx_end]
+        damping2 = 3 * self.background.H[self.idx_beg:self.idx_end+1]
         if np.all(frequency2 > 0):
             return np.sqrt(frequency2), damping2 / 2
         else:
             return np.sqrt(frequency2 + 0j), damping2 / 2
 
     def get_vacuum_ic_RST(self):
         """Get initial conditions for tensor modes for RST vacuum w.r.t. cosmic time `t`."""
-        a_i = np.exp(self.background.N[0])
+        a_i = np.exp(self.background.N[self.idx_beg])
         hk_i = 2 / np.sqrt(2 * self.k) / a_i
         dhk_i = -1j * self.k / a_i * hk_i
         return hk_i, dhk_i
```

### Comparing `primpy-2.3.9/primpy/units.py` & `primpy-2.7.8/primpy/units.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 """:mod:`primpy.units`: units and constants for primpy."""
-
 import numpy as np
 from scipy.constants import mega, giga, parsec as parsec_m
 from scipy.constants import pi, c, hbar, G, k as k_B, e
 
-
 # reduced Planck units in SI
 mp_kg = np.sqrt(hbar * c / (8 * pi * G))
 tp_s = np.sqrt(8 * pi * G * hbar / c**5)
 lp_m = np.sqrt(8 * pi * G * hbar / c**3)
+Tp_K = np.sqrt(hbar * c**5 / (8 * pi * G * k_B**2))
 
 # reduced Planck units in GeV
 mp_GeV = mp_kg * c**2 / (giga * e)
 tp_iGeV = tp_s / hbar * giga * e
 lp_iGeV = lp_m / hbar / c * giga * e
 
 # other units
 Mpc_m = mega * parsec_m
 
 # derived constants
-a_B = 8. * pi**5 * k_B**4 / 15. / (2. * pi * hbar)**3 / c**3  # radiation constant (Planck's law)
+a_B = 8 * pi**5 * k_B**4 / 15 / (2 * pi * hbar)**3 / c**3  # radiation constant (Planck's law)
```

### Comparing `primpy-2.3.9/primpy.egg-info/PKG-INFO` & `primpy-2.7.8/primpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primpy
-Version: 2.3.9
+Version: 2.7.8
 Summary: primpy: Calculations for the primordial Universe.
 Author: Lukas Hergt
 Author-email: lh561@mrao.cam.ac.uk
 License: MIT
 Keywords: PPS,cosmic inflation,initial conditions for inflation,kinetic dominance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -14,21 +14,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyoscode
 
 ================================================
 primpy: calculations for the primordial Universe
 ================================================
 :primpy: calculations for the primordial Universe
 :Author: Lukas Hergt
-:Version: 2.3.9
+:Version: 2.7.8
 :Homepage: https://github.com/lukashergt/primpy
 :Documentation: https://primpy.readthedocs.io
 
 .. image:: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml/badge.svg?branch=master
     :target: https://github.com/lukashergt/primpy/actions/workflows/pythonpackage.yml
     :alt: Build Status
 .. image:: https://codecov.io/gh/lukashergt/primpy/branch/master/graph/badge.svg?token=USS4K53PY0
```

### Comparing `primpy-2.3.9/primpy.egg-info/SOURCES.txt` & `primpy-2.7.8/primpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/setup.py` & `primpy-2.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/tests/test_bigbang.py` & `primpy-2.7.8/tests/test_bigbang.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/tests/test_efolds_inflation.py` & `primpy-2.7.8/tests/test_efolds_inflation.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 def test_basic_methods(K):
     eq = InflationEquationsN(K=K, potential=QuadraticPotential(Lambda=1))
     assert hasattr(eq, 'phi')
     assert hasattr(eq, 'dphidN')
     y0 = np.zeros(len(eq.idx))
     assert eq.H2(x=0, y=y0) == -K
     y1 = np.ones(len(eq.idx))
-    H2 = (1 - 6 * K * np.exp(-2)) / 5
+    V = 1
+    H2 = (2 * V - 6 * K * np.exp(-2)) / 5
     assert eq.H2(x=1, y=y1) == H2
     assert eq.H(x=1, y=y1) == np.sqrt(H2)
-    assert eq.w(x=1, y=y1) == (H2 - 1) / (H2 + 1)
-    assert eq.inflating(x=1, y=y1) == 1 / 2 - H2
+    assert eq.w(x=1, y=y1) == (H2/2 - V) / (H2/2 + V)
+    assert eq.inflating(x=1, y=y1) == V - H2
```

### Comparing `primpy-2.3.9/tests/test_equations.py` & `primpy-2.7.8/tests/test_equations.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     eq = Equations()
     with pytest.raises(NotImplementedError, match="Equations class must define __call__."):
         eq(x=0, y=np.zeros(3))
 
 
 @pytest.mark.filterwarnings("ignore:invalid value encountered in sqrt:RuntimeWarning")
 @pytest.mark.parametrize('K', [-1, 0, +1])
-@pytest.mark.parametrize('phi_i, pot', [(17, QuadraticPotential(mass=6e-6)),
+@pytest.mark.parametrize('phi_i, pot', [(17, QuadraticPotential(Lambda=np.sqrt(6e-6))),
                                         (6, StarobinskyPotential(Lambda=5e-2))])
 def test_equations_sol_ordering_after_postprocessing(K, phi_i, pot):
     t_i = 7e4
     N_i = 12
     for eq in [InflationEquationsT(K=K, potential=pot),
                InflationEquationsN(K=K, potential=pot, track_time=True)]:
         # integration forwards in time:
```

### Comparing `primpy-2.3.9/tests/test_events.py` & `primpy-2.7.8/tests/test_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ev = Event(None)
     with pytest.raises(NotImplementedError, match="Event class must define __call__."):
         ev(x=0, y=np.zeros(3))
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 def test_UntilTEvent(K):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     t_i = 7e4
     N_i = 10
     phi_i = 17
     t_end = 1e6
     for eq in [InflationEquationsT(K=K, potential=pot),
                InflationEquationsN(K=K, potential=pot, track_time=True)]:
         ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
@@ -33,29 +33,29 @@
         assert sol.t[-1] == approx(t_end)
         assert sol.t_events['UntilT'][-1] == approx(t_end)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_UntilNEvent(K, Eq):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     t_i = 7e4
     N_i = 10
     phi_i = 17
     N_end = 73
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [UntilNEvent(eq, N_end)]
     sol = solve(ic=ic, events=ev)
     assert sol.N[-1] == approx(N_end)
     assert sol.N_events['UntilN'][-1] == approx(N_end)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
-@pytest.mark.parametrize('Lambda', [1, np.sqrt(6e-6)])
+@pytest.mark.parametrize('Lambda', [1, 0.0025])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_InflationEvent(K, Lambda, Eq):
     t_i = 7e4
     N_i = 10
     phi_i = 17
     pot = QuadraticPotential(Lambda=Lambda)
     eq = Eq(K=K, potential=pot)
@@ -69,15 +69,15 @@
     assert sol.w[-1] == approx(-1 / 3)
     assert np.all(sol.w[1:-1] < -1 / 3)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_AfterInflationEndEvent(K, Eq):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     t_i = 7e4
     N_i = 10
     phi_i = 17
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=False),
@@ -92,15 +92,15 @@
             sol.N_events['AfterInflationEnd_dir1_term1'][0])
 
 
 @pytest.mark.filterwarnings("ignore:invalid value encountered in sqrt:RuntimeWarning")
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_Phi0Event(K, Eq):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     t_i = 7e4
     N_i = 12
     phi_i = 17
     eq = Eq(K=K, potential=pot)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(eq, +1, terminal=False),
           InflationEvent(eq, -1, terminal=False),
```

### Comparing `primpy-2.3.9/tests/test_exceptionhandling.py` & `primpy-2.7.8/tests/test_exceptionhandling.py`

 * *Files identical despite different names*

### Comparing `primpy-2.3.9/tests/test_inflation.py` & `primpy-2.7.8/tests/test_inflation.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from primpy.time.inflation import InflationEquationsT
 from primpy.efolds.inflation import InflationEquationsN
 from primpy.initialconditions import InflationStartIC, ISIC_NsOk
 from primpy.solver import solve
 
 
 def test_not_implemented_errors():
-    eq = InflationEquations(K=1, potential=QuadraticPotential(Lambda=np.sqrt(6e-6)))
+    eq = InflationEquations(K=1, potential=QuadraticPotential(Lambda=0.0025))
     with pytest.raises(NotImplementedError, match="Equations must define H2 method."):
         eq.H(x=0, y=np.zeros(4))
     with pytest.raises(NotImplementedError, match="Equations must define H2 method."):
         eq.H2(x=0, y=np.zeros(4))
     with pytest.raises(NotImplementedError, match="Equations must define w method."):
         eq.w(x=0, y=np.zeros(4))
     with pytest.raises(NotImplementedError, match="Equations must define inflating method."):
@@ -59,15 +59,15 @@
 
 def test_basic_methods_time_vs_efolds():
     tol = 1e-12
     t = 1
     N = 10
     phi = 20
     for K in [-1, 0, 1]:
-        for Lambda in [1, np.sqrt(6e-6)]:
+        for Lambda in [1, 0.0025]:
             pot = QuadraticPotential(Lambda=Lambda)
             for dphidt_squared in [100 * pot.V(phi), 2 * pot.V(phi), pot.V(phi), pot.V(phi) / 100]:
                 dphidt = -np.sqrt(dphidt_squared)
                 eq_t = InflationEquationsT(K=K, potential=pot)
                 eq_N = InflationEquationsN(K=K, potential=pot)
                 assert eq_t.idx['phi'] == 0
                 assert eq_t.idx['dphidt'] == 1
@@ -83,15 +83,15 @@
                 assert eq_t.d2Vdphi2(t, y1_t) == approx(eq_N.d2Vdphi2(N, y1_N), rel=tol, abs=tol)
                 assert eq_t.w(t, y1_t) == approx(eq_N.w(N, y1_N), rel=tol, abs=tol)
                 assert eq_t.inflating(t, y1_t) == approx(eq_N.inflating(N, y1_N), rel=tol, abs=tol)
 
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 def test_sol_time_efolds(K):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     N_i = 10
     phi_i = 17
     t_i = 7e4
     eta_i = 0
     h = 0.7
     k = np.logspace(-3, 1, 4 * 10 + 1)
     Omega_K0 = -K * 0.01
@@ -100,17 +100,17 @@
     eq_N = InflationEquationsN(K=K, potential=pot, track_eta=True, track_time=True)
     ic_t = InflationStartIC(eq_t, N_i=N_i, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
     ic_N = InflationStartIC(eq_N, N_i=N_i, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
     ev_t = [InflationEvent(eq_t, +1, terminal=False),
             InflationEvent(eq_t, -1, terminal=True)]
     ev_N = [InflationEvent(eq_N, +1, terminal=False),
             InflationEvent(eq_N, -1, terminal=True)]
-    bist = solve(ic=ic_t, events=ev_t, dense_output=True)
-    bisn = solve(ic=ic_N, events=ev_N, dense_output=True)
-    assert bist.N_tot == approx(bisn.N_tot)
+    bist = solve(ic=ic_t, events=ev_t, dense_output=True, method='DOP853', rtol=1e-12)
+    bisn = solve(ic=ic_N, events=ev_N, dense_output=True, method='DOP853', rtol=1e-12)
+    assert bist.N_tot == approx(bisn.N_tot, rel=1e-5)
 
     N2t = interp1d(bisn.N, bisn.t, kind='cubic')
     N2phi = interp1d(bisn.N, bisn.phi, kind='cubic')
     N2H = interp1d(bisn.N, bisn.H, kind='cubic')
     assert_allclose(bist.t[1:-1], N2t(bist.N[1:-1]), rtol=1e-5)
     assert_allclose(bist.phi[1:-1], N2phi(bist.N[1:-1]), rtol=1e-4)
     assert_allclose(bist.H[1:-1], N2H(bist.N[1:-1]), rtol=1e-4)
@@ -131,17 +131,23 @@
         assert bisn.a0 == 1
         bist.derive_comoving_hubble_horizon(N_star=55)
         bisn.derive_comoving_hubble_horizon(N_star=55)
         bist.derive_approx_power(N_star=55)
         bisn.derive_approx_power(N_star=55)
     assert bist.N_star == approx(bisn.N_star, rel=1e-5)
     assert bist.N_dagg == approx(bisn.N_dagg, rel=1e-5)
+    assert bist.A_s == approx(bisn.A_s, rel=1e-8)
     assert bist.n_s == approx(bisn.n_s, rel=1e-5)
     assert bist.n_run == approx(bisn.n_run, rel=1e-3)
+    assert bist.n_runrun == approx(bisn.n_runrun, rel=2e-1, abs=1e-6)
+    assert bist.A_t == approx(bisn.A_t, rel=1e-8)
     assert bist.r == approx(bisn.r, rel=1e-5)
+    assert bist.n_t == approx(bisn.n_t, rel=1e-5)
+    assert_allclose(bist.logk2logP_s(np.log(k)), bisn.logk2logP_s(np.log(k)), rtol=1e-6)
+    assert_allclose(bist.logk2logP_t(np.log(k)), bisn.logk2logP_t(np.log(k)), rtol=1e-6)
     assert_allclose(bist.P_s_approx(k) * 1e9, bisn.P_s_approx(k) * 1e9, rtol=1e-4)
     assert_allclose(bist.P_t_approx(k) * 1e9, bisn.P_t_approx(k) * 1e9, rtol=1e-3)
 
 
 def nan_inflation_end(background_sol):
     assert not np.isfinite(background_sol.N_end)
     assert not np.isfinite(background_sol.phi_end)
@@ -152,15 +158,15 @@
 
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('Eq', [InflationEquationsT, InflationEquationsN])
 def test_postprocessing_inflation_end_warnings(K, Eq):
     t_i = 1e4
     N_i = 10
     phi_i = 17
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     eq = Eq(K=K, potential=pot, verbose=True)
 
     # stop at N=20 to trigger "Inflation has not ended." warning:
     ic_early_end = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     ev = [InflationEvent(ic_early_end.equations, +1, terminal=False),
           InflationEvent(ic_early_end.equations, -1, terminal=True),
           UntilNEvent(ic_early_end.equations, 20)]
@@ -174,39 +180,38 @@
                  UntilNEvent(ic.equations, N_i + 65)]
     with pytest.warns(InflationEndWarning, match="Not tracking"):
         bist = solve(ic=ic, events=ev_no_end)
     nan_inflation_end(background_sol=bist)
 
 
 def test_Ncross_nan():
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     N_i = 18
     phi_i = 15
     t_i = 7e4
     h = 0.7
     for K in [-1, +1]:
         for eq in [InflationEquationsT(K=K, potential=pot),
                    InflationEquationsN(K=K, potential=pot)]:
             Omega_K0 = -K * 0.1
             ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
             ev = [InflationEvent(eq, +1, terminal=False),
                   InflationEvent(eq, -1, terminal=True)]
             b_sol = solve(ic=ic, events=ev)
-            print(b_sol.N_tot)
             b_sol.derive_approx_power(Omega_K0=Omega_K0, h=h)
             assert np.log(K_STAR) < np.min(b_sol.logk)
             assert np.isnan(b_sol.N_cross)
             assert np.isnan(b_sol.N_star)
             assert np.isnan(b_sol.N_dagg)
 
 
 @pytest.mark.parametrize('N_star', [30, 90])
 def test_approx_As_ns_nrun_r__with_tolerances_and_slow_roll(N_star):
     K = +1
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     t_i = 1e4
     N_i = 10
     Omega_K0 = -K * 0.01
     h = 0.7
 
     rtols = np.array([1e-12, 2.4e-14])
     As_range = np.zeros(rtols.size)
@@ -216,15 +221,15 @@
 
     ns_slow_roll = 1 - 2 / N_star
     r_slow_roll = 8 / N_star
 
     for i, rtol in enumerate(rtols):
         eq = InflationEquationsT(K=K, potential=pot)
         ic = ISIC_NsOk(equations=eq, N_i=N_i, N_star=N_star, Omega_K0=Omega_K0, h=h, t_i=t_i,
-                       phi_i_bracket=[15.21, 30])
+                       phi_i_bracket=[12, 30])
         ev = [InflationEvent(ic.equations, +1, terminal=False),
               InflationEvent(ic.equations, -1, terminal=True)]
         bist = solve(ic=ic, events=ev, rtol=rtol)
         bist.derive_approx_power(Omega_K0=Omega_K0, h=h)
         n_s = bist.n_s
         r = bist.r
         assert np.isclose(bist.N_star, N_star)
```

### Comparing `primpy-2.3.9/tests/test_initialconditions.py` & `primpy-2.7.8/tests/test_initialconditions.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,45 +4,109 @@
 import numpy as np
 from primpy.exceptionhandling import InflationStartError
 from primpy.potentials import QuadraticPotential, StarobinskyPotential
 from primpy.events import InflationEvent
 from primpy.inflation import InflationEquations
 from primpy.time.inflation import InflationEquationsT
 from primpy.efolds.inflation import InflationEquationsN
-from primpy.initialconditions import InflationStartIC, ISIC_Nt, ISIC_NsOk
+from primpy.initialconditions import SlowRollIC, InflationStartIC, ISIC_Nt, ISIC_NsOk
 from primpy.solver import solve
 
 
 def basic_ic_asserts(y0, ic, K, pot, N_i, Omega_Ki, phi_i, t_i):
     assert ic.N_i == N_i
     assert ic.Omega_Ki == Omega_Ki
     assert ic.phi_i == phi_i
-    assert ic.eta_i is None
     assert y0[0] == ic.phi_i
     if isinstance(ic.equations, InflationEquationsT):
         assert y0.size == 3
         assert ic.x_ini == t_i
         assert ic.t_i == t_i
-        assert ic.dphidt_i == -np.sqrt(ic.V_i)
         assert y0[1] == ic.dphidt_i
         assert y0[2] == ic.N_i
     elif isinstance(ic.equations, InflationEquationsN):
         assert y0.size == 2
         assert ic.t_i is None
         assert ic.x_ini == N_i
-        assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
         assert y0[1] == ic.dphidN_i
     assert ic.equations.K == K
     assert ic.equations.potential.V(phi_i) == pot.V(phi_i)
     assert ic.equations.potential.dV(phi_i) == pot.dV(phi_i)
     assert ic.equations.potential.d2V(phi_i) == pot.d2V(phi_i)
     assert ic.equations.potential.d3V(phi_i) == pot.d3V(phi_i)
 
 
-@pytest.mark.parametrize('pot', [QuadraticPotential(Lambda=np.sqrt(6e-6)),
+@pytest.mark.parametrize('pot', [QuadraticPotential(Lambda=0.0025),
+                                 StarobinskyPotential(Lambda=5e-2)])
+@pytest.mark.parametrize('K', [-1, 0, +1])
+@pytest.mark.parametrize('t_i, Eq', [(1e4, InflationEquationsT), (None, InflationEquationsN)])
+def test_SlowRollIC(pot, K, t_i, Eq):
+    phi_i = 17
+
+    # for N_i:
+    N_i = 12
+    eq = Eq(K=K, potential=pot)
+    with pytest.raises(TypeError, match="Need to specify either N_i xor Omega_Ki."):
+        SlowRollIC(equations=eq, phi_i=phi_i, t_i=t_i)
+    ic = SlowRollIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
+    y0 = np.zeros(len(ic.equations.idx))
+    ic(y0)
+    basic_ic_asserts(y0, ic, K, pot, N_i, ic.Omega_Ki, phi_i, t_i)
+
+    # for Omega_Ki:
+    if K != 0:
+        with pytest.raises(Exception, match="Primordial curvature for open universes"):
+            SlowRollIC(equations=eq, Omega_Ki=1, phi_i=phi_i, t_i=t_i)
+        Omega_Ki = -K * 0.9
+        ic = SlowRollIC(equations=eq, Omega_Ki=Omega_Ki, phi_i=phi_i, t_i=t_i)
+        y0 = np.zeros(len(ic.equations.idx))
+        ic(y0)
+        basic_ic_asserts(y0, ic, K, pot, ic.N_i, Omega_Ki, phi_i, t_i)
+
+
+def test_SlowRollIC_track():
+    t_i = 1e4
+    eta_i = 0
+    phi_i = 17
+    N_i = 12
+    K = 0
+    pot = StarobinskyPotential(Lambda=5e-2)
+    eq = InflationEquationsN(K=K, potential=pot, track_time=True, track_eta=True)
+    ic = SlowRollIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i, eta_i=eta_i)
+    y0 = np.zeros(len(ic.equations.idx))
+    ic(y0)
+    assert ic.N_i == N_i
+    assert ic.phi_i == phi_i
+    assert ic.t_i == t_i
+    assert ic.eta_i == eta_i
+    assert ic.x_ini == N_i
+    assert ic.equations.K == K
+    assert y0.size == 4
+    assert y0[0] == ic.phi_i
+    assert y0[1] == ic.dphidN_i
+    assert y0[2] == ic.t_i
+    assert y0[3] == ic.eta_i
+
+
+def test_SlowRollIC_failures():
+    with pytest.raises(InflationStartError, match="V_i / 3"):
+        pot = StarobinskyPotential(Lambda=5e-2)
+        eq = InflationEquationsT(K=1, potential=pot)
+        ic = SlowRollIC(equations=eq, N_i=0, phi_i=17)
+        y0 = np.zeros(len(ic.equations.idx))
+        ic(y0)
+    with pytest.raises(NotImplementedError, match="`equations`"):
+        pot = StarobinskyPotential(Lambda=5e-2)
+        eq = InflationEquations(K=0, potential=pot)
+        ic = SlowRollIC(equations=eq, N_i=0, phi_i=17)
+        y0 = np.zeros(len(ic.equations.idx))
+        ic(y0)
+
+
+@pytest.mark.parametrize('pot', [QuadraticPotential(Lambda=0.0025),
                                  StarobinskyPotential(Lambda=5e-2)])
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('t_i, Eq', [(1e4, InflationEquationsT), (None, InflationEquationsN)])
 def test_InflationStartIC(pot, K, t_i, Eq):
     phi_i = 17
 
     # for N_i:
@@ -55,40 +119,52 @@
     eq = Eq(K=K, potential=pot)
     with pytest.raises(TypeError, match="Need to specify either N_i or Omega_Ki."):
         InflationStartIC(equations=eq, phi_i=phi_i, t_i=t_i)
     ic = InflationStartIC(equations=eq, N_i=N_i, phi_i=phi_i, t_i=t_i)
     y0 = np.zeros(len(ic.equations.idx))
     ic(y0)
     basic_ic_asserts(y0, ic, K, pot, N_i, ic.Omega_Ki, phi_i, t_i)
+    if isinstance(ic.equations, InflationEquationsT):
+        assert ic.dphidt_i == -np.sqrt(ic.V_i)
+    elif isinstance(ic.equations, InflationEquationsN):
+        assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
 
     # for Omega_Ki:
     if K != 0:
         abs_Omega_Ki = 0.9
         Omega_Ki = -K * abs_Omega_Ki
         eq = Eq(K=K, potential=pot)
         ic = InflationStartIC(equations=eq, Omega_Ki=Omega_Ki, phi_i=phi_i, t_i=t_i)
         y0 = np.zeros(len(ic.equations.idx))
         ic(y0)
         basic_ic_asserts(y0, ic, K, pot, ic.N_i, Omega_Ki, phi_i, t_i)
+        if isinstance(ic.equations, InflationEquationsT):
+            assert ic.dphidt_i == -np.sqrt(ic.V_i)
+        elif isinstance(ic.equations, InflationEquationsN):
+            assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
         with pytest.raises(Exception, match="Primordial curvature for open universes"):
             InflationStartIC(equations=eq, Omega_Ki=1, phi_i=phi_i, t_i=t_i)
 
 
 # noinspection DuplicatedCode
 @pytest.mark.parametrize('K', [-1, 0, +1])
 @pytest.mark.parametrize('t_i, Eq', [(1e4, InflationEquationsT), (None, InflationEquationsN)])
 def test_ISIC_Nt_Ni(K, t_i, Eq):
     N_i = 11
     N_tot = 60
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     eq = Eq(K=K, potential=pot)
     ic = ISIC_Nt(equations=eq, N_i=N_i, N_tot=N_tot, t_i=t_i, phi_i_bracket=[3, 30])
     y0 = np.zeros(len(ic.equations.idx))
     ic(y0)
     basic_ic_asserts(y0, ic, K, pot, N_i, ic.Omega_Ki, ic.phi_i, t_i)
+    if isinstance(ic.equations, InflationEquationsT):
+        assert ic.dphidt_i == -np.sqrt(ic.V_i)
+    elif isinstance(ic.equations, InflationEquationsN):
+        assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
     assert ic.N_tot == N_tot
     ev = [InflationEvent(ic.equations, +1, terminal=False),
           InflationEvent(ic.equations, -1, terminal=True)]
     if isinstance(eq, InflationEquationsT):
         bist = solve(ic=ic, events=ev)
         assert pytest.approx(bist.N_tot) == N_tot
     elif isinstance(eq, InflationEquationsN):
@@ -99,24 +175,28 @@
 # noinspection DuplicatedCode
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('abs_Omega_Ki', [0.9, 10])
 @pytest.mark.parametrize('t_i, Eq', [(1e4, InflationEquationsT), (None, InflationEquationsN)])
 def test_ISIC_Nt_Oi(K, abs_Omega_Ki, t_i, Eq):
     Omega_Ki = -K * abs_Omega_Ki
     N_tot = 60
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     eq = Eq(K=K, potential=pot)
     if Omega_Ki >= 1:
         with pytest.raises(InflationStartError):
             ISIC_Nt(eq, Omega_Ki=Omega_Ki, N_tot=N_tot, t_i=t_i, phi_i_bracket=[3, 30])
     else:
         ic = ISIC_Nt(eq, Omega_Ki=Omega_Ki, N_tot=N_tot, t_i=t_i, phi_i_bracket=[3, 30])
         y0 = np.zeros(len(ic.equations.idx))
         ic(y0)
         basic_ic_asserts(y0, ic, K, pot, ic.N_i, Omega_Ki, ic.phi_i, t_i)
+        if isinstance(ic.equations, InflationEquationsT):
+            assert ic.dphidt_i == -np.sqrt(ic.V_i)
+        elif isinstance(ic.equations, InflationEquationsN):
+            assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
         assert ic.N_tot == N_tot
         ev = [InflationEvent(ic.equations, +1, terminal=False),
               InflationEvent(ic.equations, -1, terminal=True)]
         if isinstance(eq, InflationEquationsT):
             bist = solve(ic=ic, events=ev)
             assert pytest.approx(bist.N_tot) == N_tot
         elif isinstance(eq, InflationEquationsN):
@@ -124,27 +204,31 @@
             assert pytest.approx(bisn.N_tot, rel=1e-6, abs=1e-6) == N_tot
 
 
 # noinspection DuplicatedCode
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('t_i, Eq', [(1e4, InflationEquationsT), (None, InflationEquationsN)])
 def test_ISIC_NsOk(K, t_i, Eq):
-    pot = QuadraticPotential(Lambda=np.sqrt(6e-6))
+    pot = QuadraticPotential(Lambda=0.0025)
     N_star = 55
     h = 0.7
 
     # for N_i:
     N_i = 11
     Omega_K0 = -K * 0.01
     eq = Eq(K=K, potential=pot)
     ic = ISIC_NsOk(equations=eq, N_i=N_i, N_star=N_star, Omega_K0=Omega_K0, h=h, t_i=t_i,
-                   phi_i_bracket=[15, 30], verbose=True)
+                   phi_i_bracket=[15, 30], verbose=False)
     y0 = np.zeros(len(ic.equations.idx))
     ic(y0)
     basic_ic_asserts(y0, ic, K, pot, N_i, ic.Omega_Ki, ic.phi_i, t_i)
+    if isinstance(ic.equations, InflationEquationsT):
+        assert ic.dphidt_i == -np.sqrt(ic.V_i)
+    elif isinstance(ic.equations, InflationEquationsN):
+        assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
     assert ic.N_star == N_star
     assert ic.Omega_K0 == Omega_K0
     assert ic.h == h
     ev = [InflationEvent(ic.equations, +1, terminal=False),
           InflationEvent(ic.equations, -1, terminal=True)]
     b = solve(ic=ic, events=ev)
     b.derive_approx_power(Omega_K0=Omega_K0, h=h)
@@ -157,14 +241,18 @@
     Omega_K0 = -K * 0.01
     eq = Eq(K=K, potential=pot)
     ic = ISIC_NsOk(equations=eq, Omega_Ki=Omega_Ki, N_star=N_star, Omega_K0=Omega_K0, h=h, t_i=t_i,
                    phi_i_bracket=[15, 30])
     y0 = np.zeros(len(ic.equations.idx))
     ic(y0)
     basic_ic_asserts(y0, ic, K, pot, ic.N_i, Omega_Ki, ic.phi_i, t_i)
+    if isinstance(ic.equations, InflationEquationsT):
+        assert ic.dphidt_i == -np.sqrt(ic.V_i)
+    elif isinstance(ic.equations, InflationEquationsN):
+        assert ic.dphidN_i == -np.sqrt(ic.V_i) / ic.H_i
     assert ic.N_star == N_star
     assert ic.Omega_K0 == Omega_K0
     assert ic.h == h
     ev = [InflationEvent(ic.equations, +1, terminal=False),
           InflationEvent(ic.equations, -1, terminal=True)]
     b = solve(ic=ic, events=ev)
     b.derive_approx_power(Omega_K0=Omega_K0, h=h)
```

### Comparing `primpy-2.3.9/tests/test_perturbations.py` & `primpy-2.7.8/tests/test_perturbations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,95 @@
 #!/usr/bin/env python
 """Tests for `primpy.perturbation` module."""
 import pytest
 from pytest import approx
-# import itertools
 import numpy as np
 from numpy.testing import assert_allclose
-from primpy.potentials import QuadraticPotential
+from primpy.potentials import QuadraticPotential, StarobinskyPotential
 from primpy.events import InflationEvent, CollapseEvent
 from primpy.time.inflation import InflationEquationsT
 from primpy.efolds.inflation import InflationEquationsN
-from primpy.initialconditions import InflationStartIC
+from primpy.initialconditions import InflationStartIC, SlowRollIC
 from primpy.time.perturbations import PerturbationT
 from primpy.efolds.perturbations import PerturbationN
 from primpy.solver import solve
 from primpy.oscode_solver import solve_oscode
 
 
-def setup_background(K, f_i, abs_Omega_K0):
-    pot = QuadraticPotential(mass=6e-6)
+def set_background_SR():
+    pot = StarobinskyPotential(Lambda=3.3e-3)
+    N_i = 0
+    phi_i = 5.6
+    Omega_K0 = 0
+    h = 0.7
+    N_star = 55
+
+    eq_t = InflationEquationsT(K=0, potential=pot)
+    eq_n = InflationEquationsN(K=0, potential=pot)
+    t_eval = np.logspace(np.log10(5e4), np.log10(2e7), int(1e5))
+    ic_t = SlowRollIC(eq_t, N_i=N_i, phi_i=phi_i, t_i=t_eval[0])
+    ic_n = SlowRollIC(eq_n, N_i=N_i, phi_i=phi_i, t_i=None)
+    N_eval = np.linspace(ic_n.N_i, 70, int(1e5))
+    ev_t = [InflationEvent(eq_t, +1, terminal=False),
+            InflationEvent(eq_t, -1, terminal=True),
+            CollapseEvent(eq_t)]
+    ev_n = [InflationEvent(eq_n, +1, terminal=False),
+            InflationEvent(eq_n, -1, terminal=True),
+            CollapseEvent(eq_n)]
+    bsrt = solve(ic=ic_t, events=ev_t, t_eval=t_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bsrn = solve(ic=ic_n, events=ev_n, t_eval=N_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bsrt.derive_a0(Omega_K0=Omega_K0, h=h)
+    bsrn.derive_a0(Omega_K0=Omega_K0, h=h)
+    bsrt.derive_approx_power(N_star=N_star)
+    bsrn.derive_approx_power(N_star=N_star)
+
+    return bsrt, bsrn
+
+
+def test_set_background_SR():
+    bsrt, bsrn = set_background_SR()
+    assert bsrt.independent_variable == 't'
+    assert bsrn.independent_variable == 'N'
+    assert bsrt.N_tot > bsrt.N_star + 10
+    assert bsrt.N_tot == approx(bsrn.N_tot)
+    assert bsrt.N_star == approx(bsrn.N_star)
+    assert bsrt.N_cross == approx(bsrn.N_cross, rel=1e-5)
+
+
+def test_perturbations_SR():
+    bsrt, bsrn = set_background_SR()
+    ks_iMpc = np.logspace(np.log10(5e-4), np.log10(5e0), 4 * 10 + 1)
+    logk_iMpc = np.log(ks_iMpc)
+    ks_cont = ks_iMpc * bsrt.a0_Mpc
+    pps_t = solve_oscode(background=bsrt, k=ks_cont, fac_beg=100, rtol=5e-5)
+    pps_n = solve_oscode(background=bsrn, k=ks_cont, fac_beg=100, rtol=5e-5, even_grid=True)
+    assert np.isfinite(pps_t.P_s_RST).all()
+    assert np.isfinite(pps_t.P_t_RST).all()
+    assert np.isfinite(pps_n.P_s_RST).all()
+    assert np.isfinite(pps_n.P_t_RST).all()
+
+    # time vs efolds
+    assert_allclose(pps_t.P_s_RST * 1e9, pps_n.P_s_RST * 1e9, rtol=1e-3, atol=1e-6)
+    assert_allclose(pps_t.P_t_RST * 1e9, pps_n.P_t_RST * 1e9, rtol=1e-3, atol=1e-6)
+
+    # oscode vs background
+    As_t_oscode = pps_t.P_s_RST[ks_iMpc.size//2]
+    As_n_oscode = pps_n.P_s_RST[ks_iMpc.size//2]
+    assert As_t_oscode == approx(bsrt.A_s, rel=5e-2)
+    assert As_n_oscode == approx(bsrn.A_s, rel=5e-2)
+    offt = bsrt.A_s / As_t_oscode
+    offn = bsrn.A_s / As_n_oscode
+    assert_allclose(np.log(pps_t.P_s_RST*offt), bsrt.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_n.P_s_RST*offn), bsrn.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_t.P_t_RST), bsrt.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-6)
+    assert_allclose(np.log(pps_n.P_t_RST), bsrn.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-6)
+
+
+def set_background_IS(K, f_i, abs_Omega_K0):
+    pot = QuadraticPotential(Lambda=0.0025)
     phi_i = 16
     Omega_K0 = -K * abs_Omega_K0
     Omega_Ki = f_i * Omega_K0
     h = 0.7
 
     eq_t = InflationEquationsT(K=K, potential=pot)
     eq_n = InflationEquationsN(K=K, potential=pot)
@@ -31,16 +99,16 @@
     N_eval = np.linspace(ic_n.N_i, 70, int(1e5))
     ev_t = [InflationEvent(eq_t, +1, terminal=False),
             InflationEvent(eq_t, -1, terminal=True),
             CollapseEvent(eq_t)]
     ev_n = [InflationEvent(eq_n, +1, terminal=False),
             InflationEvent(eq_n, -1, terminal=True),
             CollapseEvent(eq_n)]
-    bist = solve(ic=ic_t, events=ev_t, t_eval=t_eval)
-    bisn = solve(ic=ic_n, events=ev_n, t_eval=N_eval, rtol=1e-12, atol=1e-12)
+    bist = solve(ic=ic_t, events=ev_t, t_eval=t_eval, method='DOP853', rtol=1e-12, atol=1e-13)
+    bisn = solve(ic=ic_n, events=ev_n, t_eval=N_eval, method='DOP853', rtol=1e-12, atol=1e-13)
     assert bist.independent_variable == 't'
     assert bisn.independent_variable == 'N'
     assert bist.N_tot == approx(bisn.N_tot)
     bist.derive_a0(Omega_K0=Omega_K0, h=h)
     bisn.derive_a0(Omega_K0=Omega_K0, h=h)
     assert bist.a0_Mpc == approx(bisn.a0_Mpc)
     bist.derive_approx_power(Omega_K0=Omega_K0, h=h)
@@ -49,33 +117,33 @@
 
     return bist, bisn
 
 
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('f_i', [10, 100])
 @pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
-def test_background_setup(K, f_i, abs_Omega_K0):
+def test_set_background_IS(K, f_i, abs_Omega_K0):
     if -K * f_i * abs_Omega_K0 >= 1:
         with pytest.raises(Exception):
-            setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
     else:
-        setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
 
 
 # noinspection DuplicatedCode
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('f_i', [10, 100])
 @pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
-@pytest.mark.parametrize('k_iMpc', np.logspace(-6, 0, 6 + 1))
+@pytest.mark.parametrize('k_iMpc', np.logspace(-5, 0, 5 + 1))
 def test_perturbations_frequency_damping(K, f_i, abs_Omega_K0, k_iMpc):
     if -K * f_i * abs_Omega_K0 >= 1:
         with pytest.raises(Exception):
-            setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
     else:
-        bist, bisn = setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
         k = k_iMpc * bist.a0_Mpc
         pert_t = PerturbationT(background=bist, k=k)
         pert_n = PerturbationN(background=bisn, k=k)
         assert pert_t.scalar.idx['Rk'] == 0
         assert pert_n.scalar.idx['Rk'] == 0
         assert pert_t.scalar.idx['dRk'] == 1
         assert pert_n.scalar.idx['dRk'] == 1
@@ -100,60 +168,54 @@
         freq_t, damp_t = pert_t.tensor.mukhanov_sasaki_frequency_damping()
         freq_n, damp_n = pert_n.tensor.mukhanov_sasaki_frequency_damping()
         assert np.all(freq_t > 0)
         assert np.all(freq_n > 0)
         assert np.isfinite(damp_t).all()
         assert np.isfinite(damp_n).all()
 
-        pert_t = solve_oscode(background=bist, k=k, rtol=1e-5)
-        pert_n = solve_oscode(background=bisn, k=k, rtol=1e-5, even_grid=True)
+        pert_t = solve_oscode(background=bist, k=k, rtol=5e-5)
+        pert_n = solve_oscode(background=bisn, k=k, rtol=5e-5, even_grid=True)
         for sol in ['one', 'two']:
             assert np.all(np.isfinite(getattr(getattr(pert_t.scalar, sol), 't')))
             assert np.all(np.isfinite(getattr(getattr(pert_n.scalar, sol), 'N')))
             assert np.all(np.isfinite(getattr(getattr(pert_t.tensor, sol), 't')))
             assert np.all(np.isfinite(getattr(getattr(pert_n.tensor, sol), 'N')))
-            # for scalar, a in itertools.product([pert_t.scalar, pert_n.scalar],
-            #                                    ['Rk', 'dRk', 'steptype']):
-            #     assert np.all(np.isfinite(getattr(getattr(scalar, sol), a)))
-            # for tensor, a in itertools.product([pert_t.tensor, pert_n.tensor],
-            #                                    ['hk', 'dhk', 'steptype']):
-            #     assert np.all(np.isfinite(getattr(getattr(tensor, sol), a)))
-        assert pert_n.scalar.P_s_RST == approx(pert_t.scalar.P_s_RST, rel=1e-3)
-        assert pert_n.tensor.P_t_RST == approx(pert_t.tensor.P_t_RST, rel=1e-3)
+        assert pert_n.scalar.P_s_RST == approx(pert_t.scalar.P_s_RST, rel=2e-3)
+        assert pert_n.tensor.P_t_RST == approx(pert_t.tensor.P_t_RST, rel=2e-3)
 
 
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('f_i', [10])
 @pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
 def test_perturbations_discrete_time_efolds(K, f_i, abs_Omega_K0):
     if -K * f_i * abs_Omega_K0 >= 1:
         with pytest.raises(Exception):
-            setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
     else:
-        bist, bisn = setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
         ks_disc = np.arange(1, 100, 1)
-        pps_t = solve_oscode(background=bist, k=ks_disc, rtol=1e-5)
-        pps_n = solve_oscode(background=bisn, k=ks_disc, rtol=1e-5, even_grid=True)
+        pps_t = solve_oscode(background=bist, k=ks_disc, rtol=5e-5)
+        pps_n = solve_oscode(background=bisn, k=ks_disc, rtol=5e-5, even_grid=True)
         assert np.isfinite(pps_t.P_s_RST).all()
         assert np.isfinite(pps_t.P_t_RST).all()
         assert np.isfinite(pps_n.P_s_RST).all()
         assert np.isfinite(pps_n.P_t_RST).all()
-        assert_allclose(pps_t.P_s_RST * 1e9, pps_n.P_s_RST * 1e9, rtol=1e-3, atol=1e-6)
-        assert_allclose(pps_t.P_t_RST * 1e9, pps_n.P_t_RST * 1e9, rtol=1e-3, atol=1e-6)
+        assert_allclose(np.log(pps_t.P_s_RST), np.log(pps_n.P_s_RST), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_t.P_t_RST), np.log(pps_n.P_t_RST), rtol=1e-3, atol=1e-8)
 
 
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('f_i', [10])
 @pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
 def test_perturbations_continuous_time_vs_efolds(K, f_i, abs_Omega_K0):
     if -K * f_i * abs_Omega_K0 >= 1:
         with pytest.raises(Exception):
-            setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
     else:
-        bist, bisn = setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
         ks_iMpc = np.logspace(-4, 0, 4 * 10 + 1)
         ks_cont = ks_iMpc * bist.a0_Mpc
         pps_t = solve_oscode(background=bist, k=ks_cont, rtol=1e-5)
         pps_n = solve_oscode(background=bisn, k=ks_cont, rtol=1e-5, even_grid=True)
         assert np.isfinite(pps_t.P_s_RST).all()
         assert np.isfinite(pps_t.P_t_RST).all()
         assert np.isfinite(pps_n.P_s_RST).all()
@@ -164,22 +226,23 @@
 
 @pytest.mark.parametrize('K', [-1, +1])
 @pytest.mark.parametrize('f_i', [10])
 @pytest.mark.parametrize('abs_Omega_K0', [0.09, 0.009])
 def test_perturbations_large_scales_pyoscode_vs_background(K, f_i, abs_Omega_K0):
     if -K * f_i * abs_Omega_K0 >= 1:
         with pytest.raises(Exception):
-            setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+            set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
     else:
-        bist, bisn = setup_background(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
+        bist, bisn = set_background_IS(K=K, f_i=f_i, abs_Omega_K0=abs_Omega_K0)
         ks_iMpc = np.logspace(-1, 1, 100)
+        logk_iMpc = np.log(ks_iMpc)
         ks_cont = ks_iMpc * bist.a0_Mpc
         pps_t = solve_oscode(background=bist, k=ks_cont)
         pps_n = solve_oscode(background=bisn, k=ks_cont, even_grid=True)
         assert np.isfinite(pps_t.P_s_RST).all()
         assert np.isfinite(pps_t.P_t_RST).all()
         assert np.isfinite(pps_n.P_s_RST).all()
         assert np.isfinite(pps_n.P_t_RST).all()
-        assert_allclose(pps_t.P_s_RST * 1e9, bist.P_s_approx(ks_iMpc) * 1e9, rtol=0.02, atol=1e-6)
-        assert_allclose(pps_t.P_t_RST * 1e9, bist.P_t_approx(ks_iMpc) * 1e9, rtol=0.02, atol=1e-6)
-        assert_allclose(pps_n.P_s_RST * 1e9, bisn.P_s_approx(ks_iMpc) * 1e9, rtol=0.02, atol=1e-6)
-        assert_allclose(pps_n.P_t_RST * 1e9, bisn.P_t_approx(ks_iMpc) * 1e9, rtol=0.02, atol=1e-6)
+        assert_allclose(np.log(pps_t.P_s_RST), bist.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_t.P_t_RST), bist.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_n.P_s_RST), bisn.logk2logP_s(logk_iMpc), rtol=1e-3, atol=1e-8)
+        assert_allclose(np.log(pps_n.P_t_RST), bisn.logk2logP_t(logk_iMpc), rtol=1e-3, atol=1e-8)
```

### Comparing `primpy-2.3.9/tests/test_time_inflation.py` & `primpy-2.7.8/tests/test_time_inflation.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 def test_basic_methods(K):
     eq = InflationEquationsT(K=K, potential=QuadraticPotential(Lambda=1))
     assert hasattr(eq, 'phi')
     assert hasattr(eq, 'dphidt')
     y0 = np.zeros(len(eq.idx))
     assert eq.H2(x=0, y=y0) == -K
     y1 = np.ones(len(eq.idx))
-    assert eq.H2(x=1, y=y1) == 1 / 3 - K * np.exp(-2)
-    assert eq.H(x=1, y=y1) == np.sqrt(1 / 3 - K * np.exp(-2))
-    assert eq.w(x=1, y=y1) == 0
-    assert eq.inflating(x=1, y=y1) == -0.5
+    V = 1
+    H2 = (1 / 2 + V) / 3 - K * np.exp(-2)
+    assert eq.H2(x=1, y=y1) == H2
+    assert eq.H(x=1, y=y1) == np.sqrt(H2)
+    assert eq.w(x=1, y=y1) == (1/2 - V) / (1/2 + V)
+    assert eq.inflating(x=1, y=y1) == V - 1
```

### Comparing `primpy-2.3.9/tests/test_version.py` & `primpy-2.7.8/tests/test_version.py`

 * *Files identical despite different names*

