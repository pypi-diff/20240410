# Comparing `tmp/easyaddition_quicklyfix-0.0.5.tar.gz` & `tmp/easyaddition_quicklyfix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyaddition_quicklyfix-0.0.5.tar", last modified: Wed Apr 10 11:10:34 2024, max compression
+gzip compressed data, was "easyaddition_quicklyfix-0.0.6.tar", last modified: Wed Apr 10 11:17:07 2024, max compression
```

## Comparing `easyaddition_quicklyfix-0.0.5.tar` & `easyaddition_quicklyfix-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.055285 easyaddition_quicklyfix-0.0.5/
--rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:10:34.054565 easyaddition_quicklyfix-0.0.5/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.5/README.md
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.049054 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/
--rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/__init__.py
--rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix/module.py
-drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:10:34.053858 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/
--rw-r--r--   0 agatsa     (501) staff       (20)      537 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/PKG-INFO
--rw-r--r--   0 agatsa     (501) staff       (20)      276 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/SOURCES.txt
--rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/dependency_links.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:10:33.000000 easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/top_level.txt
--rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:10:34.055509 easyaddition_quicklyfix-0.0.5/setup.cfg
--rw-r--r--   0 agatsa     (501) staff       (20)     1054 2024-04-10 11:09:58.000000 easyaddition_quicklyfix-0.0.5/setup.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:17:07.666559 easyaddition_quicklyfix-0.0.6/
+-rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:17:07.665355 easyaddition_quicklyfix-0.0.6/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)        0 2024-04-10 07:22:16.000000 easyaddition_quicklyfix-0.0.6/README.md
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:17:07.659094 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix/
+-rw-r--r--   0 agatsa     (501) staff       (20)       31 2024-04-10 10:40:21.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix/__init__.py
+-rw-r--r--   0 agatsa     (501) staff       (20)       64 2024-04-10 10:52:23.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix/module.py
+drwxr-xr-x   0 agatsa     (501) staff       (20)        0 2024-04-10 11:17:07.664536 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/
+-rw-r--r--   0 agatsa     (501) staff       (20)      580 2024-04-10 11:17:07.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/PKG-INFO
+-rw-r--r--   0 agatsa     (501) staff       (20)      322 2024-04-10 11:17:07.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/SOURCES.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)        1 2024-04-10 11:17:07.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/dependency_links.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       13 2024-04-10 11:17:07.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/requires.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       24 2024-04-10 11:17:07.000000 easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/top_level.txt
+-rw-r--r--   0 agatsa     (501) staff       (20)       38 2024-04-10 11:17:07.666782 easyaddition_quicklyfix-0.0.6/setup.cfg
+-rw-r--r--   0 agatsa     (501) staff       (20)     1048 2024-04-10 11:16:56.000000 easyaddition_quicklyfix-0.0.6/setup.py
```

### Comparing `easyaddition_quicklyfix-0.0.5/PKG-INFO` & `easyaddition_quicklyfix-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: easyaddition_quicklyfix
-Version: 0.0.5
+Version: 0.0.6
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 My first Python package with a slightly longer description
```

### Comparing `easyaddition_quicklyfix-0.0.5/easyaddition_quicklyfix.egg-info/PKG-INFO` & `easyaddition_quicklyfix-0.0.6/easyaddition_quicklyfix.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: easyaddition-quicklyfix
-Version: 0.0.5
+Version: 0.0.6
 Summary: My first Python package
 Author: Saurabh Kumar
 Author-email: saurabh.kumar@agatsa.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 My first Python package with a slightly longer description
```

### Comparing `easyaddition_quicklyfix-0.0.5/setup.py` & `easyaddition_quicklyfix-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="easyaddition_quicklyfix", 
         version=VERSION,
         author="Saurabh Kumar",
         author_email="saurabh.kumar@agatsa.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], # add any additional packages that 
-        # needs to be installed along with your package. Eg: 'caer'
+        install_requires=[
+            'numpy',
+            'pandas',
+            # Add any other dependencies here
+        ],
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
```

