# Comparing `tmp/solartoolbox-0.3.5.tar.gz` & `tmp/solartoolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solartoolbox-0.3.5.tar", last modified: Mon Dec 18 21:05:57 2023, max compression
+gzip compressed data, was "solartoolbox-0.4.0.tar", last modified: Wed Apr 10 20:59:26 2024, max compression
```

## Comparing `solartoolbox-0.3.5.tar` & `solartoolbox-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.487902 solartoolbox-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/src/solartoolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/cmv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/src/solartoolbox/dataio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/dataio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/dataio/hope_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/dataio/iotools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/dataio/nrcan_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)    33802 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/signalproc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    12883 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/src/solartoolbox/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/src/solartoolbox/visualization/vis_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/src/solartoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2023-12-18 21:05:57.000000 solartoolbox-0.3.5/src/solartoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-18 21:05:57.000000 solartoolbox-0.3.5/src/solartoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 21:05:57.000000 solartoolbox-0.3.5/src/solartoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-18 21:05:57.000000 solartoolbox-0.3.5/src/solartoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-18 21:05:57.000000 solartoolbox-0.3.5/src/solartoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 21:05:57.491902 solartoolbox-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_cmv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_signalproc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15046 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2023-12-18 21:05:49.000000 solartoolbox-0.3.5/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10295 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.409691 solartoolbox-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.409691 solartoolbox-0.4.0/src/solartoolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21734 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/cmv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/src/solartoolbox/dataio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/dataio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/dataio/hope_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/dataio/iotools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/dataio/nrcan_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34216 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/signalproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/src/solartoolbox/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/src/solartoolbox/visualization/vis_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/src/solartoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-10 20:59:26.000000 solartoolbox-0.4.0/src/solartoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 20:59:26.000000 solartoolbox-0.4.0/src/solartoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:59:26.000000 solartoolbox-0.4.0/src/solartoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 20:59:26.000000 solartoolbox-0.4.0/src/solartoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 20:59:26.000000 solartoolbox-0.4.0/src/solartoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:59:26.413691 solartoolbox-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_cmv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_signalproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-10 20:59:21.000000 solartoolbox-0.4.0/tests/test_stats.py
```

### Comparing `solartoolbox-0.3.5/LICENSE` & `solartoolbox-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Joe Ranalli
+Copyright (c) 2021-2024, Joe Ranalli
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `solartoolbox-0.3.5/setup.py` & `solartoolbox-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-ver = '0.3.5'
+ver = '0.4.0'
 
 
 setup(
     name='solartoolbox',
     version=ver,
     author="Joe Ranalli",
     author_email="jranalli@psu.edu",
```

### Comparing `solartoolbox-0.3.5/src/solartoolbox/cmv.py` & `solartoolbox-0.4.0/src/solartoolbox/cmv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import numpy as np
 from scipy.optimize import minimize_scalar, leastsq
 
 from solartoolbox.signalproc import compute_delays
 from solartoolbox.spatial import project_vectors, compute_vectors
-from solartoolbox.spatial import pol2rect, magnitude
+from solartoolbox.spatial import pol2rect, magnitude, dot
+
+from scipy.optimize import linear_sum_assignment, shgo
+from scipy.stats import linregress
 
 from enum import Enum
 import itertools
 
 
 class Flag(Enum):
     GOOD = 0
@@ -216,15 +219,15 @@
     # Pairwise QC
     pair_flags, method_out = _pairwise_qc(pairs, magnitude(vectors_cart.T),
                                           [A, B], delay, corr_lag, corr_mean,
                                           method, options)
 
     # Perform the Gagne QC, which looks for correlation on the whole set to
     # decide which pairs are worth using
-    overall_flag = None
+    overall_flag = Flag.GOOD
     if method == 'gagne':
         corr_inds = corr_lag >= 0.99
         if sum(corr_inds[pair_flags == Flag.GOOD]) < 12:
             corr_inds = corr_lag >= 0.95
         if sum(corr_inds[pair_flags == Flag.GOOD]) < 12:
             corr_inds = corr_lag >= 0.9
         if sum(corr_inds[pair_flags == Flag.GOOD]) < 12:
@@ -281,14 +284,25 @@
             overall_flag = Flag.TREND
 
         method_out['v60'] = v60
         method_out['v40'] = v40
         method_out['error_index'] = err
         method_out['velocity'] = velocity
 
