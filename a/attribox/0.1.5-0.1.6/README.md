# Comparing `tmp/attribox-0.1.5.tar.gz` & `tmp/attribox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribox-0.1.5.tar", last modified: Mon Mar 18 15:50:42 2024, max compression
+gzip compressed data, was "attribox-0.1.6.tar", last modified: Wed Apr 10 09:06:35 2024, max compression
```

## Comparing `attribox-0.1.5.tar` & `attribox-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:50:42.498780 attribox-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-18 15:50:31.000000 attribox-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-18 15:50:42.498780 attribox-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-18 15:50:31.000000 attribox-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-18 15:50:38.000000 attribox-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-18 15:50:42.498780 attribox-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:50:42.498780 attribox-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:50:42.498780 attribox-0.1.5/src/attribox/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/_abstract_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/_attri_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/_delayed_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/_this_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-18 15:50:31.000000 attribox-0.1.5/src/attribox/_typed_descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 15:50:42.498780 attribox-0.1.5/src/attribox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-18 15:50:42.000000 attribox-0.1.5/src/attribox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-18 15:50:42.000000 attribox-0.1.5/src/attribox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 15:50:42.000000 attribox-0.1.5/src/attribox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 15:50:42.000000 attribox-0.1.5/src/attribox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 09:06:23.000000 attribox-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-10 09:06:35.528988 attribox-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-10 09:06:23.000000 attribox-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-10 09:06:32.000000 attribox-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 09:06:35.528988 attribox-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.524988 attribox-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/src/attribox/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_abstract_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_attri_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_delayed_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_this_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_typed_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/src/attribox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/top_level.txt
```

### Comparing `attribox-0.1.5/PKG-INFO` & `attribox-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.5
+Version: 0.1.6
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AttriBox - Python Descriptors the Easy Way
 
 ## Installation
```

### Comparing `attribox-0.1.5/README.md` & `attribox-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/setup.cfg` & `attribox-0.1.6/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = attribox
-version = 0.1.5
+version = 0.1.6
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = Class attributes as descriptors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AsgerJon/attribox
 classifiers = 
@@ -12,15 +12,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.11
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `attribox-0.1.5/src/attribox/__init__.py` & `attribox-0.1.6/src/attribox/__init__.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox/_abstract_descriptor.py` & `attribox-0.1.6/src/attribox/_abstract_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox/_attri_box.py` & `attribox-0.1.6/src/attribox/_attri_box.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox/_delayed_descriptor.py` & `attribox-0.1.6/src/attribox/_delayed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox/_this_scope.py` & `attribox-0.1.6/src/attribox/_this_scope.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox/_typed_descriptor.py` & `attribox-0.1.6/src/attribox/_typed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.5/src/attribox.egg-info/PKG-INFO` & `attribox-0.1.6/src/attribox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.5
+Version: 0.1.6
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AttriBox - Python Descriptors the Easy Way
 
 ## Installation
```

