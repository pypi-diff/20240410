# Comparing `tmp/composio_autogen-0.1.84.tar.gz` & `tmp/composio_autogen-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.84.tar", last modified: Sun Apr  7 19:53:11 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.85.tar", last modified: Wed Apr 10 14:03:17 2024, max compression
```

## Comparing `composio_autogen-0.1.84.tar` & `composio_autogen-0.1.85.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.096268 composio_autogen-0.1.84/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 19:53:11.096084 composio_autogen-0.1.84/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.84/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.094335 composio_autogen-0.1.84/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.84/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7468 2024-04-07 18:28:35.000000 composio_autogen-0.1.84/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:53:11.095856 composio_autogen-0.1.84/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 19:53:11.000000 composio_autogen-0.1.84/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 19:52:16.000000 composio_autogen-0.1.84/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 19:53:11.096319 composio_autogen-0.1.84/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 19:52:16.000000 composio_autogen-0.1.84/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-10 14:03:17.937694 composio_autogen-0.1.85/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-10 14:03:17.937505 composio_autogen-0.1.85/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.85/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-10 14:03:17.936590 composio_autogen-0.1.85/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.85/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7468 2024-04-07 18:18:17.000000 composio_autogen-0.1.85/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-10 14:03:17.937348 composio_autogen-0.1.85/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-10 14:03:17.000000 composio_autogen-0.1.85/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-10 14:03:17.000000 composio_autogen-0.1.85/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-10 14:03:17.000000 composio_autogen-0.1.85/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-10 14:03:17.000000 composio_autogen-0.1.85/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-10 14:03:17.000000 composio_autogen-0.1.85/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-10 14:02:55.000000 composio_autogen-0.1.85/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-10 14:03:17.937731 composio_autogen-0.1.85/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-10 14:02:55.000000 composio_autogen-0.1.85/setup.py
```

### Comparing `composio_autogen-0.1.84/PKG-INFO` & `composio_autogen-0.1.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.84
+Version: 0.1.85
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.85
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.84/README.md` & `composio_autogen-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.84/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.85/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.84/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.85/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.84
+Version: 0.1.85
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.85
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.84/setup.py` & `composio_autogen-0.1.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.84",
+    version="0.1.85",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

