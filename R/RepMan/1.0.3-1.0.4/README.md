# Comparing `tmp/RepMan-1.0.3.tar.gz` & `tmp/RepMan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepMan-1.0.3.tar", last modified: Tue Apr  9 21:13:12 2024, max compression
+gzip compressed data, was "RepMan-1.0.4.tar", last modified: Tue Apr  9 22:53:04 2024, max compression
```

## Comparing `RepMan-1.0.3.tar` & `RepMan-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 21:13:07.000000 RepMan-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 21:13:12.119420 RepMan-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-09 21:13:07.000000 RepMan-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 21:13:07.000000 RepMan-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:13:12.119420 RepMan-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.115420 RepMan-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/src/RepMan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/src/repman/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25047 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanfunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanhelps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/repman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:53:04.113798 RepMan-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 22:52:59.000000 RepMan-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 22:53:04.113798 RepMan-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-09 22:52:59.000000 RepMan-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 22:52:59.000000 RepMan-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:53:04.113798 RepMan-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:53:04.109798 RepMan-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:53:04.113798 RepMan-1.0.4/src/RepMan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:53:04.000000 RepMan-1.0.4/src/RepMan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:53:04.113798 RepMan-1.0.4/src/repman/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:59.000000 RepMan-1.0.4/src/repman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-09 22:52:59.000000 RepMan-1.0.4/src/repman/_repmanclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 22:52:59.000000 RepMan-1.0.4/src/repman/_repmanfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-09 22:52:59.000000 RepMan-1.0.4/src/repman/_repmanhelps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17173 2024-04-09 22:52:59.000000 RepMan-1.0.4/src/repman/repman.py
```

### Comparing `RepMan-1.0.3/LICENSE` & `RepMan-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.3/PKG-INFO` & `RepMan-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepMan
-Version: 1.0.3
+Version: 1.0.4
 Summary: RepMan: Repository Manager (alias: Project Manager)
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `RepMan-1.0.3/README.md` & `RepMan-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.3/pyproject.toml` & `RepMan-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepMan"
-version = "1.0.3"
+version = "1.0.4"
 description = "RepMan: Repository Manager (alias: Project Manager)"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
```

