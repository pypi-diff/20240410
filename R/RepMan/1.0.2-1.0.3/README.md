# Comparing `tmp/RepMan-1.0.2.tar.gz` & `tmp/RepMan-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepMan-1.0.2.tar", last modified: Tue Apr  9 18:17:00 2024, max compression
+gzip compressed data, was "RepMan-1.0.3.tar", last modified: Tue Apr  9 21:13:12 2024, max compression
```

## Comparing `RepMan-1.0.2.tar` & `RepMan-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.318386 RepMan-1.0.2/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-06 11:46:27.000000 RepMan-1.0.2/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     5327 2024-04-09 18:17:00.317995 RepMan-1.0.2/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3129 2024-04-09 18:10:40.000000 RepMan-1.0.2/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1110 2024-04-09 15:55:56.000000 RepMan-1.0.2/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-09 18:17:00.318446 RepMan-1.0.2/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.309274 RepMan-1.0.2/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.317448 RepMan-1.0.2/src/RepMan.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     5327 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      367 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       46 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       60 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        7 2024-04-09 18:17:00.000000 RepMan-1.0.2/src/RepMan.egg-info/top_level.txt
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-09 18:17:00.316793 RepMan-1.0.2/src/repman/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-06 11:46:27.000000 RepMan-1.0.2/src/repman/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)    25047 2024-04-09 17:21:56.000000 RepMan-1.0.2/src/repman/_repmanclass.py
--rw-r--r--   0 d33pster   (501) staff       (20)     1417 2024-04-09 17:24:32.000000 RepMan-1.0.2/src/repman/_repmanfunctions.py
--rw-r--r--   0 d33pster   (501) staff       (20)    11066 2024-04-09 17:29:32.000000 RepMan-1.0.2/src/repman/_repmanhelps.py
--rw-r--r--   0 d33pster   (501) staff       (20)    15517 2024-04-09 17:24:50.000000 RepMan-1.0.2/src/repman/repman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 21:13:07.000000 RepMan-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 21:13:12.119420 RepMan-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-09 21:13:07.000000 RepMan-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 21:13:07.000000 RepMan-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:13:12.119420 RepMan-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.115420 RepMan-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/src/RepMan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 21:13:12.000000 RepMan-1.0.3/src/RepMan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:12.119420 RepMan-1.0.3/src/repman/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25047 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/_repmanhelps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-04-09 21:13:07.000000 RepMan-1.0.3/src/repman/repman.py
```

### Comparing `RepMan-1.0.2/LICENSE` & `RepMan-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.2/PKG-INFO` & `RepMan-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepMan
-Version: 1.0.2
+Version: 1.0.3
 Summary: RepMan: Repository Manager (alias: Project Manager)
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -42,14 +42,20 @@
 Requires-Dist: termcolor
 Requires-Dist: gdown
 Requires-Dist: tk
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: requests
 
