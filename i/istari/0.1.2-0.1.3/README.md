# Comparing `tmp/istari-0.1.2.tar.gz` & `tmp/istari-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istari-0.1.2.tar", last modified: Tue Apr  9 21:36:27 2024, max compression
+gzip compressed data, was "istari-0.1.3.tar", last modified: Wed Apr 10 16:00:45 2024, max compression
```

## Comparing `istari-0.1.2.tar` & `istari-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729934 istari-0.1.2/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-09 21:36:27.729693 istari-0.1.2/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.2/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.726924 istari-0.1.2/istari/
--rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-09 21:35:38.000000 istari-0.1.2/istari/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727518 istari-0.1.2/istari/admin/
--rw-r--r--   0 jay        (501) staff       (20)     1661 2024-04-09 21:28:02.000000 istari-0.1.2/istari/admin/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727718 istari-0.1.2/istari/auth/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.2/istari/auth/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.2/istari/auth/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727913 istari-0.1.2/istari/cli/
--rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.2/istari/cli/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.2/istari/cli/base.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728174 istari-0.1.2/istari/commands/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.2/istari/commands/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     2339 2024-04-09 21:32:52.000000 istari-0.1.2/istari/commands/startapp.py
--rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.2/istari/commands/startproject.py
--rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.2/istari/constants.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728426 istari-0.1.2/istari/db/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.2/istari/db/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.2/istari/db/fields.py
--rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-09 21:23:29.000000 istari-0.1.2/istari/db/models.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.728629 istari-0.1.2/istari/templates/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.2/istari/templates/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.2/istari/templates/commands.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729253 istari-0.1.2/istari/templates/plugins/
--rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.2/istari/templates/plugins/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1045 2024-04-09 02:44:58.000000 istari-0.1.2/istari/templates/plugins/base.py
--rw-r--r--   0 jay        (501) staff       (20)     1344 2024-04-09 02:35:05.000000 istari-0.1.2/istari/templates/plugins/defaultuser.py
--rw-r--r--   0 jay        (501) staff       (20)     1100 2024-04-09 03:00:11.000000 istari-0.1.2/istari/templates/plugins/drf.py
--rw-r--r--   0 jay        (501) staff       (20)     1194 2024-04-09 03:01:28.000000 istari-0.1.2/istari/templates/plugins/editable.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729373 istari-0.1.2/istari/utils/
--rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.2/istari/utils/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.729496 istari-0.1.2/istari/utils/io/
--rw-r--r--   0 jay        (501) staff       (20)     1438 2024-04-09 03:00:36.000000 istari-0.1.2/istari/utils/io/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-09 21:36:27.727406 istari-0.1.2/istari.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      763 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-09 21:36:27.000000 istari-0.1.2/istari.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-09 21:36:27.729967 istari-0.1.2/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.2/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.162116 istari-0.1.3/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-10 16:00:45.161879 istari-0.1.3/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)        9 2024-04-05 20:19:27.000000 istari-0.1.3/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.158711 istari-0.1.3/istari/
+-rw-r--r--   0 jay        (501) staff       (20)       22 2024-04-10 16:00:13.000000 istari-0.1.3/istari/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.159423 istari-0.1.3/istari/admin/
+-rw-r--r--   0 jay        (501) staff       (20)     1661 2024-04-09 21:28:02.000000 istari-0.1.3/istari/admin/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.159651 istari-0.1.3/istari/auth/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 03:18:29.000000 istari-0.1.3/istari/auth/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     3043 2024-04-06 04:11:49.000000 istari-0.1.3/istari/auth/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.159857 istari-0.1.3/istari/cli/
+-rw-r--r--   0 jay        (501) staff       (20)     2246 2024-04-07 03:00:00.000000 istari-0.1.3/istari/cli/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      282 2024-04-05 20:45:04.000000 istari-0.1.3/istari/cli/base.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.160442 istari-0.1.3/istari/commands/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:32:25.000000 istari-0.1.3/istari/commands/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      602 2024-04-10 15:59:41.000000 istari-0.1.3/istari/commands/freeze.py
+-rw-r--r--   0 jay        (501) staff       (20)     2339 2024-04-09 21:32:52.000000 istari-0.1.3/istari/commands/startapp.py
+-rw-r--r--   0 jay        (501) staff       (20)      775 2024-04-07 03:12:41.000000 istari-0.1.3/istari/commands/startproject.py
+-rw-r--r--   0 jay        (501) staff       (20)      117 2024-04-07 03:09:41.000000 istari-0.1.3/istari/constants.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.160737 istari-0.1.3/istari/db/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 00:36:56.000000 istari-0.1.3/istari/db/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1221 2024-04-06 00:37:44.000000 istari-0.1.3/istari/db/fields.py
+-rw-r--r--   0 jay        (501) staff       (20)     1307 2024-04-09 21:23:29.000000 istari-0.1.3/istari/db/models.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.160911 istari-0.1.3/istari/templates/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:01:40.000000 istari-0.1.3/istari/templates/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     4412 2024-04-08 18:29:39.000000 istari-0.1.3/istari/templates/commands.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.161390 istari-0.1.3/istari/templates/plugins/
+-rw-r--r--   0 jay        (501) staff       (20)        0 2024-04-06 21:22:01.000000 istari-0.1.3/istari/templates/plugins/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1045 2024-04-09 02:44:58.000000 istari-0.1.3/istari/templates/plugins/base.py
+-rw-r--r--   0 jay        (501) staff       (20)     1344 2024-04-09 02:35:05.000000 istari-0.1.3/istari/templates/plugins/defaultuser.py
+-rw-r--r--   0 jay        (501) staff       (20)     1100 2024-04-09 03:00:11.000000 istari-0.1.3/istari/templates/plugins/drf.py
+-rw-r--r--   0 jay        (501) staff       (20)     1194 2024-04-09 03:01:28.000000 istari-0.1.3/istari/templates/plugins/editable.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.161597 istari-0.1.3/istari/utils/
+-rw-r--r--   0 jay        (501) staff       (20)      298 2024-04-07 03:12:18.000000 istari-0.1.3/istari/utils/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.161695 istari-0.1.3/istari/utils/io/
+-rw-r--r--   0 jay        (501) staff       (20)     1438 2024-04-09 03:00:36.000000 istari-0.1.3/istari/utils/io/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)      359 2024-04-10 15:58:42.000000 istari-0.1.3/istari/utils/shell.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2024-04-10 16:00:45.159313 istari-0.1.3/istari.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      114 2024-04-10 16:00:45.000000 istari-0.1.3/istari.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      811 2024-04-10 16:00:45.000000 istari-0.1.3/istari.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2024-04-10 16:00:45.000000 istari-0.1.3/istari.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       43 2024-04-10 16:00:45.000000 istari-0.1.3/istari.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        7 2024-04-10 16:00:45.000000 istari-0.1.3/istari.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2024-04-10 16:00:45.162151 istari-0.1.3/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      462 2024-04-05 20:34:04.000000 istari-0.1.3/setup.py
```

### Comparing `istari-0.1.2/istari/admin/__init__.py` & `istari-0.1.3/istari/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/auth/models.py` & `istari-0.1.3/istari/auth/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/cli/__init__.py` & `istari-0.1.3/istari/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/commands/startapp.py` & `istari-0.1.3/istari/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/commands/startproject.py` & `istari-0.1.3/istari/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/db/fields.py` & `istari-0.1.3/istari/db/fields.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/db/models.py` & `istari-0.1.3/istari/db/models.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/templates/commands.py` & `istari-0.1.3/istari/templates/commands.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/templates/plugins/base.py` & `istari-0.1.3/istari/templates/plugins/base.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/templates/plugins/defaultuser.py` & `istari-0.1.3/istari/templates/plugins/defaultuser.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/templates/plugins/drf.py` & `istari-0.1.3/istari/templates/plugins/drf.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/templates/plugins/editable.py` & `istari-0.1.3/istari/templates/plugins/editable.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari/utils/io/__init__.py` & `istari-0.1.3/istari/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `istari-0.1.2/istari.egg-info/SOURCES.txt` & `istari-0.1.3/istari.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 istari.egg-info/top_level.txt
 istari/admin/__init__.py
 istari/auth/__init__.py
 istari/auth/models.py
 istari/cli/__init__.py
 istari/cli/base.py
 istari/commands/__init__.py
+istari/commands/freeze.py
 istari/commands/startapp.py
 istari/commands/startproject.py
 istari/db/__init__.py
 istari/db/fields.py
 istari/db/models.py
 istari/templates/__init__.py
 istari/templates/commands.py
 istari/templates/plugins/__init__.py
 istari/templates/plugins/base.py
 istari/templates/plugins/defaultuser.py
 istari/templates/plugins/drf.py
 istari/templates/plugins/editable.py
 istari/utils/__init__.py
+istari/utils/shell.py
 istari/utils/io/__init__.py
```

