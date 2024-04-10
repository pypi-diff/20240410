# Comparing `tmp/ortelius-cli-9.3.270.tar.gz` & `tmp/ortelius-cli-9.3.272.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.270.tar", last modified: Tue Apr  9 21:28:59 2024, max compression
+gzip compressed data, was "ortelius-cli-9.3.272.tar", last modified: Tue Apr  9 22:36:07 2024, max compression
```

## Comparing `ortelius-cli-9.3.270.tar` & `ortelius-cli-9.3.272.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:28:59.639604 ortelius-cli-9.3.270/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.270/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.270/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 21:28:59.638579 ortelius-cli-9.3.270/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.270/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:28:59.620467 ortelius-cli-9.3.270/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    70828 2024-04-09 21:28:41.000000 ortelius-cli-9.3.270/bin/dh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:28:59.622645 ortelius-cli-9.3.270/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-09 21:28:41.000000 ortelius-cli-9.3.270/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    71213 2024-04-09 21:28:28.000000 ortelius-cli-9.3.270/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:28:59.625827 ortelius-cli-9.3.270/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.270/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.270/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:28:59.636560 ortelius-cli-9.3.270/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 21:28:59.000000 ortelius-cli-9.3.270/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-09 21:28:59.000000 ortelius-cli-9.3.270/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-09 21:28:59.000000 ortelius-cli-9.3.270/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-09 21:28:59.000000 ortelius-cli-9.3.270/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-09 21:28:59.000000 ortelius-cli-9.3.270/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-09 21:28:59.639756 ortelius-cli-9.3.270/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-09 21:28:41.000000 ortelius-cli-9.3.270/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 22:36:07.130959 ortelius-cli-9.3.272/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.272/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.272/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 22:36:07.125479 ortelius-cli-9.3.272/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.272/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 22:36:07.112797 ortelius-cli-9.3.272/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70828 2024-04-09 22:35:52.000000 ortelius-cli-9.3.272/bin/dh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 22:36:07.114594 ortelius-cli-9.3.272/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-09 22:35:52.000000 ortelius-cli-9.3.272/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    71203 2024-04-09 22:35:31.000000 ortelius-cli-9.3.272/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 22:36:07.117287 ortelius-cli-9.3.272/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.272/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.272/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 22:36:07.123515 ortelius-cli-9.3.272/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 22:36:07.000000 ortelius-cli-9.3.272/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-09 22:36:07.000000 ortelius-cli-9.3.272/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-09 22:36:07.000000 ortelius-cli-9.3.272/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-09 22:36:07.000000 ortelius-cli-9.3.272/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-09 22:36:07.000000 ortelius-cli-9.3.272/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-09 22:36:07.131209 ortelius-cli-9.3.272/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-09 22:35:52.000000 ortelius-cli-9.3.272/setup.py
```

### Comparing `ortelius-cli-9.3.270/LICENSE` & `ortelius-cli-9.3.272/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.270/PKG-INFO` & `ortelius-cli-9.3.272/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.270
+Version: 9.3.272
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.270/README.md` & `ortelius-cli-9.3.272/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.270/bin/dh` & `ortelius-cli-9.3.272/bin/dh`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.270"
+__version__ = "9.3.272"
 
 import json
 import os
 import re
 import stat
 import sys
 from datetime import datetime
```

### Comparing `ortelius-cli-9.3.270/deployhub/dhapi.py` & `ortelius-cli-9.3.272/deployhub/dhapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,20 +104,20 @@
             res = requests.post(url, data=payload, cookies=cookies, headers={"Content-Type": "application/json", "host": "console.deployhub.com"}, timeout=300)
 
         if res is None:
             return None
 
         if res.status_code < 200 and res.status_code > 299:
             return None
-        
+
         try:
             json_data = res.json()  
             return json_data
         except ValueError:
-            return None  
+            return {}  
     except requests.exceptions.ConnectionError as conn_error:
         print(str(conn_error))
     return None
 
 
 def post_json_with_header(url, token):
     """
```

### Comparing `ortelius-cli-9.3.270/doc/deployhub.md` & `ortelius-cli-9.3.272/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.270/doc/dh.md` & `ortelius-cli-9.3.272/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.270/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.272/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.270
+Version: 9.3.272
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.270/setup.py` & `ortelius-cli-9.3.272/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.270",
+    version="9.3.272",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

