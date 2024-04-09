# Comparing `tmp/gimmetool-0.1.0.tar.gz` & `tmp/gimmetool-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimmetool-0.1.0.tar", max compression
+gzip compressed data, was "gimmetool-0.1.5.tar", max compression
```

## Comparing `gimmetool-0.1.0.tar` & `gimmetool-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.0/README.md
--rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.0/gimmetool/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.0/gimmetool/gimme.py
--rwxr-xr-x   0        0        0      616 2024-04-09 22:20:00.800445 gimmetool-0.1.0/gimmetool/gimme.sh
--rwxr-xr-x   0        0        0    24517 2024-04-09 22:24:59.532281 gimmetool-0.1.0/gimmetool/gimmetool.py
--rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.0/gimmetool/setup.py
--rwxr-xr-x   0        0        0      405 2024-04-09 21:06:42.963792 gimmetool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 gimmetool-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2523 2024-04-09 15:47:36.673732 gimmetool-0.1.5/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-09 15:47:36.669084 gimmetool-0.1.5/gimmetool/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:26:41.452357 gimmetool-0.1.5/gimmetool/gimme.py
+-rwxr-xr-x   0        0        0      616 2024-04-09 22:33:40.953646 gimmetool-0.1.5/gimmetool/gimme.sh
+-rwxr-xr-x   0        0        0    24806 2024-04-09 22:38:16.183338 gimmetool-0.1.5/gimmetool/gimmetool.py
+-rw-r--r--   0        0        0      903 2024-04-09 20:32:22.399803 gimmetool-0.1.5/gimmetool/setup.py
+-rwxr-xr-x   0        0        0      405 2024-04-09 22:37:34.604834 gimmetool-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 gimmetool-0.1.5/PKG-INFO
```

### Comparing `gimmetool-0.1.0/README.md` & `gimmetool-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.0/gimmetool/gimme.sh` & `gimmetool-0.1.5/gimmetool/gimme.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 function gimme {
   if ! command -v gimmetool &> /dev/null
   then
-    exit 1
+    return
   fi
 
   arg=$1
   case $arg in
     ("")
       gimmetool -h
       ;;
```

### Comparing `gimmetool-0.1.0/gimmetool/gimmetool.py` & `gimmetool-0.1.5/gimmetool/gimmetool.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 import sys
 import shutil
 from os import path
 import stat
 from termcolor import colored
 
 
+import pkg_resources
+
 def colored(*args):
     return args[0]
 
-
-VERSION = '0.1.4'
 CONFIG_FILE_NAME = '.gimmeconfig.json'
 
 gcmd = git.Git(path.expanduser("~/git/GitPython"))
 
 SCRIPT = """
 function gimme {
   if ! command -v gimmetool &> /dev/null
   then
-    exit 1
+    return
   fi
 
   arg=$1
   case $arg in
     ("")
       gimmetool -h
       ;;
@@ -81,15 +81,15 @@
 
     if not path.exists(path.join(Utils.get_install_dir(), 'gimmetool')) and args.command is None:
         print('gimme needs initialization:')
         print(colored('~$ sudo gimme init', 'yellow'))
         return
 
     if args.version:
-        print(VERSION)
+        print(pkg_resources.get_distribution('my-package-name').version)
         return
 
     args.func(args)
 
 def add_init_parser(subparsers: argparse._SubParsersAction):
     init_parser = subparsers.add_parser('init', help='Perform first time initialization')
 
@@ -104,14 +104,21 @@
             return
 
         install_dir = Utils.get_install_dir()
         gimmetoolpath = path.join(install_dir, 'gimmetool')
         gimmepath = path.join(install_dir, 'gimme')
 
         try:
+            repos_path = input('where do all of your repositories live [~/]?')
+            if repos_path == '':
+                repos_path = '~/'
+
+            config = Config()
+            config.add_group(path.expanduser(repos_path))
+
             config_path = input('shell config file [~/.zshrc]: ')
             if config_path == '':
                 config_path = '~/.zshrc'
 
             if not path.exists(path.expanduser(config_path)):
                 confirm_force = input(f'Could not find {config_path}. Proceed anyway? [n]: ')
                 if confirm_force.lower() != 'y' or confirm_force.lower() != 'yes':
```

### Comparing `gimmetool-0.1.0/gimmetool/setup.py` & `gimmetool-0.1.5/gimmetool/setup.py`

 * *Files identical despite different names*

### Comparing `gimmetool-0.1.0/PKG-INFO` & `gimmetool-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimmetool
-Version: 0.1.0
+Version: 0.1.5
 Summary: The multi-repo manager
 Author: Jeff
 Author-email: jhilton@qualtrics.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

