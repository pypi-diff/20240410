# Comparing `tmp/gigaanalysis-0.4.3.tar.gz` & `tmp/gigaanalysis-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigaanalysis-0.4.3.tar", last modified: Thu Mar  2 17:10:43 2023, max compression
+gzip compressed data, was "gigaanalysis-0.4.4.tar", last modified: Wed Apr 10 16:50:36 2024, max compression
```

## Comparing `gigaanalysis-0.4.3.tar` & `gigaanalysis-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2023-03-02 17:10:43.732193 gigaanalysis-0.4.3/
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     1481 2022-08-04 14:09:02.000000 gigaanalysis-0.4.3/LICENSE.txt
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     2976 2023-03-02 17:10:43.732419 gigaanalysis-0.4.3/PKG-INFO
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     1911 2023-03-02 17:02:12.000000 gigaanalysis-0.4.3/README.md
-drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2023-03-02 17:10:43.728506 gigaanalysis-0.4.3/gigaanalysis/
--rw-r--r--   0 alexanderhickey   (501) staff       (20)      301 2023-03-02 17:02:03.000000 gigaanalysis-0.4.3/gigaanalysis/__init__.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    10766 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/const.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    30936 2022-09-02 18:25:13.000000 gigaanalysis-0.4.3/gigaanalysis/contour.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    58877 2023-01-15 18:35:46.000000 gigaanalysis-0.4.3/gigaanalysis/data.py
--rwxr-xr-x   0 alexanderhickey   (501) staff       (20)    21326 2023-03-02 17:01:19.000000 gigaanalysis-0.4.3/gigaanalysis/diglock.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    21942 2022-08-04 11:48:43.000000 gigaanalysis-0.4.3/gigaanalysis/dset.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    13386 2022-08-17 18:57:58.000000 gigaanalysis-0.4.3/gigaanalysis/fit.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     1664 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/heatc.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    36373 2023-02-28 15:20:37.000000 gigaanalysis-0.4.3/gigaanalysis/highfield.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    13970 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/htsc.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     3141 2021-04-07 17:47:22.000000 gigaanalysis-0.4.3/gigaanalysis/magnetism.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)      809 2022-08-05 13:19:00.000000 gigaanalysis-0.4.3/gigaanalysis/mfunc.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     5277 2023-01-15 18:13:20.000000 gigaanalysis-0.4.3/gigaanalysis/mfunc_fft.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     4153 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/mfunc_make.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     7374 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/mfunc_trans.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     6113 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/gigaanalysis/mfunc_ufunc.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    15167 2022-09-02 19:23:21.000000 gigaanalysis-0.4.3/gigaanalysis/parse.py
--rw-r--r--   0 alexanderhickey   (501) staff       (20)    33752 2023-01-15 18:13:20.000000 gigaanalysis-0.4.3/gigaanalysis/qo.py
-drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2023-03-02 17:10:43.731710 gigaanalysis-0.4.3/gigaanalysis.egg-info/
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     2976 2023-03-02 17:10:43.000000 gigaanalysis-0.4.3/gigaanalysis.egg-info/PKG-INFO
--rw-r--r--   0 alexanderhickey   (501) staff       (20)      643 2023-03-02 17:10:43.000000 gigaanalysis-0.4.3/gigaanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderhickey   (501) staff       (20)        1 2023-03-02 17:10:43.000000 gigaanalysis-0.4.3/gigaanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderhickey   (501) staff       (20)       81 2023-03-02 17:10:43.000000 gigaanalysis-0.4.3/gigaanalysis.egg-info/requires.txt
--rw-r--r--   0 alexanderhickey   (501) staff       (20)       13 2023-03-02 17:10:43.000000 gigaanalysis-0.4.3/gigaanalysis.egg-info/top_level.txt
--rw-r--r--   0 alexanderhickey   (501) staff       (20)     1300 2023-03-02 17:10:43.733613 gigaanalysis-0.4.3/setup.cfg
--rw-r--r--   0 alexanderhickey   (501) staff       (20)       82 2022-06-13 15:13:19.000000 gigaanalysis-0.4.3/setup.py
+drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2024-04-10 16:50:36.631206 gigaanalysis-0.4.4/
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     1481 2022-08-04 14:09:02.000000 gigaanalysis-0.4.4/LICENSE.txt
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     2976 2024-04-10 16:50:36.631410 gigaanalysis-0.4.4/PKG-INFO
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     1911 2023-03-02 17:02:12.000000 gigaanalysis-0.4.4/README.md
+drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2024-04-10 16:50:36.625968 gigaanalysis-0.4.4/gigaanalysis/
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)      301 2024-04-10 16:17:35.000000 gigaanalysis-0.4.4/gigaanalysis/__init__.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    10766 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/const.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    30936 2023-09-25 17:50:07.000000 gigaanalysis-0.4.4/gigaanalysis/contour.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    58877 2023-01-15 18:35:46.000000 gigaanalysis-0.4.4/gigaanalysis/data.py
+-rwxr-xr-x   0 alexanderhickey   (501) staff       (20)    21326 2023-03-02 17:01:19.000000 gigaanalysis-0.4.4/gigaanalysis/diglock.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    21942 2022-08-04 11:48:43.000000 gigaanalysis-0.4.4/gigaanalysis/dset.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    13386 2022-08-17 18:57:58.000000 gigaanalysis-0.4.4/gigaanalysis/fit.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     1664 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/heatc.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    36373 2024-04-10 16:12:27.000000 gigaanalysis-0.4.4/gigaanalysis/highfield.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    13970 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/htsc.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     3141 2021-04-07 17:47:22.000000 gigaanalysis-0.4.4/gigaanalysis/magnetism.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)      809 2022-08-05 13:19:00.000000 gigaanalysis-0.4.4/gigaanalysis/mfunc.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     5277 2023-01-15 18:13:20.000000 gigaanalysis-0.4.4/gigaanalysis/mfunc_fft.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     4153 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/mfunc_make.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     7374 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/mfunc_trans.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     6113 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/gigaanalysis/mfunc_ufunc.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    15167 2022-09-02 19:23:21.000000 gigaanalysis-0.4.4/gigaanalysis/parse.py
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)    33752 2023-01-15 18:13:20.000000 gigaanalysis-0.4.4/gigaanalysis/qo.py
+drwxr-xr-x   0 alexanderhickey   (501) staff       (20)        0 2024-04-10 16:50:36.630799 gigaanalysis-0.4.4/gigaanalysis.egg-info/
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     2976 2024-04-10 16:50:36.000000 gigaanalysis-0.4.4/gigaanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)      643 2024-04-10 16:50:36.000000 gigaanalysis-0.4.4/gigaanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)        1 2024-04-10 16:50:36.000000 gigaanalysis-0.4.4/gigaanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)       81 2024-04-10 16:50:36.000000 gigaanalysis-0.4.4/gigaanalysis.egg-info/requires.txt
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)       13 2024-04-10 16:50:36.000000 gigaanalysis-0.4.4/gigaanalysis.egg-info/top_level.txt
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)     1300 2024-04-10 16:50:36.633656 gigaanalysis-0.4.4/setup.cfg
+-rw-r--r--   0 alexanderhickey   (501) staff       (20)       82 2022-06-13 15:13:19.000000 gigaanalysis-0.4.4/setup.py
```

### Comparing `gigaanalysis-0.4.3/LICENSE.txt` & `gigaanalysis-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/PKG-INFO` & `gigaanalysis-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigaanalysis
-Version: 0.4.3
+Version: 0.4.4
 Summary: A toolbox for processing data that can be expressed as a
 Home-page: https://github.com/alexeatscake/gigaanalysis
 Author: Alex Hickey
 Author-email: alexander.john.hickey@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/alexeatscake/gigaanalysis
 Project-URL: Documentation, https://gigaanalysis.readthedocs.io/en/latest/
