# Comparing `tmp/guan-0.1.95.tar.gz` & `tmp/guan-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guan-0.1.95.tar", last modified: Wed Apr  3 16:29:41 2024, max compression
+gzip compressed data, was "guan-0.1.96.tar", last modified: Wed Apr 10 14:35:47 2024, max compression
```

## Comparing `guan-0.1.95.tar` & `guan-0.1.96.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.666047 guan-0.1.95/
--rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.95/LICENSE
--rw-rw-rw-   0        0        0      798 2024-04-03 16:29:41.666047 guan-0.1.95/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.95/README.md
--rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.95/pyproject.toml
--rw-rw-rw-   0        0        0      641 2024-04-03 16:29:41.667921 guan-0.1.95/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.508416 guan-0.1.95/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.644086 guan-0.1.95/src/guan/
--rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.95/src/guan/Fourier_transform.py
--rw-rw-rw-   0        0        0     6572 2024-02-22 19:01:42.000000 guan-0.1.95/src/guan/Green_functions.py
--rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.95/src/guan/Hamiltonian_of_examples.py
--rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.95/src/guan/__init__.py
--rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.95/src/guan/band_structures_and_wave_functions.py
--rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.95/src/guan/basic_functions.py
--rw-rw-rw-   0        0        0     4622 2024-04-02 06:13:43.000000 guan-0.1.95/src/guan/data_processing.py
--rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.95/src/guan/decorators.py
--rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.95/src/guan/density_of_states.py
--rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.95/src/guan/figure_plotting.py
--rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.95/src/guan/file_reading_and_writing.py
--rw-rw-rw-   0        0        0    12995 2024-04-03 16:25:13.000000 guan-0.1.95/src/guan/machine_learning.py
--rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.95/src/guan/others.py
--rw-rw-rw-   0        0        0    41489 2024-03-10 21:28:40.000000 guan-0.1.95/src/guan/quantum_transport.py
--rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.95/src/guan/topological_invariant.py
-drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.664336 guan-0.1.95/src/guan.egg-info/
--rw-rw-rw-   0        0        0      798 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:35:47.384410 guan-0.1.96/
+-rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.96/LICENSE
+-rw-rw-rw-   0        0        0      798 2024-04-10 14:35:47.383413 guan-0.1.96/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.96/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.96/pyproject.toml
+-rw-rw-rw-   0        0        0      641 2024-04-10 14:35:47.385429 guan-0.1.96/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 14:35:47.205209 guan-0.1.96/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 14:35:47.358009 guan-0.1.96/src/guan/
+-rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.96/src/guan/Fourier_transform.py
+-rw-rw-rw-   0        0        0     6572 2024-02-22 19:01:42.000000 guan-0.1.96/src/guan/Green_functions.py
+-rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.96/src/guan/Hamiltonian_of_examples.py
+-rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.96/src/guan/__init__.py
+-rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.96/src/guan/band_structures_and_wave_functions.py
+-rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.96/src/guan/basic_functions.py
+-rw-rw-rw-   0        0        0     4622 2024-04-02 06:13:43.000000 guan-0.1.96/src/guan/data_processing.py
+-rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.96/src/guan/decorators.py
+-rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.96/src/guan/density_of_states.py
+-rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.96/src/guan/figure_plotting.py
+-rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.96/src/guan/file_reading_and_writing.py
+-rw-rw-rw-   0        0        0    14014 2024-04-10 14:29:46.000000 guan-0.1.96/src/guan/machine_learning.py
+-rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.96/src/guan/others.py
+-rw-rw-rw-   0        0        0    41489 2024-03-10 21:28:40.000000 guan-0.1.96/src/guan/quantum_transport.py
+-rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.96/src/guan/topological_invariant.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:35:47.383413 guan-0.1.96/src/guan.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-04-10 14:35:47.000000 guan-0.1.96/src/guan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-04-10 14:35:47.000000 guan-0.1.96/src/guan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:35:47.000000 guan-0.1.96/src/guan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 14:35:47.000000 guan-0.1.96/src/guan.egg-info/top_level.txt
```

### Comparing `guan-0.1.95/LICENSE` & `guan-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/PKG-INFO` & `guan-0.1.96/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.95
+Version: 0.1.96
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.95/setup.cfg` & `guan-0.1.96/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 7561 6e0d 0a76 6572 7369 6f6e   = guan..version
-00000020: 203d 2030 2e31 2e39 350d 0a61 7574 686f   = 0.1.95..autho
+00000020: 203d 2030 2e31 2e39 360d 0a61 7574 686f   = 0.1.96..autho
 00000030: 7220 3d20 6775 616e 6a69 6875 616e 0d0a  r = guanjihuan..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2067  author_email = g
 00000050: 7561 6e6a 6968 7561 6e40 3136 332e 636f  uanjihuan@163.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2041 6e20 6f70 656e 2073 6f75 7263 6520   An open source 
 00000080: 7079 7468 6f6e 2070 6163 6b61 6765 0d0a  python package..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `guan-0.1.95/src/guan/Fourier_transform.py` & `guan-0.1.96/src/guan/Fourier_transform.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/Green_functions.py` & `guan-0.1.96/src/guan/Green_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/Hamiltonian_of_examples.py` & `guan-0.1.96/src/guan/Hamiltonian_of_examples.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/__init__.py` & `guan-0.1.96/src/guan/__init__.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/band_structures_and_wave_functions.py` & `guan-0.1.96/src/guan/band_structures_and_wave_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/basic_functions.py` & `guan-0.1.96/src/guan/basic_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/data_processing.py` & `guan-0.1.96/src/guan/data_processing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/decorators.py` & `guan-0.1.96/src/guan/decorators.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/density_of_states.py` & `guan-0.1.96/src/guan/density_of_states.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/figure_plotting.py` & `guan-0.1.96/src/guan/figure_plotting.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/file_reading_and_writing.py` & `guan-0.1.96/src/guan/file_reading_and_writing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/machine_learning.py` & `guan-0.1.96/src/guan/machine_learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,14 +217,37 @@
 # 加载训练数据，用于批量加载训练
 def load_train_data(x_train, y_train, batch_size=32):
     from torch.utils.data import DataLoader, TensorDataset
     train_dataset = TensorDataset(x_train, y_train)
     train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
     return train_loader
 
+# 从pickle文件中读取输入数据和输出数据，用于训练或预测
+def load_input_data_and_output_data_as_torch_tensors_with_pickle(index_range=[1, 2, 3], directory='./', input_filename='input_index=', output_filename='output_index=', type=None):
+    import guan
+    import numpy as np
+    import torch
+    input_data = []
+    for index in index_range:
+        input = guan.load_data(filename=directory+input_filename+str(index))
+        input_data.append(input)
+    output_data = []
+    for index in index_range:
+        output = guan.load_data(filename=directory+output_filename+str(index))
+        output_data.append(output)
+    if type == None:
+        input_data = np.array(input_data)
+        output_data= np.array(output_data)
+    else:
+        input_data = np.array(input_data).astype(type)
+        output_data= np.array(output_data).astype(type)
+    input_data = torch.from_numpy(input_data)
+    output_data = torch.from_numpy(output_data)
+    return input_data, output_data
+
 # 数据的主成分分析PCA
 def pca_of_data(data, n_components=None, standard=1):
     from sklearn.decomposition import PCA
     if standard==1:
         from sklearn.preprocessing import StandardScaler
         scaler = StandardScaler()
         data_scaled = scaler.fit_transform(data)
```

### Comparing `guan-0.1.95/src/guan/others.py` & `guan-0.1.96/src/guan/others.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/quantum_transport.py` & `guan-0.1.96/src/guan/quantum_transport.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan/topological_invariant.py` & `guan-0.1.96/src/guan/topological_invariant.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.95/src/guan.egg-info/PKG-INFO` & `guan-0.1.96/src/guan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.95
+Version: 0.1.96
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.95/src/guan.egg-info/SOURCES.txt` & `guan-0.1.96/src/guan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

