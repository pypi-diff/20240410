# Comparing `tmp/mkdocs-windows-98-0.4.0.tar.gz` & `tmp/mkdocs-windows-98-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-windows-98-0.4.0.tar", last modified: Sun Apr  7 10:34:07 2024, max compression
+gzip compressed data, was "mkdocs-windows-98-0.4.1.tar", last modified: Wed Apr 10 13:58:55 2024, max compression
```

## Comparing `mkdocs-windows-98-0.4.0.tar` & `mkdocs-windows-98-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/top_level.txt
```

### Comparing `mkdocs-windows-98-0.4.0/LICENSE` & `mkdocs-windows-98-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.4.0/PKG-INFO` & `mkdocs-windows-98-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.4.0
+Version: 0.4.1
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
+Provides-Extra: lint
+Requires-Dist: djlint==1.34.0; extra == "lint"
+Requires-Dist: yamllint==1.32.0; extra == "lint"
 
 # mkdocs-windows-98
 
 Dust off your digital nostalgia with this MKDocs Windows 98 theme! Because sometimes, even our documents deserve to relive the glory days when screens were blurry and icons resembled pixelated hieroglyphs from a digital Stone Age.
 
 ## Related Projects
```

### Comparing `mkdocs-windows-98-0.4.0/README.md` & `mkdocs-windows-98-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.4.0/pyproject.toml` & `mkdocs-windows-98-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-windows-98"
-version = "0.4.0"
+version = "0.4.1"
 description = "Windows 98 MkDocs Theme"
 readme = "README.md"
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
 requires-python = ">=3.9"
 
@@ -22,14 +22,20 @@
   "Topic :: Software Development :: Documentation",
 ]
 
 dependencies = [
   "mkdocs>=1.5.3",
 ]
 
+[project.optional-dependencies]
+lint = [
+  "djlint==1.34.0",
+  "yamllint==1.32.0",
+]
+
 [project.entry-points."mkdocs.themes"]
 windows-98 = "mkdocs_windows_98"
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/PKG-INFO` & `mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.4.0
+Version: 0.4.1
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Documentation
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
+Provides-Extra: lint
+Requires-Dist: djlint==1.34.0; extra == "lint"
+Requires-Dist: yamllint==1.32.0; extra == "lint"
 
 # mkdocs-windows-98
 
 Dust off your digital nostalgia with this MKDocs Windows 98 theme! Because sometimes, even our documents deserve to relive the glory days when screens were blurry and icons resembled pixelated hieroglyphs from a digital Stone Age.
 
 ## Related Projects
```

