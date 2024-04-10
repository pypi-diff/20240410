# Comparing `tmp/clip2imgur-0.9.1.tar.gz` & `tmp/clip2imgur-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip2imgur-0.9.1.tar", last modified: Wed Apr 10 01:54:53 2024, max compression
+gzip compressed data, was "clip2imgur-0.9.2.tar", last modified: Wed Apr 10 02:45:30 2024, max compression
```

## Comparing `clip2imgur-0.9.1.tar` & `clip2imgur-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 01:54:53.927390 clip2imgur-0.9.1/
--rw-rw-r--   0 jaywang    (501) staff       (20)      273 2024-04-10 01:03:51.000000 clip2imgur-0.9.1/MANIFEST.in
--rw-r--r--   0 jaywang    (501) staff       (20)     5038 2024-04-10 01:54:53.927295 clip2imgur-0.9.1/PKG-INFO
--rw-r--r--   0 jaywang    (501) staff       (20)     4101 2024-04-10 01:44:11.000000 clip2imgur-0.9.1/README.md
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 01:54:53.925166 clip2imgur-0.9.1/clip2imgur/
--rw-r--r--   0 jaywang    (501) staff       (20)     6148 2024-04-10 00:59:10.000000 clip2imgur-0.9.1/clip2imgur/.DS_Store
--rw-rw-r--   0 jaywang    (501) staff       (20)      202 2024-04-10 01:51:00.000000 clip2imgur-0.9.1/clip2imgur/__init__.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 01:54:53.926451 clip2imgur-0.9.1/clip2imgur/__pycache__/
--rw-r--r--   0 jaywang    (501) staff       (20)      393 2024-04-10 01:12:01.000000 clip2imgur-0.9.1/clip2imgur/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jaywang    (501) staff       (20)     8540 2024-04-10 01:12:01.000000 clip2imgur-0.9.1/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc
--rw-r--r--   0 jaywang    (501) staff       (20)    10278 2024-04-10 01:03:23.000000 clip2imgur-0.9.1/clip2imgur/clip2imgur.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 01:54:53.926993 clip2imgur-0.9.1/clip2imgur.egg-info/
--rw-r--r--   0 jaywang    (501) staff       (20)     5038 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/PKG-INFO
--rw-r--r--   0 jaywang    (501) staff       (20)      452 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/SOURCES.txt
--rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/dependency_links.txt
--rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/not-zip-safe
--rw-r--r--   0 jaywang    (501) staff       (20)       22 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/requires.txt
--rw-r--r--   0 jaywang    (501) staff       (20)       11 2024-04-10 01:54:53.000000 clip2imgur-0.9.1/clip2imgur.egg-info/top_level.txt
--rw-rw-r--   0 jaywang    (501) staff       (20)      382 2024-04-10 01:54:53.927696 clip2imgur-0.9.1/setup.cfg
--rw-rw-r--   0 jaywang    (501) staff       (20)     1502 2024-04-10 01:52:17.000000 clip2imgur-0.9.1/setup.py
-drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 01:54:53.926792 clip2imgur-0.9.1/tests/
--rw-rw-r--   0 jaywang    (501) staff       (20)       40 2024-04-10 01:01:27.000000 clip2imgur-0.9.1/tests/__init__.py
--rw-rw-r--   0 jaywang    (501) staff       (20)      598 2024-04-10 01:51:09.000000 clip2imgur-0.9.1/tests/test_clip2imgur.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:45:30.074394 clip2imgur-0.9.2/
+-rw-rw-r--   0 jaywang    (501) staff       (20)      273 2024-04-10 01:03:51.000000 clip2imgur-0.9.2/MANIFEST.in
+-rw-r--r--   0 jaywang    (501) staff       (20)     5038 2024-04-10 02:45:30.074316 clip2imgur-0.9.2/PKG-INFO
+-rw-r--r--   0 jaywang    (501) staff       (20)     4101 2024-04-10 01:44:11.000000 clip2imgur-0.9.2/README.md
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:45:30.072144 clip2imgur-0.9.2/clip2imgur/
+-rw-r--r--   0 jaywang    (501) staff       (20)     6148 2024-04-10 00:59:10.000000 clip2imgur-0.9.2/clip2imgur/.DS_Store
+-rw-rw-r--   0 jaywang    (501) staff       (20)      202 2024-04-10 02:44:07.000000 clip2imgur-0.9.2/clip2imgur/__init__.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:45:30.073273 clip2imgur-0.9.2/clip2imgur/__pycache__/
+-rw-r--r--   0 jaywang    (501) staff       (20)      393 2024-04-10 01:12:01.000000 clip2imgur-0.9.2/clip2imgur/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jaywang    (501) staff       (20)     8540 2024-04-10 01:12:01.000000 clip2imgur-0.9.2/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc
+-rw-r--r--   0 jaywang    (501) staff       (20)    10303 2024-04-10 02:42:28.000000 clip2imgur-0.9.2/clip2imgur/clip2imgur.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:45:30.074047 clip2imgur-0.9.2/clip2imgur.egg-info/
+-rw-r--r--   0 jaywang    (501) staff       (20)     5038 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/PKG-INFO
+-rw-r--r--   0 jaywang    (501) staff       (20)      489 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/SOURCES.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/dependency_links.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)       58 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/entry_points.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)        1 2024-04-10 01:54:53.000000 clip2imgur-0.9.2/clip2imgur.egg-info/not-zip-safe
+-rw-r--r--   0 jaywang    (501) staff       (20)       22 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/requires.txt
+-rw-r--r--   0 jaywang    (501) staff       (20)       11 2024-04-10 02:45:30.000000 clip2imgur-0.9.2/clip2imgur.egg-info/top_level.txt
+-rw-rw-r--   0 jaywang    (501) staff       (20)      382 2024-04-10 02:45:30.074719 clip2imgur-0.9.2/setup.cfg
+-rw-rw-r--   0 jaywang    (501) staff       (20)     1621 2024-04-10 02:44:07.000000 clip2imgur-0.9.2/setup.py
+drwxr-xr-x   0 jaywang    (501) staff       (20)        0 2024-04-10 02:45:30.073551 clip2imgur-0.9.2/tests/
+-rw-rw-r--   0 jaywang    (501) staff       (20)       40 2024-04-10 01:01:27.000000 clip2imgur-0.9.2/tests/__init__.py
+-rw-rw-r--   0 jaywang    (501) staff       (20)      598 2024-04-10 01:51:09.000000 clip2imgur-0.9.2/tests/test_clip2imgur.py
```

### Comparing `clip2imgur-0.9.1/PKG-INFO` & `clip2imgur-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip2imgur
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple CLI that uploads your image in the clipboard to Imgur.
 Home-page: https://github.com/xiaohk/clip2imgur
 Author: Jay Wang
 Author-email: jayw@zijie.wang
 License: MIT license
 Keywords: Imgur,CLI,Image,Clipboard
 Platform: Linux
