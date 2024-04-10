# Comparing `tmp/loone-0.0.1.tar.gz` & `tmp/loone-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loone-0.0.1.tar", last modified: Wed Apr  3 17:17:04 2024, max compression
+gzip compressed data, was "loone-0.0.2.tar", last modified: Wed Apr 10 21:42:59 2024, max compression
```

## Comparing `loone-0.0.1.tar` & `loone-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.731575 loone-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-03 17:17:04.731575 loone-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-03 17:16:58.000000 loone-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.727575 loone-0.0.1/loone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:16:58.000000 loone-0.0.1/loone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.727575 loone-0.0.1/loone/data/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 17:16:58.000000 loone-0.0.1/loone/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-03 17:16:58.000000 loone-0.0.1/loone/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-03 17:16:58.000000 loone-0.0.1/loone/data/model_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-03 17:16:58.000000 loone-0.0.1/loone/data/tp_variables_regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.727575 loone-0.0.1/loone/loone_nut/
--rw-r--r--   0 runner    (1001) docker     (127)    58820 2024-04-03 17:16:58.000000 loone-0.0.1/loone/loone_nut/LOONE_NUT.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:16:58.000000 loone-0.0.1/loone/loone_nut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.731575 loone-0.0.1/loone/loone_q/
--rw-r--r--   0 runner    (1001) docker     (127)    41948 2024-04-03 17:16:58.000000 loone-0.0.1/loone/loone_q/LOONE_Q.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 17:16:58.000000 loone-0.0.1/loone/loone_q/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.731575 loone-0.0.1/loone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/ap_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/dec_tree_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/df_wsms.py
--rw-r--r--   0 runner    (1001) docker     (127)    26281 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/lo_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/lonino_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/stg_sto_ar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/thc_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/tp_mass_balance_functions_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/trib_hc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-03 17:16:58.000000 loone-0.0.1/loone/utils/wca_stages_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:17:04.731575 loone-0.0.1/loone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-03 17:17:04.000000 loone-0.0.1/loone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 17:17:04.000000 loone-0.0.1/loone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:17:04.000000 loone-0.0.1/loone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 17:17:04.000000 loone-0.0.1/loone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 17:17:04.000000 loone-0.0.1/loone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 17:16:58.000000 loone-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:17:04.731575 loone-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 21:42:54.000000 loone-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-10 21:42:59.023413 loone-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-10 21:42:54.000000 loone-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.019413 loone-0.0.2/loone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:54.000000 loone-0.0.2/loone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/loone/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 21:42:54.000000 loone-0.0.2/loone/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-10 21:42:54.000000 loone-0.0.2/loone/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-10 21:42:54.000000 loone-0.0.2/loone/data/model_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-10 21:42:54.000000 loone-0.0.2/loone/data/tp_variables_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/loone/loone_nut/
+-rw-r--r--   0 runner    (1001) docker     (127)    58820 2024-04-10 21:42:54.000000 loone-0.0.2/loone/loone_nut/LOONE_NUT.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-10 21:42:54.000000 loone-0.0.2/loone/loone_nut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/loone/loone_q/
+-rw-r--r--   0 runner    (1001) docker     (127)    41948 2024-04-10 21:42:54.000000 loone-0.0.2/loone/loone_q/LOONE_Q.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 21:42:54.000000 loone-0.0.2/loone/loone_q/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/loone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/ap_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/dec_tree_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/df_wsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26281 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/lo_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/lonino_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/stg_sto_ar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/thc_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/tp_mass_balance_functions_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/trib_hc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-10 21:42:54.000000 loone-0.0.2/loone/utils/wca_stages_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:42:59.023413 loone-0.0.2/loone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2024-04-10 21:42:59.000000 loone-0.0.2/loone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 21:42:59.000000 loone-0.0.2/loone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:42:59.000000 loone-0.0.2/loone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 21:42:59.000000 loone-0.0.2/loone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 21:42:59.000000 loone-0.0.2/loone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-10 21:42:54.000000 loone-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:42:59.023413 loone-0.0.2/setup.cfg
```

### Comparing `loone-0.0.1/PKG-INFO` & `loone-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,20 @@
-Metadata-Version: 2.1
-Name: loone
-Version: 0.0.1
-Summary: LOONE: A comprehensive water balance-nutrient-optimization model
-Author-email: Osama Tarabih <osamatarabih@usf.edu>
-Maintainer-email: Michael Souffront <msouffront@aquaveo.com>, James Dolinar <jdolinar@aquaveo.com>
-Description-Content-Type: text/markdown
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: platypus-opt==1.0.4
-Requires-Dist: scipy
-Requires-Dist: pyyaml
-
 # LOONE
 The Lake Operation Optimization of Nutrient Exports (LOONE) is a comprehensive water balance-nutrient-optimization model that comprises three coupled modules: A water balance module that simulates the water balance and operations of a reservoir, a nutrient module that simulates nutrient (phosphorus) dynamics in the water column, and an optimization engine that optimizes a reservoir’s releases into its distributaries with the objective of nutrient export minimization and/or water deficit minimization. Python 3 was chosen to develop the code because of its many high-quality libraries and a powerful community support. 
 
 ## Installation
 ```bash
 pip install loone
 ```
 
 ### Development Installation
 ```bash
 git clone <this repository>
 cd ./LOONE
-pip install -e
+pip install -e .
 ```
  
 ## How to Run LOONE?
 ```python
 """
 Data prep
     1. Add all required data to the workspace directory.
```

