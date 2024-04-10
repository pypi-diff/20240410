# Comparing `tmp/scNovel-1.1.0.tar.gz` & `tmp/scNovel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scNovel-1.1.0.tar", last modified: Sun Feb 11 13:00:52 2024, max compression
+gzip compressed data, was "scNovel-1.2.0.tar", last modified: Wed Apr 10 07:02:03 2024, max compression
```

## Comparing `scNovel-1.1.0.tar` & `scNovel-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 13:00:52.269080 scNovel-1.1.0/
--rw-rw-rw-   0        0        0     1088 2024-02-11 12:47:24.000000 scNovel-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      369 2024-02-11 13:00:52.268075 scNovel-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2383 2024-02-11 12:48:25.000000 scNovel-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-11 13:00:52.256648 scNovel-1.1.0/scNovel/
--rw-rw-rw-   0        0        0     3801 2024-02-11 12:49:30.000000 scNovel-1.1.0/scNovel/__init__.py
--rw-rw-rw-   0        0        0     2626 2024-02-11 12:47:24.000000 scNovel-1.1.0/scNovel/scNovel_IO.py
--rw-rw-rw-   0        0        0     3068 2024-02-11 12:47:24.000000 scNovel-1.1.0/scNovel/scNovel_classifier.py
--rw-rw-rw-   0        0        0     7790 2024-02-11 12:47:24.000000 scNovel-1.1.0/scNovel/score_functions.py
--rw-rw-rw-   0        0        0      587 2024-02-11 12:47:24.000000 scNovel-1.1.0/scNovel/weightsampling.py
-drwxrwxrwx   0        0        0        0 2024-02-11 13:00:52.266794 scNovel-1.1.0/scNovel.egg-info/
--rw-rw-rw-   0        0        0      369 2024-02-11 13:00:52.000000 scNovel-1.1.0/scNovel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-02-11 13:00:52.000000 scNovel-1.1.0/scNovel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 13:00:52.000000 scNovel-1.1.0/scNovel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-02-11 13:00:52.000000 scNovel-1.1.0/scNovel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-11 13:00:52.269080 scNovel-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      487 2024-02-11 12:52:26.000000 scNovel-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:02:03.139969 scNovel-1.2.0/
+-rw-rw-rw-   0        0        0     1088 2024-02-11 12:47:24.000000 scNovel-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      369 2024-04-10 07:02:03.138969 scNovel-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2392 2024-04-10 06:57:57.000000 scNovel-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 07:02:03.124570 scNovel-1.2.0/scNovel/
+-rw-rw-rw-   0        0        0     3802 2024-04-10 06:57:43.000000 scNovel-1.2.0/scNovel/__init__.py
+-rw-rw-rw-   0        0        0     2650 2024-02-11 13:14:10.000000 scNovel-1.2.0/scNovel/scNovel_IO.py
+-rw-rw-rw-   0        0        0     3068 2024-02-11 12:47:24.000000 scNovel-1.2.0/scNovel/scNovel_classifier.py
+-rw-rw-rw-   0        0        0     7790 2024-02-11 12:47:24.000000 scNovel-1.2.0/scNovel/score_functions.py
+-rw-rw-rw-   0        0        0      587 2024-02-11 12:47:24.000000 scNovel-1.2.0/scNovel/weightsampling.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:02:03.137969 scNovel-1.2.0/scNovel.egg-info/
+-rw-rw-rw-   0        0        0      369 2024-04-10 07:02:03.000000 scNovel-1.2.0/scNovel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-04-10 07:02:03.000000 scNovel-1.2.0/scNovel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 07:02:03.000000 scNovel-1.2.0/scNovel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 07:02:03.000000 scNovel-1.2.0/scNovel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 07:02:03.140970 scNovel-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      487 2024-04-10 06:59:16.000000 scNovel-1.2.0/setup.py
```

### Comparing `scNovel-1.1.0/LICENSE` & `scNovel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scNovel-1.1.0/README.md` & `scNovel-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # scRare
 
 ## Introduction
 
-scRare, a neural network framework for novel rare cell deteciton, provides a fast, accurate and user-friendly novel rare cell detection for a new single-cell RNA-seq profile. By leveraging the newly designed neural network structure and proposed two new score functions, scRare especially obtains an outperformance on novel rare cell detection((up to 16.26% more AUROC compared to the second-best method)
+scRare, a neural network framework for novel rare cell detection, provides a fast, accurate and user-friendly novel rare cell detection for a new single-cell RNA-seq profile. By leveraging the newly designed neural network structure and proposed two new score functions, scRare especially obtains an outperformance on novel rare cell detection((up to 16.26% more AUROC compared to the second-best method). 
 
 ## Requirement
 
 - Scanpy (Compatible with all versions)
-- Pytorch (With Cudatoolkit is recommanded)
+- Pytorch (With Cudatoolkit is recommended)
 - Numpy > 1.20
 - Pandas > 1.2
 
 
 
 ## Installation
 
 ```Python
-pip install scNovel
+pip install scNovel==1.1.0
 ```
 
 ## Tutorial
 
 
 [scNovel Tutorial](Experiments/scNovel_Tutorial.ipynb)
```

### Comparing `scNovel-1.1.0/scNovel/__init__.py` & `scNovel-1.2.0/scNovel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from scNovel.weightsampling import Weighted_Sampling
 from scNovel.score_functions import get_ood_scores
 
 
 
 
 
-def scRare(test = None, reference = None, label = None, processing_unit = 'cuda',score_function="sim",iteration_number=3000):
+def scNovel(test = None, reference = None, label = None, processing_unit = 'cuda',score_function="sim",iteration_number=3000):
 
     '''
 
     :param test: Input your test dataset to annotate
     :param reference: Input your reference dataset
     :param label: Input label set
     :param processing_unit: Choose which processing unit you would like to use,
```

### Comparing `scNovel-1.1.0/scNovel/scNovel_IO.py` & `scNovel-1.2.0/scNovel/scNovel_IO.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 
         #turn to label matrix
         label.columns = ['Label']
         status_dict = label['Label'].unique().tolist()
         label['transfromed'] = label['Label'].apply(lambda x: status_dict.index(x))
         label_matrix = label['transfromed'].values
 
+        #return result
         count_matrix = adata.to_df()
         return count_matrix, label_matrix, status_dict
 
     else:
         count_matrix = adata.to_df()
 
         return count_matrix
```

### Comparing `scNovel-1.1.0/scNovel/scNovel_classifier.py` & `scNovel-1.2.0/scNovel/scNovel_classifier.py`

 * *Files identical despite different names*

### Comparing `scNovel-1.1.0/scNovel/score_functions.py` & `scNovel-1.2.0/scNovel/score_functions.py`

 * *Files identical despite different names*

### Comparing `scNovel-1.1.0/scNovel/weightsampling.py` & `scNovel-1.2.0/scNovel/weightsampling.py`

 * *Files identical despite different names*