+![PyPI - Version](https://img.shields.io/pypi/v/RepMan?color=bright%20green)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/RepMan)
+![GitHub License](https://img.shields.io/github/license/d33pster/RepMan)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2FRepMan%2Fmain%2Fpyproject.toml)
+[![Build status](https://ci.appveyor.com/api/projects/status/bbptf69j4n86fthj?svg=true)](https://ci.appveyor.com/project/d33pster/repman)
+
 # Overview
 
 RepMan or Repository Manager is written on python to serve as GitHub Repo Manager for the end users.
 
 Have a lot of repositories you've been working on? Is it a hassle? RepMan is your solution.
 
 ## What RepMan offers
@@ -157,14 +163,18 @@
 repman <option> -h
 
 # or 
 
 repman <option> --help
 ```
 
+## Usage screenshots
+
+<img src='images/update.png'>
+
 ## Supported OS and architectures and notes
 - MacOS (Apple Silicon Chip - M series) (Arch - arm64) (Requires Homebrew)
 - Linux (Debian) (Arch - aarch64)
 - **If your OS and arch is not listed here, just make sure to install VSCode and git on your own, rest is same.**
 
 ## Uninstall
```

### Comparing `RepMan-1.0.2/README.md` & `RepMan-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+![PyPI - Version](https://img.shields.io/pypi/v/RepMan?color=bright%20green)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/RepMan)
+![GitHub License](https://img.shields.io/github/license/d33pster/RepMan)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2FRepMan%2Fmain%2Fpyproject.toml)
+[![Build status](https://ci.appveyor.com/api/projects/status/bbptf69j4n86fthj?svg=true)](https://ci.appveyor.com/project/d33pster/repman)
+
 # Overview
 
 RepMan or Repository Manager is written on python to serve as GitHub Repo Manager for the end users.
 
 Have a lot of repositories you've been working on? Is it a hassle? RepMan is your solution.
 
 ## What RepMan offers
@@ -109,14 +115,18 @@
 repman <option> -h
 
 # or 
 
 repman <option> --help
 ```
 
+## Usage screenshots
+
+<img src='images/update.png'>
+
 ## Supported OS and architectures and notes
 - MacOS (Apple Silicon Chip - M series) (Arch - arm64) (Requires Homebrew)
 - Linux (Debian) (Arch - aarch64)
 - **If your OS and arch is not listed here, just make sure to install VSCode and git on your own, rest is same.**
 
 ## Uninstall
```

### Comparing `RepMan-1.0.2/pyproject.toml` & `RepMan-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepMan"
-version = "1.0.2"
+version = "1.0.3"
 description = "RepMan: Repository Manager (alias: Project Manager)"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "License :: OSI Approved :: MIT License",
```

### Comparing `RepMan-1.0.2/src/RepMan.egg-info/PKG-INFO` & `RepMan-1.0.3/src/RepMan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepMan
-Version: 1.0.2
+Version: 1.0.3
 Summary: RepMan: Repository Manager (alias: Project Manager)
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -42,14 +42,20 @@
 Requires-Dist: termcolor
 Requires-Dist: gdown
 Requires-Dist: tk
 Requires-Dist: pandas
 Requires-Dist: tabulate
 Requires-Dist: requests
 
+![PyPI - Version](https://img.shields.io/pypi/v/RepMan?color=bright%20green)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/RepMan)
+![GitHub License](https://img.shields.io/github/license/d33pster/RepMan)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2FRepMan%2Fmain%2Fpyproject.toml)
+[![Build status](https://ci.appveyor.com/api/projects/status/bbptf69j4n86fthj?svg=true)](https://ci.appveyor.com/project/d33pster/repman)
+
 # Overview
 
 RepMan or Repository Manager is written on python to serve as GitHub Repo Manager for the end users.
 
 Have a lot of repositories you've been working on? Is it a hassle? RepMan is your solution.
 
 ## What RepMan offers
@@ -157,14 +163,18 @@
 repman <option> -h
 
 # or 
 
 repman <option> --help
 ```
 
+## Usage screenshots
+
+<img src='images/update.png'>
+
 ## Supported OS and architectures and notes
 - MacOS (Apple Silicon Chip - M series) (Arch - arm64) (Requires Homebrew)
 - Linux (Debian) (Arch - aarch64)
 - **If your OS and arch is not listed here, just make sure to install VSCode and git on your own, rest is same.**
 
 ## Uninstall
```

### Comparing `RepMan-1.0.2/src/repman/_repmanclass.py` & `RepMan-1.0.3/src/repman/_repmanclass.py`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.2/src/repman/_repmanfunctions.py` & `RepMan-1.0.3/src/repman/_repmanfunctions.py`

 * *Files identical despite different names*

### Comparing `RepMan-1.0.2/src/repman/_repmanhelps.py` & `RepMan-1.0.3/src/repman/_repmanhelps.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 
 from termcolor import colored
 
 class helptext:
     def __init__(self, version:str):
         self.version = version
     
+    # function to show credits
+    def credits(self):
+        print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
+        print(colored('credits\n', 'red'))
+        print('  |  Author: Soumyo Deep Gupta (@d33pster)  |')
+        print('  |  Email: deep.main.ac@gmail.com          |')
+        print('  |  copyright @d33pster                    |')
+        print('\nEND')
+        exit(0)
+    
     # function to display version and exit
     def version(self):
         print(colored('RepMan', 'blue'), ': Repository Manager (alias: Project Manager)')
         print('         version', colored(f'v{self.version}', 'red'))
         print('         author:', colored('d33pster', 'light_blue'))
         print('         GitHub:', colored('https://github.com/d33pster', 'light_blue'))
         exit(0)
```

### Comparing `RepMan-1.0.2/src/repman/repman.py` & `RepMan-1.0.3/src/repman/repman.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 ## OS Support
 # Linux -> aarch64
 # MacOs -> AppleSilicon(arm64)
 
-__version__ = '1.0.1'
+__version__ = '1.0.3'
 
 from repman._repmanfunctions import funcdefs
 from repman._repmanhelps import helptext
 from termcolor import colored
 from optioner import options
 from sys import argv
 from re import match
@@ -27,16 +27,16 @@
 def main():
     try:
         # helptext
         help = helptext(__version__)
         # functions
         funk = funcdefs(__version__)
         # create arguments
-        shortargs = ['h', 'v', 'a', 'i', 'o', 'l', 'lp', 'ae', 'al', 'u', 'sr']
-        longargs = ['help', 'version', 'add', 'init', 'open', 'list', 'list-w-path', 'add-existing', 'add-local', 'update', 'set-remote']
+        shortargs = ['h', 'v', 'a', 'i', 'o', 'l', 'lp', 'ae', 'al', 'u', 'sr', 'cred']
+        longargs = ['help', 'version', 'add', 'init', 'open', 'list', 'list-w-path', 'add-existing', 'add-local', 'update', 'set-remote', 'credits']
         
         # All args
         original = shortargs.copy()
         original.extend(longargs)
         
         # mutually exclusive args
         mutex = [
@@ -45,15 +45,16 @@
             ['o','open'],rem(original, ['o','open', 'h', 'help']),
             ['i', 'init'],rem(original, ['i', 'init', 'h', 'help']),
             ['l', 'list'],rem(original, ['l', 'list', 'h', 'help']),
             ['lp', 'list-w-path'],rem(original, ['lp', 'list-w-path', 'h', 'help']),
             ['ae', 'add-existing'],rem(original, ['ae', 'add-existing', 'h', 'help']),
             ['al', 'add-local'], rem(original, ['al', 'add-local', 'h', 'help']),
             ['u', 'update'], rem(original, ['u', 'update', 'h', 'help']),
-            ['sr', 'set-remote'], rem(original, ['sr', 'set-remote', 'h', 'help'])
+            ['sr', 'set-remote'], rem(original, ['sr', 'set-remote', 'h', 'help']),
+            ['cred', 'credits'], rem(original, ['cred', 'credits', 'h', 'help'])
         ]
         
         optctrl = options(shortargs, longargs, argv[1:], ifthisthennotthat=mutex)
         
         args, check, error, falseargs = optctrl._argparse()
         
         if not check:
@@ -98,14 +99,16 @@
                             help.addexisting_h(otherarg)
                         elif otherarg == '-al' or otherarg == '--add-local':
                             help.addlocal_h(otherarg)
                         elif otherarg == '-u' or otherarg == '--update':
                             help.update_h(otherarg)
                         elif otherarg == '-sr' or otherarg == '--set-remote':
                             help.setremote_h(otherarg)
+                        elif otherarg == '-cred' or otherarg == '--credits':
+                            help.credits()
                         else:
                             print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
                     elif len(args)<2:
                         help.base()
                     elif len(args)>2:
                         print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
                         print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
@@ -144,14 +147,16 @@
                             help.addexisting_h(otherarg)
                         elif otherarg == '-al' or otherarg == '--add-local':
                             help.addlocal_h(otherarg)
                         elif otherarg == '-u' or otherarg == '--update':
                             help.update_h(otherarg)
                         elif otherarg == '-sr' or otherarg == '--set-remote':
                             help.setremote_h(otherarg)
+                        elif otherarg == '-cred' or otherarg == '--credits':
+                            help.credits()
                         else:
                             print(colored('RepMan Err', 'red'), f': argument \'{otherarg}\' is not recognised.')
                     elif len(args)<2:
                         help.base()
                     elif len(args)>2:
                         print(colored('RepMan Err', 'red'), ': Please use one argument at a time to show help on that argument.')
                         print(colored('Format', 'blue'), ': \'repman <argument> -h\' or \'repman <argument> --help\'.')
@@ -163,14 +168,18 @@
                 else:
                     pass
                 
                 # version
                 if '-v' in args or '--version' in args:
                     help.version()
                 
+                # credits
+                if '-cred' in args or '--credits' in args:
+                    help.credits()
+                
                 # init
                 if '-i' in args:
                     index = argv.index('-i')
                     try:
                         value = argv[index+1]
                     except IndexError:
                         value = None
```

