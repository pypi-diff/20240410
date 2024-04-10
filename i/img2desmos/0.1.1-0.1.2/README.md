# Comparing `tmp/img2desmos-0.1.1.tar.gz` & `tmp/img2desmos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2desmos-0.1.1.tar", max compression
+gzip compressed data, was "img2desmos-0.1.2.tar", max compression
```

## Comparing `img2desmos-0.1.1.tar` & `img2desmos-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3797 2024-04-10 14:49:40.478490 img2desmos-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-10 14:44:59.122931 img2desmos-0.1.1/img2desmos/__init__.py
--rw-r--r--   0        0        0     3328 2024-04-10 15:08:55.035776 img2desmos-0.1.1/img2desmos/main.py
--rw-r--r--   0        0        0      558 2024-04-10 15:36:41.701235 img2desmos-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 img2desmos-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2373 2024-04-10 16:48:35.880927 img2desmos-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 16:48:35.884927 img2desmos-0.1.2/img2desmos/__init__.py
+-rw-r--r--   0        0        0     3328 2024-04-10 16:48:35.884927 img2desmos-0.1.2/img2desmos/main.py
+-rw-r--r--   0        0        0      558 2024-04-10 16:48:50.053074 img2desmos-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 img2desmos-0.1.2/PKG-INFO
```

### Comparing `img2desmos-0.1.1/README.md` & `img2desmos-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 - Python 3.11
 - Poetry
 - [Optional] Chafa (for previewing the images in terminal)
 
 ## Installation
 
 ```bash
-poetry install
+pip install img2desmos
 ```
 
 ## Usage
 
 ```bash
-poetry run python img2desmos.py --help
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    img      TEXT  Path to the image to convert into graph [default: None] [required]                                                                                                  │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --output   -o      TEXT     Output formulas file path [default: None]                                                                                                                   │
-│ --preview  -p               Preview the img in a window (chafa is required)                                                                                                                │
-│ --upper            INTEGER  Upper threshold for the edge detection [default: 200]                                                                                                       │
-│ --lower            INTEGER  Lower threshold for the edge detection [default: 100]                                                                                                       │
-│ --help                      Show this message and exit.                                                                                                                                 │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+> img2desmos --help
+                                                                                             
+ Usage: img2desmos [OPTIONS] IMG                                                             
+                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────╮
+│ *    img      TEXT  Path to the image to convert into graph [default: None] [required]    │
+╰───────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────╮
+│ --output   -o      TEXT     Output formulas file path [default: None]                     │
+│ --preview  -p               Preview the img in a window (chafa is required)               │
+│ --upper            INTEGER  Upper threshold for the edge detection [default: 200]         │
+│ --lower            INTEGER  Lower threshold for the edge detection [default: 100]         │
+│ --help                      Show this message and exit.                                   │
+╰───────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
```

### Comparing `img2desmos-0.1.1/img2desmos/main.py` & `img2desmos-0.1.2/img2desmos/main.py`

 * *Files identical despite different names*

### Comparing `img2desmos-0.1.1/pyproject.toml` & `img2desmos-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "img2desmos"
-version = "0.1.1"
+version = "0.1.2"
 description = "CLI tool to convert images to the LaTeX bezier curves formulas"
 authors = ["Perchinka <aleksei.v.lukin@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "img2desmos" }
 ]
```

### Comparing `img2desmos-0.1.1/PKG-INFO` & `img2desmos-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2desmos
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI tool to convert images to the LaTeX bezier curves formulas
 Author: Perchinka
 Author-email: aleksei.v.lukin@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -30,27 +30,30 @@
 - Python 3.11
 - Poetry
 - [Optional] Chafa (for previewing the images in terminal)
 
 ## Installation
 
 ```bash
-poetry install
+pip install img2desmos
 ```
 
 ## Usage
 
 ```bash
-poetry run python img2desmos.py --help
-╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ *    img      TEXT  Path to the image to convert into graph [default: None] [required]                                                                                                  │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --output   -o      TEXT     Output formulas file path [default: None]                                                                                                                   │
-│ --preview  -p               Preview the img in a window (chafa is required)                                                                                                                │
-│ --upper            INTEGER  Upper threshold for the edge detection [default: 200]                                                                                                       │
-│ --lower            INTEGER  Lower threshold for the edge detection [default: 100]                                                                                                       │
-│ --help                      Show this message and exit.                                                                                                                                 │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+> img2desmos --help
+                                                                                             
+ Usage: img2desmos [OPTIONS] IMG                                                             
+                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────╮
+│ *    img      TEXT  Path to the image to convert into graph [default: None] [required]    │
+╰───────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────╮
+│ --output   -o      TEXT     Output formulas file path [default: None]                     │
+│ --preview  -p               Preview the img in a window (chafa is required)               │
+│ --upper            INTEGER  Upper threshold for the edge detection [default: 200]         │
+│ --lower            INTEGER  Lower threshold for the edge detection [default: 100]         │
+│ --help                      Show this message and exit.                                   │
+╰───────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
```

