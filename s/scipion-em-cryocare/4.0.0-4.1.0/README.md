# Comparing `tmp/scipion-em-cryocare-4.0.0.tar.gz` & `tmp/scipion-em-cryocare-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryocare-4.0.0.tar", last modified: Wed Feb 14 13:27:03 2024, max compression
+gzip compressed data, was "scipion-em-cryocare-4.1.0.tar", last modified: Wed Apr 10 09:38:53 2024, max compression
```

## Comparing `scipion-em-cryocare-4.0.0.tar` & `scipion-em-cryocare-4.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:27:03.273860 scipion-em-cryocare-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-02-14 13:27:03.273860 scipion-em-cryocare-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:27:03.269860 scipion-em-cryocare-4.0.0/cryocare/
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25792 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:27:03.269860 scipion-em-cryocare-4.0.0/cryocare/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_training.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:27:03.273860 scipion-em-cryocare-4.0.0/cryocare/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/tests/test_cryoCARE_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/cryocare/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:27:03.273860 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-14 13:27:03.000000 scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 13:27:03.273860 scipion-em-cryocare-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-14 13:26:24.000000 scipion-em-cryocare-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:53.249215 scipion-em-cryocare-4.1.0/cryocare/
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25792 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/cryocare/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/cryocare/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/tests/test_cryoCARE_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/cryocare/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 09:38:53.000000 scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:38:53.253215 scipion-em-cryocare-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 09:38:11.000000 scipion-em-cryocare-4.1.0/setup.py
```

### Comparing `scipion-em-cryocare-4.0.0/CHANGES.txt` & `scipion-em-cryocare-4.1.0/CHANGES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+4.1.0:
+  Users:
+    - Binary version installed is now 0.3.0 (https://github.com/juglab/cryoCARE_pip/releases/tag/v0.3.0)
+    - We now parse GPU IDs to accept both comma-separated and space-separated specification (Thanks,
+      Ricardo Righetto).
+
 4.0.0:
  Users:
   - Prepare data protocol was removed, and now it's a step of the training protocol.
   - Hotfix: predict protocol was not setting the tilt series id to the generated tomograms.
  Developers:
   - Even/Odd present in metadata or not logic was inverted along the training and predict protocols.
   - Add a base protocol to manage these two entryways to the training and predict protocols.
```

### Comparing `scipion-em-cryocare-4.0.0/LICENSE` & `scipion-em-cryocare-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/PKG-INFO` & `scipion-em-cryocare-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-cryocare
-Version: 4.0.0
+Version: 4.1.0
 Summary: Plugin to use cryoCARE inside scipion.
 Home-page: https://github.com/scipion-em/scipion-em-cryocare
 Author: Tim-Oliver Buchholz, Scipion Team
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ===========================
         Scipion plugin for cryoCARE
```

### Comparing `scipion-em-cryocare-4.0.0/README.rst` & `scipion-em-cryocare-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/__init__.py` & `scipion-em-cryocare-4.1.0/cryocare/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 from pyworkflow.utils import Environ
 from cryocare.constants import CRYOCARE_ENV_ACTIVATION, DEFAULT_ACTIVATION_CMD, CRYOCARE_ENV_NAME, \
     CRYOCARE_DEFAULT_VERSION, CRYOCARE_HOME, CRYOCARE_CUDA_LIB, CRYOCARE
 
 _logo = "icon.png"
 _references = ['buchholz2019cryo']
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 
 class Plugin(pwem.Plugin):
     _homeVar = CRYOCARE_HOME
     _url = 'https://github.com/scipion-em/scipion-em-cryocare'
 
     @classmethod
```

### Comparing `scipion-em-cryocare-4.0.0/cryocare/bibtex.py` & `scipion-em-cryocare-4.1.0/cryocare/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/constants.py` & `scipion-em-cryocare-4.1.0/cryocare/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'you@yourinstitution.email'
 # *
 # **************************************************************************
 
 CRYOCARE_HOME = 'CRYOCARE_HOME'
 V0_2_2 = '0.2.2'
-CRYOCARE_DEFAULT_VERSION = V0_2_2
+V0_3_0 = '0.3.0'
+CRYOCARE_DEFAULT_VERSION = V0_3_0
 CRYOCARE = 'cryoCARE'
 CRYOCARE_ENV_NAME = '%s-%s' % (CRYOCARE, CRYOCARE_DEFAULT_VERSION)
 CRYOCARE_ENV_ACTIVATION = 'CRYOCARE_ENV_ACTIVATION'
 DEFAULT_ACTIVATION_CMD = 'conda activate %s' % CRYOCARE_ENV_NAME
 CRYOCARE_CUDA_LIB = 'CRYOCARE_CUDA_LIB'
 
 TRAIN_DATA_DIR = 'train_data'
```

### Comparing `scipion-em-cryocare-4.0.0/cryocare/icon.png` & `scipion-em-cryocare-4.1.0/cryocare/icon.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/objects.py` & `scipion-em-cryocare-4.1.0/cryocare/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols/__init__.py` & `scipion-em-cryocare-4.1.0/cryocare/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_base.py` & `scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_load_model.py` & `scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_load_model.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_predict.py` & `scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,27 +101,38 @@
         tomoSet = self.tomo.get() if self.areEvenOddLinked.get() else self.evenTomos.get()
         self.sRate = tomoSet.getSamplingRate()
         if self.areEvenOddLinked.get():
             tomoList = [tomo.clone() for tomo in self.tomo.get()]
             tomoListEven = []
             tomoListOdd = []
             for tomo in tomoList:
+
                 odd, even = tomo.getHalfMaps().split(',')
-                tomoListEven.append(even)
-                tomoListOdd.append(odd)
+
+                oddTomo = Tomogram()
+                oddTomo.copyInfo(tomo)
+                oddTomo.setLocation(odd)
+
+                evenTomo = Tomogram()
+                evenTomo.copyInfo(tomo)
+                evenTomo.setLocation(even)
+
+                tomoListEven.append(evenTomo)
+                tomoListOdd.append(oddTomo)
+
         else:
             tomoListEven = [tomo.clone() for tomo in self.evenTomos.get()]
             tomoListOdd = [tomo.clone() for tomo in self.oddTomos.get()]
         return tomoListEven, tomoListOdd
 
-    def preparePredictStep(self, tsId, evenTomo, oddTomo):
+    def preparePredictStep(self, tsId, evenTomoPath, oddTomoPath):
         config = {
             'path': self.model.get().getPath(),
-            'even': evenTomo,
-            'odd': oddTomo,
+            'even': evenTomoPath,
+            'odd': oddTomoPath,
             'n_tiles': [int(i) for i in self.n_tiles.get().split()],
             'output': self._getOutputPath(tsId),
             'overwrite': False
         }
         with open(self.getConfigPath(tsId), 'w+') as f:
             json.dump(config, f, indent=2)
```

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols/protocol_training.py` & `scipion-em-cryocare-4.1.0/cryocare/protocols/protocol_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pyworkflow.utils import makePath, moveFile
 from scipion.constants import PYTHON
 
 from cryocare import Plugin
 from cryocare.constants import TRAIN_DATA_DIR, TRAIN_DATA_FN, TRAIN_DATA_CONFIG, VALIDATION_DATA_FN, CRYOCARE_MODEL
 from cryocare.objects import CryocareModel
 
-
 # Tilt axis values
 X_AXIS = 0
 Y_AXIS = 1
 Z_AXIS = 2
 X_AXIS_LABEL = 'X'
 Y_AXIS_LABEL = 'Y'
 Z_AXIS_LABEL = 'Z'
@@ -164,15 +163,15 @@
         self._configPath = self._getExtraPath('train_config.json')
 
     def prepareTrainingDataStep(self):
 
         if self.areEvenOddLinked.get():
             fnOdd, fnEven = self.getOddEvenLists()
         else:
-            self._getListOfTomoNames(self.evenTomos.get() )
+            self._getListOfTomoNames(self.evenTomos.get())
             fnOdd = self._getListOfTomoNames(self.oddTomos.get())
             fnEven = self._getListOfTomoNames(self.evenTomos.get())
 
         config = {
             'even': fnEven,
             'odd': fnOdd,
             'patch_shape': 3 * [self.patch_shape.get()],
@@ -201,16 +200,22 @@
             'model_name': CRYOCARE_MODEL,
             'path': self._getExtraPath()
         }
         with open(self._configPath, 'w+') as f:
             json.dump(config, f, indent=2)
 
     def trainingStep(self):
+
+        # We do this to accept both GPU specified as '0' 1 2 3' or '0,1,2,3':
+        gpuId = getattr(self, params.GPU_LIST).getListFromValues()
+        gpuId = ' '.join(map(str, gpuId))
+
+        # print(gpuId)
         Plugin.runCryocare(self, PYTHON, '$(which cryoCARE_train.py) --conf {}'.format(self._configPath),
-                           gpuId=getattr(self, params.GPU_LIST).get())
+                           gpuId=gpuId)
 
     def createOutputStep(self):
         model = CryocareModel(model_file=getModelName(self),
                               train_data_dir=self._getTrainDataDir())
         self._defineOutputs(**{Outputobjects.model.name: model})
 
         if self.areEvenOddLinked.get():
@@ -224,17 +229,17 @@
         summary = []
 
         if self.isFinished():
             summary.append("Generated training data info:\n"
                            "train_data_file = *{}*\n"
                            "validation_data_file = *{}*\n"
                            "patch_size = *{}*".format(
-                            self._getTrainDataFile(),
-                            self._getValidationDataFile(),
-                            self.patch_shape.get()))
+                self._getTrainDataFile(),
+                self._getValidationDataFile(),
+                self.patch_shape.get()))
         return summary
 
     def _validate(self):
         validateMsgs = []
         sideLength = self.patch_shape.get()
 
         if self.areEvenOddLinked.get():
```

### Comparing `scipion-em-cryocare-4.0.0/cryocare/protocols.conf` & `scipion-em-cryocare-4.1.0/cryocare/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/tests/__init__.py` & `scipion-em-cryocare-4.1.0/cryocare/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/tests/test_cryoCARE_workflow.py` & `scipion-em-cryocare-4.1.0/cryocare/tests/test_cryoCARE_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/cryocare/utils.py` & `scipion-em-cryocare-4.1.0/cryocare/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/PKG-INFO` & `scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-cryocare
-Version: 4.0.0
+Version: 4.1.0
 Summary: Plugin to use cryoCARE inside scipion.
 Home-page: https://github.com/scipion-em/scipion-em-cryocare
 Author: Tim-Oliver Buchholz, Scipion Team
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ===========================
         Scipion plugin for cryoCARE
```

### Comparing `scipion-em-cryocare-4.0.0/scipion_em_cryocare.egg-info/SOURCES.txt` & `scipion-em-cryocare-4.1.0/scipion_em_cryocare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryocare-4.0.0/setup.py` & `scipion-em-cryocare-4.1.0/setup.py`

 * *Files identical despite different names*

