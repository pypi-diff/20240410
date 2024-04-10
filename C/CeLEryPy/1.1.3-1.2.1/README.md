# Comparing `tmp/CeLEryPy-1.1.3.tar.gz` & `tmp/CeLEryPy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CeLEryPy-1.1.3.tar", last modified: Tue Sep 26 15:34:42 2023, max compression
+gzip compressed data, was "CeLEryPy-1.2.1.tar", last modified: Wed Apr 10 20:17:49 2024, max compression
```

## Comparing `CeLEryPy-1.1.3.tar` & `CeLEryPy-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-09-26 15:34:42.098112 CeLEryPy-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-09-26 15:34:42.085297 CeLEryPy-1.1.3/CeLEry/
--rw-rw-rw-   0        0        0     5857 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/ClusterVAE.py
--rw-rw-rw-   0        0        0    14878 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/DNN.py
--rw-rw-rw-   0        0        0     3845 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/TrainerExe.py
--rw-rw-rw-   0        0        0      192 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/__init__.py
--rw-rw-rw-   0        0        0     9286 2023-03-10 20:58:27.000000 CeLEryPy-1.1.3/CeLEry/data_augmentation.py
--rw-rw-rw-   0        0        0     4764 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/datasetgenemap.py
--rw-rw-rw-   0        0        0    16371 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/fit_functions.py
--rw-rw-rw-   0        0        0     1670 2023-09-26 15:13:40.000000 CeLEryPy-1.1.3/CeLEry/layers.py
--rw-rw-rw-   0        0        0      135 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/types_.py
--rw-rw-rw-   0        0        0    18159 2023-05-18 16:53:05.000000 CeLEryPy-1.1.3/CeLEry/util.py
--rw-rw-rw-   0        0        0    14324 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/CeLEry/util_Mouse.py
-drwxrwxrwx   0        0        0        0 2023-09-26 15:34:42.097032 CeLEryPy-1.1.3/CeLEryPy.egg-info/
--rw-rw-rw-   0        0        0     3630 2023-09-26 15:34:42.000000 CeLEryPy-1.1.3/CeLEryPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-09-26 15:34:42.000000 CeLEryPy-1.1.3/CeLEryPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-26 15:34:42.000000 CeLEryPy-1.1.3/CeLEryPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-09-26 15:34:42.000000 CeLEryPy-1.1.3/CeLEryPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-09-26 15:34:42.000000 CeLEryPy-1.1.3/CeLEryPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3630 2023-09-26 15:34:42.098112 CeLEryPy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/README.md
--rw-rw-rw-   0        0        0      886 2023-09-26 15:27:25.000000 CeLEryPy-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-26 15:34:42.098112 CeLEryPy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-10 19:04:58.000000 CeLEryPy-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:17:49.387133 CeLEryPy-1.2.1/
+drwxrwxrwx   0        0        0        0 2024-04-10 20:17:49.370929 CeLEryPy-1.2.1/CeLEry/
+-rw-rw-rw-   0        0        0     5857 2022-08-27 19:37:20.000000 CeLEryPy-1.2.1/CeLEry/ClusterVAE.py
+-rw-rw-rw-   0        0        0    14878 2022-11-11 17:11:42.000000 CeLEryPy-1.2.1/CeLEry/DNN.py
+-rw-rw-rw-   0        0        0     3845 2022-08-27 20:26:09.000000 CeLEryPy-1.2.1/CeLEry/TrainerExe.py
+-rw-rw-rw-   0        0        0      192 2024-02-01 01:30:41.000000 CeLEryPy-1.2.1/CeLEry/__init__.py
+-rw-rw-rw-   0        0        0     9286 2023-03-13 19:14:23.000000 CeLEryPy-1.2.1/CeLEry/data_augmentation.py
+-rw-rw-rw-   0        0        0     4764 2022-08-27 19:37:20.000000 CeLEryPy-1.2.1/CeLEry/datasetgenemap.py
+-rw-rw-rw-   0        0        0    16371 2022-11-10 19:02:17.000000 CeLEryPy-1.2.1/CeLEry/fit_functions.py
+-rw-rw-rw-   0        0        0     1670 2023-10-04 00:57:59.000000 CeLEryPy-1.2.1/CeLEry/layers.py
+-rw-rw-rw-   0        0        0      135 2022-08-27 19:37:20.000000 CeLEryPy-1.2.1/CeLEry/types_.py
+-rw-rw-rw-   0        0        0    20101 2023-12-07 03:57:59.000000 CeLEryPy-1.2.1/CeLEry/util.py
+-rw-rw-rw-   0        0        0    14324 2022-11-24 20:02:56.000000 CeLEryPy-1.2.1/CeLEry/util_Mouse.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:17:49.387133 CeLEryPy-1.2.1/CeLEryPy.egg-info/
+-rw-rw-rw-   0        0        0     3635 2024-04-10 20:17:49.000000 CeLEryPy-1.2.1/CeLEryPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-10 20:17:49.000000 CeLEryPy-1.2.1/CeLEryPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 20:17:49.000000 CeLEryPy-1.2.1/CeLEryPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-10 20:17:49.000000 CeLEryPy-1.2.1/CeLEryPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 20:17:49.000000 CeLEryPy-1.2.1/CeLEryPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2022-08-27 19:37:20.000000 CeLEryPy-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3635 2024-04-10 20:17:49.387133 CeLEryPy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2022-09-29 03:12:28.000000 CeLEryPy-1.2.1/README.md
+-rw-rw-rw-   0        0        0      891 2024-02-01 01:30:41.000000 CeLEryPy-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 20:17:49.387133 CeLEryPy-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-08-27 19:37:20.000000 CeLEryPy-1.2.1/setup.py
```

### Comparing `CeLEryPy-1.1.3/CeLEry/ClusterVAE.py` & `CeLEryPy-1.2.1/CeLEry/ClusterVAE.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/DNN.py` & `CeLEryPy-1.2.1/CeLEry/DNN.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/TrainerExe.py` & `CeLEryPy-1.2.1/CeLEry/TrainerExe.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/data_augmentation.py` & `CeLEryPy-1.2.1/CeLEry/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/datasetgenemap.py` & `CeLEryPy-1.2.1/CeLEry/datasetgenemap.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/fit_functions.py` & `CeLEryPy-1.2.1/CeLEry/fit_functions.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/layers.py` & `CeLEryPy-1.2.1/CeLEry/layers.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEry/util.py` & `CeLEryPy-1.2.1/CeLEry/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -421,7 +421,53 @@
     # Normalize the expression data per cell and apply log transformation
     sc.pp.normalize_per_cell(adata)
     sc.pp.log1p(adata)
 
     # Return the processed AnnData object
     return adata
 
