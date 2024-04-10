# Comparing `tmp/gerber_writer-0.4.2.20.tar.gz` & `tmp/gerber_writer-0.4.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerber_writer-0.4.2.20.tar", last modified: Mon Apr  8 09:42:33 2024, max compression
+gzip compressed data, was "gerber_writer-0.4.2.21.tar", last modified: Wed Apr 10 19:42:45 2024, max compression
```

## Comparing `gerber_writer-0.4.2.20.tar` & `gerber_writer-0.4.2.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2023-12-04 16:10:40.000000 gerber_writer-0.4.2.20/LICENSE
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2743 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1981 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/README.rst
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1068 2024-03-26 17:03:58.000000 gerber_writer-0.4.2.20/pyproject.toml
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/setup.cfg
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.921345 gerber_writer-0.4.2.20/src/
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.921345 gerber_writer-0.4.2.20/src/gerber_writer/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       78 2024-03-26 16:34:58.000000 gerber_writer-0.4.2.20/src/gerber_writer/__init__.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.2.20/src/gerber_writer/lutils.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/src/gerber_writer/macros.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/src/gerber_writer/padmasters.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.20/src/gerber_writer/writer.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.2.20/src/gerber_writer/writer_test.py
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2743 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      418 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/SOURCES.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/dependency_links.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-08 09:42:33.000000 gerber_writer-0.4.2.20/src/gerber_writer.egg-info/top_level.txt
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-08 09:42:33.925345 gerber_writer-0.4.2.20/tests/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/tests/test_arcs.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.20/tests/test_contours.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2024-04-09 14:53:35.000000 gerber_writer-0.4.2.21/LICENSE
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2763 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1981 2024-04-09 14:53:35.000000 gerber_writer-0.4.2.21/README.rst
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1032 2024-04-09 18:45:13.000000 gerber_writer-0.4.2.21/pyproject.toml
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/setup.cfg
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 19:42:45.479123 gerber_writer-0.4.2.21/src/
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/src/gerber_writer/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       78 2024-04-09 18:45:13.000000 gerber_writer-0.4.2.21/src/gerber_writer/__init__.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.2.21/src/gerber_writer/lutils.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.21/src/gerber_writer/macros.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.21/src/gerber_writer/padmasters.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.21/src/gerber_writer/writer.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.2.21/src/gerber_writer/writer_test.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/src/gerber_writer.egg-info/
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2763 2024-04-10 19:42:45.000000 gerber_writer-0.4.2.21/src/gerber_writer.egg-info/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      418 2024-04-10 19:42:45.000000 gerber_writer-0.4.2.21/src/gerber_writer.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-10 19:42:45.000000 gerber_writer-0.4.2.21/src/gerber_writer.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-10 19:42:45.000000 gerber_writer-0.4.2.21/src/gerber_writer.egg-info/top_level.txt
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 19:42:45.483123 gerber_writer-0.4.2.21/tests/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.21/tests/test_arcs.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.21/tests/test_contours.py
```

### Comparing `gerber_writer-0.4.2.20/LICENSE` & `gerber_writer-0.4.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/PKG-INFO` & `gerber_writer-0.4.2.21/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.2.20
+Version: 0.4.2.21
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/alaindef/gerber_writer_project
-Project-URL: Documentation, https://alaindef.github.io/
+Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
+Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
```

### Comparing `gerber_writer-0.4.2.20/README.rst` & `gerber_writer-0.4.2.21/README.rst`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/pyproject.toml` & `gerber_writer-0.4.2.21/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-[project]
-name = "gerber_writer"
-version = "0.4.2.20"
-authors = [
-  { name="Karel Tavernier", email="karel_tavernier@hotmail.com" },
-]
-description = "A library to write Gerber files"
-readme = "README.rst"
-license = { text ="Apache 2.0 License" }
-requires-python = ">=3.9"
-keywords = ["Gerber", "RS-274X", "PCB", "CAD", "CAM", "library"]
-dependencies = []
-
-classifiers = [
-    "Programming Language :: Python :: 3",
-	"License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-	"Development Status :: 5 - Production/Stable",
-	"Intended Audience :: Developers",
-	"Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
-	"Topic :: Software Development :: Libraries",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/alaindef/gerber_writer_project"
-#"Homepage" = "https://github.com/Karel-Tavernier/gerber_writer"
-#"Documentation"= "https://karel-tavernier.github.io/gerber_writer/"
-"Documentation"= "https://alaindef.github.io/"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+[project]
+name = "gerber_writer"
+version = "0.4.2.21"
+authors = [
+  { name="Karel Tavernier", email="karel_tavernier@hotmail.com" },
+]
+description = "A library to write Gerber files"
+readme = "README.rst"
+license = { text ="Apache 2.0 License" }
+requires-python = ">=3.9"
+keywords = ["Gerber", "RS-274X", "PCB", "CAD", "CAM", "library"]
+dependencies = []
+
+classifiers = [
+    "Programming Language :: Python :: 3",
+	"License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+	"Development Status :: 5 - Production/Stable",
+	"Intended Audience :: Developers",
+	"Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
+	"Topic :: Software Development :: Libraries",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Karel-Tavernier/gerber_writer"
+"Documentation"= "https://karel-tavernier.github.io/gerber_writer/"
+#"Documentation"= "https://alaindef.github.io/"
```

### Comparing `gerber_writer-0.4.2.20/src/gerber_writer/macros.py` & `gerber_writer-0.4.2.21/src/gerber_writer/macros.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/src/gerber_writer/padmasters.py` & `gerber_writer-0.4.2.21/src/gerber_writer/padmasters.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/src/gerber_writer/writer.py` & `gerber_writer-0.4.2.21/src/gerber_writer/writer.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/src/gerber_writer/writer_test.py` & `gerber_writer-0.4.2.21/src/gerber_writer/writer_test.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/src/gerber_writer.egg-info/PKG-INFO` & `gerber_writer-0.4.2.21/src/gerber_writer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.2.20
+Version: 0.4.2.21
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/alaindef/gerber_writer_project
-Project-URL: Documentation, https://alaindef.github.io/
+Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
+Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
```

### Comparing `gerber_writer-0.4.2.20/tests/test_arcs.py` & `gerber_writer-0.4.2.21/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.20/tests/test_contours.py` & `gerber_writer-0.4.2.21/tests/test_contours.py`

 * *Files identical despite different names*

