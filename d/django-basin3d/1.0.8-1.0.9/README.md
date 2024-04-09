# Comparing `tmp/django-basin3d-1.0.8.tar.gz` & `tmp/django-basin3d-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-basin3d-1.0.8.tar", last modified: Wed Apr  3 11:41:37 2024, max compression
+gzip compressed data, was "django-basin3d-1.0.9.tar", last modified: Tue Apr  9 22:34:08 2024, max compression
```

## Comparing `django-basin3d-1.0.8.tar` & `django-basin3d-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.591920 django-basin3d-1.0.8/django_basin3d/
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/django_basin3d/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/migrations/0002_alter_attributemapping_id_alter_datasource_id.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/django_basin3d/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/synthesis/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/synthesis/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/django_basin3d/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/templatetags/str_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/django_basin3d/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/django_basin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-03 11:41:37.000000 django-basin3d-1.0.8/django_basin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 11:41:37.000000 django-basin3d-1.0.8/django_basin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:41:37.000000 django-basin3d-1.0.8/django_basin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 11:41:37.000000 django-basin3d-1.0.8/django_basin3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 11:41:37.000000 django-basin3d-1.0.8/django_basin3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/doecode.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 11:41:32.000000 django-basin3d-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:41:37.595919 django-basin3d-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.793666 django-basin3d-1.0.9/django_basin3d/
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/django_basin3d/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/migrations/0002_alter_attributemapping_id_alter_datasource_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/django_basin3d/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/synthesis/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14040 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/synthesis/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/django_basin3d/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/templatetags/str_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/django_basin3d/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/django_basin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-09 22:34:08.000000 django-basin3d-1.0.9/django_basin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 22:34:08.000000 django-basin3d-1.0.9/django_basin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:34:08.000000 django-basin3d-1.0.9/django_basin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 22:34:08.000000 django-basin3d-1.0.9/django_basin3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 22:34:08.000000 django-basin3d-1.0.9/django_basin3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/doecode.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-09 22:34:03.000000 django-basin3d-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:34:08.797666 django-basin3d-1.0.9/setup.cfg
```

### Comparing `django-basin3d-1.0.8/LICENSE` & `django-basin3d-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/PKG-INFO` & `django-basin3d-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.8
+Version: 1.0.9
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -61,15 +61,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basin3d==1.0.2
+Requires-Dist: basin3d==1.0.3
 Requires-Dist: django==4.0
 Requires-Dist: djangorestframework
 Requires-Dist: django-filter
 Requires-Dist: markdown
 Requires-Dist: pygments
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `django-basin3d-1.0.8/README.md` & `django-basin3d-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/__init__.py` & `django-basin3d-1.0.9/django_basin3d/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/admin.py` & `django-basin3d-1.0.9/django_basin3d/admin.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/catalog.py` & `django-basin3d-1.0.9/django_basin3d/catalog.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/migrations/0001_initial.py` & `django-basin3d-1.0.9/django_basin3d/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/migrations/0002_alter_attributemapping_id_alter_datasource_id.py` & `django-basin3d-1.0.9/django_basin3d/migrations/0002_alter_attributemapping_id_alter_datasource_id.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/models.py` & `django-basin3d-1.0.9/django_basin3d/models.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/serializers.py` & `django-basin3d-1.0.9/django_basin3d/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/settings.py` & `django-basin3d-1.0.9/django_basin3d/settings.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/synthesis/__init__.py` & `django-basin3d-1.0.9/django_basin3d/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/synthesis/serializers.py` & `django-basin3d-1.0.9/django_basin3d/synthesis/serializers.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/synthesis/viewsets.py` & `django-basin3d-1.0.9/django_basin3d/synthesis/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/urls.py` & `django-basin3d-1.0.9/django_basin3d/urls.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/views.py` & `django-basin3d-1.0.9/django_basin3d/views.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d/viewsets.py` & `django-basin3d-1.0.9/django_basin3d/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/django_basin3d.egg-info/PKG-INFO` & `django-basin3d-1.0.9/django_basin3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-basin3d
-Version: 1.0.8
+Version: 1.0.9
 Summary: BASIN-3D Django Web Framework
 Author-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>, Charuleka Varadharajan <cvaradharajan@lbl.gov>
 Maintainer-email: Valerie C Hendrix <vchendrix@lbl.gov>, Danielle Svehla Christianson <dschristianson@lbl.gov>
 License: Broker for Assimilation, Synthesis and Integration of eNvironmental Diverse, Distributed Datasets (BASIN-3D) Copyright (c) 2019, The
         Regents of the University of California, through Lawrence Berkeley National
         Laboratory (subject to receipt of any required approvals from the U.S.
         Dept. of Energy).  All rights reserved.
@@ -61,15 +61,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: basin3d==1.0.2
+Requires-Dist: basin3d==1.0.3
 Requires-Dist: django==4.0
 Requires-Dist: djangorestframework
 Requires-Dist: django-filter
 Requires-Dist: markdown
 Requires-Dist: pygments
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `django-basin3d-1.0.8/django_basin3d.egg-info/SOURCES.txt` & `django-basin3d-1.0.9/django_basin3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/doecode.yml` & `django-basin3d-1.0.9/doecode.yml`

 * *Files identical despite different names*

### Comparing `django-basin3d-1.0.8/pyproject.toml` & `django-basin3d-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 description = "BASIN-3D Django Web Framework"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = '>=3.8,<3.11'
 dependencies = [
-    'basin3d==1.0.2',
+    'basin3d==1.0.3',
     'django==4.0',
     'djangorestframework',
     'django-filter',
     'markdown',
     'pygments'
 ]
```