### Comparing `loone-0.0.1/README.md` & `loone-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,47 @@
+Metadata-Version: 2.1
+Name: loone
+Version: 0.0.2
+Summary: LOONE: A comprehensive water balance-nutrient-optimization model
+Author-email: Osama Tarabih <osamatarabih@usf.edu>
+Maintainer-email: Michael Souffront <msouffront@aquaveo.com>, James Dolinar <jdolinar@aquaveo.com>
+License: BSD-3-Clause License
+        
+        Copyright (c) 2024 University of South Florida
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: platypus-opt==1.0.4
+Requires-Dist: scipy
+Requires-Dist: pyyaml
+
 # LOONE
 The Lake Operation Optimization of Nutrient Exports (LOONE) is a comprehensive water balance-nutrient-optimization model that comprises three coupled modules: A water balance module that simulates the water balance and operations of a reservoir, a nutrient module that simulates nutrient (phosphorus) dynamics in the water column, and an optimization engine that optimizes a reservoir’s releases into its distributaries with the objective of nutrient export minimization and/or water deficit minimization. Python 3 was chosen to develop the code because of its many high-quality libraries and a powerful community support. 
 
 ## Installation
 ```bash
 pip install loone
 ```
 
 ### Development Installation
 ```bash
 git clone <this repository>
 cd ./LOONE
-pip install -e
+pip install -e .
 ```
  
 ## How to Run LOONE?
 ```python
 """
 Data prep
     1. Add all required data to the workspace directory.
```

### Comparing `loone-0.0.1/loone/data/data.py` & `loone-0.0.2/loone/data/data.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/data/model_variables.py` & `loone-0.0.2/loone/data/model_variables.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/data/tp_variables_regions.py` & `loone-0.0.2/loone/data/tp_variables_regions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/loone_nut/LOONE_NUT.py` & `loone-0.0.2/loone/loone_nut/LOONE_NUT.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/loone_q/LOONE_Q.py` & `loone-0.0.2/loone/loone_q/LOONE_Q.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/__init__.py` & `loone-0.0.2/loone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/ap_functions.py` & `loone-0.0.2/loone/utils/ap_functions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/dec_tree_functions.py` & `loone-0.0.2/loone/utils/dec_tree_functions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/df_wsms.py` & `loone-0.0.2/loone/utils/df_wsms.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/lo_functions.py` & `loone-0.0.2/loone/utils/lo_functions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/lonino_functions.py` & `loone-0.0.2/loone/utils/lonino_functions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/stg_sto_ar.py` & `loone-0.0.2/loone/utils/stg_sto_ar.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/thc_class.py` & `loone-0.0.2/loone/utils/thc_class.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/tp_mass_balance_functions_regions.py` & `loone-0.0.2/loone/utils/tp_mass_balance_functions_regions.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/trib_hc.py` & `loone-0.0.2/loone/utils/trib_hc.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone/utils/wca_stages_class.py` & `loone-0.0.2/loone/utils/wca_stages_class.py`

 * *Files identical despite different names*

### Comparing `loone-0.0.1/loone.egg-info/PKG-INFO` & `loone-0.0.2/loone.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Metadata-Version: 2.1
 Name: loone
-Version: 0.0.1
+Version: 0.0.2
 Summary: LOONE: A comprehensive water balance-nutrient-optimization model
 Author-email: Osama Tarabih <osamatarabih@usf.edu>
 Maintainer-email: Michael Souffront <msouffront@aquaveo.com>, James Dolinar <jdolinar@aquaveo.com>
+License: BSD-3-Clause License
+        
+        Copyright (c) 2024 University of South Florida
+        
+        Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+        
+        - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+        - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+        - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: platypus-opt==1.0.4
 Requires-Dist: scipy
 Requires-Dist: pyyaml
 
@@ -20,15 +33,15 @@
 pip install loone
 ```
 
 ### Development Installation
 ```bash
 git clone <this repository>
 cd ./LOONE
-pip install -e
+pip install -e .
 ```
  
 ## How to Run LOONE?
 ```python
 """
 Data prep
     1. Add all required data to the workspace directory.
```

### Comparing `loone-0.0.1/loone.egg-info/SOURCES.txt` & `loone-0.0.2/loone.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 loone/__init__.py
 loone.egg-info/PKG-INFO
 loone.egg-info/SOURCES.txt
 loone.egg-info/dependency_links.txt
 loone.egg-info/requires.txt
```

### Comparing `loone-0.0.1/pyproject.toml` & `loone-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loone"
-version = "0.0.1"
+version = "0.0.2"
 description = "LOONE: A comprehensive water balance-nutrient-optimization model"
 readme = "README.md"
+license = { file = "LICENSE" }
 authors = [
     { name = "Osama Tarabih", email = "osamatarabih@usf.edu" },
 ]
 maintainers = [
     { name = "Michael Souffront", email = "msouffront@aquaveo.com" },
     { name = "James Dolinar", email = "jdolinar@aquaveo.com" },
 ]
```

