# Comparing `tmp/python-iArt-1.0.0.tar.gz` & `tmp/python-iArt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iArt-1.0.0.tar", last modified: Tue Apr  9 04:14:38 2024, max compression
+gzip compressed data, was "python-iArt-1.0.1.tar", last modified: Wed Apr 10 06:34:07 2024, max compression
```

## Comparing `python-iArt-1.0.0.tar` & `python-iArt-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.621149 python-iArt-1.0.0/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-09 04:14:38.620740 python-iArt-1.0.0/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.0/README.md
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.617679 python-iArt-1.0.0/iArt/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.0/iArt/__init__.py
--rw-r--r--   0 jiaweizhang   (501) staff       (20)    18113 2024-04-09 03:47:51.000000 python-iArt-1.0.0/iArt/iArt.py
-drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-09 04:14:38.619996 python-iArt-1.0.0/python_iArt.egg-info/
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/PKG-INFO
--rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/SOURCES.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/dependency_links.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/requires.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-09 04:14:38.000000 python-iArt-1.0.0/python_iArt.egg-info/top_level.txt
--rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-09 04:14:38.621318 python-iArt-1.0.0/setup.cfg
--rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-09 04:14:30.000000 python-iArt-1.0.0/setup.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-10 06:34:07.472749 python-iArt-1.0.1/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-10 06:34:07.472393 python-iArt-1.0.1/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     3930 2024-04-09 03:41:46.000000 python-iArt-1.0.1/README.md
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-10 06:34:07.469592 python-iArt-1.0.1/iArt/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       48 2024-04-09 03:34:10.000000 python-iArt-1.0.1/iArt/__init__.py
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)    18099 2024-04-10 06:33:23.000000 python-iArt-1.0.1/iArt/iArt.py
+drwxr-xr-x   0 jiaweizhang   (501) staff       (20)        0 2024-04-10 06:34:07.471707 python-iArt-1.0.1/python_iArt.egg-info/
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     5230 2024-04-10 06:34:07.000000 python-iArt-1.0.1/python_iArt.egg-info/PKG-INFO
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)      222 2024-04-10 06:34:07.000000 python-iArt-1.0.1/python_iArt.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        1 2024-04-10 06:34:07.000000 python-iArt-1.0.1/python_iArt.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       66 2024-04-10 06:34:07.000000 python-iArt-1.0.1/python_iArt.egg-info/requires.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)        5 2024-04-10 06:34:07.000000 python-iArt-1.0.1/python_iArt.egg-info/top_level.txt
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)       38 2024-04-10 06:34:07.472923 python-iArt-1.0.1/setup.cfg
+-rw-r--r--   0 jiaweizhang   (501) staff       (20)     1059 2024-04-10 06:33:55.000000 python-iArt-1.0.1/setup.py
```

### Comparing `python-iArt-1.0.0/PKG-INFO` & `python-iArt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.0
+Version: 1.0.1
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.0/README.md` & `python-iArt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-iArt-1.0.0/iArt/iArt.py` & `python-iArt-1.0.1/iArt/iArt.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         if len(columns_to_impute)>0:
             print(f"Missing Rate After Imputation for X: {missing_rate_after * 100}")
             print(f"Columns Imputed for X: {imputed_columns}")
         print(f"Columns Not Imputed for X: {not_imputed_columns}")
     
     return X
 
-def test(*,Z, X, Y, G='bayesianridge', S=None,L = 10000,threshholdForX = 0.2, mode = 'strata',verbose = False, covariate_adjustment = 0, random_state=None, alternative = "greater", alpha = 0.05):
+def test(*,Z, X, Y, G='linear', S=None,L = 10000,threshholdForX = 0.2, mode = 'strata',verbose = False, covariate_adjustment = 0, random_state=None, alternative = "greater", alpha = 0.05):
     """Imputation-Assisted Randomization Tests (iArt) for testing 
     the null hypothesis that the treatment has no effect on the outcome.
 
     Parameters
     ----------
     Z : array_like
         Z is the array of observed treatment indicators
@@ -356,15 +356,15 @@
     
     S : array_like, default: None
         S is the array of observed strata indicators
         
     threshholdForX : float, default: 0.1
         The threshhold for missing outcome to be imputed in advance in covariate X
 
-    G : str or function, default: 'bayesianridge'
+    G : str or function, default: 'linear'
         A string for the eight available choice or a function that takes 
         (Z, M, Y_k) as input and returns the imputed complete values 
 
     L : int, default: 10000
         The number of Monte Carlo simulations 
 
     mode : {'strata','cluster'}, default: 'strata'
```

### Comparing `python-iArt-1.0.0/python_iArt.egg-info/PKG-INFO` & `python-iArt-1.0.1/python_iArt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iArt
-Version: 1.0.0
+Version: 1.0.1
 Summary: iArt: A Generalized Framework for Imputation-Assisted Randomization Tests
 Home-page: https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py
 Author: Siyu Heng, Jiawei Zhang, and Yang Feng
 Author-email: siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu
 License: UNKNOWN
 Description: # iArt: Imputation-Assisted Randomization Tests
```

### Comparing `python-iArt-1.0.0/setup.py` & `python-iArt-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="python-iArt",
-    version="1.0.0",
+    version="1.0.1",
     author="Siyu Heng, Jiawei Zhang, and Yang Feng",
     author_email="siyuheng@nyu.edu,jz4721@nyu.edu,yang.feng@nyu.edu",
     description="iArt: A Generalized Framework for Imputation-Assisted Randomization Tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Imputation-Assisted-Randomization-Tests/iArt-py",
     packages=find_packages(),
```

