# Comparing `tmp/quantminer-0.2.0.tar.gz` & `tmp/quantminer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.2.0.tar", last modified: Wed Apr 10 19:49:27 2024, max compression
+gzip compressed data, was "quantminer-0.3.0.tar", last modified: Wed Apr 10 21:11:22 2024, max compression
```

## Comparing `quantminer-0.2.0.tar` & `quantminer-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.107282 quantminer-0.2.0/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 19:49:27.107162 quantminer-0.2.0/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.2.0/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.105564 quantminer-0.2.0/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.2.0/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.106856 quantminer-0.2.0/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.2.0/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.2.0/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.2.0/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    18235 2024-04-10 19:48:51.000000 quantminer-0.2.0/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 19:49:27.106341 quantminer-0.2.0/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 19:49:27.000000 quantminer-0.2.0/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 19:49:27.107322 quantminer-0.2.0/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 19:48:58.000000 quantminer-0.2.0/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.601206 quantminer-0.3.0/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:11:22.601090 quantminer-0.3.0/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.0/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.599569 quantminer-0.3.0/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.0/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.600711 quantminer-0.3.0/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.0/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.0/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.0/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    18829 2024-04-10 21:09:44.000000 quantminer-0.3.0/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.600079 quantminer-0.3.0/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 21:11:22.601247 quantminer-0.3.0/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 21:10:56.000000 quantminer-0.3.0/setup.py
```

### Comparing `quantminer-0.2.0/quantminer/classes/pivot_pip.py` & `quantminer-0.3.0/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.2.0/quantminer/classes/seqkmeans.py` & `quantminer-0.3.0/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.2.0/quantminer/pipminer.py` & `quantminer-0.3.0/quantminer/pipminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,36 @@
         print("Risk of Ruin : ", qt.stats.risk_of_ruin(ser))
         print("Sharpe : ", qt.stats.sharpe(ser))
         print("Avg Win : ", qt.stats.avg_win(ser))
         print("Avg Loss : ", qt.stats.avg_loss(ser))
         print("Avg Return : ", qt.stats.avg_return(ser))
 
 
+    def transform(self, data:Union[List, np.ndarray]):
+        """
+        Generate labels for a full dataset.
+        """
+        # Preprocess Data
+        data = self._preprocess_data(data, test_mode=True)
+
+        # Generate data windows
+        windows = self._generate_training_set(data)
+
+        # Transform the Data
+        _pivots, _unique_indices = self._transform_data(windows)
+
+        # Generate the cluster labels
+        _l = self._agent_cluster.predict(_pivots)
+        indices = _unique_indices + self.n_lookback - 1
+        _labels = self._assign_cluster_labels(data, _l, indices)
+
+        return _labels
+        
+
+
     def generate_signal(self, data: List[np.ndarray]):
         """
         This generates signal for one data window.
 
         Return:
             signal, pivots : Tuple containing the predicted signal, and the list of pivots points.
         """
@@ -589,19 +611,18 @@
 
     train_data = train_data["close"].dropna(axis=0)
     train_data = train_data.to_numpy()
 
     test_data = test_data["close"].dropna(axis=0)
     test_data = test_data.to_numpy()
 
-    miner = Miner(25, 5)
-    miner.fit(train_data)
+    # miner = Miner(25, 5)
+    # miner.fit(train_data)
 
-    miner.save_model(parent_path / 'pipminer.pkl')
+    # miner.save_model(parent_path / 'pipminer.pkl')
 
-    miner = Miner.load_model(parent_path / 'pipminer.pkl')
+    miner : Miner = Miner.load_model(parent_path / 'pipminer.pkl')
 
-    with open(parent_path / 'pipminer.pkl', 'rb') as file:
-        miner = pickle.load(file)
+    print(miner.transform(test_data))
 
-    miner.test(test_data)
+    # miner.test(test_data)
     print('Successful')
```

### Comparing `quantminer-0.2.0/setup.py` & `quantminer-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.2.0', 
+    version='0.3.0', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