### Comparing `RepMan-1.0.3/src/RepMan.egg-info/PKG-INFO` & `RepMan-1.0.4/src/RepMan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepMan
-Version: 1.0.3
+Version: 1.0.4
 Summary: RepMan: Repository Manager (alias: Project Manager)
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `RepMan-1.0.3/src/repman/_repmanclass.py` & `RepMan-1.0.4/src/repman/_repmanclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # RepMan Class File
 #
 
 from termcolor import colored
 from os import getcwd as pwd, popen as getoutputof, system as run, chdir, listdir, environ, makedirs
 from os.path import expanduser, join, basename, exists as there, dirname, abspath
 from pathlib import Path
-from tkinter import filedialog
 from re import search, match
 import pandas as pd
 from tabulate import tabulate
 from shutil import copytree
 import subprocess
 import platform
 import requests
@@ -238,14 +237,20 @@
                 
                 # change to the path
                 try:
                     chdir(path)
                 except UnboundLocalError:
                     print(colored('RepMan', 'red'), f": no project named {projectname}.")
                     exit(1)
+                    
+                # run git pull for safety
+                print('RepMan:', colored('Pulling', 'yellow'), end='\r')
+                subprocess.Popen(['git', 'pull'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+                print('                                       ', end='\r')
+                print('RepMan:', colored('Pulled.', 'blue'))
                 # get files that are changed.
                 files = getoutputof('git diff --name-only').readlines()
                 files2 = getoutputof('git ls-files --others --exclude-standard').readlines()
                 msgs = []
                 for file in files:
                     file = file.replace('\n','')
                     commitmsg = input('RepMan -> Enter commit msg for ' + colored(f'{join(basename(path), file)}', 'blue') + ': ')
@@ -267,14 +272,15 @@
                 branch = getoutputof('git rev-parse --abbrev-ref HEAD').read().replace('\n','')
                 print('RepMan: Resolved current branch ->', colored(f'{branch}', 'blue'))
                 
                 print('RepMan:', colored('Pushing', 'yellow'), end='\r')
                 subprocess.Popen(['git', 'push', '-u', 'origin', f'{branch}'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
                 print('                                                      ', end='\r')
                 print('RepMan:', colored('Pushed', 'green'))
+                exit(0)
         except ConnectionError:
             print(colored('RepMan','red'), ': Please connect to the internet to use this feature.')
             exit(1)
 
     ############## OPEN FUNCTION INSIDE REPMAN CLASS #############################
     def open(self, projects:list[str]):
         count = 0
@@ -313,22 +319,28 @@
             path = abspath(path)
             # if already inside the project directory
             if dirname(path) == self.path:
                 # add entry in the .projects file
                 with open(join(self.dotfolder, '.projects'), 'a') as projfile:
                     projfile.write(basename(path)+':'+path+'\n')
                 print('RepMan:', colored(f'Added {basename(path)} -> {path}', 'green'))
+                newpath = path
             else:
                 ## copy
                 try:
                     newpath = copytree(path, join(self.path, basename(path)))
                 except FileNotFoundError:
                     print(colored('RepMan', 'red'), f': No such file in this directory. <- {path}')
                     exit(1)
                 print('RepMan:', colored(f'Added {basename(path)} -> {newpath}', 'green'))
+            
+            chdir(newpath)
+            # change git rule
+            subprocess.Popen(['git', 'config', 'pull.rebase', 'true'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
+            print('RepMan:', colored('Changed git pull rebase to true.', 'blue'))
     
     ############## ADD FUNCTION INSIDE REPMAN CLASS #############################
     def add(self, url:str):
         # set project path
         self.path = environ['REPMAN_PROJECT_PATH']
         chdir(self.path)
         # check format -> must be github link or <username>/<repo>
@@ -430,15 +442,19 @@
                 print('RepMan:', colored(f"git found -> v{getoutputof('git -v').readline().replace('\n','').split(' ')[2]}", 'green'))
             ## GIT INSTALL END ##
             
             ## Project Folder check ##
             if self.path == '':
                 print(colored(' Choose a Project folder...', 'blue'), end='\r')
                 # -> get filepath
-                self.path = filedialog.askdirectory(initialdir=self.workingpath, title='select project path')
+                try:
+                    from tkinter import filedialog
+                    self.path = filedialog.askdirectory(initialdir=self.workingpath, title='select project path')
+                except ModuleNotFoundError:
+                    self.path = input('Enter Project path: ')
             else:
                 pass
                 
             # -> resolve where to save the project path
             if platform.system()=='Linux' or platform.system()=='Darwin':
                 # -> go to home dir
                 chdir(expanduser('~'))
```

### Comparing `RepMan-1.0.3/src/repman/_repmanfunctions.py` & `RepMan-1.0.4/src/repman/_repmanfunctions.py`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.3/src/repman/_repmanhelps.py` & `RepMan-1.0.4/src/repman/_repmanhelps.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         print('  |  Author: Soumyo Deep Gupta (@d33pster)  |')
         print('  |  Email: deep.main.ac@gmail.com          |')
         print('  |  copyright @d33pster                    |')
         print('\nEND')
         exit(0)
     
     # function to display version and exit
-    def version(self):
+    def version_s(self):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print('         version', colored(f'v{self.version}', 'red'))
         print('         author:', colored('d33pster', 'light_blue'))
         print('         GitHub:', colored('https://github.com/d33pster', 'light_blue'))
         exit(0)
     
     # function to print general help
```

### Comparing `RepMan-1.0.3/src/repman/repman.py` & `RepMan-1.0.4/src/repman/repman.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python3
 
 ## OS Support
 # Linux -> aarch64
 # MacOs -> AppleSilicon(arm64)
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 from repman._repmanfunctions import funcdefs
 from repman._repmanhelps import helptext
 from termcolor import colored
 from optioner import options
 from sys import argv
 from re import match
 
