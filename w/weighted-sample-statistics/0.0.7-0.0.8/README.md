# Comparing `tmp/weighted_sample_statistics-0.0.7.tar.gz` & `tmp/weighted_sample_statistics-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_sample_statistics-0.0.7.tar", last modified: Wed Apr 10 19:16:41 2024, max compression
+gzip compressed data, was "weighted_sample_statistics-0.0.8.tar", last modified: Wed Apr 10 19:22:03 2024, max compression
```

## Comparing `weighted_sample_statistics-0.0.7.tar` & `weighted_sample_statistics-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.831225 weighted_sample_statistics-0.0.7/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.7/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.0.7/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.7/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 19:15:28.000000 weighted_sample_statistics-0.0.7/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.0.7/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:16:41.831225 weighted_sample_statistics-0.0.7/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.0.7/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.827225 weighted_sample_statistics-0.0.7/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.827225 weighted_sample_statistics-0.0.7/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.7/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.0.7/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.0.7/docs/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.7/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1367 2024-04-10 19:16:41.831225 weighted_sample_statistics-0.0.7/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.7/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.819225 weighted_sample_statistics-0.0.7/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.827225 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      936 2024-04-10 18:53:13.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    20116 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/core.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/main.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     8358 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/utils.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/variable_properties.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.831225 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      161 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 19:16:41.000000 weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:16:41.831225 weighted_sample_statistics-0.0.7/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.7/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      538 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.7/tests/test_weighted_sample_statistics.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.7/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.826391 weighted_sample_statistics-0.0.8/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.8/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.0.8/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.8/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 19:21:02.000000 weighted_sample_statistics-0.0.8/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.0.8/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:22:03.826391 weighted_sample_statistics-0.0.8/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.0.8/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.822391 weighted_sample_statistics-0.0.8/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.822391 weighted_sample_statistics-0.0.8/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.8/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.0.8/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.0.8/docs/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.8/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1367 2024-04-10 19:22:03.826391 weighted_sample_statistics-0.0.8/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.8/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.814390 weighted_sample_statistics-0.0.8/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.822391 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      911 2024-04-10 19:20:41.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    20106 2024-04-10 19:19:59.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/core.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/main.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     8358 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/utils.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/variable_properties.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.826391 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      161 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 19:22:03.000000 weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:22:03.826391 weighted_sample_statistics-0.0.8/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.8/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      538 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.8/tests/test_weighted_sample_statistics.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.8/tox.ini
```

### Comparing `weighted_sample_statistics-0.0.7/.coveragerc` & `weighted_sample_statistics-0.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/.gitignore` & `weighted_sample_statistics-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/.readthedocs.yml` & `weighted_sample_statistics-0.0.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/CONTRIBUTING.rst` & `weighted_sample_statistics-0.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/LICENSE.txt` & `weighted_sample_statistics-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/PKG-INFO` & `weighted_sample_statistics-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.0.7
+Version: 0.0.8
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `weighted_sample_statistics-0.0.7/README.rst` & `weighted_sample_statistics-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/docs/Makefile` & `weighted_sample_statistics-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/docs/conf.py` & `weighted_sample_statistics-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/docs/index.rst` & `weighted_sample_statistics-0.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/setup.cfg` & `weighted_sample_statistics-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/setup.py` & `weighted_sample_statistics-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/__init__.py` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
 
 try:
-    # Change here if project is renamed and does not equal the package name
+    # Change here if the project is renamed and does not equal the package name
     dist_name = __name__
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from .core import (
-    Weightedweighted_sample_statistics as Weightedweighted_sample_statistics,
-)
+from .core import WeightedSampleStatistics as WeightedSampleStatistics
 from .variable_properties import VariableProperties as VariableProperties
 from .utils import rename_all_variables as rename_all_variables
 from .utils import make_negation_name as make_negation_name
 from .utils import get_records_select as get_records_select
```

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/core.py` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .utils import make_negation_name
 
 DataFrameType = Union[DataFrame, None]
 
 logger = logging.getLogger(__name__)
 
 
-class Weightedweighted_sample_statistics:
+class WeightedSampleStatistics:
     """
     Calculate weighted_sample_statistics for summations
 
     Parameters
     ----------
     group_keys: iterable
         The variables to use to group
```

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/main.py` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/main.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/utils.py` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/utils.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics/variable_properties.py` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics/variable_properties.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/PKG-INFO` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.0.7
+Version: 0.0.8
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `weighted_sample_statistics-0.0.7/src/weighted_sample_statistics.egg-info/SOURCES.txt` & `weighted_sample_statistics-0.0.8/src/weighted_sample_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/tests/test_weighted_sample_statistics.py` & `weighted_sample_statistics-0.0.8/tests/test_weighted_sample_statistics.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.7/tox.ini` & `weighted_sample_statistics-0.0.8/tox.ini`

 * *Files identical despite different names*

