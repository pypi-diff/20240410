# Comparing `tmp/ntv_numpy-0.1.0.tar.gz` & `tmp/ntv_numpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntv_numpy-0.1.0.tar", last modified: Wed Apr 10 13:50:11 2024, max compression
+gzip compressed data, was "ntv_numpy-0.1.1.tar", last modified: Wed Apr 10 20:36:51 2024, max compression
```

## Comparing `ntv_numpy-0.1.0.tar` & `ntv_numpy-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:50:11.422932 ntv_numpy-0.1.0/
--rw-rw-rw-   0        0        0    10905 2024-04-10 13:50:11.422433 ntv_numpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10132 2024-04-09 14:22:08.000000 ntv_numpy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 13:50:11.413968 ntv_numpy-0.1.0/ntv_numpy/
--rw-rw-rw-   0        0        0     1563 2024-04-10 06:55:40.000000 ntv_numpy-0.1.0/ntv_numpy/__init__.py
--rw-rw-rw-   0        0        0    14738 2024-04-09 21:42:42.000000 ntv_numpy-0.1.0/ntv_numpy/data_array.py
--rw-rw-rw-   0        0        0    24520 2024-04-09 21:45:12.000000 ntv_numpy-0.1.0/ntv_numpy/ndarray.py
--rw-rw-rw-   0        0        0     5054 2024-03-05 23:18:41.000000 ntv_numpy-0.1.0/ntv_numpy/ntv_numpy.ini
--rw-rw-rw-   0        0        0    12366 2024-04-09 21:53:06.000000 ntv_numpy-0.1.0/ntv_numpy/numpy_ntv_connector.py
--rw-rw-rw-   0        0        0    16413 2024-04-10 12:55:37.000000 ntv_numpy-0.1.0/ntv_numpy/xconnector.py
--rw-rw-rw-   0        0        0    16394 2024-04-10 12:33:19.000000 ntv_numpy-0.1.0/ntv_numpy/xdataset.py
--rw-rw-rw-   0        0        0     9691 2024-04-10 08:34:11.000000 ntv_numpy-0.1.0/ntv_numpy/xndarray.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:50:11.421437 ntv_numpy-0.1.0/ntv_numpy.egg-info/
--rw-rw-rw-   0        0        0    10905 2024-04-10 13:50:11.000000 ntv_numpy-0.1.0/ntv_numpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-04-10 13:50:11.000000 ntv_numpy-0.1.0/ntv_numpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:50:11.000000 ntv_numpy-0.1.0/ntv_numpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-10 13:50:11.000000 ntv_numpy-0.1.0/ntv_numpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 13:50:11.000000 ntv_numpy-0.1.0/ntv_numpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-10 13:50:11.423429 ntv_numpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2024-04-10 13:35:35.000000 ntv_numpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 13:50:11.419946 ntv_numpy-0.1.0/tests/
--rw-rw-rw-   0        0        0    24858 2024-04-10 06:54:44.000000 ntv_numpy-0.1.0/tests/test_ntv_numpy.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:36:51.311863 ntv_numpy-0.1.1/
+-rw-rw-rw-   0        0        0    10905 2024-04-10 20:36:51.311365 ntv_numpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2024-04-09 14:22:08.000000 ntv_numpy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 20:36:51.303896 ntv_numpy-0.1.1/ntv_numpy/
+-rw-rw-rw-   0        0        0     1563 2024-04-10 06:55:40.000000 ntv_numpy-0.1.1/ntv_numpy/__init__.py
+-rw-rw-rw-   0        0        0    14738 2024-04-09 21:42:42.000000 ntv_numpy-0.1.1/ntv_numpy/data_array.py
+-rw-rw-rw-   0        0        0    24520 2024-04-09 21:45:12.000000 ntv_numpy-0.1.1/ntv_numpy/ndarray.py
+-rw-rw-rw-   0        0        0     5054 2024-03-05 23:18:41.000000 ntv_numpy-0.1.1/ntv_numpy/ntv_numpy.ini
+-rw-rw-rw-   0        0        0    12366 2024-04-09 21:53:06.000000 ntv_numpy-0.1.1/ntv_numpy/numpy_ntv_connector.py
+-rw-rw-rw-   0        0        0    16413 2024-04-10 12:55:37.000000 ntv_numpy-0.1.1/ntv_numpy/xconnector.py
+-rw-rw-rw-   0        0        0    16394 2024-04-10 12:33:19.000000 ntv_numpy-0.1.1/ntv_numpy/xdataset.py
+-rw-rw-rw-   0        0        0     9691 2024-04-10 08:34:11.000000 ntv_numpy-0.1.1/ntv_numpy/xndarray.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:36:51.309870 ntv_numpy-0.1.1/ntv_numpy.egg-info/
+-rw-rw-rw-   0        0        0    10905 2024-04-10 20:36:51.000000 ntv_numpy-0.1.1/ntv_numpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-04-10 20:36:51.000000 ntv_numpy-0.1.1/ntv_numpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 20:36:51.000000 ntv_numpy-0.1.1/ntv_numpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-10 20:36:51.000000 ntv_numpy-0.1.1/ntv_numpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 20:36:51.000000 ntv_numpy-0.1.1/ntv_numpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-10 20:36:51.312360 ntv_numpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2024-04-10 20:33:13.000000 ntv_numpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 20:36:51.308377 ntv_numpy-0.1.1/tests/
+-rw-rw-rw-   0        0        0    24858 2024-04-10 06:54:44.000000 ntv_numpy-0.1.1/tests/test_ntv_numpy.py
```

### Comparing `ntv_numpy-0.1.0/PKG-INFO` & `ntv_numpy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntv_numpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
 Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ntv_numpy-0.1.0/README.md` & `ntv_numpy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/__init__.py` & `ntv_numpy-0.1.1/ntv_numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/data_array.py` & `ntv_numpy-0.1.1/ntv_numpy/data_array.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/ndarray.py` & `ntv_numpy-0.1.1/ntv_numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/ntv_numpy.ini` & `ntv_numpy-0.1.1/ntv_numpy/ntv_numpy.ini`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/numpy_ntv_connector.py` & `ntv_numpy-0.1.1/ntv_numpy/numpy_ntv_connector.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/xconnector.py` & `ntv_numpy-0.1.1/ntv_numpy/xconnector.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/xdataset.py` & `ntv_numpy-0.1.1/ntv_numpy/xdataset.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy/xndarray.py` & `ntv_numpy-0.1.1/ntv_numpy/xndarray.py`

 * *Files identical despite different names*

### Comparing `ntv_numpy-0.1.0/ntv_numpy.egg-info/PKG-INFO` & `ntv_numpy-0.1.1/ntv_numpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntv_numpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
 Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ntv_numpy-0.1.0/setup.py` & `ntv_numpy-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ntv_numpy",
-    version="0.1.0",
+    version="0.1.1",
     description="NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/ntv-numpy/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
```

### Comparing `ntv_numpy-0.1.0/tests/test_ntv_numpy.py` & `ntv_numpy-0.1.1/tests/test_ntv_numpy.py`

 * *Files identical despite different names*

