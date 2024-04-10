# Comparing `tmp/solvency2_data-0.1.7.tar.gz` & `tmp/solvency2_data-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solvency2_data-0.1.7.tar", last modified: Mon Feb 24 07:02:22 2020, max compression
+gzip compressed data, was "solvency2_data-0.2.0.tar", max compression
```

## Comparing `solvency2_data-0.1.7.tar` & `solvency2_data-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,13 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3189 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3875 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.960959 solvency2_data-0.1.7/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4948 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.960959 solvency2_data-0.1.7/solvency2_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/solvency2_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16290 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/solvency2_data/solvency2_data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/solvency2_data.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3875 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-02-24 07:02:22.000000 solvency2_data-0.1.7/solvency2_data.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 07:02:22.964961 solvency2_data-0.1.7/tests/test_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/test_data/README.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12421 2020-02-24 07:01:42.000000 solvency2_data-0.1.7/tests/test_solvency2_data.py
+-rw-r--r--   0        0        0     1356 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1573 2024-04-10 06:44:12.000000 solvency2_data-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-10 06:44:06.000000 solvency2_data-0.2.0/README.md
+-rw-r--r--   0        0        0      233 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/__init__.py
+-rw-r--r--   0        0        0     4688 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/alternative_extrapolation.py
+-rw-r--r--   0        0        0    16171 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/eiopa_data.py
+-rw-r--r--   0        0        0    15807 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/rfr.py
+-rw-r--r--   0        0        0     6314 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/scraping.py
+-rw-r--r--   0        0        0    15376 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/smith_wilson.py
+-rw-r--r--   0        0        0       83 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/solvency2_data.cfg
+-rw-r--r--   0        0        0     8100 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/sqlite_handler.py
+-rw-r--r--   0        0        0     1760 2024-04-09 11:12:58.000000 solvency2_data-0.2.0/solvency2_data/util.py
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 solvency2_data-0.2.0/PKG-INFO
```

### Comparing `solvency2_data-0.1.7/LICENSE` & `solvency2_data-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-MIT/X License
-
-Copyright (C) 2019 De Nederlandsche Bank
-
-Permission is hereby granted, free of charge, to any person obtaining a copy 
-of this software and associated documentation files (the "Software"), to deal 
-in the Software without restriction, including without limitation the rights 
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
-copies of the Software, and to permit persons to whom the Software is 
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all 
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-SOFTWARE.
-
-Except as contained in this notice, the name of De Nederlandsche Bank shall not 
-be used in advertising or otherwise to promote the sale, use or other dealings in 
-this software without prior written authorization from De Nederlandsche Bank.
+MIT/X License
+
+Copyright (C) 2019 De Nederlandsche Bank
+
+Permission is hereby granted, free of charge, to any person obtaining a copy 
+of this software and associated documentation files (the "Software"), to deal 
+in the Software without restriction, including without limitation the rights 
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell 
+copies of the Software, and to permit persons to whom the Software is 
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all 
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+SOFTWARE.
+
+Except as contained in this notice, the name of De Nederlandsche Bank shall not 
+be used in advertising or otherwise to promote the sale, use or other dealings in 
+this software without prior written authorization from De Nederlandsche Bank.
```