+        # Compute a few extra statistics for the good pairs
+        try:
+            _, _, r_corr, _, std_err = linregress(delay_good, cmv_dir_dist)
+        except ValueError:
+            r_corr = 0
+            std_err = 0
+        ngood = len(vectors_good)
+        method_out['r_corr'] = r_corr
+        method_out['stderr_corr'] = std_err
+        method_out['ngood'] = ngood
+
     elif method == 'gagne':
         # Function to apply least squares to
         def resid(p, lag, coeff_vecs):
             dx, dy = coeff_vecs[:, 0], coeff_vecs[:, 1]
             ax, ay = p[0], p[1]
             # Residual as defined in Gagne 2018 equation 3
             return lag - (dx * ax + dy * ay)
@@ -325,14 +339,104 @@
     outdata.wind_angle = cmv_theta
     outdata.wind_speed = cmv_vel
     outdata.method_data = method_out
 
     return cmv_vel, cmv_theta, outdata
 
 
+def optimum_subset(cmvx, cmvy, n=10):
+    """
+    Chooses a subset of vectors from within a full set of vectors, based on
+    optimizing the most diverse angles available. Operates in 2 quadrants only,
+    subject to the assumption that anti-parallels are also undesirable.
+
+    This is useful for getting vectors that represent a variety of directions.
+    For example, given all the CMVs for a whole year, this will provide a list
+    of the time periods with the most varied cloud motion directions. One use
+    case is in field analysis where the most diverse set of CMVs is needed to
+    get the highest probability of perpendicular vector pairs.
+
+    Parameters
+    ----------
+    cmvx : pd.Series
+        A list of x-components of the CMVs
+
+    cmvy : pd.Series
+        A list of y-components of the CMVs
+
+    n : int
+        The number of vectors to select
+
+    Returns
+    -------
+    indices : list
+        The indices of the CMVs that are most diverse. Indices are positional
+        within the input arrays. For example, could be used to reduce a
+        DataFrame to the most diverse CMVs by using df.iloc[indices]
+    """
+
+    # Compute unit vectors representing the CMVs
+    cld_spd = []
+    for x, y in zip(cmvx, cmvy):
+        cld_spd.append(magnitude((x, y)))
+    cld_spd = np.array(cld_spd)
+    cmv_x = cmvx / cld_spd
+    cmv_y = cmvy / cld_spd
+    cmv_vecs = np.array([cmv_x, cmv_y]).T
+
+    def calc_cost(ang_0):
+        """
+        Compute the cost function associated with using each CMV as a member of
+        the set relative to the ideal set of equally spaced vectors.
+
+        Parameters
+        ----------
+        ang_0 : the rotation angle of the ideal vectors in radians
+
+        Returns
+        -------
+        cost : the total cost of the assignment
+        indices : the indices of the CMVs in the optimal assignment
+        """
+        # Compute unit vectors equally distributed around 180 deg.
+        ideal_angs = np.arange(0, n) / n * np.pi + ang_0
+        ideal_vecs = np.array([np.cos(ideal_angs), np.sin(ideal_angs)]).T
+
+        # Compute cost as dot products between each CMV and each ideal vector
+        # Absolute value used because both parallel and anti-parallel are bad
+        # for our case.
+        dots = -np.array([np.abs(dot(cmv_vecs.T, ideal_vec))
+                          for ideal_vec in ideal_vecs])
+
+        # Compute the optimal assignment of CMVs to maximize alignment with the
+        # ideal vectors. Relative cost could be used to compare multiple zero
+        # angles.
+        r_ind, c_ind = linear_sum_assignment(dots)
+        cost = dots[r_ind, c_ind].sum()
+        return cost, c_ind
+
+    def cost_wrapper(ang_0):
+        """
+        The minimizer only works on a single output, so in this case we wrap it
+        """
+        return calc_cost(ang_0)[0]  # return only the cost
+
+    # The bounds of the optimization are limited by the spacing between ideal
+    # vectors.
+    bounds = [(0, np.pi / n)]
+
+    #  What we're optimizing here is a rotation angle for the set of ideal vecs
+    y = shgo(cost_wrapper, bounds)
+
+    # Use the optimized angle to figure out which CMVs to use
+    final_cost, indices = calc_cost(y.x[0])
+
+    return indices
+
+
 def _pairwise_qc(pairs, spacing, sigs, delay, peak_corr, mean_corr,
                  method, options=None):
     """
     Perform pairwise QC on the CMV signals according to method
 
     Parameters
     ----------
@@ -464,14 +568,17 @@
         method_out = {
             'error_index': None,  # The Error Index
             'velocity': None,  # Velocity for each pair
             'v60': None,  # 60th percentile velocity
             'v40': None,  # 40th percentile velocity
             'r_qc': [],  # Ratio of peak to mean xcorr
             'var_s': [],  # Variation ratio of signals [s0, s1]
+            'r_corr': None,  # Corr. coeff. for dist/delay for good pairs
+            'stderr_corr': None,  # Std. error for dist/delay for good pairs
+            'ngood': None,  # Number of good pairs
         }
     elif method == 'gagne':
         defaults = {
             'ktlim': 0.4,
         }
         method_out = {
             'pcov': None,  # Covariance matrix from least squares
```

### Comparing `solartoolbox-0.3.5/src/solartoolbox/dataio/hope_campaign.py` & `solartoolbox-0.4.0/src/solartoolbox/dataio/hope_campaign.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/src/solartoolbox/dataio/iotools.py` & `solartoolbox-0.4.0/src/solartoolbox/dataio/iotools.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/src/solartoolbox/dataio/nrcan_data.py` & `solartoolbox-0.4.0/src/solartoolbox/dataio/nrcan_data.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/src/solartoolbox/irradiance.py` & `solartoolbox-0.4.0/src/solartoolbox/irradiance.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/src/solartoolbox/signalproc.py` & `solartoolbox-0.4.0/src/solartoolbox/signalproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,26 +229,26 @@
 
     overlap : float (default 0.5)
         Percentage overlap between the averages
 
     window : string (default 'hamming')
         The window type to use.
 
-    detrend : string
+    detrend : string or None
         Detrend type ('linear' or 'constant'). See scipy.signal.psdxx for more
         information.
 
     Returns
     -------
-    output : DataFrame
-        Pandas object containing the transfer function and coherence with an
-        index of the frequency.
-        Columns are:
-            'tf' - the complex transfer function
-            'coh' - the coherence
+    tf : pd.DataFrame
+        Complex valued transfer function indexed by the frequency and
+        containing the same columns as the input
+    coh : pd.DataFrame
+        the coherence indexed by the frequency and containing the same
+        columns as the input
     """
     dt = (input_tsig.index[1] - input_tsig.index[0]).total_seconds()
     fs = 1/dt
 
     if isinstance(output_tsig, pd.Series):
         return averaged_tf(input_tsig, pd.DataFrame(output_tsig),
                            navgs, overlap, window, detrend)
