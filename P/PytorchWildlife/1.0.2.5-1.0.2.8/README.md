# Comparing `tmp/PytorchWildlife-1.0.2.5.tar.gz` & `tmp/PytorchWildlife-1.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PytorchWildlife-1.0.2.5.tar", last modified: Wed Mar 27 21:22:36 2024, max compression
+gzip compressed data, was "PytorchWildlife-1.0.2.8.tar", last modified: Tue Apr  9 22:43:58 2024, max compression
```

## Comparing `PytorchWildlife-1.0.2.5.tar` & `PytorchWildlife-1.0.2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     1070 2024-03-27 21:10:03.000000 PytorchWildlife-1.0.2.5/LICENSE
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)    20578 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/PKG-INFO
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PW_FT_classification/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       38 2024-03-27 21:10:03.000000 PytorchWildlife-1.0.2.5/PW_FT_classification/__init__.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     7449 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PW_FT_classification/main.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PytorchWildlife/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)      315 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/__init__.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PytorchWildlife/data/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       49 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/data/__init__.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     3764 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/data/datasets.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     5526 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/data/transforms.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PytorchWildlife/models/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       54 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/__init__.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       21 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/__init__.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)      100 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/__init__.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     3162 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/amazon.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     5315 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/base_classifier.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     2297 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/opossum.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     2548 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/serengeti.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       21 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/__init__.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       56 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/__init__.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     6024 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/base_detector.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     1499 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/megadetector.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/PytorchWildlife/utils/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       47 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/utils/__init__.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     1874 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/utils/misc.py
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     6032 2024-03-27 21:10:04.000000 PytorchWildlife-1.0.2.5/PytorchWildlife/utils/post_process.py
-drwxr-xr-x   0 andreshernandezcelisimetaver  (1028) users      (100)        0 2024-03-27 21:22:36.050019 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)    20578 2024-03-27 21:22:36.000000 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/PKG-INFO
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     1098 2024-03-27 21:22:36.000000 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/SOURCES.txt
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)        1 2024-03-27 21:22:36.000000 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/dependency_links.txt
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)      148 2024-03-27 21:22:36.000000 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/requires.txt
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       37 2024-03-27 21:22:36.000000 PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/top_level.txt
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)    19732 2024-03-27 21:21:57.000000 PytorchWildlife-1.0.2.5/README.md
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)       38 2024-03-27 21:22:36.054019 PytorchWildlife-1.0.2.5/setup.cfg
--rw-r--r--   0 andreshernandezcelisimetaver  (1028) users      (100)     1432 2024-03-27 21:18:20.000000 PytorchWildlife-1.0.2.5/setup.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.069585 PytorchWildlife-1.0.2.8/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     1070 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/LICENSE
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)    20648 2024-04-09 22:43:58.069056 PytorchWildlife-1.0.2.8/PKG-INFO
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.050755 PytorchWildlife-1.0.2.8/PW_FT_classification/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       38 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PW_FT_classification/__init__.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     7449 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PW_FT_classification/main.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.051464 PytorchWildlife-1.0.2.8/PytorchWildlife/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)      315 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/__init__.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.060665 PytorchWildlife-1.0.2.8/PytorchWildlife/data/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       49 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/__init__.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     3764 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/datasets.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     5526 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/transforms.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.061142 PytorchWildlife-1.0.2.8/PytorchWildlife/models/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       54 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/__init__.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.061715 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       21 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/__init__.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.064648 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)      100 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/__init__.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     3162 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/amazon.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     5315 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/base_classifier.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     2297 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/opossum.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     2548 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/serengeti.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.065041 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       21 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/__init__.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.066205 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       56 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/__init__.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     6024 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/base_detector.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     1499 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/megadetector.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.067602 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       47 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/__init__.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     1874 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/misc.py
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     6670 2024-04-09 22:31:58.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/post_process.py
+drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.068049 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)    20648 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/PKG-INFO
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     1098 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)        1 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)      148 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/requires.txt
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       37 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/top_level.txt
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)    19803 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/README.md
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)       38 2024-04-09 22:43:58.069643 PytorchWildlife-1.0.2.8/setup.cfg
+-rw-r--r--   0 zhongqimiao   (501) staff       (20)     1432 2024-04-09 22:37:03.000000 PytorchWildlife-1.0.2.8/setup.py
```

### Comparing `PytorchWildlife-1.0.2.5/LICENSE` & `PytorchWildlife-1.0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PKG-INFO` & `PytorchWildlife-1.0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PytorchWildlife
-Version: 1.0.2.5
+Version: 1.0.2.8
 Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
 Home-page: https://github.com/microsoft/CameraTraps/
 Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
 License: MIT
 Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha
