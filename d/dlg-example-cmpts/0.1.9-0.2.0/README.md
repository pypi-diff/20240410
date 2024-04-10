# Comparing `tmp/dlg_example_cmpts-0.1.9.tar.gz` & `tmp/dlg_example_cmpts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlg_example_cmpts-0.1.9.tar", last modified: Mon Feb  7 11:22:57 2022, max compression
+gzip compressed data, was "dlg_example_cmpts-0.2.0.tar", last modified: Wed Apr 10 12:12:29 2024, max compression
```

## Comparing `dlg_example_cmpts-0.1.9.tar` & `dlg_example_cmpts-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:22:57.161469 dlg_example_cmpts-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/Containerfile
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-02-07 11:22:57.161469 dlg_example_cmpts-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:22:57.157469 dlg_example_cmpts-0.1.9/dlg_example_cmpts/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15865 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:22:57.161469 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-02-07 11:22:56.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-02-07 11:22:56.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 11:22:56.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-02-07 11:22:56.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-07 11:22:56.000000 dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 11:22:57.161469 dlg_example_cmpts-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 11:22:57.161469 dlg_example_cmpts-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    17442 2022-02-07 11:22:46.000000 dlg_example_cmpts-0.1.9/tests/test_cmpts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:29.242574 dlg_example_cmpts-0.2.0/dlg_example_cmpts/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-10 12:12:29.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-10 12:12:29.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:12:29.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 12:12:29.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 12:12:29.000000 dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/dlg_example_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13770 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_funcs/fourier_transform_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/dlg_example_funcs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:29.246574 dlg_example_cmpts-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/tests/test_cmpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 12:12:20.000000 dlg_example_cmpts-0.2.0/tests/test_funcs.py
```

### Comparing `dlg_example_cmpts-0.1.9/LICENSE` & `dlg_example_cmpts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlg_example_cmpts-0.1.9/PKG-INFO` & `dlg_example_cmpts-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dlg_example_cmpts
-Version: 0.1.9
-Summary: DALiuGE Component Examples created by ICRAR
-Home-page: https://github.com/ICRAR/daliuge-component-examples/
-Author: andreas.wicenec@icrar.org
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
 
 # DALiuGE example components
 
 [![codecov](https://codecov.io/gh/ICRAR/daliuge-component-examples/branch/main/graph/badge.svg?token=daliuge-component-examples_token_here)](https://codecov.io/gh/ICRAR/daliuge-component-examples)
 [![CI](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -28,14 +17,14 @@
 ```bash
 pip install dlg_example_cmpts
 ```
 ### Engine in Docker container
 ```bash
 docker exec -t daliuge-engine bash -c 'pip install --prefix=$DLG_ROOT/code dlg_example_cmpts'
 ```
+NOTE: If you had this package installed already you will need to re-start the engine after that.
 ## Usage
 For example the MyBranch component will be available to the engine when you specify 
 ```
 dlg_example_cmpts.apps.MyBranch
 ```
 in the AppClass field of a Python Branch component. The EAGLE palette associated with these components are also generated and can be loaded directly into EAGLE. In that case all the fields are correctly populated for the respective components.
-
```

### Comparing `dlg_example_cmpts-0.1.9/README.md` & `dlg_example_cmpts-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: dlg_example_cmpts
+Version: 0.2.0
+Summary: DALiuGE Component Examples created by ICRAR
+Home-page: https://github.com/ICRAR/daliuge-component-examples/
+Author: andreas.wicenec@icrar.org
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: daliuge-engine>=2.3.2
+Requires-Dist: matplotlib
+Requires-Dist: blockdag
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: codecov; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: gitchangelog; extra == "test"
+Requires-Dist: mkdocs; extra == "test"
 
 # DALiuGE example components
 
 [![codecov](https://codecov.io/gh/ICRAR/daliuge-component-examples/branch/main/graph/badge.svg?token=daliuge-component-examples_token_here)](https://codecov.io/gh/ICRAR/daliuge-component-examples)
 [![CI](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -17,13 +39,14 @@
 ```bash
 pip install dlg_example_cmpts
 ```
 ### Engine in Docker container
 ```bash
 docker exec -t daliuge-engine bash -c 'pip install --prefix=$DLG_ROOT/code dlg_example_cmpts'
 ```
+NOTE: If you had this package installed already you will need to re-start the engine after that.
 ## Usage
 For example the MyBranch component will be available to the engine when you specify 
 ```
 dlg_example_cmpts.apps.MyBranch
 ```
-in the AppClass field of a Python Branch component. The EAGLE palette associated with these components are also generated and can be loaded directly into EAGLE. In that case all the fields are correctly populated for the respective components.
+in the AppClass field of a Python Branch component. The EAGLE palette associated with these components are also generated and can be loaded directly into EAGLE. In that case all the fields are correctly populated for the respective components.
```

### Comparing `dlg_example_cmpts-0.1.9/dlg_example_cmpts.egg-info/PKG-INFO` & `dlg_example_cmpts-0.2.0/dlg_example_cmpts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Metadata-Version: 2.1
-Name: dlg-example-cmpts
-Version: 0.1.9
+Name: dlg_example_cmpts
+Version: 0.2.0
 Summary: DALiuGE Component Examples created by ICRAR
 Home-page: https://github.com/ICRAR/daliuge-component-examples/
 Author: andreas.wicenec@icrar.org
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: daliuge-engine>=2.3.2
+Requires-Dist: matplotlib
+Requires-Dist: blockdag
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: black; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: codecov; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: gitchangelog; extra == "test"
+Requires-Dist: mkdocs; extra == "test"
 
 # DALiuGE example components
 
 [![codecov](https://codecov.io/gh/ICRAR/daliuge-component-examples/branch/main/graph/badge.svg?token=daliuge-component-examples_token_here)](https://codecov.io/gh/ICRAR/daliuge-component-examples)
 [![CI](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/daliuge-component-examples/actions/workflows/main.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -28,14 +39,14 @@
 ```bash
 pip install dlg_example_cmpts
 ```
 ### Engine in Docker container
 ```bash
 docker exec -t daliuge-engine bash -c 'pip install --prefix=$DLG_ROOT/code dlg_example_cmpts'
 ```
+NOTE: If you had this package installed already you will need to re-start the engine after that.
 ## Usage
 For example the MyBranch component will be available to the engine when you specify 
 ```
 dlg_example_cmpts.apps.MyBranch
 ```
 in the AppClass field of a Python Branch component. The EAGLE palette associated with these components are also generated and can be loaded directly into EAGLE. In that case all the fields are correctly populated for the respective components.
-
```

### Comparing `dlg_example_cmpts-0.1.9/setup.py` & `dlg_example_cmpts-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `dlg_example_cmpts-0.1.9/tests/test_cmpts.py` & `dlg_example_cmpts-0.2.0/tests/test_cmpts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-from dlg import drop
-import pytest, unittest
+"""
+Test module for example components.
+"""
+
+from glob import glob
 import os
 import pickle
-import urllib
+import requests
 import http
+import logging
+import json
+from time import sleep
+import pytest, unittest
+
+import numpy as np
 
-from glob import glob
 from dlg import droputils
+from dlg.apps.simple import RandomArrayApp
 
 from dlg_example_cmpts import (
     MyBranch,
     LengthCheck,
     MyDataDROP,
     FileGlob,
-    PickOne,
     String2JSON,
     ExtractColumn,
     AdvUrlRetrieve,
     GenericGather,
 )
-from dlg.apps.simple import RandomArrayApp
-from dlg.drop import FileDROP, InMemoryDROP, NullDROP
-from dlg.ddap_protocol import DROPStates
-import logging
-import json
-import numpy as np
-from time import sleep
+
+try:
+    from dlg.data.drops import InMemoryDROP, NullDROP
+except ImportError:
+    from dlg.drop import InMemoryDROP, NullDROP
 
 logger = logging.Logger(__name__)
 
 given = pytest.mark.parametrize
 
 
 class TestMyApps(unittest.TestCase):
@@ -97,17 +103,15 @@
         """
         Execute the actual test given the arrayDROP on input
         """
         b = LengthCheck("b", "b")  # the branch drop
         n = InMemoryDROP("n", "n")  # the memory drop for the NO branch
         y = InMemoryDROP("y", "y")  # the memory drop for the YES branch
         if not isinstance(arrayDROP, InMemoryDROP):
-            startDrop = NullDROP(
-                "i", "i"
-            )  # just to be able to start the execution
+            startDrop = NullDROP("i", "i")  # just to be able to start the execution
             m = InMemoryDROP("m", "m")  # the receiving drop
             startDrop.addConsumer(arrayDROP)
             m.addProducer(arrayDROP)
             m.addConsumer(b)
         else:
             startDrop = m = arrayDROP
             startDrop.addConsumer(b)
@@ -177,14 +181,15 @@
         l = RandomArrayApp("l", "l")
         l.integer = False
         l.size = 0
         (oid, check, length) = self._runLengthTest(l)
         self.assertEqual(oid, "n")
         self.assertEqual(check, length)
 
+    @pytest.mark.filterwarnings("ignore::pytest.PytestUnhandledThreadExceptionWarning")
     def test_LengthCheck_wrongType(self):
         # check wrong type
         w = InMemoryDROP("w", "w")
         b = LengthCheck("b", "b")  # the branch drop
         n = InMemoryDROP("n", "n")  # the memory drop for the NO branch
         y = InMemoryDROP("y", "y")  # the memory drop for the YES branch
         w.addConsumer(b)
@@ -215,66 +220,30 @@
         g.filepath = os.path.dirname(os.path.realpath(__file__))
         fileList = glob(f"{g.filepath}/{g.wildcard}")
         with droputils.DROPWaiterCtx(self, m, timeout=10):
             i.setCompleted()
         res = pickle.loads(droputils.allDropContents(m))
         self.assertEqual(fileList, res)
 
-    def test_PickOne_class(self):
+    def test_FileGlob_class_nomatch(self):
         """
-        Testing the PickOne app
+        Testing the globbing method finding *this* file
         """
         i = NullDROP("i", "i")  # just to be able to start the execution
-        l = RandomArrayApp("l", "l")
-        l.integer = True
-        l.high = 100
-        l.size = 10
-        a = InMemoryDROP("a", "a", type="array", nm="start_array")
-        p = PickOne("p", "p")
-        r = InMemoryDROP("r", "r", type="array", nm="rest_array")
-        o = InMemoryDROP("o", "o", type="scalar", nm="value")
-
-        i.addConsumer(l)
-        a.addProducer(l)
-        p.addInput(a)
-        r.addProducer(p)  # this should contain the rest elements
-        o.addProducer(p)  # this should contain the first element
-        with droputils.DROPWaiterCtx(self, o, timeout=10):
+        g = FileGlob("g", "g")
+        m = InMemoryDROP("m", "m")
+        g.addInput(i)
+        m.addProducer(g)
+        g.wildcard = os.path.basename("rubbish")
+        g.filepath = os.path.dirname(os.path.realpath(__file__))
+        fileList = glob(f"{g.filepath}/{g.wildcard}")
+        with droputils.DROPWaiterCtx(self, m, timeout=10):
             i.setCompleted()
-        in_array = pickle.loads(droputils.allDropContents(a))
-        first = pickle.loads(droputils.allDropContents(o))
-        rest_array = pickle.loads(droputils.allDropContents(r))
-        self.assertEqual(in_array[0], first)
-        self.assertEqual(all(in_array[1:]), all(rest_array))
-
-    def test_PickOne_wrong_input_type(self):
-        """
-        Testing the PickOne with wrong input type
-        """
-        a = InMemoryDROP("a", "a", type="array", nm="start_array")
-        a.write(pickle.dumps(1))  # this is scalar not array
-        p = PickOne("p", "p")
-        a.addConsumer(p)
-        with self.assertRaises(TypeError):
-            a.setCompleted()
-            p.readData()
-
-    def test_PickOne_0dim(self):
-        """
-        Testing the PickOne with 0dim input
-        """
-        a = InMemoryDROP("a", "a")
-        a.write(pickle.dumps(np.array(1)))  # this is 0dim not array
-        a.name = "start_array"
-        p = PickOne("p", "p")
-
-        p.addInput(a)
-        with droputils.DROPWaiterCtx(self, p, timeout=10):
-            a.setCompleted()
-        self.assertRaises(TypeError)
+        res = pickle.loads(droputils.allDropContents(m))
+        self.assertEqual(fileList, res)
 
     def test_String2JSON(self):
         """
         Testing String2JSON with correct input
         """
         example = b'[{"a":1, "b":2},[1,2,3,4,5]]'
         a = InMemoryDROP("a", "a")
@@ -387,15 +356,15 @@
         o = InMemoryDROP("o", "o")
         o.name = "content"
 
         e.addInput(a)
         e.addOutput(o)
         with droputils.DROPWaiterCtx(self, o, timeout=10):
             a.setCompleted()
-        self.assertRaises(urllib.error.URLError)
+        self.assertRaises(requests.exceptions.RequestException)
 
     def test_AdvUrlRetrieve_invalidUrl(self):
         """
         Testing AdvUrlRetrieve with invalid URL
         """
         testContent = {"args": {"daliuge": "great"}}
         testUrl = "https://dummy\ get?daliuge=%i0"
@@ -429,15 +398,15 @@
         e = AdvUrlRetrieve("e", "e")
         e.urlTempl = testUrl
         # o = InMemoryDROP("o", "o")
         # o.name = "content"
 
         e.addInput(a)
         # e.addOutput(o)
-        with droputils.DROPWaiterCtx(self, e, timeout=10):
+        with droputils.DROPWaiterCtx(self, e, timeout=2):
             a.setCompleted()
         # content = json.loads(pickle.loads(droputils.allDropContents(a)))
         # self.assertEqual(content["args"], testContent["args"])
         with self.assertRaisesRegex(Exception, "At least one output required"):
             raise Exception("At least one output required")
 
     def test_AdvUrlRetrieve_wrongType(self):
@@ -503,14 +472,19 @@
         content = content = droputils.allDropContents(o)
         self.assertEqual(content, b"a" * 10 + b"b" * 10)
 
     def test_myData_class(self):
         """
         Dummy getIO method test for data drop
         """
-        assert MyDataDROP("a", "a").getIO() == "Hello from MyDataDROP"
+        a = MyDataDROP("a", "a")
+        a.content = "Hello World"
+        a.setCompleted()
+        content = droputils.allDropContents(a)
+        assert content == b"Hello World"
 
     def test_myData_dataURL(self):
         """
         Dummy dataURL method test for data drop
         """
-        assert MyDataDROP("a", "a").dataURL == "Hello from the dataURL method"
+        a = MyDataDROP("a", "a")
+        assert a.dataURL == "null://data.url/Hello"
```

