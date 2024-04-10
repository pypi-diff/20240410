# Comparing `tmp/galitime-0.1.0.tar.gz` & `tmp/galitime-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galitime-0.1.0.tar", last modified: Wed Apr 10 09:20:46 2024, max compression
+gzip compressed data, was "galitime-0.1.1.tar", last modified: Wed Apr 10 09:58:37 2024, max compression
```

## Comparing `galitime-0.1.0.tar` & `galitime-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:20:46.748700 galitime-0.1.0/
--rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.0/LICENSE.txt
--rw-r--r--   0 karel      (503) staff       (20)     3189 2024-04-10 09:20:46.747597 galitime-0.1.0/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)     2611 2024-04-10 09:18:29.000000 galitime-0.1.0/README.rst
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:20:46.646910 galitime-0.1.0/galitime/
--rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.0/galitime/__init__.py
--rwxr-xr-x   0 karel      (503) staff       (20)     3507 2024-04-10 08:55:54.000000 galitime-0.1.0/galitime/galitime.py
--rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.0/galitime/increment_version.py
--rw-r--r--   0 karel      (503) staff       (20)       79 2024-04-10 08:26:04.000000 galitime-0.1.0/galitime/version.py
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:20:46.720290 galitime-0.1.0/galitime.egg-info/
--rw-r--r--   0 karel      (503) staff       (20)     3189 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/entry_points.txt
--rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/requires.txt
--rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-10 09:20:46.000000 galitime-0.1.0/galitime.egg-info/top_level.txt
--rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-10 09:20:46.748827 galitime-0.1.0/setup.cfg
--rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.0/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.209878 galitime-0.1.1/
+-rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.1/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)     3225 2024-04-10 09:58:37.202445 galitime-0.1.1/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     2647 2024-04-10 09:56:38.000000 galitime-0.1.1/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.107995 galitime-0.1.1/galitime/
+-rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.1/galitime/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     3507 2024-04-10 08:55:54.000000 galitime-0.1.1/galitime/galitime.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.1/galitime/increment_version.py
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-10 09:58:23.000000 galitime-0.1.1/galitime/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.194224 galitime-0.1.1/galitime.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     3225 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-10 09:58:37.000000 galitime-0.1.1/galitime.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-10 09:58:37.210220 galitime-0.1.1/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.1/setup.py
```

### Comparing `galitime-0.1.0/LICENSE.txt` & `galitime-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galitime-0.1.0/PKG-INFO` & `galitime-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galitime
-Version: 0.1.0
+Version: 0.1.1
 Summary: description
 Home-page: https://github.com/karel-brinda/galitime
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,49 +21,49 @@
 
 .. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
     :target: https://github.com/karel-brinda/galitime
 .. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/galitime.svg
     :target: https://github.com/karel-brinda/galitime/releases/
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/galitime.svg
     :target: https://pypi.org/project/galitime/
-.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
-    :target: https://doi.org/10.5281/zenodo.10945896
+.. |zenodo-badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10953105.svg
+    :target: https://doi.org/10.5281/zenodo.10953105
 .. |ci-tests-badge| image:: https://github.com/karel-brinda/galitime/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/karel-brinda/galitime/actions/
 
-|info-badge| |github-release-badge| |pypi-badge| |ci-tests-badge|
+|info-badge| |github-release-badge| |pypi-badge| |zenodo-badge| |ci-tests-badge|
 
 
 Introduction
 ------------
 