```

### Comparing `clip2imgur-0.9.1/README.md` & `clip2imgur-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.1/clip2imgur/.DS_Store` & `clip2imgur-0.9.2/clip2imgur/.DS_Store`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.1/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc` & `clip2imgur-0.9.2/clip2imgur/__pycache__/clip2imgur.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `clip2imgur-0.9.1/clip2imgur/clip2imgur.py` & `clip2imgur-0.9.2/clip2imgur/clip2imgur.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,10 +320,14 @@
             return
 
         return int(time()) < int(self.auth_values.time) + int(
             self.auth_values.expires_in
         )
 
 
+def main():
+    app = Clip2imgurApp()
+    app.run()
+
+
 if __name__ == "__main__":
-    cli = Clip2imgurApp()
-    cli.run()
+    main()
```

### Comparing `clip2imgur-0.9.1/clip2imgur.egg-info/PKG-INFO` & `clip2imgur-0.9.2/clip2imgur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip2imgur
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple CLI that uploads your image in the clipboard to Imgur.
 Home-page: https://github.com/xiaohk/clip2imgur
 Author: Jay Wang
 Author-email: jayw@zijie.wang
 License: MIT license
 Keywords: Imgur,CLI,Image,Clipboard
 Platform: Linux
```

### Comparing `clip2imgur-0.9.1/setup.py` & `clip2imgur-0.9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,10 +43,15 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     name="clip2imgur",
     packages=find_packages(include=["clip2imgur", "clip2imgur.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/xiaohk/clip2imgur",
-    version="0.9.1",
+    version="0.9.2",
     zip_safe=False,
+    entry_points={
+        "console_scripts": [
+            "clip2imgur=clip2imgur.clip2imgur:main",
+        ],
+    },
 )
```

### Comparing `clip2imgur-0.9.1/tests/test_clip2imgur.py` & `clip2imgur-0.9.2/tests/test_clip2imgur.py`

 * *Files identical despite different names*

