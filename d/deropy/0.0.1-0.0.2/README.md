# Comparing `tmp/deropy-0.0.1.tar.gz` & `tmp/deropy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.0.1.tar", last modified: Wed Apr 10 13:49:32 2024, max compression
+gzip compressed data, was "deropy-0.0.2.tar", last modified: Wed Apr 10 14:47:19 2024, max compression
```

## Comparing `deropy-0.0.1.tar` & `deropy-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxr-x   0 lcances   (1000) lcances   (1000)        0 2024-04-10 13:49:32.769355 deropy-0.0.1/
--rw-r--r--   0 lcances   (1000) lcances   (1000)      487 2024-04-10 13:49:32.769355 deropy-0.0.1/PKG-INFO
-drwxrwxr-x   0 lcances   (1000) lcances   (1000)        0 2024-04-10 13:49:32.765355 deropy-0.0.1/deropy/
--rw-rw-r--   0 lcances   (1000) lcances   (1000)        0 2024-04-05 18:54:12.000000 deropy-0.0.1/deropy/__init__.py
-drwxrwxr-x   0 lcances   (1000) lcances   (1000)        0 2024-04-10 13:49:32.765355 deropy-0.0.1/deropy/commands/
--rw-rw-r--   0 lcances   (1000) lcances   (1000)        0 2024-04-07 12:19:49.000000 deropy-0.0.1/deropy/commands/__init__.py
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      666 2024-04-09 09:12:56.000000 deropy-0.0.1/deropy/commands/deploy.py
--rw-rw-r--   0 lcances   (1000) lcances   (1000)     9473 2024-04-09 19:22:52.000000 deropy-0.0.1/deropy/commands/generate.py
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      433 2024-04-10 13:23:08.000000 deropy-0.0.1/deropy/commands/init.py
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      386 2024-04-10 13:36:59.000000 deropy-0.0.1/deropy/main.py
--rw-rw-r--   0 lcances   (1000) lcances   (1000)     3241 2024-04-10 13:30:34.000000 deropy-0.0.1/deropy/test.py
-drwxrwxr-x   0 lcances   (1000) lcances   (1000)        0 2024-04-10 13:49:32.765355 deropy-0.0.1/deropy.egg-info/
--rw-r--r--   0 lcances   (1000) lcances   (1000)      487 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/PKG-INFO
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      362 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/SOURCES.txt
--rw-rw-r--   0 lcances   (1000) lcances   (1000)        1 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/dependency_links.txt
--rw-rw-r--   0 lcances   (1000) lcances   (1000)       46 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/entry_points.txt
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      107 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/requires.txt
--rw-rw-r--   0 lcances   (1000) lcances   (1000)        7 2024-04-10 13:49:32.000000 deropy-0.0.1/deropy.egg-info/top_level.txt
--rw-rw-r--   0 lcances   (1000) lcances   (1000)       38 2024-04-10 13:49:32.769355 deropy-0.0.1/setup.cfg
--rw-rw-r--   0 lcances   (1000) lcances   (1000)      803 2024-04-10 13:49:13.000000 deropy-0.0.1/setup.py
-drwxrwxr-x   0 lcances   (1000) lcances   (1000)        0 2024-04-10 13:49:32.769355 deropy-0.0.1/tests/
--rw-rw-r--   0 lcances   (1000) lcances   (1000)     1245 2024-04-09 19:48:37.000000 deropy-0.0.1/tests/test_SC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 14:47:19.126374 deropy-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-10 14:47:12.000000 deropy-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.122374 deropy-0.0.2/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:47:19.126374 deropy-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-10 14:47:12.000000 deropy-0.0.2/setup.py
```

### Comparing `deropy-0.0.1/deropy/commands/deploy.py` & `deropy-0.0.2/deropy/commands/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import click
 import json
 
-from commands.generate import _generate_class, _generate_tests
+from deropy.commands.generate import _generate_class, _generate_tests
 
 @click.command('deploy')
 @click.argument('file', type=click.Path())
 @click.option('-g', '--generate', is_flag=True, help='Generate the SC file')
 def deploy(file, generate):
     sc_txid = _deploy(file)
     click.echo(f'Transaction ID: {sc_txid}')
```

### Comparing `deropy-0.0.1/deropy/commands/generate.py` & `deropy-0.0.2/deropy/commands/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,18 @@
         
         return output
 
     functions = {}
     for line in lines:
         if "Function " in line and not "End Function" in line:
             function_name = get_function_name(line)
+
+            if not function_name[0].isupper():
+                continue
+
             parameters = get_function_parameters(line)
             functions[function_name] = parameters
 
     return functions
 
 def _generate_read_method(scid):
         return [
```

### Comparing `deropy-0.0.1/setup.py` & `deropy-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.0.1',
-    url='https://github.com/lcances/pydero',
+    version=os.getenv('DEROPY_VERSION') or '0.0.2',
+    url='https://github.com/lcances/deropy',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'click==8.0.4',
         'requests==2.27.1',
         'coloredlogs==15.0.1',
         'pyperclip==1.8.2',
         'python-dotenv==0.20.0',
```