-
 # list value removing function
 def rem(original:list[str], remove:list[str]) -> list[str]:
     removed:list[str] = []
     for x in original:
         if x not in remove:
             removed.append(x)
     
     return removed
 
 # main function
 def main():
     try:
         # helptext
-        help = helptext(__version__)
+        helptex = helptext(__version__)
         # functions
         funk = funcdefs(__version__)
         # create arguments
         shortargs = ['h', 'v', 'a', 'i', 'o', 'l', 'lp', 'ae', 'al', 'u', 'sr', 'cred']
         longargs = ['help', 'version', 'add', 'init', 'open', 'list', 'list-w-path', 'add-existing', 'add-local', 'update', 'set-remote', 'credits']
         
         # All args
@@ -78,41 +77,41 @@
                         index = args.index('-h')
                         if index==0:
                             otherarg = args[1]
                         else:
                             otherarg = args[0]
                         
                         if otherarg=='-h' or otherarg=='--help':
-                            help.base()
+                            helptex.base()
                         elif otherarg=='-v' or otherarg=='--version':
-                            help.version_h(otherarg)
+                            helptex.version_h(otherarg)
                         elif otherarg=='-i' or otherarg=='--init':
-                            help.init_h(otherarg)
+                            helptex.init_h(otherarg)
                         elif otherarg=='-a' or otherarg=='--add':
-                            help.add_h(otherarg)
+                            helptex.add_h(otherarg)
                         elif otherarg=='-o' or otherarg=='--open':
-                            help.open_h(otherarg)
+                            helptex.open_h(otherarg)
                         elif otherarg == '-l' or otherarg == '--list':
-                            help.list_h(otherarg)
+                            helptex.list_h(otherarg)
                         elif otherarg == '-lp' or otherarg == '--list-w-path':
-                            help.listwpath_h(otherarg)
+                            helptex.listwpath_h(otherarg)
                         elif otherarg == '-ae' or otherarg == '--add-existing':
-                            help.addexisting_h(otherarg)
+                            helptex.addexisting_h(otherarg)
                         elif otherarg == '-al' or otherarg == '--add-local':
-                            help.addlocal_h(otherarg)
+                            helptex.addlocal_h(otherarg)
                         elif otherarg == '-u' or otherarg == '--update':
-                            help.update_h(otherarg)
+                            helptex.update_h(otherarg)
                         elif otherarg == '-sr' or otherarg == '--set-remote':
-                            help.setremote_h(otherarg)
+                            helptex.setremote_h(otherarg)
                         elif otherarg == '-cred' or otherarg == '--credits':
-                            help.credits()
+                            helptex.credits()
                         else:
                             print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
                     elif len(args)<2:
-                        help.base()
+                        helptex.base()
                     elif len(args)>2:
                         print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
                         print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
                         exit(1)
                     else:
                         print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
                         print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
@@ -126,59 +125,57 @@
                         index = args.index('--help')
                         if index==0:
                             otherarg = args[1]
                         else:
                             otherarg = args[0]
                         
                         if otherarg=='-h' or otherarg=='--help':
-                            help.base()
+                            helptex.base()
                         elif otherarg=='-v' or otherarg=='--version':
-                            help.version_h(otherarg)
+                            helptex.version_h(otherarg)
                         elif otherarg=='-i' or otherarg=='--init':
-                            help.init_h(otherarg)
+                            helptex.init_h(otherarg)
                         elif otherarg=='-a' or otherarg=='--add':
-                            help.add_h(otherarg)
+                            helptex.add_h(otherarg)
                         elif otherarg=='-o' or otherarg=='--open':
-                            help.open_h(otherarg)
+                            helptex.open_h(otherarg)
                         elif otherarg == '-l' or otherarg == '--list':
