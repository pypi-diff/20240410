# Comparing `tmp/botnikkk-0.0.9.tar.gz` & `tmp/botnikkk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.0.9.tar", last modified: Mon Apr  1 20:08:03 2024, max compression
+gzip compressed data, was "botnikkk-0.1.0.tar", last modified: Wed Apr 10 17:35:32 2024, max compression
```

## Comparing `botnikkk-0.0.9.tar` & `botnikkk-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:08:03.257394 botnikkk-0.0.9/
--rw-rw-rw-   0        0        0     2314 2024-04-01 20:08:03.253401 botnikkk-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2024-04-01 19:23:18.000000 botnikkk-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 20:08:03.241396 botnikkk-0.0.9/botnikkk/
--rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.9/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.9/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:08:03.251398 botnikkk-0.0.9/botnikkk.egg-info/
--rw-rw-rw-   0        0        0     2314 2024-04-01 20:08:03.000000 botnikkk-0.0.9/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 20:08:03.000000 botnikkk-0.0.9/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:08:03.000000 botnikkk-0.0.9/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 20:08:03.000000 botnikkk-0.0.9/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 20:08:03.000000 botnikkk-0.0.9/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 20:08:03.257394 botnikkk-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-04-01 20:08:02.000000 botnikkk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:35:32.513722 botnikkk-0.1.0/
+-rw-rw-rw-   0        0        0     1094 2024-04-10 17:07:38.000000 botnikkk-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3274 2024-04-10 17:35:32.510316 botnikkk-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2579 2024-04-10 17:09:44.000000 botnikkk-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 17:35:32.493497 botnikkk-0.1.0/botnikkk/
+-rw-rw-rw-   0        0        0      212 2024-04-10 17:07:38.000000 botnikkk-0.1.0/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     3208 2024-04-10 17:35:18.000000 botnikkk-0.1.0/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-10 17:35:32.507946 botnikkk-0.1.0/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     3274 2024-04-10 17:35:32.000000 botnikkk-0.1.0/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-04-10 17:35:32.000000 botnikkk-0.1.0/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 17:35:32.000000 botnikkk-0.1.0/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-10 17:35:32.000000 botnikkk-0.1.0/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 17:35:32.000000 botnikkk-0.1.0/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 17:35:32.513722 botnikkk-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-10 16:09:19.000000 botnikkk-0.1.0/setup.py
```

### Comparing `botnikkk-0.0.9/PKG-INFO` & `botnikkk-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.9
+Version: 0.1.0
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: screeninfo
 Requires-Dist: asyncio
 
 
+<p align="center">
+  <img src="https://raw.githubusercontent.com/Botnikkk/botnikkk-package/main/images/logo.jpg"/>
+</p>
 
 # botnikkk  
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 Developed by BotNikkk / Nikkk
 
@@ -39,15 +43,21 @@
 
 1. symbol : determines what symbol will fill in the blank space, deault parameter = " "
 
 ```python
 botnikkk.centre('text',symbol='=')
 ```
 
-2. str_end : determines what symbol will print as end= in print statement, deault parameter = "\n"
+2. left_alignment : determines the space that will be used on the left hand side of the centred string, defaul parameter = None/calculated automatically
+
+```python
+botnikkk.centre('text', left_alignment=23)
+```
+
+3. str_end : determines what symbol will print as end= in print statement, deault parameter = "\n"
 
 ```python
 botnikkk.centre('text',str_end='\r')
 ```
 
 ## 2. format_input() function
 
@@ -92,8 +102,27 @@
     #some code
     await botnikkk.redirect("screen_name")
     #some more code
 
 asyncio.run(function())
 ```
 
-check out : https://botnikkk.github.io
+## 4. get_alignments() function
+
+Usage = takes a string as input and returns a dictionary containing the designing alignments of the said string in the form :
+```python
+dic =  {"left_align" : value , "left_gap" : value, "right_gap" : value , "default_gap" : value }
+``` 
+which can be used to format a string accoring to the alignment format of package in such form :
+```python
+print_string = left_align*" " + "|" + left_gap*" " + string + right_gap*" " + |*" 
+"
+``` 
+
+```python
+import botnikkk
+
+alignments = botnikkk.get_alignments("string")
+```
+
+
+check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.9/botnikkk.egg-info/PKG-INFO` & `botnikkk-0.1.0/botnikkk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.9
+Version: 0.1.0
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: screeninfo
 Requires-Dist: asyncio
 
 
+<p align="center">
+  <img src="https://raw.githubusercontent.com/Botnikkk/botnikkk-package/main/images/logo.jpg"/>
+</p>
 
 # botnikkk  
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 Developed by BotNikkk / Nikkk
 
@@ -39,15 +43,21 @@
 
 1. symbol : determines what symbol will fill in the blank space, deault parameter = " "
 
 ```python
 botnikkk.centre('text',symbol='=')
 ```
 
-2. str_end : determines what symbol will print as end= in print statement, deault parameter = "\n"
+2. left_alignment : determines the space that will be used on the left hand side of the centred string, defaul parameter = None/calculated automatically
+
+```python
+botnikkk.centre('text', left_alignment=23)
+```
+
+3. str_end : determines what symbol will print as end= in print statement, deault parameter = "\n"
 
 ```python
 botnikkk.centre('text',str_end='\r')
 ```
 
 ## 2. format_input() function
 
@@ -92,8 +102,27 @@
     #some code
     await botnikkk.redirect("screen_name")
     #some more code
 
 asyncio.run(function())
 ```
 
-check out : https://botnikkk.github.io
+## 4. get_alignments() function
+
+Usage = takes a string as input and returns a dictionary containing the designing alignments of the said string in the form :
+```python
+dic =  {"left_align" : value , "left_gap" : value, "right_gap" : value , "default_gap" : value }
+``` 
+which can be used to format a string accoring to the alignment format of package in such form :
+```python
+print_string = left_align*" " + "|" + left_gap*" " + string + right_gap*" " + |*" 
+"
+``` 
+
+```python
+import botnikkk
+
+alignments = botnikkk.get_alignments("string")
+```
+
+
+check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.9/setup.py` & `botnikkk-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