```

### Comparing `gigaanalysis-0.4.3/README.md` & `gigaanalysis-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/const.py` & `gigaanalysis-0.4.4/gigaanalysis/const.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/contour.py` & `gigaanalysis-0.4.4/gigaanalysis/contour.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
 
     def optermise_argument(self, arguments, **kwargs):
         """Minimise the negative log marginal likelihood.
 
         This uses :func:`scipy.optimize.minimize` to change the value of 
         keyword arguments to minimise the value from 
         :meth:`calculate_log_mlh`. This should take both into account the 
-        model complexity and the quality of the kit to the data.
+        model complexity and the quality of the fit to the data.
         Keyword arguments are passed to :func:`scipy.optimize.minimize`, a 
         very useful one is `bounds` which is a list of tuples of the lower 
         then upper bounds.
 
         Parameters
         ----------
         arguments : dict
```

### Comparing `gigaanalysis-0.4.3/gigaanalysis/data.py` & `gigaanalysis-0.4.4/gigaanalysis/data.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/diglock.py` & `gigaanalysis-0.4.4/gigaanalysis/diglock.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/dset.py` & `gigaanalysis-0.4.4/gigaanalysis/dset.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/fit.py` & `gigaanalysis-0.4.4/gigaanalysis/fit.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/heatc.py` & `gigaanalysis-0.4.4/gigaanalysis/heatc.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/highfield.py` & `gigaanalysis-0.4.4/gigaanalysis/highfield.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
         ----------
         smooth_points : float
             The time window to fit the polynomial for smoothing, in seconds.
         smooth_order : int, optional
             The order of the poly to fit for the smoothing, the default is 2.
         """
         self._has_locked()
