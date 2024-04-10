# Comparing `tmp/roma-1.4.4.tar.gz` & `tmp/roma-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roma-1.4.4.tar", last modified: Thu Mar 21 10:56:52 2024, max compression
+gzip compressed data, was "roma-1.4.5.tar", last modified: Wed Apr 10 08:06:37 2024, max compression
```

## Comparing `roma-1.4.4.tar` & `roma-1.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-03-21 10:56:52.078969 roma-1.4.4/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21068 2023-02-08 15:17:32.000000 roma-1.4.4/LICENSE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2023-02-08 15:17:32.000000 roma-1.4.4/NOTICE
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4731 2024-03-21 10:56:52.078969 roma-1.4.4/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4253 2023-08-22 14:47:59.000000 roma-1.4.4/README.md
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.4.4/pyproject.toml
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-03-21 10:56:52.074969 roma-1.4.4/roma/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      171 2023-08-22 14:47:59.000000 roma-1.4.4/roma/__init__.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3700 2023-07-26 13:01:51.000000 roma-1.4.4/roma/internal.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19424 2023-10-01 08:45:51.000000 roma-1.4.4/roma/mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15174 2023-11-20 13:44:58.000000 roma-1.4.4/roma/transforms.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21763 2024-03-21 10:47:03.000000 roma-1.4.4/roma/utils.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-03-21 10:56:52.078969 roma-1.4.4/roma.egg-info/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4731 2024-03-21 10:56:52.000000 roma-1.4.4/roma.egg-info/PKG-INFO
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      370 2024-03-21 10:56:52.000000 roma-1.4.4/roma.egg-info/SOURCES.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2024-03-21 10:56:52.000000 roma-1.4.4/roma.egg-info/dependency_links.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2024-03-21 10:56:52.000000 roma-1.4.4/roma.egg-info/top_level.txt
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2024-03-21 10:56:52.078969 roma-1.4.4/setup.cfg
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2024-03-21 10:31:40.000000 roma-1.4.4/setup.py
-drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-03-21 10:56:52.078969 roma-1.4.4/test/
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1018 2023-02-08 15:17:32.000000 roma-1.4.4/test/test_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8868 2023-10-01 08:28:10.000000 roma-1.4.4/test/test_mappings.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3808 2023-06-21 22:50:53.000000 roma-1.4.4/test/test_procrustes_derivatives.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    13116 2023-11-20 13:51:39.000000 roma-1.4.4/test/test_transforms.py
--rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15720 2024-03-21 10:30:37.000000 roma-1.4.4/test/test_utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     1468 2024-04-08 09:35:19.000000 roma-1.4.5/LICENSE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     2276 2024-04-08 09:35:19.000000 roma-1.4.5/NOTICE
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4685 2024-04-10 08:06:37.597433 roma-1.4.5/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4207 2024-04-08 09:35:19.000000 roma-1.4.5/README.md
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      103 2023-02-08 15:17:32.000000 roma-1.4.5/pyproject.toml
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/roma/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      135 2024-04-08 09:35:19.000000 roma-1.4.5/roma/__init__.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3665 2024-04-08 09:35:19.000000 roma-1.4.5/roma/internal.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    19388 2024-04-08 09:35:19.000000 roma-1.4.5/roma/mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15139 2024-04-08 09:35:19.000000 roma-1.4.5/roma/transforms.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    21728 2024-04-08 09:35:19.000000 roma-1.4.5/roma/utils.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/roma.egg-info/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     4685 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/PKG-INFO
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      370 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/SOURCES.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        1 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/dependency_links.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)        5 2024-04-10 08:06:37.000000 roma-1.4.5/roma.egg-info/top_level.txt
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)       38 2024-04-10 08:06:37.597433 roma-1.4.5/setup.cfg
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      672 2024-04-08 09:35:19.000000 roma-1.4.5/setup.py
+drwxr-xr-x   0 rbregier (1809414175) DomainUsers (1809400513)        0 2024-04-10 08:06:37.597433 roma-1.4.5/test/
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)      982 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     8832 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_mappings.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)     3772 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_procrustes_derivatives.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    13180 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_transforms.py
+-rw-r--r--   0 rbregier (1809414175) DomainUsers (1809400513)    15684 2024-04-08 09:35:19.000000 roma-1.4.5/test/test_utils.py
```

### Comparing `roma-1.4.4/NOTICE` & `roma-1.4.5/NOTICE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 RoMa
-Copyright (c) 2021 NAVER Corp.
+Copyright (c) 2020 NAVER Corp.
 
 This project contains subcomponents with separate copyright notices and license terms. 
 Your use of the source code for these subcomponents is subject to the terms and conditions of the following licenses.
 
 =====================================================================================================================
 
 SciPy (https://github.com/scipy/scipy)
```

### Comparing `roma-1.4.4/PKG-INFO` & `roma-1.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.4.4
+Version: 1.4.5
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # *RoMa*: A lightweight library to deal with 3D rotations in PyTorch.
@@ -66,15 +66,14 @@
 T = roma.Rigid(R, t)
 # Composing and inverting transformations
 identity = T @ T.inverse()
 # Casting the result to a batch of 4x4 homogeneous matrices
 M = identity.to_homogeneous()
 ```
 
-
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
@@ -85,15 +84,15 @@
 **For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
 to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
 You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
 **With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
 
 
 ## License
-*RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
+*RoMa*, Copyright (c) 2020 NAVER Corp., is licensed under the 3-Clause BSD License (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
 - [__Romain Brégier, Deep Regression on Manifolds: a 3D Rotation Case Study.__ in _2021 International Conference on 3D Vision (3DV)_, 2021.](https://arxiv.org/abs/2103.16317)
```

### Comparing `roma-1.4.4/README.md` & `roma-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 T = roma.Rigid(R, t)
 # Composing and inverting transformations
 identity = T @ T.inverse()
 # Casting the result to a batch of 4x4 homogeneous matrices
 M = identity.to_homogeneous()
 ```
 
-
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
@@ -70,15 +69,15 @@
 **For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
 to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
 You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
 **With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
 
 
 ## License
-*RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
+*RoMa*, Copyright (c) 2020 NAVER Corp., is licensed under the 3-Clause BSD License (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
 - [__Romain Brégier, Deep Regression on Manifolds: a 3D Rotation Case Study.__ in _2021 International Conference on 3D Vision (3DV)_, 2021.](https://arxiv.org/abs/2103.16317)
```

### Comparing `roma-1.4.4/roma/internal.py` & `roma-1.4.5/roma/internal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
+# 3-Clause BSD License.
 """
 Set of functions for internal module use.
 """
 
 import torch
 
 # SVD decomposition
```

### Comparing `roma-1.4.4/roma/mappings.py` & `roma-1.4.5/roma/mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
-
+# 3-Clause BSD License.
 """
 Various mappings between different rotation representations.
 """
 
 import torch
 import roma.internal
```

### Comparing `roma-1.4.4/roma/transforms.py` & `roma-1.4.5/roma/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
+# 3-Clause BSD License.
 """
 Spatial transformations parameterized by rotation matrices, unit quaternions and more.
 
 Example of use
 ~~~~~~~~~~~~~~
 
 .. literalinclude :: ../../examples/snippets/transforms.py
```

### Comparing `roma-1.4.4/roma/utils.py` & `roma-1.4.5/roma/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
+# 3-Clause BSD License.
 """
 Various utility functions related to rotation representations.
 """
 
 import torch
 import numpy as np
 import roma.internal
```

### Comparing `roma-1.4.4/roma.egg-info/PKG-INFO` & `roma-1.4.5/roma.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: roma
-Version: 1.4.4
+Version: 1.4.5
 Summary: A lightweight library to deal with 3D rotations in PyTorch.
 Home-page: https://github.com/naver/roma
 Author: Romain Brégier
 Author-email: romain.bregier@naverlabs.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # *RoMa*: A lightweight library to deal with 3D rotations in PyTorch.
@@ -66,15 +66,14 @@
 T = roma.Rigid(R, t)
 # Composing and inverting transformations
 identity = T @ T.inverse()
 # Casting the result to a batch of 4x4 homogeneous matrices
 M = identity.to_homogeneous()
 ```
 
-
 ## Installation
 The easiest way to install *RoMa* is to use pip:
 ```
 pip install roma
 ```
 
 Alternatively one can install the latest version of *RoMa* directly from the source repository:
@@ -85,15 +84,15 @@
 **For pytorch versions older than 1.8**, we recommend installing [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)
 to achieve a significant speed-up with `special_procrustes` on CUDA GPUs.
 You can check that this module is properly loaded using the function `roma.utils.is_torch_batch_svd_available()`.
 **With recent pytorch installations (torch>=1.8), `torch-batch-svd` is no longer needed or used.**
 
 
 ## License
-*RoMa*, Copyright (c) 2021 NAVER Corp., is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 license (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
+*RoMa*, Copyright (c) 2020 NAVER Corp., is licensed under the 3-Clause BSD License (see [license](https://github.com/naver/roma/blob/master/LICENSE)).
 
 Bits of code were adapted from SciPy. Documentation is generated, distributed and displayed with the support of Sphinx and other materials (see [notice](https://github.com/naver/roma/blob/master/NOTICE)).
 
 ## References
 For a more in-depth discussion regarding differentiable mappings on the rotation space, please refer to:
 - [__Romain Brégier, Deep Regression on Manifolds: a 3D Rotation Case Study.__ in _2021 International Conference on 3D Vision (3DV)_, 2021.](https://arxiv.org/abs/2103.16317)
```

### Comparing `roma-1.4.4/setup.py` & `roma-1.4.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="roma",
-    version="1.4.4",
+    version="1.4.5",
     author="Romain Brégier",
     author_email="romain.bregier@naverlabs.com",
     description="A lightweight library to deal with 3D rotations in PyTorch.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/naver/roma",
     packages=["roma"],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: Free for non-commercial use",
+        "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `roma-1.4.4/test/test_derivatives.py` & `roma-1.4.5/test/test_derivatives.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
-
+# 3-Clause BSD License.
 import torch
 import unittest
 from test.utils import *
 
 # Test of test utils
 class TestDerivatives(unittest.TestCase):
     def test_derivatives(self):
```

### Comparing `roma-1.4.4/test/test_mappings.py` & `roma-1.4.5/test/test_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
-
+# 3-Clause BSD License.
 import unittest
 import torch
 import roma
 import numpy as np
 from test.utils import is_close
 
 def is_close(A, B, eps1 = 1e-5, eps2 = 1e-5):
```

### Comparing `roma-1.4.4/test/test_procrustes_derivatives.py` & `roma-1.4.5/test/test_procrustes_derivatives.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
-
+# 3-Clause BSD License.
 import torch
 import roma
 import unittest
 from test import utils
 
 class TestProcrustesDerivatives(unittest.TestCase):
     def test_derivatives(self):
```

### Comparing `roma-1.4.4/test/test_transforms.py` & `roma-1.4.5/test/test_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# RoMa
+# Copyright (c) 2020 NAVER Corp.
+# 3-Clause BSD License.
 import torch
 import roma
 from roma.transforms import *
 import unittest
 import itertools
 
 class TestTransforms(unittest.TestCase):
```

### Comparing `roma-1.4.4/test/test_utils.py` & `roma-1.4.5/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # RoMa
 # Copyright (c) 2020 NAVER Corp.
-# CC BY-NC-SA 4.0
-# Available only for non-commercial use.
-
+# 3-Clause BSD License.
 import unittest
 import torch
 import numpy as np
 import roma
 import roma.internal
 from test.utils import is_close
```

