# Comparing `tmp/neural-commons-0.0.6.tar.gz` & `tmp/neural-commons-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.0.6.tar", last modified: Wed Apr 10 16:50:10 2024, max compression
+gzip compressed data, was "neural-commons-0.0.7.tar", last modified: Wed Apr 10 17:10:50 2024, max compression
```

## Comparing `neural-commons-0.0.6.tar` & `neural-commons-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.176476 neural-commons-0.0.6/
--rw-rw-rw-   0        0        0      455 2024-04-10 16:50:10.175478 neural-commons-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.153478 neural-commons-0.0.6/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.160478 neural-commons-0.0.6/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0    10089 2024-04-08 14:26:47.000000 neural-commons-0.0.6/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.174477 neural-commons-0.0.6/neural_commons/modules/
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0     2818 2024-04-08 14:36:12.000000 neural-commons-0.0.6/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      844 2024-04-10 16:44:22.000000 neural-commons-0.0.6/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0     1350 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/PreTrainedLayer.py
--rw-rw-rw-   0        0        0      886 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.0.6/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      300 2024-04-07 23:57:05.000000 neural-commons-0.0.6/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:50:10.158478 neural-commons-0.0.6/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      757 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 16:50:10.000000 neural-commons-0.0.6/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 16:50:10.176476 neural-commons-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      968 2024-04-10 16:46:59.000000 neural-commons-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:10:50.591752 neural-commons-0.0.7/
+-rw-rw-rw-   0        0        0      455 2024-04-10 17:10:50.590751 neural-commons-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 17:10:50.570753 neural-commons-0.0.7/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:10:50.575751 neural-commons-0.0.7/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0    10089 2024-04-08 14:26:47.000000 neural-commons-0.0.7/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:10:50.588752 neural-commons-0.0.7/neural_commons/modules/
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0     2818 2024-04-08 14:36:12.000000 neural-commons-0.0.7/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      844 2024-04-10 16:44:22.000000 neural-commons-0.0.7/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0     1350 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/PreTrainedLayer.py
+-rw-rw-rw-   0        0        0      886 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.0.7/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.0.7/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      342 2024-04-10 17:10:01.000000 neural-commons-0.0.7/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:10:50.574753 neural-commons-0.0.7/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-04-10 17:10:50.000000 neural-commons-0.0.7/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2024-04-10 17:10:50.000000 neural-commons-0.0.7/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:10:50.000000 neural-commons-0.0.7/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-10 17:10:50.000000 neural-commons-0.0.7/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 17:10:50.000000 neural-commons-0.0.7/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 17:10:50.591752 neural-commons-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      968 2024-04-10 17:10:10.000000 neural-commons-0.0.7/setup.py
```

### Comparing `neural-commons-0.0.6/neural_commons/helpers/torch_helper.py` & `neural-commons-0.0.7/neural_commons/helpers/torch_helper.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.0.7/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.0.7/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/PreTrainedLayer.py` & `neural-commons-0.0.7/neural_commons/modules/PreTrainedLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/RndNonLinearFunction.py` & `neural-commons-0.0.7/neural_commons/modules/RndNonLinearFunction.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/RndProjection.py` & `neural-commons-0.0.7/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/SMoE.py` & `neural-commons-0.0.7/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.0.7/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.0.7/neural_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-commons-0.0.6/setup.py` & `neural-commons-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.0.0',
```

