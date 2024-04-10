# Comparing `tmp/img2desmos-0.1.2.tar.gz` & `tmp/img2desmos-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2desmos-0.1.2.tar", max compression
+gzip compressed data, was "img2desmos-1.0.0.tar", max compression
```

## Comparing `img2desmos-0.1.2.tar` & `img2desmos-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2373 2024-04-10 16:48:35.880927 img2desmos-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-10 16:48:35.884927 img2desmos-0.1.2/img2desmos/__init__.py
--rw-r--r--   0        0        0     3328 2024-04-10 16:48:35.884927 img2desmos-0.1.2/img2desmos/main.py
--rw-r--r--   0        0        0      558 2024-04-10 16:48:50.053074 img2desmos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 img2desmos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2511 2024-04-10 17:59:49.098646 img2desmos-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 17:59:49.130646 img2desmos-1.0.0/img2desmos/__init__.py
+-rw-r--r--   0        0        0     3328 2024-04-10 17:59:49.130646 img2desmos-1.0.0/img2desmos/main.py
+-rw-r--r--   0        0        0      558 2024-04-10 18:00:03.602634 img2desmos-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 img2desmos-1.0.0/PKG-INFO
```

### Comparing `img2desmos-0.1.2/README.md` & `img2desmos-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Img2Desmos
 
 This is a simple python script that converts an image to the bezier curves which can be plotted on desmos.
 
 ![image](https://github.com/Perchinka/img2desmos/assets/34923601/9579d060-ae62-4a45-bca7-415ef9858876)
 
-
 ## Requirements
 
 - Python 3.11
 - Poetry
-- [Optional] Chafa (for previewing the images in terminal)
+- [Optional] Chafa (for previewing images in terminal)
 
 ## Installation
 
 ```bash
 pip install img2desmos
 ```
 
@@ -32,7 +31,14 @@
 │ --preview  -p               Preview the img in a window (chafa is required)               │
 │ --upper            INTEGER  Upper threshold for the edge detection [default: 200]         │
 │ --lower            INTEGER  Lower threshold for the edge detection [default: 100]         │
 │ --help                      Show this message and exit.                                   │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
+
+Formulas will be pasted into clipboard
+
+# Demo
+
+https://github.com/Perchinka/img2desmos/assets/34923601/b34c509b-6fae-4e57-8f8f-7d76a0139e42
+
```

### Comparing `img2desmos-0.1.2/img2desmos/main.py` & `img2desmos-1.0.0/img2desmos/main.py`

 * *Files identical despite different names*

### Comparing `img2desmos-0.1.2/pyproject.toml` & `img2desmos-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "img2desmos"
-version = "0.1.2"
+version = "1.0.0"
 description = "CLI tool to convert images to the LaTeX bezier curves formulas"
 authors = ["Perchinka <aleksei.v.lukin@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "img2desmos" }
 ]
```

### Comparing `img2desmos-0.1.2/PKG-INFO` & `img2desmos-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2desmos
-Version: 0.1.2
+Version: 1.0.0
 Summary: CLI tool to convert images to the LaTeX bezier curves formulas
 Author: Perchinka
 Author-email: aleksei.v.lukin@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,20 +20,19 @@
 
 # Img2Desmos
 
 This is a simple python script that converts an image to the bezier curves which can be plotted on desmos.
 
 ![image](https://github.com/Perchinka/img2desmos/assets/34923601/9579d060-ae62-4a45-bca7-415ef9858876)
 
-
 ## Requirements
 
 - Python 3.11
 - Poetry
-- [Optional] Chafa (for previewing the images in terminal)
+- [Optional] Chafa (for previewing images in terminal)
 
 ## Installation
 
 ```bash
 pip install img2desmos
 ```
 
@@ -53,7 +52,14 @@
 │ --upper            INTEGER  Upper threshold for the edge detection [default: 200]         │
 │ --lower            INTEGER  Lower threshold for the edge detection [default: 100]         │
 │ --help                      Show this message and exit.                                   │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
+Formulas will be pasted into clipboard
+
+# Demo
+
+https://github.com/Perchinka/img2desmos/assets/34923601/b34c509b-6fae-4e57-8f8f-7d76a0139e42
+
+
```