-                            help.list_h(otherarg)
+                            helptex.list_h(otherarg)
                         elif otherarg == '-lp' or otherarg == '--list-w-path':
-                            help.listwpath_h(otherarg)
+                            helptex.listwpath_h(otherarg)
                         elif otherarg == '-ae' or otherarg == '--add-existing':
-                            help.addexisting_h(otherarg)
+                            helptex.addexisting_h(otherarg)
                         elif otherarg == '-al' or otherarg == '--add-local':
-                            help.addlocal_h(otherarg)
+                            helptex.addlocal_h(otherarg)
                         elif otherarg == '-u' or otherarg == '--update':
-                            help.update_h(otherarg)
+                            helptex.update_h(otherarg)
                         elif otherarg == '-sr' or otherarg == '--set-remote':
-                            help.setremote_h(otherarg)
+                            helptex.setremote_h(otherarg)
                         elif otherarg == '-cred' or otherarg == '--credits':
-                            help.credits()
+                            helptex.credits()
                         else:
                             print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
                     elif len(args)<2:
-                        help.base()
+                        helptex.base()
                     elif len(args)>2:
                         print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
                         print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
                         exit(1)
                     else:
                         print(colored('RepMan Err', 'red'), ': Could not resolve arguments.')
                         print(colored('RepMan Hint', 'blue'), ': Run \'repman -h\' or \'repman --help\'.')
                         exit(1)
-                else:
-                    pass
                 
                 # version
                 if '-v' in args or '--version' in args:
-                    help.version()
+                    helptex.version_s()
                 
                 # credits
                 if '-cred' in args or '--credits' in args:
-                    help.credits()
+                    helptex.credits()
                 
                 # init
                 if '-i' in args:
                     index = argv.index('-i')
                     try:
                         value = argv[index+1]
                     except IndexError:
@@ -312,25 +309,27 @@
                     value:list[str] = []
                     try:
                         for i in range(index+1, len(argv)):
                             value.append(argv[i])
                     except IndexError:
                         print(colored('RepMan', 'red'), ': \'-al\' needs atleast one value.')
                         exit(1)
+                    
+                    funk.addlocal(value)
                 elif '--add-local' in args:
                     index = argv.index('--add-local')
                     value:list[str] = []
                     try:
                         for i in range(index+1, len(argv)):
                             value.append(argv[i])
                     except IndexError:
                         print(colored('RepMan', 'red'), ': \'--add-local\' needs atleast one value.')
                         exit(1)
                     
-                funk.addlocal(value)
+                    funk.addlocal(value)
                 
                 # set remote
                 if '-sr' in args:
                     index = argv.index('-sr')
                     value:list[str] = []
                     try:
                         for i in range(index+1, len(argv)):
@@ -347,14 +346,36 @@
                                 remote = v
                             else:
                                 project = v
                         funk.setremote(project, remote)
                     else:
                         print(colored('RepMan', 'red')+': \'-sr\' accepts only two values')
                         exit(1)
+                elif '--set-remote' in args:
+                    index = argv.index('--set-remote')
+                    value:list[str] = []
+                    try:
+                        for i in range(index+1, len(argv)):
+                            value.append(argv[i])
+                    except IndexError:
+                        print(colored('RepMan', 'red')+': \'--set-remote\' needs two values. <project> and <remote>')
+                        exit(1)
+                    
+                    project:str = ''
+                    remote:str = ''
+                    if len(value)==2:
+                        for v in value:
+                            if match(r'^https://github.com/\w+/\w+', v) or match(r'^\w+/\w+', v):
+                                remote = v
+                            else:
+                                project = v
+                        funk.setremote(project, remote)
+                    else:
+                        print(colored('RepMan', 'red')+': \'--set-remote\' accepts only two values')
+                        exit(1)
                     
     except KeyboardInterrupt:
         print('\n'+colored('RepMan', 'red')+": Decide Karen!")
                 
 
 if __name__=='__main__':
     try:
```

