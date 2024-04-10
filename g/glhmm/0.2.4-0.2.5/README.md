# Comparing `tmp/glhmm-0.2.4.tar.gz` & `tmp/glhmm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glhmm-0.2.4.tar", last modified: Tue Apr  9 13:52:53 2024, max compression
+gzip compressed data, was "glhmm-0.2.5.tar", last modified: Tue Apr  9 14:05:19 2024, max compression
```

## Comparing `glhmm-0.2.4.tar` & `glhmm-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.915955 glhmm-0.2.4/
--rw-r--r--   0 admin      (501) staff       (20)    35149 2023-03-08 15:43:34.000000 glhmm-0.2.4/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 13:52:53.915430 glhmm-0.2.4/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      942 2024-03-25 09:06:49.000000 glhmm-0.2.4/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.911255 glhmm-0.2.4/glhmm/
--rw-r--r--   0 admin      (501) staff       (20)    16487 2024-01-20 15:34:39.000000 glhmm-0.2.4/glhmm/auxiliary.py
--rw-r--r--   0 admin      (501) staff       (20)    85908 2024-04-09 13:48:56.000000 glhmm-0.2.4/glhmm/glhmm.py
--rw-r--r--   0 admin      (501) staff       (20)    69169 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/graphics.py
--rw-r--r--   0 admin      (501) staff       (20)    11236 2024-02-28 16:36:16.000000 glhmm-0.2.4/glhmm/io.py
--rw-r--r--   0 admin      (501) staff       (20)    65221 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/palm_functions.py
--rw-r--r--   0 admin      (501) staff       (20)    87246 2023-12-12 10:51:17.000000 glhmm-0.2.4/glhmm/prediction.py
--rw-r--r--   0 admin      (501) staff       (20)    16779 2023-05-14 21:28:03.000000 glhmm-0.2.4/glhmm/preproc.py
--rw-r--r--   0 admin      (501) staff       (20)   136831 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/statistics.py
--rw-r--r--   0 admin      (501) staff       (20)    11894 2024-04-09 08:41:41.000000 glhmm-0.2.4/glhmm/utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 13:52:53.914237 glhmm-0.2.4/glhmm.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      373 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-18 19:06:24.000000 glhmm-0.2.4/glhmm.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)      139 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        6 2024-04-09 13:52:53.000000 glhmm-0.2.4/glhmm.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)      409 2024-03-25 09:06:36.000000 glhmm-0.2.4/pyproject.toml
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-09 13:52:53.916061 glhmm-0.2.4/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)      581 2024-04-09 13:52:37.000000 glhmm-0.2.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 14:05:19.390939 glhmm-0.2.5/
+-rw-r--r--   0 admin      (501) staff       (20)    35149 2023-03-08 15:43:34.000000 glhmm-0.2.5/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 14:05:19.390462 glhmm-0.2.5/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      942 2024-03-25 09:06:49.000000 glhmm-0.2.5/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 14:05:19.385926 glhmm-0.2.5/glhmm/
+-rw-r--r--   0 admin      (501) staff       (20)    16487 2024-01-20 15:34:39.000000 glhmm-0.2.5/glhmm/auxiliary.py
+-rw-r--r--   0 admin      (501) staff       (20)    85916 2024-04-09 14:01:47.000000 glhmm-0.2.5/glhmm/glhmm.py
+-rw-r--r--   0 admin      (501) staff       (20)    69169 2024-04-09 08:41:41.000000 glhmm-0.2.5/glhmm/graphics.py
+-rw-r--r--   0 admin      (501) staff       (20)    11236 2024-02-28 16:36:16.000000 glhmm-0.2.5/glhmm/io.py
+-rw-r--r--   0 admin      (501) staff       (20)    65221 2024-04-09 08:41:41.000000 glhmm-0.2.5/glhmm/palm_functions.py
+-rw-r--r--   0 admin      (501) staff       (20)    87246 2023-12-12 10:51:17.000000 glhmm-0.2.5/glhmm/prediction.py
+-rw-r--r--   0 admin      (501) staff       (20)    16779 2023-05-14 21:28:03.000000 glhmm-0.2.5/glhmm/preproc.py
+-rw-r--r--   0 admin      (501) staff       (20)   136831 2024-04-09 08:41:41.000000 glhmm-0.2.5/glhmm/statistics.py
+-rw-r--r--   0 admin      (501) staff       (20)    11894 2024-04-09 08:41:41.000000 glhmm-0.2.5/glhmm/utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-09 14:05:19.389340 glhmm-0.2.5/glhmm.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      775 2024-04-09 14:05:19.000000 glhmm-0.2.5/glhmm.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      373 2024-04-09 14:05:19.000000 glhmm-0.2.5/glhmm.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-09 14:05:19.000000 glhmm-0.2.5/glhmm.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-18 19:06:24.000000 glhmm-0.2.5/glhmm.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)      139 2024-04-09 14:05:19.000000 glhmm-0.2.5/glhmm.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        6 2024-04-09 14:05:19.000000 glhmm-0.2.5/glhmm.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)      409 2024-03-25 09:06:36.000000 glhmm-0.2.5/pyproject.toml
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-09 14:05:19.391039 glhmm-0.2.5/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      581 2024-04-09 14:04:49.000000 glhmm-0.2.5/setup.py
```

### Comparing `glhmm-0.2.4/LICENSE` & `glhmm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/PKG-INFO` & `glhmm-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhmm
-Version: 0.2.4
+Version: 0.2.5
 Summary: Gaussian Linear Hidden Markov Model
 Home-page: https://github.com/vidaurre/glhmm
 Author: Diego Vidaurre
 Author-email: Diego Vidaurre <dvidaurre@cfin.au.dk>
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `glhmm-0.2.4/README.md` & `glhmm-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/auxiliary.py` & `glhmm-0.2.5/glhmm/auxiliary.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/glhmm.py` & `glhmm-0.2.5/glhmm/glhmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1304,23 +1304,23 @@
 
         # Y, covariance
         if shared_covmat:
             C = self.get_covariance_matrix()
             if diagonal_covmat:
                 Y += rng.normal(loc=np.zeros(q),scale=C,size=Y.shape)
             else:
-                Y += rng.multivariate_normal(loc=np.zeros(q),cov=C,size=Y.shape)
+                Y += rng.multivariate_normal(mean=np.zeros(q),cov=C,size=Y.shape[0])
         else:
             for k in range(K):
                 C = self.get_covariance_matrix(k)
                 if diagonal_covmat:
                     Y += rng.normal(loc=np.zeros(q),scale=C,size=Y.shape)  \
                         * np.expand_dims(Gamma[:,k],axis=1)
                 else:
-                    Y += rng.multivariate_normal(loc=np.zeros(q),cov=C,size=Y.shape) \
+                    Y += rng.multivariate_normal(mean=np.zeros(q),cov=C,size=Y.shape[0]) \
                         * np.expand_dims(Gamma[:,k],axis=1)
 
         if X is None: 
             return Y,Gamma
         else:
             return X,Y,Gamma
```

