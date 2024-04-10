# Comparing `tmp/vtjson-1.6.6.tar.gz` & `tmp/vtjson-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.6.6.tar", last modified: Mon Apr  8 13:55:27 2024, max compression
+gzip compressed data, was "vtjson-1.6.7.tar", last modified: Wed Apr 10 11:50:07 2024, max compression
```

## Comparing `vtjson-1.6.6.tar` & `vtjson-1.6.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:55:27.624529 vtjson-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 13:55:23.000000 vtjson-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-08 13:55:27.624529 vtjson-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-04-08 13:55:23.000000 vtjson-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 13:55:23.000000 vtjson-1.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:55:27.624529 vtjson-1.6.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:55:27.624529 vtjson-1.6.6/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 13:55:27.000000 vtjson-1.6.6/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-08 13:55:23.000000 vtjson-1.6.6/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:50:07.681743 vtjson-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 11:50:01.000000 vtjson-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-04-10 11:50:07.681743 vtjson-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-10 11:50:01.000000 vtjson-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 11:50:01.000000 vtjson-1.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:50:07.681743 vtjson-1.6.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:50:07.681743 vtjson-1.6.7/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 11:50:07.000000 vtjson-1.6.7/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24065 2024-04-10 11:50:01.000000 vtjson-1.6.7/vtjson.py
```

### Comparing `vtjson-1.6.6/LICENSE` & `vtjson-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.6/PKG-INFO` & `vtjson-1.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.6
+Version: 1.6.7
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -302,15 +302,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-For many more examples see the file `test_validate.py` in the source distribution.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario.
```

### Comparing `vtjson-1.6.6/README.md` & `vtjson-1.6.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-For many more examples see the file `test_validate.py` in the source distribution.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario.
```

### Comparing `vtjson-1.6.6/pyproject.toml` & `vtjson-1.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.6/vtjson.egg-info/PKG-INFO` & `vtjson-1.6.7/vtjson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.6
+Version: 1.6.7
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -302,15 +302,15 @@
 ...
 vtjson.ValidationError: object['fruit'] (value:dog) is not of type 'fruit'
 >>> object = {"fruit" : "apple"}
 >>> validate(schema, object)
 ...
 vtjson.ValidationError: object['price'] is missing
 ```
-For many more examples see the file `test_validate.py` in the source distribution.
+A good source of more advanced examples is the file <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a> in the source distribution of Fishtest. Another source of examples is the file <a href=https://raw.githubusercontent.com/vdbergh/vtjson/main/test_validate.py>`test_validate.py`</a> in the source distribution of `vtjson`.
 ## FAQ
 Q: Why not just use the Python implementation of `JSON schema` (see https://pypi.org/project/jsonschema/)?
 
 A: Various reasons.
 - A `vtjson` schema is much more concise than a `JSON` schema!
 - `vtjson` can validate objects which are more general than strictly `JSON`. See the introductory example above. 
 - More fundamentally, the design philosophy of `vtsjon` is different. A `JSON` schema  is language independent and fully declarative. These are very nice properties but, this being said, declarative languages have a tendency to suffer from feature creep as they try to deal with more and more exotic use cases (e.g. `css`).  A `vtjson` schema on the other hand leverages the versatility of the Python language. It is generally declarative, with a limited, but easily extendable set of primitives. But if more functionality is needed then it can be extended by using appropriate bits of Python code (as the `ordered_pair` example below illustrates). In practice this is what you will need in any case since a purely declarative language will never be able to deal with every possible validation scenario.
```

### Comparing `vtjson-1.6.6/vtjson.py` & `vtjson-1.6.7/vtjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.6.6"
+__version__ = "1.6.7"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
```

