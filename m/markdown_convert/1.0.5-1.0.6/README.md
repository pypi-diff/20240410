# Comparing `tmp/markdown_convert-1.0.5.tar.gz` & `tmp/markdown_convert-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.5.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.6.tar", max compression
```

## Comparing `markdown_convert-1.0.5.tar` & `markdown_convert-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.5/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-09 13:22:04.777161 markdown_convert-1.0.5/README.md
--rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.5/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.5/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.5/markdown_convert/code.css
--rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.0.5/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.5/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.5/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5984 2024-04-09 12:18:10.414947 markdown_convert-1.0.5/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.5/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      541 2024-04-09 12:13:03.121058 markdown_convert-1.0.5/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.5/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-10 06:55:51.115678 markdown_convert-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1773 2024-04-10 11:18:33.740020 markdown_convert-1.0.6/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.0.6/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.6/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.6/markdown_convert/code.css
+-rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.0.6/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.0.6/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.6/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5984 2024-04-09 12:18:10.414947 markdown_convert-1.0.6/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.6/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.0.6/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.6/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      659 2024-04-10 11:23:43.555289 markdown_convert-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 markdown_convert-1.0.6/PKG-INFO
```

### Comparing `markdown_convert-1.0.5/LICENSE` & `markdown_convert-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/README.md` & `markdown_convert-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
+
 <img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
-`markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
+`markdown-convert` is an elegant command-line tool that converts Markdown files to PDF, powered by the amazing `markdown2` and `weasyprint` libraries.
+
+Unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies when running on Linux.
 
-It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
+If you're running Windows, you only need to install the GTK-3 runtime from the following link: [GTK-3 Runtime Installer](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases).
 
 ### Features
 
 - ⚡️ Supports live compilation, so you can preview your PDF in real-time as you type.
 - 🌸 Comes with beautiful CSS out of the box, making your documents look great from the start.
 - 🎨 Syntax highlighting for code blocks included.
 - 🪐 Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
```

### Comparing `markdown_convert-1.0.5/markdown_convert/__main__.py` & `markdown_convert-1.0.6/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/markdown_convert/code.css` & `markdown_convert-1.0.6/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/markdown_convert/default.css` & `markdown_convert-1.0.6/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/markdown_convert/modules/convert.py` & `markdown_convert-1.0.6/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/markdown_convert/modules/resources.py` & `markdown_convert-1.0.6/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/markdown_convert/modules/utils.py` & `markdown_convert-1.0.6/markdown_convert/modules/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """
 Utility functions for string manipulation.
 Author: @julynx
 """
 
+import platform
+
 
 def color(color_code, text):
     """
     Colorize text.
 
     Args:
         text (str): The text to colorize.
         color (str): The color code.
 
     Returns:
         str: The colorized text.
     """
+
+    # Disable if running on Windows
+    if platform.system() == "Windows":
+        return text
+
     return f"\033[{color_code}m{text}\033[0m"
 
 
 def drop_duplicates(lst):
     """
     Drops duplicates from the given list.
```

### Comparing `markdown_convert-1.0.5/markdown_convert/modules/validate.py` & `markdown_convert-1.0.6/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.5/pyproject.toml` & `markdown_convert-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.5"
+version = "1.0.6"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 argsdict = "1.0.0"
-setuptools = "^49.6.0"
+setuptools = ">=46.0.0"
 weasyprint = "^61.2"
 markdown2 = "^2.4.13"
 
 [tool.poetry.scripts]
 markdown-convert = "markdown_convert.__main__:main"
```

### Comparing `markdown_convert-1.0.5/PKG-INFO` & `markdown_convert-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.0.5
+Version: 1.0.6
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -12,28 +12,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argsdict (==1.0.0)
 Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
-Requires-Dist: setuptools (>=49.6.0,<50.0.0)
+Requires-Dist: setuptools (>=46.0.0)
 Requires-Dist: weasyprint (>=61.2,<62.0)
 Description-Content-Type: text/markdown
 
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
+
 <img src='https://i.imgur.com/SZIz2gY.png' width='80%'>
 
-`markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
+`markdown-convert` is an elegant command-line tool that converts Markdown files to PDF, powered by the amazing `markdown2` and `weasyprint` libraries.
+
+Unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies when running on Linux.
 
-It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
+If you're running Windows, you only need to install the GTK-3 runtime from the following link: [GTK-3 Runtime Installer](https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer/releases).
 
 ### Features
 
 - ⚡️ Supports live compilation, so you can preview your PDF in real-time as you type.
 - 🌸 Comes with beautiful CSS out of the box, making your documents look great from the start.
 - 🎨 Syntax highlighting for code blocks included.
 - 🪐 Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
```

