# Comparing `tmp/abenity-1.3.0.tar.gz` & `tmp/abenity-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abenity-1.3.0.tar", last modified: Mon Jan  8 21:12:17 2024, max compression
+gzip compressed data, was "abenity-1.4.0.tar", last modified: Tue Apr  9 18:42:49 2024, max compression
```

## Comparing `abenity-1.3.0.tar` & `abenity-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-01-08 21:12:17.727297 abenity-1.3.0/
--rw-r--r--   0 brent      (501) staff       (20)     1109 2024-01-05 14:06:08.000000 abenity-1.3.0/LICENSE
--rw-r--r--   0 brent      (501) staff       (20)      766 2024-01-08 21:12:17.727090 abenity-1.3.0/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      241 2024-01-05 14:06:08.000000 abenity-1.3.0/README.md
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-01-08 21:12:17.725643 abenity-1.3.0/abenity/
--rw-r--r--   0 brent      (501) staff       (20)     1147 2024-01-05 14:06:08.000000 abenity-1.3.0/abenity/__init__.py
--rw-r--r--   0 brent      (501) staff       (20)     6662 2024-01-05 14:06:08.000000 abenity-1.3.0/abenity/client.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-01-08 21:12:17.726766 abenity-1.3.0/abenity.egg-info/
--rw-r--r--   0 brent      (501) staff       (20)      766 2024-01-08 21:12:17.000000 abenity-1.3.0/abenity.egg-info/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      236 2024-01-08 21:12:17.000000 abenity-1.3.0/abenity.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (501) staff       (20)        1 2024-01-08 21:12:17.000000 abenity-1.3.0/abenity.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (501) staff       (20)       68 2024-01-08 21:12:17.000000 abenity-1.3.0/abenity.egg-info/requires.txt
--rw-r--r--   0 brent      (501) staff       (20)        8 2024-01-08 21:12:17.000000 abenity-1.3.0/abenity.egg-info/top_level.txt
--rw-r--r--   0 brent      (501) staff       (20)       38 2024-01-08 21:12:17.727345 abenity-1.3.0/setup.cfg
--rw-r--r--   0 brent      (501) staff       (20)     1380 2024-01-08 21:11:23.000000 abenity-1.3.0/setup.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-01-08 21:12:17.726441 abenity-1.3.0/tests/
--rw-r--r--   0 brent      (501) staff       (20)     4389 2024-01-05 14:06:08.000000 abenity-1.3.0/tests/test_sso.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-04-09 18:42:49.675951 abenity-1.4.0/
+-rw-r--r--   0 brent      (501) staff       (20)     1109 2024-01-05 14:06:08.000000 abenity-1.4.0/LICENSE
+-rw-r--r--   0 brent      (501) staff       (20)      764 2024-04-09 18:42:49.675768 abenity-1.4.0/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      241 2024-01-05 14:06:08.000000 abenity-1.4.0/README.md
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-04-09 18:42:49.674479 abenity-1.4.0/abenity/
+-rw-r--r--   0 brent      (501) staff       (20)     1147 2024-01-05 14:06:08.000000 abenity-1.4.0/abenity/__init__.py
+-rw-r--r--   0 brent      (501) staff       (20)     6662 2024-04-09 18:29:00.000000 abenity-1.4.0/abenity/client.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-04-09 18:42:49.675466 abenity-1.4.0/abenity.egg-info/
+-rw-r--r--   0 brent      (501) staff       (20)      764 2024-04-09 18:42:49.000000 abenity-1.4.0/abenity.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      236 2024-04-09 18:42:49.000000 abenity-1.4.0/abenity.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (501) staff       (20)        1 2024-04-09 18:42:49.000000 abenity-1.4.0/abenity.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (501) staff       (20)       66 2024-04-09 18:42:49.000000 abenity-1.4.0/abenity.egg-info/requires.txt
+-rw-r--r--   0 brent      (501) staff       (20)        8 2024-04-09 18:42:49.000000 abenity-1.4.0/abenity.egg-info/top_level.txt
+-rw-r--r--   0 brent      (501) staff       (20)       38 2024-04-09 18:42:49.676005 abenity-1.4.0/setup.cfg
+-rw-r--r--   0 brent      (501) staff       (20)     1378 2024-04-09 18:34:59.000000 abenity-1.4.0/setup.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-04-09 18:42:49.675168 abenity-1.4.0/tests/
+-rw-r--r--   0 brent      (501) staff       (20)     4389 2024-04-09 18:31:59.000000 abenity-1.4.0/tests/test_sso.py
```

### Comparing `abenity-1.3.0/LICENSE` & `abenity-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abenity-1.3.0/PKG-INFO` & `abenity-1.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: abenity
-Version: 1.3.0
+Version: 1.4.0
 Summary: Abenity API client
 Home-page: https://github.com/abenity/abenity-python
 Author: Abenity
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: pycryptodome==3.19.1
+Requires-Dist: pycryptodome==3.20
 Requires-Dist: six==1.16.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 
 A Python library for using the Abenity API.
```

### Comparing `abenity-1.3.0/abenity/__init__.py` & `abenity-1.4.0/abenity/__init__.py`

 * *Files identical despite different names*

### Comparing `abenity-1.3.0/abenity/client.py` & `abenity-1.4.0/abenity/client.py`

 * *Files identical despite different names*

### Comparing `abenity-1.3.0/abenity.egg-info/PKG-INFO` & `abenity-1.4.0/abenity.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: abenity
-Version: 1.3.0
+Version: 1.4.0
 Summary: Abenity API client
 Home-page: https://github.com/abenity/abenity-python
 Author: Abenity
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
-Requires-Dist: pycryptodome==3.19.1
+Requires-Dist: pycryptodome==3.20
 Requires-Dist: six==1.16.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 
 A Python library for using the Abenity API.
```

### Comparing `abenity-1.3.0/setup.py` & `abenity-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 setup(
     name='abenity',
     packages=['abenity'],
-    version='1.3.0',
+    version='1.4.0',
 
     description='Abenity API client',
     long_description='A Python library for using the Abenity API.',
     url='https://github.com/abenity/abenity-python',
     author='Abenity',
     license='MIT',
     cmdclass={'test': PyTest},
@@ -37,13 +37,13 @@
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.10',
     ],
     setup_requires=['setuptools>=17.1'],
     install_requires=[
         'requests>=2.31.0',
-        'pycryptodome==3.19.1',
+        'pycryptodome==3.20',
         'six==1.16.0'
     ],
     extras_require={'testing': ['pytest']},
     tests_require=['pytest'],
 )
```

### Comparing `abenity-1.3.0/tests/test_sso.py` & `abenity-1.4.0/tests/test_sso.py`

 * *Files identical despite different names*

