# Comparing `tmp/weighted_sample_statistics-0.0.9.tar.gz` & `tmp/weighted_sample_statistics-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_sample_statistics-0.0.9.tar", last modified: Wed Apr 10 19:34:04 2024, max compression
+gzip compressed data, was "weighted_sample_statistics-0.1.0.tar", last modified: Wed Apr 10 19:54:37 2024, max compression
```

## Comparing `weighted_sample_statistics-0.0.9.tar` & `weighted_sample_statistics-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.730376 weighted_sample_statistics-0.0.9/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.9/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.0.9/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.9/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 19:31:17.000000 weighted_sample_statistics-0.0.9/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.0.9/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:34:04.730376 weighted_sample_statistics-0.0.9/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.0.9/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.722376 weighted_sample_statistics-0.0.9/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.722376 weighted_sample_statistics-0.0.9/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.9/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.0.9/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.0.9/docs/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.0.9/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1367 2024-04-10 19:34:04.730376 weighted_sample_statistics-0.0.9/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.9/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.718376 weighted_sample_statistics-0.0.9/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.726376 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      985 2024-04-10 19:30:26.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    20106 2024-04-10 19:19:59.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/core.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/main.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9889 2024-04-10 19:30:39.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/utils.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/variable_properties.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.726376 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      161 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 19:34:04.000000 weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:34:04.726376 weighted_sample_statistics-0.0.9/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.0.9/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      515 2024-04-10 19:33:28.000000 weighted_sample_statistics-0.0.9/tests/test_weighted_sample_statistics.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.0.9/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.0/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.0/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 19:52:50.000000 weighted_sample_statistics-0.1.0/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.1.0/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.753780 weighted_sample_statistics-0.1.0/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.753780 weighted_sample_statistics-0.1.0/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.1.0/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.1.0/docs/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.0/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1367 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.749779 weighted_sample_statistics-0.1.0/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.757779 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1045 2024-04-10 19:52:20.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    20106 2024-04-10 19:19:59.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/core.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/main.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15146 2024-04-10 19:52:33.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/utils.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/variable_properties.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      161 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      515 2024-04-10 19:33:28.000000 weighted_sample_statistics-0.1.0/tests/test_weighted_sample_statistics.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/tox.ini
```

### Comparing `weighted_sample_statistics-0.0.9/.coveragerc` & `weighted_sample_statistics-0.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/.gitignore` & `weighted_sample_statistics-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/.readthedocs.yml` & `weighted_sample_statistics-0.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/CONTRIBUTING.rst` & `weighted_sample_statistics-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/LICENSE.txt` & `weighted_sample_statistics-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/PKG-INFO` & `weighted_sample_statistics-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.0.9
+Version: 0.1.0
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `weighted_sample_statistics-0.0.9/README.rst` & `weighted_sample_statistics-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/docs/Makefile` & `weighted_sample_statistics-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/docs/conf.py` & `weighted_sample_statistics-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/docs/index.rst` & `weighted_sample_statistics-0.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/setup.cfg` & `weighted_sample_statistics-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/setup.py` & `weighted_sample_statistics-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/__init__.py` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 
 from .core import WeightedSampleStatistics as WeightedSampleStatistics
 from .variable_properties import VariableProperties as VariableProperties
 from .utils import rename_all_variables as rename_all_variables
 from .utils import make_negation_name as make_negation_name
 from .utils import get_records_select as get_records_select
 from .utils import prepare_df_for_statistics as prepare_df_for_statistics
+from .utils import reorganise_stat_df as reorganise_stat_df
```

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/core.py` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/core.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/main.py` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/main.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics/variable_properties.py` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/variable_properties.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/PKG-INFO` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.0.9
+Version: 0.1.0
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `weighted_sample_statistics-0.0.9/src/weighted_sample_statistics.egg-info/SOURCES.txt` & `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/tests/test_weighted_sample_statistics.py` & `weighted_sample_statistics-0.1.0/tests/test_weighted_sample_statistics.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.0.9/tox.ini` & `weighted_sample_statistics-0.1.0/tox.ini`

 * *Files identical despite different names*