@@ -284,20 +284,18 @@
     _, psdyy = signal.welch(output_tsig, fs=fs, window=window,
                             nperseg=nperseg, detrend=detrend,
                             noverlap=noverlap, scaling='density')
     freqs, csdxy = signal.csd(input_tsig, output_tsig, fs=fs, window=window,
                               nperseg=nperseg, detrend=detrend,
                               noverlap=noverlap)
 
-    # try:
-    tf = csdxy / psdxx
-    coh = np.abs(csdxy) ** 2 / (psdxx * psdyy)
-    # except ValueError:
-    #     tf = csdxy.T / np.expand_dims(psdxx, axis=1)
-    #     coh = np.abs(csdxy) ** 2 / (np.expand_dims(psdxx, axis=1) * psdyy)
+    # Calculating manually allows for vectorization and is faster
+    with np.errstate(divide='ignore', invalid='ignore'):
+        tf = csdxy / psdxx
+        coh = np.abs(csdxy) ** 2 / (psdxx * psdyy)
 
     # Calculate the coherence
     # _, coh = signal.coherence(input_tsig, output_tsig, fs=fs, window=window,
     #                           nperseg=nperseg, noverlap=noverlap,
     #                           detrend=detrend)
 
     tf = pd.DataFrame(tf.T, index=freqs, columns=cols)
@@ -374,30 +372,39 @@
         The coherence limit to use for filtering the phase. Set to None to
         include all points.
     freq_limit : float
         The frequency limit to use for filtering the phase. Set to None to
         include all points.
     method : str
         The method to use for computing the delay. Options are:
