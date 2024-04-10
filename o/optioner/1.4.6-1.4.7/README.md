# Comparing `tmp/optioner-1.4.6.tar.gz` & `tmp/optioner-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.6.tar", last modified: Mon Apr  8 12:05:14 2024, max compression
+gzip compressed data, was "optioner-1.4.7.tar", last modified: Wed Apr 10 06:23:54 2024, max compression
```

## Comparing `optioner-1.4.6.tar` & `optioner-1.4.7.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.468043 optioner-1.4.6/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.6/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-08 12:05:14.467644 optioner-1.4.6/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-08 12:04:40.000000 optioner-1.4.6/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-08 12:04:56.000000 optioner-1.4.6/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-08 12:05:14.468110 optioner-1.4.6/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.464171 optioner-1.4.6/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.6/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-08 12:05:14.467042 optioner-1.4.6/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-08 12:05:14.000000 optioner-1.4.6/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     6973 2024-04-03 21:24:07.000000 optioner-1.4.6/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 06:23:54.519703 optioner-1.4.7/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.7/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6301 2024-04-10 06:23:54.519252 optioner-1.4.7/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     4065 2024-04-10 03:37:27.000000 optioner-1.4.7/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-10 06:22:19.000000 optioner-1.4.7/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-10 06:23:54.519773 optioner-1.4.7/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 06:23:54.514500 optioner-1.4.7/src/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.7/src/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 06:23:54.518640 optioner-1.4.7/src/optioner.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6301 2024-04-10 06:23:54.000000 optioner-1.4.7/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      258 2024-04-10 06:23:54.000000 optioner-1.4.7/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-10 06:23:54.000000 optioner-1.4.7/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-10 06:23:54.000000 optioner-1.4.7/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)     6832 2024-04-10 06:22:05.000000 optioner-1.4.7/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 06:23:54.517741 optioner-1.4.7/tests/
+-rw-r--r--   0 d33pster   (501) staff       (20)      939 2024-04-10 06:15:16.000000 optioner-1.4.7/tests/test_basic.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      185 2024-04-10 06:04:09.000000 optioner-1.4.7/tests/test_compulsory_args.py
```

### Comparing `optioner-1.4.6/LICENSE` & `optioner-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.6/PKG-INFO` & `optioner-1.4.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.6
+Version: 1.4.7
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -40,22 +40,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
+![PyPI - Version](https://img.shields.io/pypi/v/optioner)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner)
+![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner)
+![GitHub License](https://img.shields.io/github/license/d33pster/optioner)
+[![Build status](https://ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/optioner)
 
-![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
-![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
-![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
-<br><br><br>
-v1.4.6
+<br>
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.6 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.7 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -22,25 +22,24 @@
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.0 Description-Content-Type: text/markdown License-File: LICENSE # optioner
-![Static Badge](https://img.shields.io/badge/pypi-available-
-brightgreen?style=flat&logo=python&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Windows-supported-
-blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/MacOS-supported-
-blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
-
-
-v1.4.6
+![PyPI - Version](https://img.shields.io/pypi/v/optioner) ![Python Version from
+PEP 621 TOML](https://img.shields.io/python/required-version-
+toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner) ![Dependents (via
+libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner) !
+[GitHub License](https://img.shields.io/github/license/d33pster/optioner) [!
+[Build status](https://ci.appveyor.com/api/projects/status/
+qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/
+optioner)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.6/pyproject.toml` & `optioner-1.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.6"
+version = "1.4.7"
 description = "Argument Parser"
 requires-python = ">=3.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.4.6/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.7/src/optioner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.6
+Version: 1.4.7
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -40,22 +40,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
+![PyPI - Version](https://img.shields.io/pypi/v/optioner)
+![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner)
+![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner)
+![GitHub License](https://img.shields.io/github/license/d33pster/optioner)
+[![Build status](https://ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/optioner)
 
-![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
-![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
-![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
-<br><br><br>
-v1.4.6
+<br>
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.6 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.7 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -22,25 +22,24 @@
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.0 Description-Content-Type: text/markdown License-File: LICENSE # optioner
-![Static Badge](https://img.shields.io/badge/pypi-available-
-brightgreen?style=flat&logo=python&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
-![Static Badge](https://img.shields.io/badge/Windows-supported-
-blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/MacOS-supported-
-blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
-img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
-
-
-v1.4.6
+![PyPI - Version](https://img.shields.io/pypi/v/optioner) ![Python Version from
+PEP 621 TOML](https://img.shields.io/python/required-version-
+toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner) ![Dependents (via
+libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner) !
+[GitHub License](https://img.shields.io/github/license/d33pster/optioner) [!
+[Build status](https://ci.appveyor.com/api/projects/status/
+qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
+![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/
+optioner)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.6/src/optioner.py` & `optioner-1.4.7/src/optioner.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,24 +137,23 @@
             str | tuple | None_: returns value of argument or None
         """
         if len(arg)>2:
             arg = '--' + arg
         else:
             arg = '-' + arg
         
+        index = self._args.index(arg)
+        
+        result: list[str] = []
+        
         try:
-            for i in range(len(self._args)):
-                if self._args[i] == arg:
-                    if count==1:
-                        return self._args[i+1]
-                    else:
-                        k = 1
-                        result = []
-                        while(count>0):
-                            result.append(self._args[i+k])
-                            k += 1
-                            count -= 1
-                        return tuple(result)
+            for i in range(index+1, index+1+count):
+                result.append(self._args[i])
         except IndexError:
-            raise RuntimeError(f'{arg} expects {count} arguments.')
+            raise RuntimeError(f'\'{arg}\' expects {count} arg(s).')
         
-        return None
+        if len(result)==0:
+            return None
+        elif len(result)==1:
+            return result[0]
+        elif len(result)>1:
+            return tuple(result)
```