### Comparing `glhmm-0.2.4/glhmm/graphics.py` & `glhmm-0.2.5/glhmm/graphics.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/io.py` & `glhmm-0.2.5/glhmm/io.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/palm_functions.py` & `glhmm-0.2.5/glhmm/palm_functions.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/prediction.py` & `glhmm-0.2.5/glhmm/prediction.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/preproc.py` & `glhmm-0.2.5/glhmm/preproc.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/statistics.py` & `glhmm-0.2.5/glhmm/statistics.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm/utils.py` & `glhmm-0.2.5/glhmm/utils.py`

 * *Files identical despite different names*

### Comparing `glhmm-0.2.4/glhmm.egg-info/PKG-INFO` & `glhmm-0.2.5/glhmm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhmm
-Version: 0.2.4
+Version: 0.2.5
 Summary: Gaussian Linear Hidden Markov Model
 Home-page: https://github.com/vidaurre/glhmm
 Author: Diego Vidaurre
 Author-email: Diego Vidaurre <dvidaurre@cfin.au.dk>
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `glhmm-0.2.4/setup.py` & `glhmm-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='glhmm',
-    version='0.2.4',
+    version='0.2.5',
     description='Gaussian Linear Hidden Markov Model',
     url='https://github.com/vidaurre/glhmm',
     author='Diego Vidaurre',
     author_email = "dvidaurre@cfin.au.dk",
     readme = "README.md",
     install_requires=['scipy','numpy','scikit-learn','matplotlib','numba','seaborn', 'pandas','igraph', 'tqdm', 'scikit-image','statsmodels'],
     packages=["glhmm"],
```