-Software for benchmarking programs using [GNU Time](https://www.gnu.org/software/time/).
+Software for benchmarking programs using `GNU Time <https://www.gnu.org/software/time/>`_.
 
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
     # brew install gnu-time # on OS X
     conda install -y -c bioconda -c conda-forge galitime
-    galitime --log time.log  ls
+    galitime --log time.log ls
 
 
 
 Installation
 ------------
 
 Dependencies
 ~~~~~~~~~~~~
 
 Galitime has no dependencies beyond Python 3. However, on OS X
-it requires the GNU version of the `time` command (`gtime`),
-which can be installed by `brew install gnu-time`.
+it requires the GNU version of the :code:`time` command (:code:`gtime`),
+which can be installed by :code:`brew install gnu-time`.
 
 
 Using Bioconda
 ~~~~~~~~~~~~~~
 
 .. code-block:: bash
```

### Comparing `galitime-0.1.0/README.rst` & `galitime-0.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 
 .. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
     :target: https://github.com/karel-brinda/galitime
 .. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/galitime.svg
     :target: https://github.com/karel-brinda/galitime/releases/
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/galitime.svg
     :target: https://pypi.org/project/galitime/
-.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
-    :target: https://doi.org/10.5281/zenodo.10945896
+.. |zenodo-badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10953105.svg
+    :target: https://doi.org/10.5281/zenodo.10953105
 .. |ci-tests-badge| image:: https://github.com/karel-brinda/galitime/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/karel-brinda/galitime/actions/
 
-|info-badge| |github-release-badge| |pypi-badge| |ci-tests-badge|
+|info-badge| |github-release-badge| |pypi-badge| |zenodo-badge| |ci-tests-badge|
 
 
 Introduction
 ------------
 
-Software for benchmarking programs using [GNU Time](https://www.gnu.org/software/time/).
+Software for benchmarking programs using `GNU Time <https://www.gnu.org/software/time/>`_.
 
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
     # brew install gnu-time # on OS X
     conda install -y -c bioconda -c conda-forge galitime
-    galitime --log time.log  ls
+    galitime --log time.log ls
 
 
 
 Installation
 ------------
 
 Dependencies
 ~~~~~~~~~~~~
 
 Galitime has no dependencies beyond Python 3. However, on OS X
-it requires the GNU version of the `time` command (`gtime`),
-which can be installed by `brew install gnu-time`.
+it requires the GNU version of the :code:`time` command (:code:`gtime`),
+which can be installed by :code:`brew install gnu-time`.
 
 
 Using Bioconda
 ~~~~~~~~~~~~~~
 
 .. code-block:: bash
```

### Comparing `galitime-0.1.0/galitime/galitime.py` & `galitime-0.1.1/galitime/galitime.py`

 * *Files identical despite different names*

### Comparing `galitime-0.1.0/galitime.egg-info/PKG-INFO` & `galitime-0.1.1/galitime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galitime
-Version: 0.1.0
+Version: 0.1.1
 Summary: description
 Home-page: https://github.com/karel-brinda/galitime
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,49 +21,49 @@
 
 .. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
     :target: https://github.com/karel-brinda/galitime
 .. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/galitime.svg
     :target: https://github.com/karel-brinda/galitime/releases/
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/galitime.svg
     :target: https://pypi.org/project/galitime/
-.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
-    :target: https://doi.org/10.5281/zenodo.10945896
+.. |zenodo-badge| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10953105.svg
+    :target: https://doi.org/10.5281/zenodo.10953105
 .. |ci-tests-badge| image:: https://github.com/karel-brinda/galitime/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/karel-brinda/galitime/actions/
 
-|info-badge| |github-release-badge| |pypi-badge| |ci-tests-badge|
+|info-badge| |github-release-badge| |pypi-badge| |zenodo-badge| |ci-tests-badge|
 
 
 Introduction
 ------------
 
-Software for benchmarking programs using [GNU Time](https://www.gnu.org/software/time/).
+Software for benchmarking programs using `GNU Time <https://www.gnu.org/software/time/>`_.
 
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
     # brew install gnu-time # on OS X
     conda install -y -c bioconda -c conda-forge galitime
-    galitime --log time.log  ls
+    galitime --log time.log ls
 
 
 
 Installation
 ------------
 
 Dependencies
 ~~~~~~~~~~~~
 
 Galitime has no dependencies beyond Python 3. However, on OS X
-it requires the GNU version of the `time` command (`gtime`),
-which can be installed by `brew install gnu-time`.
+it requires the GNU version of the :code:`time` command (:code:`gtime`),
+which can be installed by :code:`brew install gnu-time`.
 
 
 Using Bioconda
 ~~~~~~~~~~~~~~
 
 .. code-block:: bash
```

### Comparing `galitime-0.1.0/setup.py` & `galitime-0.1.1/setup.py`

 * *Files identical despite different names*

