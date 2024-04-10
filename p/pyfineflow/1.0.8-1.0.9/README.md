# Comparing `tmp/pyfineflow-1.0.8.tar.gz` & `tmp/pyfineflow-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfineflow-1.0.8.tar", last modified: Sun Apr  7 14:09:03 2024, max compression
+gzip compressed data, was "pyfineflow-1.0.9.tar", last modified: Wed Apr 10 11:57:29 2024, max compression
```

## Comparing `pyfineflow-1.0.8.tar` & `pyfineflow-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/
--rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1142 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.932138 pyfineflow-1.0.8/pyfineflow/
--rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/__init__.py
--rw-rw-rw-   0        0        0    16364 2024-04-06 14:33:16.000000 pyfineflow-1.0.8/pyfineflow/core.py
--rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/log_conf.py
--rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/schemas.py
--rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.0.8/pyfineflow/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/pyfineflow.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-07 14:09:01.000000 pyfineflow-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:57:29.581475 pyfineflow-1.0.9/
+-rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1142 2024-04-10 11:57:29.580948 pyfineflow-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 11:57:29.566714 pyfineflow-1.0.9/pyfineflow/
+-rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.0.9/pyfineflow/__init__.py
+-rw-rw-rw-   0        0        0     1586 2024-04-10 11:38:17.000000 pyfineflow-1.0.9/pyfineflow/__main__.py
+-rw-rw-rw-   0        0        0    16364 2024-04-06 14:33:16.000000 pyfineflow-1.0.9/pyfineflow/core.py
+-rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.0.9/pyfineflow/log_conf.py
+-rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.0.9/pyfineflow/schemas.py
+-rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.0.9/pyfineflow/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 11:57:29.578812 pyfineflow-1.0.9/pyfineflow.egg-info/
+-rw-rw-rw-   0        0        0     1142 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 11:57:29.000000 pyfineflow-1.0.9/pyfineflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 11:57:29.582487 pyfineflow-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      676 2024-04-10 11:57:20.000000 pyfineflow-1.0.9/setup.py
```

### Comparing `pyfineflow-1.0.8/LICENSE` & `pyfineflow-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.8/PKG-INFO` & `pyfineflow-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.8
+Version: 1.0.9
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.0.8/pyfineflow/core.py` & `pyfineflow-1.0.9/pyfineflow/core.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.8/pyfineflow/log_conf.py` & `pyfineflow-1.0.9/pyfineflow/log_conf.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.8/pyfineflow/schemas.py` & `pyfineflow-1.0.9/pyfineflow/schemas.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.8/pyfineflow/utils.py` & `pyfineflow-1.0.9/pyfineflow/utils.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.8/pyfineflow.egg-info/PKG-INFO` & `pyfineflow-1.0.9/pyfineflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.8
+Version: 1.0.9
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.0.8/setup.py` & `pyfineflow-1.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 # --skip-existing 覆盖
 # python setup.py sdist bdist_wheel
 # twine upload dist/* --skip-existing
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyfineflow',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(exclude=['__pycache__']),
     description='python nodes server for fineflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'fastapi',
-    ]
+        'fastapi[all]~=0.110.1',
+    ],
+    entry_points={
+        'console_scripts': [
+            'pyfineflow = pyfineflow.__main__:main'
+        ]
+    }
 )
```

