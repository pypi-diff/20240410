# Comparing `tmp/pygo-jwt-0.0.8.tar.gz` & `tmp/pygo-jwt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygo-jwt-0.0.8.tar", last modified: Tue Apr  2 23:43:17 2024, max compression
+gzip compressed data, was "pygo-jwt-0.0.9.tar", last modified: Tue Apr  9 21:48:03 2024, max compression
```

## Comparing `pygo-jwt-0.0.8.tar` & `pygo-jwt-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.553476 pygo-jwt-0.0.8/pygo_jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/b64_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.553476 pygo-jwt-0.0.8/pygo_jwt/go/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.553476 pygo-jwt-0.0.8/pygo_jwt/go/core/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/core/conversions.go
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/core/misc.go
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/core/private_factory.go
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/core/public_factory.go
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/core/sign_verify.go
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/go.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/pygo_jwt/go/util/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/util/b64_util.go
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/util/hash_util.go
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/util/json_util.go
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/util/str_util.go
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/util/type_alias.go
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/wrapper.go
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/wrapper_util.go
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/go/wrapper_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_jwt/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/pygo_jwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-02 23:43:17.000000 pygo-jwt-0.0.8/pygo_jwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 23:43:17.000000 pygo-jwt-0.0.8/pygo_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:43:17.000000 pygo-jwt-0.0.8/pygo_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 23:43:17.000000 pygo-jwt-0.0.8/pygo_jwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 23:43:17.000000 pygo-jwt-0.0.8/pygo_jwt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/pygo_tools_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_tools_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/pygo_tools_lib/wrapper_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:43:17.557476 pygo-jwt-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/tests/test-handle-panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/tests/test-pygo-jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-02 23:42:55.000000 pygo-jwt-0.0.8/tests/test-pyjwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.574627 pygo-jwt-0.0.9/pygo_jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/b64_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.574627 pygo-jwt-0.0.9/pygo_jwt/go/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/pygo_jwt/go/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/core/conversions.go
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/core/misc.go
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/core/private_factory.go
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/core/public_factory.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/core/sign_verify.go
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/go.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/pygo_jwt/go/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/util/b64_util.go
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/util/hash_util.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/util/json_util.go
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/util/str_util.go
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/util/type_alias.go
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/wrapper.go
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/wrapper_util.go
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/go/wrapper_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/jwt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_jwt/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/pygo_jwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 21:48:03.000000 pygo-jwt-0.0.9/pygo_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 21:48:03.000000 pygo-jwt-0.0.9/pygo_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:48:03.000000 pygo-jwt-0.0.9/pygo_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 21:48:03.000000 pygo-jwt-0.0.9/pygo_jwt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/pygo_tools_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_tools_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pygo_tools_lib/wrapper_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:48:03.578627 pygo-jwt-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/tests/test-handle-panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/tests/test-pygo-jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 21:47:42.000000 pygo-jwt-0.0.9/tests/test-pyjwt.py
```

### Comparing `pygo-jwt-0.0.8/PKG-INFO` & `pygo-jwt-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pygo-jwt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Encode and Decode RS256 JSON Web Tokens with Python and Go
-Author: Rajan Khullar
-Author-email: rkhullar03@gmail.com
-License: MIT NON-AI
-Project-URL: Source, https://github.com/rkhullar/python-libraries/tree/main/pygo-jwt
-Requires-Python: >=3.10, <4.0
+Author-email: Rajan Khullar <rkhullar03@gmail.com>
+License: MIT NON-AI License
+Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-jwt
+Keywords: python,golang,jwt,rsa
+Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: cffi
 
 ## pygo-jwt
 
 This project focuses on managing JSON Web Tokens signed with RS256. Inspired by [pyjwt](https://pypi.org/project/PyJWT),
 this library provides core encode and decode functionality, utilizing the standard `crypto` package within Go instead of
 [cryptography](https://pypi.org/project/cryptography).
```

### Comparing `pygo-jwt-0.0.8/pygo_jwt/b64_util.py` & `pygo-jwt-0.0.9/pygo_jwt/b64_util.py`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/core/conversions.go` & `pygo-jwt-0.0.9/pygo_jwt/go/core/conversions.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/core/misc.go` & `pygo-jwt-0.0.9/pygo_jwt/go/core/misc.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/core/private_factory.go` & `pygo-jwt-0.0.9/pygo_jwt/go/core/private_factory.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/core/public_factory.go` & `pygo-jwt-0.0.9/pygo_jwt/go/core/public_factory.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/core/sign_verify.go` & `pygo-jwt-0.0.9/pygo_jwt/go/core/sign_verify.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/util/b64_util.go` & `pygo-jwt-0.0.9/pygo_jwt/go/util/b64_util.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/util/hash_util.go` & `pygo-jwt-0.0.9/pygo_jwt/go/util/hash_util.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/util/json_util.go` & `pygo-jwt-0.0.9/pygo_jwt/go/util/json_util.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/wrapper.go` & `pygo-jwt-0.0.9/pygo_jwt/go/wrapper.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/go/wrapper_util.go` & `pygo-jwt-0.0.9/pygo_jwt/go/wrapper_util.go`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/jwt_util.py` & `pygo-jwt-0.0.9/pygo_jwt/jwt_util.py`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt/wrapper.py` & `pygo-jwt-0.0.9/pygo_jwt/wrapper.py`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/pygo_jwt.egg-info/PKG-INFO` & `pygo-jwt-0.0.9/pygo_jwt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pygo-jwt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Encode and Decode RS256 JSON Web Tokens with Python and Go
-Author: Rajan Khullar
-Author-email: rkhullar03@gmail.com
-License: MIT NON-AI
-Project-URL: Source, https://github.com/rkhullar/python-libraries/tree/main/pygo-jwt
-Requires-Python: >=3.10, <4.0
+Author-email: Rajan Khullar <rkhullar03@gmail.com>
+License: MIT NON-AI License
+Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-jwt
+Keywords: python,golang,jwt,rsa
+Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: cffi
 
 ## pygo-jwt
 
 This project focuses on managing JSON Web Tokens signed with RS256. Inspired by [pyjwt](https://pypi.org/project/PyJWT),
 this library provides core encode and decode functionality, utilizing the standard `crypto` package within Go instead of
 [cryptography](https://pypi.org/project/cryptography).
```

### Comparing `pygo-jwt-0.0.8/pygo_jwt.egg-info/SOURCES.txt` & `pygo-jwt-0.0.9/pygo_jwt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 MANIFEST.in
-config.json
+pyproject.toml
 readme.md
-setup.py
 pygo_jwt/__init__.py
 pygo_jwt/b64_util.py
 pygo_jwt/errors.py
 pygo_jwt/jwt_util.py
 pygo_jwt/time_util.py
 pygo_jwt/wrapper.py
 pygo_jwt.egg-info/PKG-INFO
 pygo_jwt.egg-info/SOURCES.txt
 pygo_jwt.egg-info/dependency_links.txt
-pygo_jwt.egg-info/requires.txt
 pygo_jwt.egg-info/top_level.txt
 pygo_jwt/go/Makefile
 pygo_jwt/go/go.mod
 pygo_jwt/go/wrapper.go
 pygo_jwt/go/wrapper_util.go
 pygo_jwt/go/wrapper_util.h
 pygo_jwt/go/core/conversions.go
```

### Comparing `pygo-jwt-0.0.8/pygo_tools_lib/wrapper_util.py` & `pygo-jwt-0.0.9/pygo_tools_lib/wrapper_util.py`

 * *Files identical despite different names*

### Comparing `pygo-jwt-0.0.8/readme.md` & `pygo-jwt-0.0.9/readme.md`

 * *Files identical despite different names*

