# Comparing `tmp/clamnibs-0.1.1.tar.gz` & `tmp/clamnibs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clamnibs-0.1.1.tar", last modified: Wed Apr 10 13:09:22 2024, max compression
+gzip compressed data, was "clamnibs-0.1.2.tar", last modified: Wed Apr 10 13:19:21 2024, max compression
```

## Comparing `clamnibs-0.1.1.tar` & `clamnibs-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 13:09:22.304422 clamnibs-0.1.1/
--rw-rw-rw-   0        0        0     1093 2024-02-08 09:42:07.000000 clamnibs-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       24 2024-04-10 12:59:07.000000 clamnibs-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1014 2024-04-10 13:09:22.304422 clamnibs-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-02-08 10:15:32.000000 clamnibs-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 13:09:22.304422 clamnibs-0.1.1/clamnibs.egg-info/
--rw-rw-rw-   0        0        0     1014 2024-04-10 13:09:22.000000 clamnibs-0.1.1/clamnibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-10 13:09:22.000000 clamnibs-0.1.1/clamnibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:09:22.000000 clamnibs-0.1.1/clamnibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-10 13:09:22.000000 clamnibs-0.1.1/clamnibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 13:09:22.000000 clamnibs-0.1.1/clamnibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      175 2024-04-09 15:47:10.000000 clamnibs-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 13:09:22.304422 clamnibs-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      912 2024-04-10 13:07:26.000000 clamnibs-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:19:21.933398 clamnibs-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2024-02-08 09:42:07.000000 clamnibs-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-04-10 12:59:07.000000 clamnibs-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1014 2024-04-10 13:19:21.932166 clamnibs-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-02-08 10:15:32.000000 clamnibs-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 13:19:21.900398 clamnibs-0.1.2/clamnibs/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:17:50.000000 clamnibs-0.1.2/clamnibs/__init__.py
+-rw-rw-rw-   0        0        0     9122 2024-03-23 17:42:25.000000 clamnibs-0.1.2/clamnibs/base.py
+-rw-rw-rw-   0        0        0    10996 2024-03-18 12:15:24.000000 clamnibs-0.1.2/clamnibs/beamformer.py
+-rw-rw-rw-   0        0        0     8010 2024-03-18 12:26:54.000000 clamnibs-0.1.2/clamnibs/misc.py
+-rw-rw-rw-   0        0        0     7769 2024-03-18 12:11:20.000000 clamnibs-0.1.2/clamnibs/sensor.py
+-rw-rw-rw-   0        0        0    16012 2024-03-25 09:08:00.000000 clamnibs-0.1.2/clamnibs/source.py
+-rw-rw-rw-   0        0        0    31382 2024-04-09 15:37:41.000000 clamnibs-0.1.2/clamnibs/stats.py
+-rw-rw-rw-   0        0        0     4033 2024-03-18 12:46:51.000000 clamnibs-0.1.2/clamnibs/viz.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:19:21.932166 clamnibs-0.1.2/clamnibs.egg-info/
+-rw-rw-rw-   0        0        0     1014 2024-04-10 13:19:21.000000 clamnibs-0.1.2/clamnibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-10 13:19:21.000000 clamnibs-0.1.2/clamnibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:19:21.000000 clamnibs-0.1.2/clamnibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2024-04-10 13:19:21.000000 clamnibs-0.1.2/clamnibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 13:19:21.000000 clamnibs-0.1.2/clamnibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      175 2024-04-09 15:47:10.000000 clamnibs-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:19:21.933398 clamnibs-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      912 2024-04-10 13:18:25.000000 clamnibs-0.1.2/setup.py
```

### Comparing `clamnibs-0.1.1/LICENSE` & `clamnibs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clamnibs-0.1.1/PKG-INFO` & `clamnibs-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clamnibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Analysis of closed-loop amplitude-modulated non-invasive brain stimulation experiments
 Home-page: https://github.com/davidhaslacher/clam-nibs
 Author: David Haslacher
 Author-email: haslacherdavid@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clamnibs-0.1.1/clamnibs.egg-info/PKG-INFO` & `clamnibs-0.1.2/clamnibs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clamnibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Analysis of closed-loop amplitude-modulated non-invasive brain stimulation experiments
 Home-page: https://github.com/davidhaslacher/clam-nibs
 Author: David Haslacher
 Author-email: haslacherdavid@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clamnibs-0.1.1/setup.py` & `clamnibs-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='clamnibs',
-    version='0.1.1',
+    version='0.1.2',
     description='Analysis of closed-loop amplitude-modulated non-invasive brain stimulation experiments',
     long_description='This toolbox contains all software required to implement closed-loop amplitude-modulated non-invasive brain stimulation (CLAM-NIBS) and evaluate the resulting electroencephalography (EEG) or magnetoencephalography (MEG) data.',
     author='David Haslacher',
     author_email='haslacherdavid@gmail.com',
     url='https://github.com/davidhaslacher/clam-nibs',
     packages=find_packages(),
     install_requires=requirements,
```