-        smooth_points = int(np.ciel(smooth_time/self.fs/2)*2 + 1)
+        smooth_points = int(np.ceil(smooth_time/self.fs/2)*2 + 1)
         self.loc_Volt = savgol_filter(self.loc_Volt, smooth_points,
             smooth_order,)
         self.loc_Volt_out = savgol_filter(self.loc_Volt_out, smooth_points,
             smooth_order,)
 
     def rephase(self, phase_shift, trial=False):
         """Rephases the signal to the new phase.
```

### Comparing `gigaanalysis-0.4.3/gigaanalysis/htsc.py` & `gigaanalysis-0.4.4/gigaanalysis/htsc.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/magnetism.py` & `gigaanalysis-0.4.4/gigaanalysis/magnetism.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/mfunc.py` & `gigaanalysis-0.4.4/gigaanalysis/mfunc.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/mfunc_fft.py` & `gigaanalysis-0.4.4/gigaanalysis/mfunc_fft.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/mfunc_make.py` & `gigaanalysis-0.4.4/gigaanalysis/mfunc_make.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/mfunc_trans.py` & `gigaanalysis-0.4.4/gigaanalysis/mfunc_trans.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/mfunc_ufunc.py` & `gigaanalysis-0.4.4/gigaanalysis/mfunc_ufunc.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/parse.py` & `gigaanalysis-0.4.4/gigaanalysis/parse.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis/qo.py` & `gigaanalysis-0.4.4/gigaanalysis/qo.py`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/gigaanalysis.egg-info/PKG-INFO` & `gigaanalysis-0.4.4/gigaanalysis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigaanalysis
-Version: 0.4.3
+Version: 0.4.4
 Summary: A toolbox for processing data that can be expressed as a
 Home-page: https://github.com/alexeatscake/gigaanalysis
 Author: Alex Hickey
 Author-email: alexander.john.hickey@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source Code, https://github.com/alexeatscake/gigaanalysis
 Project-URL: Documentation, https://gigaanalysis.readthedocs.io/en/latest/
```

### Comparing `gigaanalysis-0.4.3/gigaanalysis.egg-info/SOURCES.txt` & `gigaanalysis-0.4.4/gigaanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gigaanalysis-0.4.3/setup.cfg` & `gigaanalysis-0.4.4/setup.cfg`

 * *Files identical despite different names*

