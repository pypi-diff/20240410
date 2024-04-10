# Comparing `tmp/scipion-em-modelangelo-3.1.tar.gz` & `tmp/scipion-em-modelangelo-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-modelangelo-3.1.tar", last modified: Wed Sep 20 09:03:25 2023, max compression
+gzip compressed data, was "scipion-em-modelangelo-3.1.1.tar", last modified: Wed Apr 10 09:44:38 2024, max compression
```

## Comparing `scipion-em-modelangelo-3.1.tar` & `scipion-em-modelangelo-3.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.641571 scipion-em-modelangelo-3.1/modelangelo/
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26218 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/logo.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/modelangelo/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/protocols/protocol_model_angelo.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/modelangelo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/tests/tests_model_angelo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/modelangelo/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/modelangelo/viewers/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-20 09:03:25.000000 scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 09:03:25.645571 scipion-em-modelangelo-3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-09-20 09:01:32.000000 scipion-em-modelangelo-3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/modelangelo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/logo.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/modelangelo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/protocols/protocol_model_angelo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/modelangelo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/tests/tests_model_angelo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/modelangelo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/modelangelo/viewers/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 09:44:38.000000 scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:44:38.092229 scipion-em-modelangelo-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-10 09:44:09.000000 scipion-em-modelangelo-3.1.1/setup.py
```

### Comparing `scipion-em-modelangelo-3.1/LICENSE` & `scipion-em-modelangelo-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/PKG-INFO` & `scipion-em-modelangelo-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-modelangelo
-Version: 3.1
+Version: 3.1.1
 Summary: Scipion plugin for modelangelo.
 Home-page: https://github.com/scipion-em/scipion-em-modelangelo
 Author: Pablo Conesa
 Author-email: scipion@cnb.cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-modelangelo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-modelangelo/
```

### Comparing `scipion-em-modelangelo-3.1/README.rst` & `scipion-em-modelangelo-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/__init__.py` & `scipion-em-modelangelo-3.1.1/modelangelo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 from scipion.install.funcs import VOID_TGZ
 
 from .constants import *
 
-__version__ = "3.1"
+__version__ = "3.1.1"
 _logo = "logo.jpeg"
 _references = ['jamali2023']
 
 
 class Plugin(pwem.Plugin):
 
     @classmethod
@@ -64,15 +64,15 @@
         cudaLib = cls.getVar(MODEL_ANGELO_CUDA_LIB)
         environ.addLibrary(cudaLib)
 
         return environ
 
     @classmethod
     def getActivationCmd(cls, version):
-        return'conda activate modelangelo-' + version
+        return 'conda activate modelangelo-' + version
 
     @classmethod
     def defineBinaries(cls, env):
 
         def defineModelAngeloInstallation(version):
             installed = "last-pull-%s.txt" % dt.now().strftime("%y%h%d-%H%M%S")
 
@@ -87,16 +87,16 @@
                            tar=VOID_TGZ,
                            default=True)
 
         def getCondaInstallation(version):
             installationCmd = cls.getCondaActivationCmd()
             installationCmd += 'conda create -y -n modelangelo-' + version + ' python=3.10 && '
             installationCmd += cls.getActivationCmd(version) + ' && '
-            installationCmd += 'conda install -y pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia && '
-            installationCmd += 'cd model-angelo && pip install -r requirements.txt && '
+            installationCmd += 'conda install -y pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia && '
+            installationCmd += 'cd model-angelo && '
             installationCmd += 'pip install -e . && '
             installationCmd += 'touch ../env-created.txt'
 
             return installationCmd
 
         defineModelAngeloInstallation(MA_VERSION)
```

### Comparing `scipion-em-modelangelo-3.1/modelangelo/bibtex.py` & `scipion-em-modelangelo-3.1.1/modelangelo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/constants.py` & `scipion-em-modelangelo-3.1.1/modelangelo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/logo.jpeg` & `scipion-em-modelangelo-3.1.1/modelangelo/logo.jpeg`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/protocols/__init__.py` & `scipion-em-modelangelo-3.1.1/modelangelo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/protocols/protocol_model_angelo.py` & `scipion-em-modelangelo-3.1.1/modelangelo/protocols/protocol_model_angelo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/tests/__init__.py` & `scipion-em-modelangelo-3.1.1/modelangelo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/tests/tests_model_angelo.py` & `scipion-em-modelangelo-3.1.1/modelangelo/tests/tests_model_angelo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/viewers/__init__.py` & `scipion-em-modelangelo-3.1.1/modelangelo/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/modelangelo/viewers/viewer.py` & `scipion-em-modelangelo-3.1.1/modelangelo/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/PKG-INFO` & `scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-modelangelo
-Version: 3.1
+Version: 3.1.1
 Summary: Scipion plugin for modelangelo.
 Home-page: https://github.com/scipion-em/scipion-em-modelangelo
 Author: Pablo Conesa
 Author-email: scipion@cnb.cnb.csic.es
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-modelangelo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-modelangelo/
```

### Comparing `scipion-em-modelangelo-3.1/scipion_em_modelangelo.egg-info/SOURCES.txt` & `scipion-em-modelangelo-3.1.1/scipion_em_modelangelo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-modelangelo-3.1/setup.py` & `scipion-em-modelangelo-3.1.1/setup.py`

 * *Files identical despite different names*