+def get_common_genes(Qdata, Rdata):
+    """
+    This function identifies the common genes present in two different datasets.
+
+    Args:
+    Qdata (DataFrame): A DataFrame containing query data, with gene names in the 'genename' column.
+    Rdata (DataFrame): A DataFrame containing reference data, also with gene names in the 'genename' column.
+
+    Returns:
+    list: A list of gene names that are common to both Qdata and Rdata.
+    """
+    # Extracting gene names from the 'genename' column of Qdata
+    Qgene = Qdata.var["genename"].tolist()
+    # Extracting gene names from the 'genename' column of Rdata
+    Rgene = Rdata.var["genename"].tolist()
+    # Finding the intersection of gene lists to get common genes
+    Gene_common = list(set(Qgene).intersection(Rgene))
+    # Returning the list of common genes
+    return Gene_common
+
+
+def drop_NaN(adata):
+    """
+    Removes columns from an AnnData object's .X attribute that contain NaN values and
+    returns a new AnnData object.
+
+    Args:
+    adata (AnnData): An AnnData object containing gene expression data.
+
+    Returns:
+    AnnData: A new AnnData object with columns containing NaN values removed from the .X attribute.
+    """
+    # Check if .X is a sparse matrix and convert it to a dense format if necessary
+    if issubclass(type(adata.X), np.ndarray):
+        X_dense = adata.X
+    else:
+        X_dense = adata.X.toarray()  # For sparse matrices
+    # Create a mask for columns that do not contain NaN values
+    non_nan_col_mask = ~np.isnan(X_dense).any(axis=0)
+    # Filter the columns in .X using the mask
+    X_filtered = X_dense[:, non_nan_col_mask]
+    # Update the .var DataFrame to reflect the removal of columns
+    var_filtered = adata.var.iloc[non_nan_col_mask]
+    # Create a new AnnData object with the filtered data
+    new_adata = sc.AnnData(X=X_filtered, obs=adata.obs, var=var_filtered)
+    return new_adata
```

### Comparing `CeLEryPy-1.1.3/CeLEry/util_Mouse.py` & `CeLEryPy-1.2.1/CeLEry/util_Mouse.py`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/CeLEryPy.egg-info/PKG-INFO` & `CeLEryPy-1.2.1/CeLEryPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CeLEryPy
-Version: 1.1.3
+Version: 1.2.1
 Summary: Leverage spatial transcriptomics data to recover cell locations in single-cell RNA RNA-seq
 Author-email: Qihuang Zhang <qihuang.zh@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Dist: pandas>=1.4
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: scanpy>=1.5
 Requires-Dist: scikit-image
 Requires-Dist: anndata
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 
 # CeLEry
 ## Leveraging  spatial  transcriptomics  data  to  recover cell  locationsin  single-cell RNA-seq with CeLEry
 
 ### Qihuang Zhang, Jian Hu, Kejie Li, Baohong Zhang, David Dai, Edward B. Lee, Rui Xiao, Mingyao Li*
 
 Single-cell RNA sequencing provides resourceful information to study the cells systematically. However, their locational information is usually unavailable. We present CeLEry, a supervised deep learning algorithm to recover the origin of tissues in assist of spatial transcriptomic data, integrating a data augmentation procedure via variational autoencoder to improve the robustness of methods in the overfitting and the data contamination. CeLEry provides a generic framework and can be implemented in multiple tasks depending on the research objectives, including the spatial coordinates discovery as well as the layer discovery. It can make use of the information of multiple tissues of spatial transcriptomics data. Thorough assessments exhibit that CeLEry achieves a leading performance compared to the state-of-art methods. We illustrated the usage of CeLEry in the discovery of neuron cell layers to study the development of Alzheimer's disease. The identified cell location information is valuable in many downstream analyses and can be indicative of the spatial organization of the tissues.
```

