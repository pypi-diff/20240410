# Comparing `tmp/PathMePy-Gustoon-0.3.1.tar.gz` & `tmp/PathMePy-Gustoon-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathMePy-Gustoon-0.3.1.tar", last modified: Sun Apr  7 09:25:07 2024, max compression
+gzip compressed data, was "PathMePy-Gustoon-0.4.tar", last modified: Wed Apr 10 15:28:48 2024, max compression
```

## Comparing `PathMePy-Gustoon-0.3.1.tar` & `PathMePy-Gustoon-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 09:25:07.613675 PathMePy-Gustoon-0.3.1/
--rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1234 2024-04-07 09:25:07.605677 PathMePy-Gustoon-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 09:25:07.567698 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon/
--rw-rw-rw-   0        0        0     1501 2024-04-07 08:50:03.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon/PathMePy.py
--rw-rw-rw-   0        0        0      148 2024-04-07 08:43:57.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:25:07.602678 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/
--rw-rw-rw-   0        0        0     1234 2024-04-07 09:25:07.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-07 09:25:07.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 09:25:07.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-07 09:25:07.000000 PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      853 2024-04-07 09:14:26.000000 PathMePy-Gustoon-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 09:25:07.614685 PathMePy-Gustoon-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1304 2024-04-07 09:18:30.000000 PathMePy-Gustoon-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:28:48.227448 PathMePy-Gustoon-0.4/
+-rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1372 2024-04-10 15:28:48.224450 PathMePy-Gustoon-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 15:28:48.173478 PathMePy-Gustoon-0.4/PathMePy_Gustoon/
+-rw-rw-rw-   0        0        0     1658 2024-04-10 15:24:23.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon/PathMePy.py
+-rw-rw-rw-   0        0        0      181 2024-04-10 15:24:15.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 15:28:48.221451 PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/
+-rw-rw-rw-   0        0        0     1372 2024-04-10 15:28:47.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-10 15:28:48.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 15:28:47.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-10 15:28:47.000000 PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      993 2024-04-10 15:27:39.000000 PathMePy-Gustoon-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 15:28:48.227448 PathMePy-Gustoon-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2024-04-10 15:28:02.000000 PathMePy-Gustoon-0.4/setup.py
```

### Comparing `PathMePy-Gustoon-0.3.1/LICENSE.txt` & `PathMePy-Gustoon-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PathMePy-Gustoon-0.3.1/PKG-INFO` & `PathMePy-Gustoon-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.3.1
+Version: 0.4
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.2
@@ -20,15 +20,17 @@
 
 ## Content
 You need to import this package with `import PathMePy_Gustoon`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
+`UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
 
 ## Explanation
 `PathMePyDir(path)` function is for temporaly add a directory in your user PATH variable,
 `PathMePyUserScriptFolder()` function is for add the Python User Script Folder to the user PATH variable,
 `IsAlreadyOnPath(path)` function return if an element is on the PATH or not,
+`UserScriptFolderIsAlreadyOnPath()` function return if the User Script folder is on the PATH or not,
 `Current_Path` is a variable with the current path,
 `Current_Path_Formated` is a formatted version of `Current_Path` that changes each PATH separator with a newline.
```

### Comparing `PathMePy-Gustoon-0.3.1/PathMePy_Gustoon/PathMePy.py` & `PathMePy-Gustoon-0.4/PathMePy_Gustoon/PathMePy.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 def IsAlreadyOnPath(path):
     if path in Current_Path_Formated:
         return True
     else:
         return False
 
+def UserScriptFolderIsAlreadyOnPath():
+    if site.getusersitepackages() in Current_Path_Formated:
+        return True
+    else:
+        return False
+
 def PathMePyDir(path):
     path = os.path.abspath(path)
     if not os.path.exists(path):
         raise PathNotFoundError("The path " + path + " doesn't exist.")
     elif platform.system() != "Windows" and platform.system() != "Linux" :
         os.system('export PATH=$PATH:' + path)
     elif platform.system() == "Windows" :
```

### Comparing `PathMePy-Gustoon-0.3.1/PathMePy_Gustoon.egg-info/PKG-INFO` & `PathMePy-Gustoon-0.4/PathMePy_Gustoon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.3.1
+Version: 0.4
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.2
@@ -20,15 +20,17 @@
 
 ## Content
 You need to import this package with `import PathMePy_Gustoon`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
+`UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
 
 ## Explanation
 `PathMePyDir(path)` function is for temporaly add a directory in your user PATH variable,
 `PathMePyUserScriptFolder()` function is for add the Python User Script Folder to the user PATH variable,
 `IsAlreadyOnPath(path)` function return if an element is on the PATH or not,
+`UserScriptFolderIsAlreadyOnPath()` function return if the User Script folder is on the PATH or not,
 `Current_Path` is a variable with the current path,
 `Current_Path_Formated` is a formatted version of `Current_Path` that changes each PATH separator with a newline.
```

### Comparing `PathMePy-Gustoon-0.3.1/README.md` & `PathMePy-Gustoon-0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 ## Content
 You need to import this package with `import PathMePy_Gustoon`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
+`UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
 
 ## Explanation
 `PathMePyDir(path)` function is for temporaly add a directory in your user PATH variable,
 `PathMePyUserScriptFolder()` function is for add the Python User Script Folder to the user PATH variable,
 `IsAlreadyOnPath(path)` function return if an element is on the PATH or not,
+`UserScriptFolderIsAlreadyOnPath()` function return if the User Script folder is on the PATH or not,
 `Current_Path` is a variable with the current path,
 `Current_Path_Formated` is a formatted version of `Current_Path` that changes each PATH separator with a newline.
```

### Comparing `PathMePy-Gustoon-0.3.1/setup.py` & `PathMePy-Gustoon-0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 name='PathMePy-Gustoon',
-version='0.3.1',
+version='0.4',
 author='Gustoon',
 author_email='',
 description='A tool to add scripts to Path',
 long_description="""
 # PathMePy
 A tool to add scripts to Path
 
@@ -15,22 +15,25 @@
 
 ## Content
 You need to import this package with `import PathMePy_Gustoon`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
+`UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
 
 ## Explanation
 `PathMePyDir(path)` function is for temporaly add a directory in your user PATH variable,
 `PathMePyUserScriptFolder()` function is for add the Python User Script Folder to the user PATH variable,
 `IsAlreadyOnPath(path)` function return if an element is on the PATH or not,
+`UserScriptFolderIsAlreadyOnPath()` function return if the User Script folder is on the PATH or not,
 `Current_Path` is a variable with the current path,
-`Current_Path_Formated` is a formatted version of `Current_Path` that changes each PATH separator with a newline.""",
+`Current_Path_Formated` is a formatted version of `Current_Path` that changes each PATH separator with a newline.
+""",
 long_description_content_type='text/markdown',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: OS Independent',
 ],
```

