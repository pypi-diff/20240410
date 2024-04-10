# Comparing `tmp/datalad-cds-0.0.1.tar.gz` & `tmp/datalad-cds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad-cds-0.0.1.tar", last modified: Wed Feb 21 16:32:55 2024, max compression
+gzip compressed data, was "datalad-cds-0.0.2.tar", last modified: Wed Apr 10 12:08:31 2024, max compression
```

## Comparing `datalad-cds-0.0.1.tar` & `datalad-cds-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.600229 datalad-cds-0.0.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/cli_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/docs/source/python_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.600229 datalad-cds-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.604229 datalad-cds-0.0.1/src/datalad_cds/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/src/datalad_cds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/src/datalad_cds/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/src/datalad_cds/cds_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/src/datalad_cds/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/src/datalad_cds/download_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/src/datalad_cds/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/src/datalad_cds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-21 16:32:55.000000 datalad-cds-0.0.1/src/datalad_cds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:55.608229 datalad-cds-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/tests/test_download_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-02-21 16:32:45.000000 datalad-cds-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.445830 datalad-cds-0.0.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/cli_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/docs/source/python_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.445830 datalad-cds-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.449830 datalad-cds-0.0.2/src/datalad_cds/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/src/datalad_cds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/src/datalad_cds/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/src/datalad_cds/cds_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/src/datalad_cds/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/src/datalad_cds/download_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/src/datalad_cds/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/src/datalad_cds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 12:08:31.000000 datalad-cds-0.0.2/src/datalad_cds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:31.453830 datalad-cds-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/test_cds_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/test_download_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-10 12:08:24.000000 datalad-cds-0.0.2/versioneer.py
```

### Comparing `datalad-cds-0.0.1/LICENSE` & `datalad-cds-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/PKG-INFO` & `datalad-cds-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-cds
-Version: 0.0.1
+Version: 0.0.2
 Summary: DataLad extension for downloading from the Copernicus Climate Data Store
 Author: Matthias Riße
 Author-email: The DataLad Team and Contributors <team@datalad.org>, Benedikt Bulich <b.bulich@fz-juelich.de>, Daniel Klauß <daniel.klauss@alumni.fh-aachen.de>, Laurens Jan van Haaren <l.van.haaren@fz-juelich.de>, Matthias Riße <m.risse@fz-juelich.de>
 Maintainer-email: Matthias Riße <m.risse@fz-juelich.de>
 License: # Main Copyright/License
         
         DataLad, including all examples, code snippets and attached
```

### Comparing `datalad-cds-0.0.1/README.md` & `datalad-cds-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/_datalad_buildsupport/__init__.py` & `datalad-cds-0.0.2/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/_datalad_buildsupport/formatters.py` & `datalad-cds-0.0.2/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/_datalad_buildsupport/setup.py` & `datalad-cds-0.0.2/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/docs/Makefile` & `datalad-cds-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/docs/README.md` & `datalad-cds-0.0.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/docs/source/_static/datalad_logo.png` & `datalad-cds-0.0.2/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/docs/source/conf.py` & `datalad-cds-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/docs/source/index.rst` & `datalad-cds-0.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/pyproject.toml` & `datalad-cds-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/src/datalad_cds/__init__.py` & `datalad-cds-0.0.2/src/datalad_cds/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/src/datalad_cds/cds_remote.py` & `datalad-cds-0.0.2/src/datalad_cds/cds_remote.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/src/datalad_cds/download_cds.py` & `datalad-cds-0.0.2/src/datalad_cds/download_cds.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/src/datalad_cds/spec.py` & `datalad-cds-0.0.2/src/datalad_cds/spec.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.1/src/datalad_cds.egg-info/PKG-INFO` & `datalad-cds-0.0.2/src/datalad_cds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-cds
-Version: 0.0.1
+Version: 0.0.2
 Summary: DataLad extension for downloading from the Copernicus Climate Data Store
 Author: Matthias Riße
 Author-email: The DataLad Team and Contributors <team@datalad.org>, Benedikt Bulich <b.bulich@fz-juelich.de>, Daniel Klauß <daniel.klauss@alumni.fh-aachen.de>, Laurens Jan van Haaren <l.van.haaren@fz-juelich.de>, Matthias Riße <m.risse@fz-juelich.de>
 Maintainer-email: Matthias Riße <m.risse@fz-juelich.de>
 License: # Main Copyright/License
         
         DataLad, including all examples, code snippets and attached
```

### Comparing `datalad-cds-0.0.1/src/datalad_cds.egg-info/SOURCES.txt` & `datalad-cds-0.0.2/src/datalad_cds.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -27,10 +27,11 @@
 src/datalad_cds.egg-info/SOURCES.txt
 src/datalad_cds.egg-info/dependency_links.txt
 src/datalad_cds.egg-info/entry_points.txt
 src/datalad_cds.egg-info/requires.txt
 src/datalad_cds.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_cds_remote.py
 tests/test_download_cds.py
 tests/test_register.py
 tests/test_spec.py
```

### Comparing `datalad-cds-0.0.1/tests/test_download_cds.py` & `datalad-cds-0.0.2/tests/test_download_cds.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     },
 }
 
 
 @pytest.mark.parametrize("cds_request", [request_dict, json.dumps(request_dict)])
 def test_download_cds(cds_request: Union[str, dict], empty_dataset: da.Dataset) -> None:
     dataset = empty_dataset
-    dataset.configuration("set", [("remote.cds.dry-run", "true")], scope="local")
     dataset.download_cds(
         cds_request,
         path="download.grib",
     )
     actual_request = datalad_cds.spec.Spec.from_json(
         (dataset.pathobj / "download.grib").read_text()
     )
```

### Comparing `datalad-cds-0.0.1/versioneer.py` & `datalad-cds-0.0.2/versioneer.py`

 * *Files identical despite different names*

