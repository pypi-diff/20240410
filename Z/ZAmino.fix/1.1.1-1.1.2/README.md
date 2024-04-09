# Comparing `tmp/ZAmino.fix-1.1.1.tar.gz` & `tmp/ZAmino.fix-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZAmino.fix-1.1.1.tar", last modified: Thu Mar 21 03:19:10 2024, max compression
+gzip compressed data, was "ZAmino.fix-1.1.2.tar", last modified: Tue Apr  9 22:12:07 2024, max compression
```

## Comparing `ZAmino.fix-1.1.1.tar` & `ZAmino.fix-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.611418 ZAmino.fix-1.1.1/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 ZAmino.fix-1.1.1/LICENSE
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      633 2024-03-21 03:19:10.611418 ZAmino.fix-1.1.1/PKG-INFO
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 ZAmino.fix-1.1.1/README.md
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.611418 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      633 2024-03-21 03:19:10.000000 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-03-21 03:19:10.000000 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-03-21 03:19:10.000000 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       79 2024-03-21 03:19:10.000000 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/requires.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-03-21 03:19:10.000000 ZAmino.fix-1.1.1/ZAmino.fix.egg-info/top_level.txt
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.601418 ZAmino.fix-1.1.1/ZAminofix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      299 2024-03-21 03:16:09.000000 ZAmino.fix-1.1.1/ZAminofix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 ZAmino.fix-1.1.1/ZAminofix/acm.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.601418 ZAmino.fix-1.1.1/ZAminofix/asyncfix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.1/ZAminofix/asyncfix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.1/ZAminofix/asyncfix/acm.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.1/ZAminofix/asyncfix/client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 ZAmino.fix-1.1.1/ZAminofix/asyncfix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.1/ZAminofix/asyncfix/sub_client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   100222 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.1/ZAminofix/client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.601418 ZAmino.fix-1.1.1/ZAminofix/lib/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.1/ZAminofix/lib/__init__.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-03-21 03:19:10.611418 ZAmino.fix-1.1.1/ZAminofix/lib/util/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 ZAmino.fix-1.1.1/ZAminofix/lib/util/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.1/ZAminofix/lib/util/exceptions.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     3912 2024-03-21 03:13:53.000000 ZAmino.fix-1.1.1/ZAminofix/lib/util/headers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 ZAmino.fix-1.1.1/ZAminofix/lib/util/helpers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198051 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.1/ZAminofix/lib/util/objects.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 ZAmino.fix-1.1.1/ZAminofix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   117552 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.1/ZAminofix/sub_client.py
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-03-21 03:19:10.611418 ZAmino.fix-1.1.1/setup.cfg
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      742 2024-03-21 03:18:58.000000 ZAmino.fix-1.1.1/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 ZAmino.fix-1.1.2/LICENSE
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      599 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/PKG-INFO
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 ZAmino.fix-1.1.2/README.md
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      599 2024-04-09 22:12:07.000000 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-04-09 22:12:07.000000 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-04-09 22:12:07.000000 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       79 2024-04-09 22:12:07.000000 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/requires.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-04-09 22:12:07.000000 ZAmino.fix-1.1.2/ZAmino.fix.egg-info/top_level.txt
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.574999 ZAmino.fix-1.1.2/ZAminofix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      691 2024-04-09 16:12:50.000000 ZAmino.fix-1.1.2/ZAminofix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 ZAmino.fix-1.1.2/ZAminofix/acm.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/ZAminofix/asyncfix/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.2/ZAminofix/asyncfix/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.2/ZAminofix/asyncfix/acm.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.2/ZAminofix/asyncfix/client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 ZAmino.fix-1.1.2/ZAminofix/asyncfix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.2/ZAminofix/asyncfix/sub_client.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   100222 2023-05-21 20:55:10.000000 ZAmino.fix-1.1.2/ZAminofix/client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/ZAminofix/lib/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.2/ZAminofix/lib/__init__.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/ZAminofix/lib/util/
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 ZAmino.fix-1.1.2/ZAminofix/lib/util/__init__.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.2/ZAminofix/lib/util/exceptions.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4107 2024-04-09 22:04:36.000000 ZAmino.fix-1.1.2/ZAminofix/lib/util/headers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 ZAmino.fix-1.1.2/ZAminofix/lib/util/helpers.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198051 2023-01-20 07:25:50.000000 ZAmino.fix-1.1.2/ZAminofix/lib/util/objects.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13193 2023-05-21 21:07:28.000000 ZAmino.fix-1.1.2/ZAminofix/socket.py
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   117552 2023-04-06 18:02:18.000000 ZAmino.fix-1.1.2/ZAminofix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-04-09 22:12:07.584999 ZAmino.fix-1.1.2/setup.cfg
+-rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      701 2024-04-09 22:10:57.000000 ZAmino.fix-1.1.2/setup.py
```

### Comparing `ZAmino.fix-1.1.1/LICENSE` & `ZAmino.fix-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/PKG-INFO` & `ZAmino.fix-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.1
+Version: 1.1.2
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Author-email: hgdcytdgh@gmail.com
 Keywords: ZAminoZAmino.fixaminoapps,amino.fix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
