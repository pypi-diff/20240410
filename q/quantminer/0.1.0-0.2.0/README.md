# Comparing `tmp/quantminer-0.1.0.tar.gz` & `tmp/quantminer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.1.0.tar", last modified: Wed Apr 10 12:29:42 2024, max compression
+gzip compressed data, was "quantminer-0.2.0.tar", last modified: Wed Apr 10 19:49:27 2024, max compression
```

## Comparing `quantminer-0.1.0.tar` & `quantminer-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 12:29:42.587038 quantminer-0.1.0/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 12:29:42.586920 quantminer-0.1.0/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.1.0/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 12:29:42.585907 quantminer-0.1.0/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.1.0/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 12:29:42.586763 quantminer-0.1.0/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.1.0/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.1.0/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.1.0/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    18209 2024-04-10 12:07:40.000000 quantminer-0.1.0/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 12:29:42.586442 quantminer-0.1.0/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 12:29:42.000000 quantminer-0.1.0/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 12:29:42.000000 quantminer-0.1.0/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 12:29:42.000000 quantminer-0.1.0/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 12:29:42.000000 quantminer-0.1.0/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 12:29:42.000000 quantminer-0.1.0/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 12:29:42.587076 quantminer-0.1.0/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 10:55:02.000000 quantminer-0.1.0/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.107282 quantminer-0.2.0/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 19:49:27.107162 quantminer-0.2.0/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.2.0/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.105564 quantminer-0.2.0/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.2.0/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.106856 quantminer-0.2.0/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.2.0/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.2.0/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.2.0/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    18235 2024-04-10 19:48:51.000000 quantminer-0.2.0/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.106341 quantminer-0.2.0/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 19:49:27.107322 quantminer-0.2.0/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 19:48:58.000000 quantminer-0.2.0/setup.py
```

### Comparing `quantminer-0.1.0/quantminer/classes/pivot_pip.py` & `quantminer-0.2.0/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.1.0/quantminer/classes/seqkmeans.py` & `quantminer-0.2.0/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.1.0/quantminer/pipminer.py` & `quantminer-0.2.0/quantminer/pipminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
         self.n_pivots = n_pivots
         self.hold_period = hold_period
 
         self._model_type = model_type
 
         # Store Training Data
         self._data: List = []
-        self._data_train_X: List[np.ndarray] = []
-        self._data_train_y: List[np.ndarray] = []
+        self._data_train_X: Union[List, np.ndarray] = []
+        self._data_train_y: Union[List, np.ndarray] = []
 
         # Store Clusters Assignments
-        self._unique_pip_indices : np.ndarray = []
+        self._unique_pip_indices : Union[List, np.ndarray]= []
         self._cluster_labels = []
 
         # Store Selected Cluster Labels
         self._cluster_labels_long = []
         self._cluster_labels_short = []
 
         # Store the dimensionality reduction agent
```

### Comparing `quantminer-0.1.0/setup.py` & `quantminer-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.1.0', 
+    version='0.2.0', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