-            'diff' - unwrap phase and take derivative
+            'diff' - unwrap phase and take derivative (*not well validated)
             'fit' - fit a line to the phase
+            'multi' - fit a line to the phase for multiple tfs at once
 
     Returns
     -------
     delay : float
         The delay in seconds
-
+    ix : np.array(bool)
+        The mask used for filtering the phase
     """
 
     def _delay_fitter(x, delval):
         """
         Helper function for use with curve_fit. Computes the modeled phase.
-        :param x: the transfer function frequency
-        :param delval: The 'real' phase to fit the group delay to
-        :return: the modeled phase
+        Parameters
+        ----------
+        x :
+            the transfer function frequency
+        delval :
+            The 'real' phase to fit the group delay to
+        Returns
+        -------
+        model :
+            the modeled phase
         """
         # model = np.unwrap(np.angle(np.ones_like(x) *
         #                            np.exp(2 * np.pi * 1j * x * -delval)))
         # Simplifies to a linear relationship
         model = 2 * np.pi * x * -delval
         return model
 
@@ -453,16 +460,16 @@
         tfv = tf.values.flatten()
         gd = -np.diff(np.unwrap(np.angle(tfv))) / np.diff(tf.index)
         gd = np.append(gd, gd[-1])
         gd = gd/(2*np.pi)
         avg_del = np.sum(gd * ix.flatten() / np.sum(ix))
         return avg_del, ix
 
-    # Method 2: curve fit the phase
     elif method == 'fit':
+        # Method 2: curve fit the phase
         if not np.any(np.array(np.shape(tf)) == 1):
             raise ValueError('tf must be a 1D array for method: fit')
         try:
             return (curve_fit(_delay_fitter,
                               np.expand_dims(tf.index, axis=1)[ix],
                               np.unwrap(np.angle(tf.loc[ix]).flatten()))[0],
                     ix)
@@ -472,14 +479,15 @@
                 warn('Curve fit failed due to coherence limit. Returning NaN')
                 return np.nan, ix
 
             else:
                 warn('Curve fit failed for unknown reason. Returning NaN')
                 return np.nan, ix
     elif method == "multi":
+        # Method 3 : Operate on multiple tfs at a time using fit method
 
         # The guess for the delays
         guess = np.zeros((1, np.size(tf, axis=1)))
 
         # Get subsets on the frequency axis to simplify fitting
         ix_freq1 = ix_freq[:, 0]
         if isinstance(tf, (pd.DataFrame, pd.Series)):
@@ -563,19 +571,19 @@
 
     Returns
     -------
     delay : array(float)
         Time lag between the two timeseries at the maximum value of the cross
         correlation. Values are always integer multiples of the sampling period
         as the max correlation values are limited to the discrete time steps.
-    extra_data : dict{} or None
-        if compute_extras was true, additional info will be returned. Fields
-        are:
+    extra_data : dict{}
+        Additional data about the correlations. Values are:
+            'peak_corr' - the peak value of the correlation for each input ts
             'mean_corr' - the mean correlation for each input timeseries
-            'zero_zorr' - the correlation at zero_lag for each input timeseries
+            'zero_corr' - the correlation at zero_lag for each input timeseries
     """
     lags = signal.correlation_lags(len(ts_in), len(ts_in))
     dt = (ts_in.index[1] - ts_in.index[0]).total_seconds()
     lags = lags * dt
 
     ts_inm = ts_in
     ts_outm = ts_out
@@ -676,16 +684,17 @@
         The transfer function, produced by signalproc.averaged_tf. The index
         must contain the frequency in Hz.
     delay : float
         The delay to apply to the transfer function. Units are in seconds.
 
     Returns
     -------
-    A copy of the transfer function with the delay applied in rotating
-    the phase.
+    tf : pd.DataFrame
+        A copy of the transfer function with the delay applied in rotating
+        the phase.
     """
 
     tfi = tf.copy().values.flatten()
 
     # Equation for rotating the phase by a delay
     tf = tfi * np.exp(2 * np.pi * 1j * tf.index * -delay)
 
@@ -814,15 +823,15 @@
             camfilt * np.exp(1j * camfreq * (2 * np.pi) * -t_delay))
     return pd.Series(camfilt, index=camfreq)
 
 
 def apply_filter(input_tsig, comp_filt):
     """
     Apply a filter to a signal, and return the filtered signal. Works to align
