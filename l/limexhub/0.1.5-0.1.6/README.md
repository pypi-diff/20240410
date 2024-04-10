# Comparing `tmp/limexhub-0.1.5.tar.gz` & `tmp/limexhub-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limexhub-0.1.5.tar", last modified: Tue Apr  9 09:25:41 2024, max compression
+gzip compressed data, was "limexhub-0.1.6.tar", last modified: Tue Apr  9 16:06:46 2024, max compression
```

## Comparing `limexhub-0.1.5.tar` & `limexhub-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.199358 limexhub-0.1.5/
--rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.5/LICENSE
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 09:25:41.199231 limexhub-0.1.5/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.5/README.md
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.198467 limexhub-0.1.5/limexhub/
--rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.5/limexhub/__init__.py
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2236 2024-04-09 09:22:09.000000 limexhub-0.1.5/limexhub/restapi.py
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 09:25:41.199059 limexhub-0.1.5/limexhub.egg-info/
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/SOURCES.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/dependency_links.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/requires.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 09:25:41.000000 limexhub-0.1.5/limexhub.egg-info/top_level.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-09 09:25:41.199400 limexhub-0.1.5/setup.cfg
--rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-09 09:25:00.000000 limexhub-0.1.5/setup.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.304426 limexhub-0.1.6/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.6/LICENSE
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 16:06:46.304313 limexhub-0.1.6/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.6/README.md
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.303541 limexhub-0.1.6/limexhub/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.6/limexhub/__init__.py
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2944 2024-04-09 16:06:37.000000 limexhub-0.1.6/limexhub/restapi.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-09 16:06:46.304150 limexhub-0.1.6/limexhub.egg-info/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/requires.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-09 16:06:46.000000 limexhub-0.1.6/limexhub.egg-info/top_level.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-09 16:06:46.304468 limexhub-0.1.6/setup.cfg
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-09 14:38:32.000000 limexhub-0.1.6/setup.py
```

### Comparing `limexhub-0.1.5/LICENSE` & `limexhub-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.5/PKG-INFO` & `limexhub-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.5/README.md` & `limexhub-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.5/limexhub.egg-info/PKG-INFO` & `limexhub-0.1.6/limexhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.5/setup.py` & `limexhub-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='limexhub',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     include_package_data=True,
     description='A simple API wrapper for Limex DataHub',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Limex-com/limexhub-python',
     author='V.Arbuzov',
```

