# Comparing `tmp/markdown_convert-1.0.3.tar.gz` & `tmp/markdown_convert-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.3.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.4.tar", max compression
```

## Comparing `markdown_convert-1.0.3.tar` & `markdown_convert-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.3/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-09 13:06:15.345703 markdown_convert-1.0.3/README.md
--rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.3/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.3/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.3/markdown_convert/code.css
--rw-r--r--   0        0        0     5433 2024-04-09 12:35:37.486669 markdown_convert-1.0.3/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.3/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.3/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5984 2024-04-09 12:18:10.414947 markdown_convert-1.0.3/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.3/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      541 2024-04-09 12:13:03.121058 markdown_convert-1.0.3/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.3/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-09 13:06:51.570084 markdown_convert-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-09 13:22:04.777161 markdown_convert-1.0.4/README.md
+-rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.4/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.4/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.4/markdown_convert/code.css
+-rw-r--r--   0        0        0     5433 2024-04-09 12:35:37.486669 markdown_convert-1.0.4/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.4/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.4/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5984 2024-04-09 12:18:10.414947 markdown_convert-1.0.4/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.4/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      541 2024-04-09 12:13:03.121058 markdown_convert-1.0.4/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.4/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-09 13:22:13.773127 markdown_convert-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.4/PKG-INFO
```

### Comparing `markdown_convert-1.0.3/LICENSE` & `markdown_convert-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/README.md` & `markdown_convert-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
-<img src='https://i.imgur.com/GOpzEfy.png' width='80%'>
+<img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
 
 It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
 
 ### Features
```

### Comparing `markdown_convert-1.0.3/markdown_convert/__main__.py` & `markdown_convert-1.0.4/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/code.css` & `markdown_convert-1.0.4/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/default.css` & `markdown_convert-1.0.4/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/modules/convert.py` & `markdown_convert-1.0.4/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/modules/resources.py` & `markdown_convert-1.0.4/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/modules/utils.py` & `markdown_convert-1.0.4/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/markdown_convert/modules/validate.py` & `markdown_convert-1.0.4/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.3/pyproject.toml` & `markdown_convert-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.3"
+version = "1.0.4"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.0.3/PKG-INFO` & `markdown_convert-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.0.3
+Version: 1.0.4
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
-<img src='https://i.imgur.com/GOpzEfy.png' width='80%'>
+<img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
 
 It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
 
 ### Features
```