@@ -31,15 +31,15 @@
 
 ![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
 
 <div align="center"> 
 <font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
 <br>
 <hr>
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://badge.fury.io/py/PytorchWildlife.svg" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
 <a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
 <a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
 <!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
 <a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
 <a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
@@ -48,14 +48,15 @@
 </div>
 
 
 ## ✅ Update highlights (Version 1.0.2)
 - [x] Added Google Colab demos.
 - [x] Added Snapshot Serengeti classification model into the model zoo.
 - [x] Added Classification fine-tuning module.
+- [x] Added a Docker Image for ease of installation.
 
 ## 🔥 Future highlights
 - [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
 - [ ] Direct Timelapse format outputs for both detection and classification.
 - [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
 - [ ] Direct LILA connection for more training/validation data.
 - [ ] More pretrained detection and classification models to expand the current model zoo.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.5 Summary: a PyTorch
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.8 Summary: a PyTorch
 Collaborative Deep Learning Framework for Conservation. Home-page: https://
 github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
 Keywords:
 pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -14,53 +14,54 @@
 Requires-Dist: torchvision==0.11.2 Requires-Dist: torchaudio==0.10.1 Requires-
 Dist: tqdm==4.66.1 Requires-Dist: Pillow==10.1.0 Requires-Dist:
 supervision==0.16.0 Requires-Dist: gradio==4.8.0 Requires-Dist: ultralytics-
 yolov5 Requires-Dist: chardet ![image](https://microsoft.github.io/CameraTraps/
 assets/Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
-_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:
-   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-_D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-    _b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
-       _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-_J_o_i_n___u_s_!_-
-                       _b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
+_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
+ _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
+   _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
+ _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
+                   _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
 ## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
 Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. ## ð¥ Future highlights - [ ]
-MegaDetectorV6 with multiple model sizes for both optimized performance and
-low-budget devices like camera systems. - [ ] Direct Timelapse format outputs
-for both detection and classification. - [ ] A detection model fine-tuning
-module to fine-tune your own detection model for Pytorch-Wildlife. - [ ] Direct
-LILA connection for more training/validation data. - [ ] More pretrained
-detection and classification models to expand the current model zoo. To check
-the full version of the roadmap with completed tasks and long term goals,
-please click [here!](roadmaps.md). ## ð¾ Introduction At the core of our
-mission is the desire to create a harmonious space where conservation
-scientists from all over the globe can unite. Where they're able to share,
-grow, use datasets and deep learning architectures for wildlife conservation.
-We've been inspired by the potential and capabilities of Megadetector, and we
-deeply value its contributions to the community. As we forge ahead with
-Pytorch-Wildlife, under which Megadetector now resides, please know that we
-remain committed to supporting, maintaining, and developing Megadetector,
-ensuring its continued relevance, expansion, and utility. Pytorch-Wildlife is
-pip installable: ``` pip install PytorchWildlife ``` To use the newest version
-of MegaDetector with all the existing functionalities, you can use our [Hugging
-Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or
-simply load the model with **Pytorch-Wildlife**. The weights will be
-automatically downloaded: ```python from PytorchWildlife.models import
-detection as pw_detection detection_model = pw_detection.MegaDetectorV5() ```
-For those interested in accessing the previous MegaDetector repository, which
-utilizes the same `MegaDetector v5` model weights and was primarily developed
-by Dan Morris during his time at Microsoft, please visit the [archive](https://
-github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit
-this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main)
-that Dan Morris is actively maintaining. >[!TIP] >If you have any questions
+Classification fine-tuning module. - [x] Added a Docker Image for ease of
+installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
+model sizes for both optimized performance and low-budget devices like camera
+systems. - [ ] Direct Timelapse format outputs for both detection and
+classification. - [ ] A detection model fine-tuning module to fine-tune your
+own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
+training/validation data. - [ ] More pretrained detection and classification
+models to expand the current model zoo. To check the full version of the
+roadmap with completed tasks and long term goals, please click [here!]
+(roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
+create a harmonious space where conservation scientists from all over the globe
+can unite. Where they're able to share, grow, use datasets and deep learning
+architectures for wildlife conservation. We've been inspired by the potential
+and capabilities of Megadetector, and we deeply value its contributions to the
+community. As we forge ahead with Pytorch-Wildlife, under which Megadetector
+now resides, please know that we remain committed to supporting, maintaining,
+and developing Megadetector, ensuring its continued relevance, expansion, and
+utility. Pytorch-Wildlife is pip installable: ``` pip install PytorchWildlife
+``` To use the newest version of MegaDetector with all the existing
+functionalities, you can use our [Hugging Face interface](https://
+huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model
+with **Pytorch-Wildlife**. The weights will be automatically downloaded:
+```python from PytorchWildlife.models import detection as pw_detection
+detection_model = pw_detection.MegaDetectorV5() ``` For those interested in
+accessing the previous MegaDetector repository, which utilizes the same
+`MegaDetector v5` model weights and was primarily developed by Dan Morris
+during his time at Microsoft, please visit the [archive](https://github.com/
+microsoft/CameraTraps/blob/main/archive) directory, or you can visit this
+[forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that
+Dan Morris is actively maintaining. >[!TIP] >If you have any questions
 regarding MegaDetector and Pytorch-Wildlife, please [email us]
 (zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://
 img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)]
 (https://discord.gg/TeEVxzaYtm) ## ð Welcome to Pytorch-Wildlife Version 1.0
 **PyTorch-Wildlife** is a platform to create, modify, and share powerful AI
 conservation models. These models can be used for a variety of applications,
 including camera trap images, overhead images, underwater images, or
```

### Comparing `PytorchWildlife-1.0.2.5/PW_FT_classification/main.py` & `PytorchWildlife-1.0.2.8/PW_FT_classification/main.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/data/datasets.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/data/datasets.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/data/transforms.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/data/transforms.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/amazon.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/amazon.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/base_classifier.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/base_classifier.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/opossum.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/opossum.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/classification/resnet/serengeti.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/serengeti.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/base_detector.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/base_detector.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/models/detection/yolov5/megadetector.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/megadetector.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/utils/misc.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife/utils/post_process.py` & `PytorchWildlife-1.0.2.8/PytorchWildlife/utils/post_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,38 +77,51 @@
                     image=cv2.cvtColor(cropped_img, cv2.COLOR_RGB2BGR),
                     image_name="{}_{}_{}".format(
                         int(cat), i, entry["img_id"].rsplit(os.sep, 1)[1]
                     ),
                 )
 
 
-def save_detection_json(results, output_dir, categories=None):
+def save_detection_json(results, output_dir, categories=None, exclude_category_ids=[]):
     """
     Save detection results to a JSON file.
 
     Args:
         results (list):
             Detection results containing image ID, bounding boxes, category, and confidence.
         output_dir (str):
             Path to save the output JSON file.
         categories (list, optional):
             List of categories for detected objects. Defaults to None.
+        exclude_category_ids (list, optional):
+            List of category IDs to exclude from the output. Defaults to []. Category IDs can be found in the definition of each models.
     """
     json_results = {"annotations": [], "categories": categories}
     with open(output_dir, "w") as f:
         for r in results:
-            json_results["annotations"].append(
-                {
-                    "img_id": r["img_id"],
-                    "bbox": r["detections"].xyxy.astype(int).tolist(),
-                    "category": r["detections"].class_id.tolist(),
-                    "confidence": r["detections"].confidence.tolist(),
-                }
-            )
-        json.dump(json_results, f)
+
+            # Category filtering
+            img_id = r["img_id"]
+            category = r["detections"].class_id
+
+            bbox = r["detections"].xyxy.astype(int)[~np.isin(category, exclude_category_ids)]
+            confidence =  r["detections"].confidence[~np.isin(category, exclude_category_ids)]
+            category = category[~np.isin(category, exclude_category_ids)]
+
+            if not all([x in exclude_category_ids for x in category]):
+                json_results["annotations"].append(
+                    {
+                        "img_id": img_id,
+                        "bbox": bbox.tolist(),
+                        "category": category.tolist(),
+                        "confidence": confidence.tolist(),
+                    }
+                )
+
+        json.dump(json_results, f, indent=4)
 
 
 def save_detection_classification_json(
     det_results, clf_results, output_path, det_categories=None, clf_categories=None
 ):
     """
     Save classification results to a JSON file.
```

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/PKG-INFO` & `PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PytorchWildlife
-Version: 1.0.2.5
+Version: 1.0.2.8
 Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
 Home-page: https://github.com/microsoft/CameraTraps/
 Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
 License: MIT
 Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha
@@ -31,15 +31,15 @@
 
 ![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
 
 <div align="center"> 
 <font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
 <br>
 <hr>
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://badge.fury.io/py/PytorchWildlife.svg" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
 <a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
 <a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
 <!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
 <a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
 <a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
@@ -48,14 +48,15 @@
 </div>
 
 
 ## ✅ Update highlights (Version 1.0.2)
 - [x] Added Google Colab demos.
 - [x] Added Snapshot Serengeti classification model into the model zoo.
 - [x] Added Classification fine-tuning module.
+- [x] Added a Docker Image for ease of installation.
 
 ## 🔥 Future highlights
 - [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
 - [ ] Direct Timelapse format outputs for both detection and classification.
 - [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
 - [ ] Direct LILA connection for more training/validation data.
 - [ ] More pretrained detection and classification models to expand the current model zoo.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.5 Summary: a PyTorch
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.8 Summary: a PyTorch
 Collaborative Deep Learning Framework for Conservation. Home-page: https://
 github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
 Keywords:
 pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -14,53 +14,54 @@
 Requires-Dist: torchvision==0.11.2 Requires-Dist: torchaudio==0.10.1 Requires-
 Dist: tqdm==4.66.1 Requires-Dist: Pillow==10.1.0 Requires-Dist:
 supervision==0.16.0 Requires-Dist: gradio==4.8.0 Requires-Dist: ultralytics-
 yolov5 Requires-Dist: chardet ![image](https://microsoft.github.io/CameraTraps/
 assets/Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
-_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:
-   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-_D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-    _b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
-       _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-_J_o_i_n___u_s_!_-
-                       _b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
+_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
+ _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
+   _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
+ _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
+                   _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
 ## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
 Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. ## ð¥ Future highlights - [ ]
-MegaDetectorV6 with multiple model sizes for both optimized performance and
-low-budget devices like camera systems. - [ ] Direct Timelapse format outputs
-for both detection and classification. - [ ] A detection model fine-tuning
-module to fine-tune your own detection model for Pytorch-Wildlife. - [ ] Direct
-LILA connection for more training/validation data. - [ ] More pretrained
-detection and classification models to expand the current model zoo. To check
-the full version of the roadmap with completed tasks and long term goals,
-please click [here!](roadmaps.md). ## ð¾ Introduction At the core of our
-mission is the desire to create a harmonious space where conservation
-scientists from all over the globe can unite. Where they're able to share,
-grow, use datasets and deep learning architectures for wildlife conservation.
-We've been inspired by the potential and capabilities of Megadetector, and we
-deeply value its contributions to the community. As we forge ahead with
-Pytorch-Wildlife, under which Megadetector now resides, please know that we
-remain committed to supporting, maintaining, and developing Megadetector,
-ensuring its continued relevance, expansion, and utility. Pytorch-Wildlife is
-pip installable: ``` pip install PytorchWildlife ``` To use the newest version
-of MegaDetector with all the existing functionalities, you can use our [Hugging
-Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or
-simply load the model with **Pytorch-Wildlife**. The weights will be
-automatically downloaded: ```python from PytorchWildlife.models import
-detection as pw_detection detection_model = pw_detection.MegaDetectorV5() ```
-For those interested in accessing the previous MegaDetector repository, which
-utilizes the same `MegaDetector v5` model weights and was primarily developed
-by Dan Morris during his time at Microsoft, please visit the [archive](https://
-github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit
-this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main)
-that Dan Morris is actively maintaining. >[!TIP] >If you have any questions
+Classification fine-tuning module. - [x] Added a Docker Image for ease of
+installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
+model sizes for both optimized performance and low-budget devices like camera
+systems. - [ ] Direct Timelapse format outputs for both detection and
+classification. - [ ] A detection model fine-tuning module to fine-tune your
+own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
+training/validation data. - [ ] More pretrained detection and classification
+models to expand the current model zoo. To check the full version of the
+roadmap with completed tasks and long term goals, please click [here!]
+(roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
+create a harmonious space where conservation scientists from all over the globe
+can unite. Where they're able to share, grow, use datasets and deep learning
+architectures for wildlife conservation. We've been inspired by the potential
+and capabilities of Megadetector, and we deeply value its contributions to the
+community. As we forge ahead with Pytorch-Wildlife, under which Megadetector
+now resides, please know that we remain committed to supporting, maintaining,
+and developing Megadetector, ensuring its continued relevance, expansion, and
+utility. Pytorch-Wildlife is pip installable: ``` pip install PytorchWildlife
+``` To use the newest version of MegaDetector with all the existing
+functionalities, you can use our [Hugging Face interface](https://
+huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model
+with **Pytorch-Wildlife**. The weights will be automatically downloaded:
+```python from PytorchWildlife.models import detection as pw_detection
+detection_model = pw_detection.MegaDetectorV5() ``` For those interested in
+accessing the previous MegaDetector repository, which utilizes the same
+`MegaDetector v5` model weights and was primarily developed by Dan Morris
+during his time at Microsoft, please visit the [archive](https://github.com/
+microsoft/CameraTraps/blob/main/archive) directory, or you can visit this
+[forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that
+Dan Morris is actively maintaining. >[!TIP] >If you have any questions
 regarding MegaDetector and Pytorch-Wildlife, please [email us]
 (zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://
 img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)]
 (https://discord.gg/TeEVxzaYtm) ## ð Welcome to Pytorch-Wildlife Version 1.0
 **PyTorch-Wildlife** is a platform to create, modify, and share powerful AI
 conservation models. These models can be used for a variety of applications,
 including camera trap images, overhead images, underwater images, or
```

### Comparing `PytorchWildlife-1.0.2.5/PytorchWildlife.egg-info/SOURCES.txt` & `PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.5/README.md` & `PytorchWildlife-1.0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
 
 <div align="center"> 
 <font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
 <br>
 <hr>
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://badge.fury.io/py/PytorchWildlife.svg" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
 <a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
 <a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
 <!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
 <a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
 <a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
@@ -17,14 +17,15 @@
 </div>
 
 
 ## ✅ Update highlights (Version 1.0.2)
 - [x] Added Google Colab demos.
 - [x] Added Snapshot Serengeti classification model into the model zoo.
 - [x] Added Classification fine-tuning module.
+- [x] Added a Docker Image for ease of installation.
 
 ## 🔥 Future highlights
 - [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
 - [ ] Direct Timelapse format outputs for both detection and classification.
 - [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
 - [ ] Direct LILA connection for more training/validation data.
 - [ ] More pretrained detection and classification models to expand the current model zoo.
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
 ![image](https://microsoft.github.io/CameraTraps/assets/
 Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
-_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/
-_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:
-   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-_D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-    _b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/
-       _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-_J_o_i_n___u_s_!_-
-                       _b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
+_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
+ _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
+   _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
+ _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
+                   _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
 ## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
 Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. ## ð¥ Future highlights - [ ]
-MegaDetectorV6 with multiple model sizes for both optimized performance and
-low-budget devices like camera systems. - [ ] Direct Timelapse format outputs
-for both detection and classification. - [ ] A detection model fine-tuning
-module to fine-tune your own detection model for Pytorch-Wildlife. - [ ] Direct
-LILA connection for more training/validation data. - [ ] More pretrained
-detection and classification models to expand the current model zoo. To check
-the full version of the roadmap with completed tasks and long term goals,
-please click [here!](roadmaps.md). ## ð¾ Introduction At the core of our
-mission is the desire to create a harmonious space where conservation
-scientists from all over the globe can unite. Where they're able to share,
-grow, use datasets and deep learning architectures for wildlife conservation.
-We've been inspired by the potential and capabilities of Megadetector, and we
-deeply value its contributions to the community. As we forge ahead with
-Pytorch-Wildlife, under which Megadetector now resides, please know that we
-remain committed to supporting, maintaining, and developing Megadetector,
-ensuring its continued relevance, expansion, and utility. Pytorch-Wildlife is
-pip installable: ``` pip install PytorchWildlife ``` To use the newest version
-of MegaDetector with all the existing functionalities, you can use our [Hugging
-Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or
-simply load the model with **Pytorch-Wildlife**. The weights will be
-automatically downloaded: ```python from PytorchWildlife.models import
-detection as pw_detection detection_model = pw_detection.MegaDetectorV5() ```
-For those interested in accessing the previous MegaDetector repository, which
-utilizes the same `MegaDetector v5` model weights and was primarily developed
-by Dan Morris during his time at Microsoft, please visit the [archive](https://
-github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit
-this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main)
-that Dan Morris is actively maintaining. >[!TIP] >If you have any questions
+Classification fine-tuning module. - [x] Added a Docker Image for ease of
+installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
+model sizes for both optimized performance and low-budget devices like camera
+systems. - [ ] Direct Timelapse format outputs for both detection and
+classification. - [ ] A detection model fine-tuning module to fine-tune your
+own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
+training/validation data. - [ ] More pretrained detection and classification
+models to expand the current model zoo. To check the full version of the
+roadmap with completed tasks and long term goals, please click [here!]
+(roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
+create a harmonious space where conservation scientists from all over the globe
+can unite. Where they're able to share, grow, use datasets and deep learning
+architectures for wildlife conservation. We've been inspired by the potential
+and capabilities of Megadetector, and we deeply value its contributions to the
+community. As we forge ahead with Pytorch-Wildlife, under which Megadetector
+now resides, please know that we remain committed to supporting, maintaining,
+and developing Megadetector, ensuring its continued relevance, expansion, and
+utility. Pytorch-Wildlife is pip installable: ``` pip install PytorchWildlife
+``` To use the newest version of MegaDetector with all the existing
+functionalities, you can use our [Hugging Face interface](https://
+huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model
+with **Pytorch-Wildlife**. The weights will be automatically downloaded:
+```python from PytorchWildlife.models import detection as pw_detection
+detection_model = pw_detection.MegaDetectorV5() ``` For those interested in
+accessing the previous MegaDetector repository, which utilizes the same
+`MegaDetector v5` model weights and was primarily developed by Dan Morris
+during his time at Microsoft, please visit the [archive](https://github.com/
+microsoft/CameraTraps/blob/main/archive) directory, or you can visit this
+[forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that
+Dan Morris is actively maintaining. >[!TIP] >If you have any questions
 regarding MegaDetector and Pytorch-Wildlife, please [email us]
 (zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://
 img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)]
 (https://discord.gg/TeEVxzaYtm) ## ð Welcome to Pytorch-Wildlife Version 1.0
 **PyTorch-Wildlife** is a platform to create, modify, and share powerful AI
 conservation models. These models can be used for a variety of applications,
 including camera trap images, overhead images, underwater images, or
```

### Comparing `PytorchWildlife-1.0.2.5/setup.py` & `PytorchWildlife-1.0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding="utf8") as file:
         long_description = file.read()
 setup(
     name='PytorchWildlife',
-    version='1.0.2.5', 
+    version='1.0.2.8', 
     packages=find_packages(),
     url='https://github.com/microsoft/CameraTraps/',  
     license='MIT',
     author='Andres Hernandez, Zhongqi Miao',
     author_email='v-herandres@microsoft.com, zhongqimiao@microsoft.com',  
     description='a PyTorch Collaborative Deep Learning Framework for Conservation.',
     long_description=long_description,
```

