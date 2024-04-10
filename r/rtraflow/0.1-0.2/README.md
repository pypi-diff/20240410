# Comparing `tmp/rtraflow-0.1.tar.gz` & `tmp/rtraflow-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtraflow-0.1.tar", last modified: Wed Apr 10 06:19:52 2024, max compression
+gzip compressed data, was "rtraflow-0.2.tar", last modified: Wed Apr 10 06:39:54 2024, max compression
```

## Comparing `rtraflow-0.1.tar` & `rtraflow-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:19:52.791325 rtraflow-0.1/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      396 2024-04-10 06:19:52.791039 rtraflow-0.1/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:19:52.789867 rtraflow-0.1/rtraflow/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:13:58.000000 rtraflow-0.1/rtraflow/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:14:08.000000 rtraflow-0.1/rtraflow/connector.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:19:52.790745 rtraflow-0.1/rtraflow.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      396 2024-04-10 06:19:52.000000 rtraflow-0.1/rtraflow.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      210 2024-04-10 06:19:52.000000 rtraflow-0.1/rtraflow.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-10 06:19:52.000000 rtraflow-0.1/rtraflow.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 06:19:52.000000 rtraflow-0.1/rtraflow.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 06:19:52.000000 rtraflow-0.1/rtraflow.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-10 06:19:52.791528 rtraflow-0.1/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      621 2024-04-10 06:16:46.000000 rtraflow-0.1/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:39:54.860036 rtraflow-0.2/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      396 2024-04-10 06:39:54.859831 rtraflow-0.2/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:39:54.859048 rtraflow-0.2/rtraflow/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:13:58.000000 rtraflow-0.2/rtraflow/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:14:08.000000 rtraflow-0.2/rtraflow/connector.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-10 06:39:54.859647 rtraflow-0.2/rtraflow.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      396 2024-04-10 06:39:54.000000 rtraflow-0.2/rtraflow.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      210 2024-04-10 06:39:54.000000 rtraflow-0.2/rtraflow.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-10 06:39:54.000000 rtraflow-0.2/rtraflow.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 06:39:54.000000 rtraflow-0.2/rtraflow.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        9 2024-04-10 06:39:54.000000 rtraflow-0.2/rtraflow.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-10 06:39:54.860079 rtraflow-0.2/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      621 2024-04-10 06:31:54.000000 rtraflow-0.2/setup.py
```

### Comparing `rtraflow-0.1/setup.py` & `rtraflow-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rtraflow',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Udit Raj',
     author_email='udit_2312res708@iitp.ac.in',
     description='Package for RTRAConnect functionality',
```