### Comparing `CeLEryPy-1.1.3/LICENSE` & `CeLEryPy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/PKG-INFO` & `CeLEryPy-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CeLEryPy
-Version: 1.1.3
+Version: 1.2.1
 Summary: Leverage spatial transcriptomics data to recover cell locations in single-cell RNA RNA-seq
 Author-email: Qihuang Zhang <qihuang.zh@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Dist: pandas>=1.4
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: scanpy>=1.5
 Requires-Dist: scikit-image
 Requires-Dist: anndata
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 
 # CeLEry
 ## Leveraging  spatial  transcriptomics  data  to  recover cell  locationsin  single-cell RNA-seq with CeLEry
 
 ### Qihuang Zhang, Jian Hu, Kejie Li, Baohong Zhang, David Dai, Edward B. Lee, Rui Xiao, Mingyao Li*
 
 Single-cell RNA sequencing provides resourceful information to study the cells systematically. However, their locational information is usually unavailable. We present CeLEry, a supervised deep learning algorithm to recover the origin of tissues in assist of spatial transcriptomic data, integrating a data augmentation procedure via variational autoencoder to improve the robustness of methods in the overfitting and the data contamination. CeLEry provides a generic framework and can be implemented in multiple tasks depending on the research objectives, including the spatial coordinates discovery as well as the layer discovery. It can make use of the information of multiple tissues of spatial transcriptomics data. Thorough assessments exhibit that CeLEry achieves a leading performance compared to the state-of-art methods. We illustrated the usage of CeLEry in the discovery of neuron cell layers to study the development of Alzheimer's disease. The identified cell location information is valuable in many downstream analyses and can be indicative of the spatial organization of the tissues.
```

### Comparing `CeLEryPy-1.1.3/README.md` & `CeLEryPy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CeLEryPy-1.1.3/pyproject.toml` & `CeLEryPy-1.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CeLEryPy"
-version = "1.1.3"
+version = "1.2.1"
 description = "Leverage spatial transcriptomics data to recover cell locations in single-cell RNA RNA-seq"
 readme = "README.md"
 authors = [{ name = "Qihuang Zhang", email = "qihuang.zh@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,14 +20,14 @@
     "pandas >= 1.4",
     "numpy >= 1.20",
     "scipy",
     "tqdm",
     "scanpy >= 1.5",
     "scikit-image",
     "anndata",
-    "sklearn",
+    "scikit-learn",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/QihuangZhang/CeLEry"
```

