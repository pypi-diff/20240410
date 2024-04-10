# Comparing `tmp/deepof-0.6.tar.gz` & `tmp/deepof-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepof-0.6.tar", last modified: Wed Nov 15 10:44:57 2023, max compression
+gzip compressed data, was "deepof-0.6.1.tar", max compression
```

## Comparing `deepof-0.6.tar` & `deepof-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,18 @@
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.387410 deepof-0.6/
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     1070 2023-11-06 00:21:53.000000 deepof-0.6/LICENSE
--rw-r--r--   0 lucasmiranda   (501) staff       (20)       77 2023-11-06 00:21:53.000000 deepof-0.6/MANIFEST.in
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    12503 2023-11-15 10:44:57.387134 deepof-0.6/PKG-INFO
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     9799 2023-11-15 10:32:07.000000 deepof-0.6/README.md
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.367048 deepof-0.6/deepof/
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     6148 2023-11-15 10:38:41.000000 deepof-0.6/deepof/.DS_Store
--rw-r--r--   0 lucasmiranda   (501) staff       (20)       38 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__init__.py
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.373717 deepof-0.6/deepof/__pycache__/
--rw-r--r--   0 lucasmiranda   (501) staff       (20)      104 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)      153 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    55981 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/data.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     8804 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/hypermodels.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     2802 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/hypermodels.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    14803 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/model_utils.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    18566 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/model_utils.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     9325 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    16680 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    26124 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/pose_utils.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    26524 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/preprocess.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    37167 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    41428 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     4586 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/visuals.cpython-36.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     3538 2023-11-06 00:21:53.000000 deepof-0.6/deepof/__pycache__/visuals.cpython-39.pyc
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    29664 2023-11-06 00:21:53.000000 deepof-0.6/deepof/annotation_utils.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)   103948 2023-11-06 00:21:53.000000 deepof-0.6/deepof/data.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    15179 2023-11-06 00:21:53.000000 deepof-0.6/deepof/deepof_train_embeddings.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     8268 2023-11-06 00:21:53.000000 deepof-0.6/deepof/hypermodels.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    61514 2023-11-06 00:21:53.000000 deepof-0.6/deepof/model_utils.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    78570 2023-11-06 00:21:53.000000 deepof-0.6/deepof/models.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    49719 2023-11-06 00:21:53.000000 deepof-0.6/deepof/post_hoc.py
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.374343 deepof-0.6/deepof/trained_models/
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     6148 2023-11-15 10:38:41.000000 deepof-0.6/deepof/trained_models/.DS_Store
--rw-r--r--   0 lucasmiranda   (501) staff       (20)        0 2023-11-06 00:21:53.000000 deepof-0.6/deepof/trained_models/.gitkeep
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.376549 deepof-0.6/deepof/trained_models/deepof_supervised/
--rw-r--r--   0 lucasmiranda   (501) staff       (20) 10139395 2023-11-15 10:37:13.000000 deepof-0.6/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    76742 2023-11-06 00:21:53.000000 deepof-0.6/deepof/utils.py
--rw-r--r--   0 lucasmiranda   (501) staff       (20)   100735 2023-11-06 00:21:53.000000 deepof-0.6/deepof/visuals.py
-drwxr-xr-x   0 lucasmiranda   (501) staff       (20)        0 2023-11-15 10:44:57.368420 deepof-0.6/deepof.egg-info/
--rw-r--r--   0 lucasmiranda   (501) staff       (20)    12503 2023-11-15 10:44:57.000000 deepof-0.6/deepof.egg-info/PKG-INFO
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     1217 2023-11-15 10:44:57.000000 deepof-0.6/deepof.egg-info/SOURCES.txt
--rw-r--r--   0 lucasmiranda   (501) staff       (20)        1 2023-11-15 10:44:57.000000 deepof-0.6/deepof.egg-info/dependency_links.txt
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     1234 2023-11-15 10:44:57.000000 deepof-0.6/deepof.egg-info/requires.txt
--rw-r--r--   0 lucasmiranda   (501) staff       (20)        7 2023-11-15 10:44:57.000000 deepof-0.6/deepof.egg-info/top_level.txt
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     1344 2023-11-06 00:27:13.000000 deepof-0.6/requirements.txt
--rw-r--r--   0 lucasmiranda   (501) staff       (20)       38 2023-11-15 10:44:57.387457 deepof-0.6/setup.cfg
--rw-r--r--   0 lucasmiranda   (501) staff       (20)     1027 2023-11-15 10:44:34.000000 deepof-0.6/setup.py
+-rw-r--r--   0        0        0     1070 2023-11-06 00:21:53.366438 deepof-0.6.1/LICENSE
+-rw-r--r--   0        0        0     9801 2024-04-10 15:21:33.390157 deepof-0.6.1/README.md
+-rw-r--r--   0        0        0     6148 2023-11-15 10:38:41.176080 deepof-0.6.1/deepof/.DS_Store
+-rw-r--r--   0        0        0       38 2023-11-06 00:21:53.366751 deepof-0.6.1/deepof/__init__.py
+-rw-r--r--   0        0        0    29664 2023-11-06 00:21:53.368751 deepof-0.6.1/deepof/annotation_utils.py
+-rw-r--r--   0        0        0   103948 2024-04-01 13:48:27.887411 deepof-0.6.1/deepof/data.py
+-rw-r--r--   0        0        0    15179 2023-11-06 00:21:53.369068 deepof-0.6.1/deepof/deepof_train_embeddings.py
+-rw-r--r--   0        0        0     8268 2023-11-06 00:21:53.369153 deepof-0.6.1/deepof/hypermodels.py
+-rw-r--r--   0        0        0    61514 2023-12-03 17:30:37.818174 deepof-0.6.1/deepof/model_utils.py
+-rw-r--r--   0        0        0    78570 2023-11-06 00:21:53.369434 deepof-0.6.1/deepof/models.py
+-rw-r--r--   0        0        0    49719 2023-12-08 11:46:57.236557 deepof-0.6.1/deepof/post_hoc.py
+-rw-r--r--   0        0        0     6148 2023-11-15 10:38:41.178048 deepof-0.6.1/deepof/trained_models/.DS_Store
+-rw-r--r--   0        0        0        0 2023-11-06 00:21:53.369733 deepof-0.6.1/deepof/trained_models/.gitkeep
+-rw-r--r--   0        0        0      133 2023-12-03 17:30:37.819353 deepof-0.6.1/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
+-rw-r--r--   0        0        0    76742 2023-11-06 00:21:53.369979 deepof-0.6.1/deepof/utils.py
+-rw-r--r--   0        0        0   100735 2024-04-01 13:48:27.889276 deepof-0.6.1/deepof/visuals.py
+-rw-r--r--   0        0        0     3211 2024-04-10 16:13:41.009681 deepof-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    12476 1970-01-01 00:00:00.000000 deepof-0.6.1/PKG-INFO
```

### Comparing `deepof-0.6/LICENSE` & `deepof-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepof-0.6/PKG-INFO` & `deepof-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,72 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.6
-Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut amd SLEAP
-Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
-Author: Lucas Miranda
+Version: 0.6.1
+Summary: 
+Author: lucas_miranda
 Author-email: lucas_miranda@psych.mpg.de
+Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: POT (>=0.8.2,<0.9.0)
+Requires-Dist: Shapely (>=1.8.4,<2.0.0)
+Requires-Dist: av (==9.2.0)
+Requires-Dist: catboost (>=1.1.1,<2.0.0)
+Requires-Dist: dask-image (>=2022.9.0,<2023.0.0)
+Requires-Dist: h5py (>=3.7.0,<4.0.0)
+Requires-Dist: imageio-ffmpeg (>=0.4.7,<0.5.0)
+Requires-Dist: imblearn (>=0.0,<0.1)
+Requires-Dist: ipykernel (>=6.16.0,<7.0.0)
+Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
+Requires-Dist: jupyter-client (==7.3.2)
+Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: keras-tcn (>=3.5.0,<4.0.0) ; platform_machine != "arm64" or platform_system != "Darwin"
+Requires-Dist: keras-tcn-macos (>=1.0,<2.0) ; platform_machine == "arm64" and platform_system == "Darwin"
+Requires-Dist: keras-tuner (>=1.0.3,<2.0.0) ; platform_machine != "arm64" or platform_system != "Darwin"
+Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: matplotlib (==3.7.2)
+Requires-Dist: moviepy (>=1.0.3,<2.0.0)
+Requires-Dist: networkx (>=2.8.7,<3.0.0)
+Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pomegranate (==1.0.4)
+Requires-Dist: regex (>=2022.9.13,<2023.0.0)
+Requires-Dist: ruptures (==1.1.8)
+Requires-Dist: scikit-learn (==1.2.0)
+Requires-Dist: seglearn (>=1.2.5,<2.0.0)
+Requires-Dist: segment-anything (>=1.0,<2.0)
+Requires-Dist: shap (>=0.41.0,<0.42.0)
+Requires-Dist: sktime (>=0.24.0,<0.25.0)
+Requires-Dist: sleap-io (>=0.0.9,<0.0.10)
+Requires-Dist: spektral (==1.3.1)
+Requires-Dist: statannotations (>=0.5.0,<0.6.0)
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Requires-Dist: tables (==3.8.0)
+Requires-Dist: tensorflow (==2.11.0) ; platform_machine != "arm64" or platform_system != "Darwin"
+Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64" and platform_system == "Darwin"
+Requires-Dist: tensorflow-probability (==0.19.0)
+Requires-Dist: tifffile (>=2022.8.12,<2023.0.0)
+Requires-Dist: torch (==2.0.1) ; sys_platform != "linux"
+Requires-Dist: torch (==2.0.1) ; sys_platform == "linux"
+Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux"
+Requires-Dist: torchvision (==0.15.2) ; sys_platform == "linux"
+Requires-Dist: tornado (==6.1)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PIMS>=0.6.1
-Requires-Dist: POT>=0.8.2
-Requires-Dist: Shapely>=1.8.5.post1
-Requires-Dist: catboost>=1.1.1
-Requires-Dist: dask_image>=2022.9.0
-Requires-Dist: imageio-ffmpeg>=0.4.8
-Requires-Dist: imbalanced_learn>=0.10.1
-Requires-Dist: imblearn>=0.0
-Requires-Dist: joblib>=1.2.0
-Requires-Dist: jupyter-sphinx==0.4.0
-Requires-Dist: jupyter_sphinx>=0.4.0
-Requires-Dist: keras-tcn-macos>=1.0; platform_machine == "arm64" and platform_system == "Darwin"
-Requires-Dist: keras-tcn>=3.5.0; platform_machine != "arm64" or platform_system != "Darwin"
-Requires-Dist: keras_tuner>=1.3.3
-Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: nbsphinx>=0.8.7
-Requires-Dist: networkx>=2.8.8
-Requires-Dist: numpy>=1.23.5
-Requires-Dist: opencv_python>=4.7.0.72
-Requires-Dist: pandas~=1.5
-Requires-Dist: pomegranate>=1.0.0
-Requires-Dist: regex>=2022.10.31
-Requires-Dist: regex>=2022.3.15
-Requires-Dist: ruptures>=1.1.7
-Requires-Dist: scikit_learn==1.2.0
-Requires-Dist: scipy>=1.7.3
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: seglearn>=1.2.5
-Requires-Dist: segment-anything==1.0
-Requires-Dist: setuptools>=67.6.1
-Requires-Dist: shap>=0.41.0
-Requires-Dist: sktime==0.24.0
-Requires-Dist: sleap-io==0.0.9
-Requires-Dist: spektral>=1.2.0
-Requires-Dist: sphinx-press-theme==0.8.0
-Requires-Dist: sphinx-rtd-theme==1.3.0
-Requires-Dist: sphinxcontrib-applehelp==1.0.7
-Requires-Dist: sphinxcontrib-devhelp==1.0.5
-Requires-Dist: sphinxcontrib-htmlhelp==2.0.4
-Requires-Dist: sphinxcontrib-jquery==4.1
-Requires-Dist: sphinxcontrib-jsmath==1.0.1
-Requires-Dist: sphinxcontrib-napoleon==0.7
-Requires-Dist: sphinxcontrib-qthelp==1.0.6
-Requires-Dist: sphinxcontrib-serializinghtml==1.1.9
-Requires-Dist: statannotations>=0.5.0
-Requires-Dist: statsmodels>=0.13
-Requires-Dist: tables>=3.7.0
-Requires-Dist: tensorboard>=2.11.2
-Requires-Dist: tensorflow-macos>=2.11.0; platform_machine == "arm64" and platform_system == "Darwin"
-Requires-Dist: tensorflow>=2.11.0; platform_machine != "arm64" or platform_system != "Darwin"
-Requires-Dist: tensorflow_probability>=0.19.0
-Requires-Dist: torch==2.0.0
-Requires-Dist: torchvision==0.15.1
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: tqdm>=4.65.0
-Requires-Dist: umap_learn>=0.5.3
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.6-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.6.1-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
 
 <br>
 
 <div align="center">
@@ -246,7 +236,8 @@
 
  This project has received funding from the European Union's Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No.  813533
  <div align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b7/Flag_of_Europe.svg/255px-Flag_of_Europe.svg.png">
 </div>
 
 ---
+
```

### Comparing `deepof-0.6/README.md` & `deepof-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.6-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.6.1-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
 
 <br>
 
 <div align="center">
```

### Comparing `deepof-0.6/deepof/.DS_Store` & `deepof-0.6.1/deepof/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/annotation_utils.py` & `deepof-0.6.1/deepof/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/data.py` & `deepof-0.6.1/deepof/data.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/deepof_train_embeddings.py` & `deepof-0.6.1/deepof/deepof_train_embeddings.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/hypermodels.py` & `deepof-0.6.1/deepof/hypermodels.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/model_utils.py` & `deepof-0.6.1/deepof/model_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/models.py` & `deepof-0.6.1/deepof/models.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/post_hoc.py` & `deepof-0.6.1/deepof/post_hoc.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/trained_models/.DS_Store` & `deepof-0.6.1/deepof/trained_models/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/utils.py` & `deepof-0.6.1/deepof/utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6/deepof/visuals.py` & `deepof-0.6.1/deepof/visuals.py`

 * *Files identical despite different names*