-    the frequency axis of the computed filter with the
+    the frequency axis of the computed filter with the input signal.
 
     Parameters
     ----------
     input_tsig : pandas.Series or DataFrame
         Pandas type that contains the time signal
 
     comp_filt : Series, DataFrame
```

### Comparing `solartoolbox-0.3.5/src/solartoolbox/spatial.py` & `solartoolbox-0.4.0/src/solartoolbox/spatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
     vec : numeric
         the 2-D cartesian vector as an (x, y) indexable
 
     Returns
     -------
     (xi, yi) : numeric
         the 2-D cartesian vector scaled to a magnitude of 1
-
     """
     return vec / magnitude(vec)
 
 
 def magnitude(vec):
     """
     Get the magnitude of a vector
@@ -250,15 +249,14 @@
     vec : numeric
         the 2-D cartesian vector as an (x, y) indexable
 
     Returns
     -------
     magnitude : numeric
         the magnitude of the vector
-
     """
     return np.sqrt(vec[0]**2+vec[1]**2)
 
 
 def rect2pol(x, y):
     """
     2D cartesian vector to polar form
@@ -271,15 +269,14 @@
     y : numeric
         the y position
 
     Returns
     -------
     (r, theta) : numeric
         the polar form (r, theta) with theta in +/- pi radians
-
     """
     r = magnitude([x, y])
     theta = np.arctan2(y, x)
     return r, theta
 
 
 def pol2rect(r, theta):
@@ -293,16 +290,14 @@
     theta : numeric
         the angle coordinate in radians
 
     Returns
     -------
     (x, y) : numeric
         a tuple of the vector
-
-
     """
 
     x = r * np.cos(theta)
     y = r * np.sin(theta)
     return x, y
```

### Comparing `solartoolbox-0.3.5/src/solartoolbox/stats.py` & `solartoolbox-0.4.0/src/solartoolbox/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,15 @@
     if pct:
         return darr(series * 100 / 1000, tau=tau, moving_avg=False, pct=False)
 
     darr_val = np.abs(series.diff(tau)).sum(axis=0)
 
     return darr_val
 
+
 def calc_quantile(timeseries, n_days="30d", quantile=0.9):
     """
     Calculate a single-day percentile-based summary of data by aggregating
     multiple days.
 
     So the timeseries output on any given day represents the quantile-th
     percentile value over the past n-days during any particular timestamp.
@@ -341,15 +342,15 @@
     quality control algorithm for distributed photovoltaic array power output.
     Solar Energy. 143. 120-131.
     https://www.researchgate.net/publication/312145487_QCPV_A_quality_control_algorithm_for_distributed_photovoltaic_array_power_output
     """
 
     ts = timeseries.copy()  # copy the data
 
-    out_df = pd.DataFrame()  # Create an empty holder
+    out_df = pd.Series()  # Create an empty holder
 
     end_day = ts.index.date[-1]  # the final day of the dataset
 
     # Loop over all unique days in the timeseries
     for date_start in pd.unique(ts.index.date):
         # Window starts on date_start. Window ends on date_end
         date_end = date_start + pd.to_timedelta(n_days)
@@ -378,18 +379,19 @@
 
         # p90's index is only time, so modify it to include the full date
         p90.index = pd.to_datetime(np.repeat(str(date_end) + " ",
                                              len(p90.index)) +
                                    p90.index.astype(str))
 
         # Concat this day onto the output object
-        out_df = pd.concat((out_df, p90))
+        out_df = pd.concat((out_df, p90), axis=0)
 
     # localize the timeseries and the column names back to the input
     out_df = out_df.tz_localize(ts.index.tz).reindex(ts.index)
+    out_df = pd.DataFrame(out_df)
     try:
         out_df.columns = [name+'_quant' for name in ts.columns]
     except AttributeError:
         try:
             out_df.columns = [ts.name + '_quant']
         except AttributeError:
             raise AttributeError('Unable to generate name of column')