```

### Comparing `ZAmino.fix-1.1.1/ZAmino.fix.egg-info/PKG-INFO` & `ZAmino.fix-1.1.2/ZAmino.fix.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.1
+Version: 1.1.2
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Author-email: hgdcytdgh@gmail.com
 Keywords: ZAminoZAmino.fixaminoapps,amino.fix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
```

### Comparing `ZAmino.fix-1.1.1/ZAmino.fix.egg-info/SOURCES.txt` & `ZAmino.fix-1.1.2/ZAmino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/acm.py` & `ZAmino.fix-1.1.2/ZAminofix/acm.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/asyncfix/acm.py` & `ZAmino.fix-1.1.2/ZAminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/asyncfix/client.py` & `ZAmino.fix-1.1.2/ZAminofix/asyncfix/client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/asyncfix/socket.py` & `ZAmino.fix-1.1.2/ZAminofix/asyncfix/socket.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/asyncfix/sub_client.py` & `ZAmino.fix-1.1.2/ZAminofix/asyncfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/client.py` & `ZAmino.fix-1.1.2/ZAminofix/client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/lib/util/exceptions.py` & `ZAmino.fix-1.1.2/ZAminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/lib/util/headers.py` & `ZAmino.fix-1.1.2/ZAminofix/lib/util/headers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from ZAminofix.lib.util import signature
-
+import random
 from uuid import uuid4
 
+iphone_model = f"Apple iPhone{random.randint(0, 99999)}"
+ios_version = "iOS v16.5"
+main_version = "Main/3.12.2"
+
+
 sid = None
 device_id = None
 userId = None
-user_agent = None
+user_agent = f"{iphone_model},1 {ios_version} {main_version}"
+print(user_agent)
 
 class ApisHeaders:
     def __init__(self, data = None, type = None, deviceId: str = None, sig: str = None):
 
         headers = {
             "Accept-Language": "en-US",
             "Content-Type": "application/x-www-form-urlencoded",
```

### Comparing `ZAmino.fix-1.1.1/ZAminofix/lib/util/helpers.py` & `ZAmino.fix-1.1.2/ZAminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/lib/util/objects.py` & `ZAmino.fix-1.1.2/ZAminofix/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/socket.py` & `ZAmino.fix-1.1.2/ZAminofix/socket.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/ZAminofix/sub_client.py` & `ZAmino.fix-1.1.2/ZAminofix/sub_client.py`

 * *Files identical despite different names*

### Comparing `ZAmino.fix-1.1.1/setup.py` & `ZAmino.fix-1.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="ZAmino.fix",
     author="ZOOM",
-    version="1.1.1",
-    author_email="hgdcytdgh@gmail.com",
+    version="1.1.2",
     description="Aminofix update. https://t.me/ZAminoZ",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
     	'ZAmino'
     	'ZAmino.fix'
```

