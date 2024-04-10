# Comparing `tmp/pyopia-1.1.1.tar.gz` & `tmp/pyopia-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopia-1.1.1.tar", max compression
+gzip compressed data, was "pyopia-1.1.2.tar", max compression
```

## Comparing `pyopia-1.1.1.tar` & `pyopia-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1457 2023-12-13 09:28:40.495689 pyopia-1.1.1/LICENSE
--rw-r--r--   0        0        0     4914 2023-12-13 09:28:40.495689 pyopia-1.1.1/README.md
--rw-r--r--   0        0        0       22 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/__init__.py
--rw-r--r--   0        0        0    13442 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/background.py
--rw-r--r--   0        0        0     5409 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/classify.py
--rw-r--r--   0        0        0     4592 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/cli.py
--rw-r--r--   0        0        0       24 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/instrument/__init__.py
--rw-r--r--   0        0        0    20997 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/instrument/holo.py
--rw-r--r--   0        0        0     4202 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/instrument/silcam.py
--rw-r--r--   0        0        0     5520 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/io.py
--rw-r--r--   0        0        0    11669 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/pipeline.py
--rw-r--r--   0        0        0     1348 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/plotting.py
--rw-r--r--   0        0        0    20266 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/process.py
--rw-r--r--   0        0        0    27652 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/statistics.py
--rw-r--r--   0        0        0       24 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/tests/__init__.py
--rw-r--r--   0        0        0     8157 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/tests/test_pipeline.py
--rw-r--r--   0        0        0     2608 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyopia/tests/testdata.py
--rw-r--r--   0        0        0     1843 2023-12-13 09:28:40.503689 pyopia-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7049 1970-01-01 00:00:00.000000 pyopia-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1457 2024-04-10 19:18:57.233724 pyopia-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4914 2024-04-10 19:18:57.233724 pyopia-1.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/__init__.py
+-rw-r--r--   0        0        0    13442 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/background.py
+-rw-r--r--   0        0        0     5409 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/classify.py
+-rw-r--r--   0        0        0     4592 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/cli.py
+-rw-r--r--   0        0        0       24 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/instrument/__init__.py
+-rw-r--r--   0        0        0    20997 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/instrument/holo.py
+-rw-r--r--   0        0        0     4202 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/instrument/silcam.py
+-rw-r--r--   0        0        0     5520 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/io.py
+-rw-r--r--   0        0        0    11669 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/pipeline.py
+-rw-r--r--   0        0        0     1348 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/plotting.py
+-rw-r--r--   0        0        0    20266 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/process.py
+-rw-r--r--   0        0        0    27652 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/statistics.py
+-rw-r--r--   0        0        0       24 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/tests/__init__.py
+-rw-r--r--   0        0        0     8157 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/tests/test_pipeline.py
+-rw-r--r--   0        0        0     2608 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyopia/tests/testdata.py
+-rw-r--r--   0        0        0     1843 2024-04-10 19:18:57.241724 pyopia-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7049 1970-01-01 00:00:00.000000 pyopia-1.1.2/PKG-INFO
```

### Comparing `pyopia-1.1.1/LICENSE` & `pyopia-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/README.md` & `pyopia-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/background.py` & `pyopia-1.1.2/pyopia/background.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/classify.py` & `pyopia-1.1.2/pyopia/classify.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/cli.py` & `pyopia-1.1.2/pyopia/cli.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/instrument/holo.py` & `pyopia-1.1.2/pyopia/instrument/holo.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/instrument/silcam.py` & `pyopia-1.1.2/pyopia/instrument/silcam.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/io.py` & `pyopia-1.1.2/pyopia/io.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/pipeline.py` & `pyopia-1.1.2/pyopia/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/plotting.py` & `pyopia-1.1.2/pyopia/plotting.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/process.py` & `pyopia-1.1.2/pyopia/process.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/statistics.py` & `pyopia-1.1.2/pyopia/statistics.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/tests/test_pipeline.py` & `pyopia-1.1.2/pyopia/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyopia/tests/testdata.py` & `pyopia-1.1.2/pyopia/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `pyopia-1.1.1/pyproject.toml` & `pyopia-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 pytest-error-for-skips = "^2.0.2"
 nbclient = "0.7"
 sphinx = "5.0"
 sphinx-rtd-theme = ">=0.5.0"
 sphinxcontrib-napoleon = ">=0.7"
 sphinx-togglebutton = "^0.3.2"
 sphinx-copybutton = "^0.5.2"
-readthedocs-sphinx-search = "^0.3.1"
+readthedocs-sphinx-search = "^0.3.2"
 myst-nb = "^0.17.2"
 jupyter-book = "^0.15.1"
 ipykernel = ">=6.19.4"
 urllib3 = "<2.0"
 gdown = "^4.7.1"
 cmocean = "^3.0.3"
 toml = "^0.10.2"
```

### Comparing `pyopia-1.1.1/PKG-INFO` & `pyopia-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOPIA
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python Ocean Particle Image Analysis toolbox.
 Home-page: https://github.com/sintef/pyopia
 Keywords: Ocean,Particles,Imaging,Measurement,Size distribution
 Author: Emlyn Davies
 Author-email: emlyn.davies@sintef.no
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 Requires-Dist: myst-nb (>=0.17.2,<0.18.0)
 Requires-Dist: nbclient (==0.7)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas[computation] (>=2.1.1,<3.0.0)
 Requires-Dist: poetry-version-plugin (>=0.2.0,<0.3.0)
 Requires-Dist: pytest (>=7.2.0)
 Requires-Dist: pytest-error-for-skips (>=2.0.2,<3.0.0)
-Requires-Dist: readthedocs-sphinx-search (>=0.3.1,<0.4.0)
+Requires-Dist: readthedocs-sphinx-search (>=0.3.2,<0.4.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: scipy (>=1.11.2,<2.0.0)
 Requires-Dist: sphinx (==5.0)
 Requires-Dist: sphinx-copybutton (>=0.5.2,<0.6.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.0)
 Requires-Dist: sphinx-togglebutton (>=0.3.2,<0.4.0)
 Requires-Dist: sphinxcontrib-napoleon (>=0.7)
```