```

### Comparing `solartoolbox-0.3.5/src/solartoolbox/visualization/vis_tools.py` & `solartoolbox-0.4.0/src/solartoolbox/visualization/vis_tools.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/src/solartoolbox.egg-info/SOURCES.txt` & `solartoolbox-0.4.0/src/solartoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/tests/test_cmv.py` & `solartoolbox-0.4.0/tests/test_cmv.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     # Directions sometimes get wonky near the 0/360 boundary
     assert (cld_dir == approx(theta, rel=0.01) or
             cld_dir == approx(theta+2*np.pi, rel=0.01))
 
 
 def test_cmv_gagne_data():
     datafile = "../demos/data/sample_plant_1.h5"
-    pos_utm = pd.read_hdf(datafile, mode="r", key="latlon")
+    pos_utm = pd.read_hdf(datafile, mode="r", key="utm")
     df = pd.read_hdf(datafile, mode="r", key="data_a")
 
     hourlymax = np.mean(df.quantile(0.95))
     kt = df / hourlymax
 
     cld_spd_gag, cld_dir_gag, dat_gag = cmv.compute_cmv(kt, pos_utm,
                                                         reference_id=None,
@@ -112,15 +112,15 @@
     assert cld_spd_gag == approx(10.53, abs=0.01)
     assert cld_dir_gag == approx(3.68, abs=0.01)
     assert sum(dat_gag.pair_flag == cmv.Flag.GOOD) == 574
 
 
 def test_cmv_jamaly_data():
     datafile = "../demos/data/sample_plant_1.h5"
-    pos_utm = pd.read_hdf(datafile, mode="r", key="latlon")
+    pos_utm = pd.read_hdf(datafile, mode="r", key="utm")
     df = pd.read_hdf(datafile, mode="r", key="data_a")
 
     hourlymax = np.mean(df.quantile(0.95))
     kt = df / hourlymax
 
     cld_spd_jam, cld_dir_jam, dat_jam = cmv.compute_cmv(kt, pos_utm,
                                                         reference_id=None,
@@ -130,22 +130,40 @@
     assert cld_dir_jam == approx(3.29, abs=0.01)
     assert sum(dat_jam.pair_flag == cmv.Flag.GOOD) == 12709
 
 def test_cmv_jamaly_data_ref():
     # A test using a reference when we calculate the CMV
 
     datafile = "../demos/data/sample_plant_1.h5"
-    pos_utm = pd.read_hdf(datafile, mode="r", key="latlon")
+    pos_utm = pd.read_hdf(datafile, mode="r", key="utm")
     df = pd.read_hdf(datafile, mode="r", key="data_a")
 
     hourlymax = np.mean(df.quantile(0.95))
     kt = df / hourlymax
 
     cld_spd_jam, cld_dir_jam, dat_jam = cmv.compute_cmv(kt, pos_utm,
                                                         reference_id=pos_utm.index[0],
                                                         method='jamaly')
 
 
     # Known values calculated on 11/3/2023
     assert cld_spd_jam == approx(9.3911, abs=0.01)
     assert cld_dir_jam == approx(3.665955, abs=0.01)
     assert sum(dat_jam.pair_flag == cmv.Flag.GOOD) == 64
+
+
+def test_optimum_subset_base():
+    angles = np.linspace(0, np.pi, 9)
+    magnitudes = np.linspace(1, 6, 9)
+    vx = magnitudes * np.cos(angles)
+    vy = magnitudes * np.sin(angles)
+    indices = cmv.optimum_subset(vx, vy, n=4)
+    assert np.sort(np.rad2deg(angles[indices])) == approx(np.sort(np.array([0, 45, 90, 135])))
+
+
+def test_optimum_subset_rotate():
+    angles = np.linspace(0, np.pi, 9) + np.pi/4
+    magnitudes = np.linspace(1, 6, 9)
+    vx = magnitudes * np.cos(angles)
+    vy = magnitudes * np.sin(angles)
+    indices = cmv.optimum_subset(vx, vy, n=4)
+    assert np.sort(np.rad2deg(angles[indices])) == approx(np.sort(np.array([45, 90, 135, 180])))
```

### Comparing `solartoolbox-0.3.5/tests/test_irradiance.py` & `solartoolbox-0.4.0/tests/test_irradiance.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/tests/test_signalproc.py` & `solartoolbox-0.4.0/tests/test_signalproc.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/tests/test_spatial.py` & `solartoolbox-0.4.0/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `solartoolbox-0.3.5/tests/test_stats.py` & `solartoolbox-0.4.0/tests/test_stats.py`

 * *Files identical despite different names*

