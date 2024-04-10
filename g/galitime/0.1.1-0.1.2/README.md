# Comparing `tmp/galitime-0.1.1.tar.gz` & `tmp/galitime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galitime-0.1.1.tar", last modified: Wed Apr 10 09:58:37 2024, max compression
+gzip compressed data, was "galitime-0.1.2.tar", last modified: Wed Apr 10 21:51:21 2024, max compression
```

## Comparing `galitime-0.1.1.tar` & `galitime-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.209878 galitime-0.1.1/
--rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.1/LICENSE.txt
--rw-r--r--   0 karel      (503) staff       (20)     3225 2024-04-10 09:58:37.202445 galitime-0.1.1/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)     2647 2024-04-10 09:56:38.000000 galitime-0.1.1/README.rst
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.107995 galitime-0.1.1/galitime/
--rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.1/galitime/__init__.py
--rwxr-xr-x   0 karel      (503) staff       (20)     3507 2024-04-10 08:55:54.000000 galitime-0.1.1/galitime/galitime.py
--rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.1/galitime/increment_version.py
--rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-10 09:58:23.000000 galitime-0.1.1/galitime/version.py
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 09:58:37.194224 galitime-0.1.1/galitime.egg-info/
--rw-r--r--   0 karel      (503) staff       (20)     3225 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-10 09:58:37.000000 galitime-0.1.1/galitime.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/entry_points.txt
--rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/requires.txt
--rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-10 09:58:36.000000 galitime-0.1.1/galitime.egg-info/top_level.txt
--rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-10 09:58:37.210220 galitime-0.1.1/setup.cfg
--rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.1/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.962725 galitime-0.1.2/
+-rw-r--r--   0 karel      (503) staff       (20)     1070 2024-04-10 08:29:59.000000 galitime-0.1.2/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)     3840 2024-04-10 21:51:21.961913 galitime-0.1.2/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     3262 2024-04-10 13:08:53.000000 galitime-0.1.2/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.850400 galitime-0.1.2/galitime/
+-rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 galitime-0.1.2/galitime/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)     5687 2024-04-10 12:53:23.000000 galitime-0.1.2/galitime/galitime.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 galitime-0.1.2/galitime/increment_version.py
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-10 21:47:41.000000 galitime-0.1.2/galitime/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-10 21:51:21.961051 galitime-0.1.2/galitime.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     3840 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-10 21:51:21.000000 galitime-0.1.2/galitime.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-10 21:51:21.962809 galitime-0.1.2/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     1351 2024-04-10 08:28:25.000000 galitime-0.1.2/setup.py
```

### Comparing `galitime-0.1.1/LICENSE.txt` & `galitime-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galitime-0.1.1/PKG-INFO` & `galitime-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galitime
-Version: 0.1.1
+Version: 0.1.2
 Summary: description
 Home-page: https://github.com/karel-brinda/galitime
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,15 +41,15 @@
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
-    # brew install gnu-time # on OS X
+    if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
     conda install -y -c bioconda -c conda-forge galitime
     galitime --log time.log ls
 
 
 
 Installation
 ------------
@@ -97,15 +97,33 @@
 
     options:
       -h, --help            show this help message and exit
       --log LOG             Path to the log file with benchmark statistics (if the directory doesn't exist, it will be created).
       --experiment EXPERIMENT
                             Name of the experiment (to be attached to the output)
       -v                    show program's version number and exit
-    
+
+
+Output
+------
+
+* ``experiment`` - Name of the experiment, if provided via ``-n``
+* ``real_s`` - Real time in seconds (wall clock time)
+* ``user_s`` - User CPU time in seconds (user mode, excluding system calls)
+* ``sys_s`` - System CPU time in seconds (kernel mode)
+* ``percent_cpu`` - CPU usage percentage
+* ``ram_kb`` - Maximum RAM usage in kilobytes
+* ``fs_inputs`` - File system read read operations count
+* ``fs_outputs`` - File system write operations count
+* ``python_real_s`` - Python-measured real time in seconds
+* ``command`` - Command executed, with tabs replaced by spaces
+
+
+
+
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/galitime/issues>`_.
```

### Comparing `galitime-0.1.1/README.rst` & `galitime-0.1.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
-    # brew install gnu-time # on OS X
+    if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
     conda install -y -c bioconda -c conda-forge galitime
     galitime --log time.log ls
 
 
 
 Installation
 ------------
@@ -79,15 +79,33 @@
 
     options:
       -h, --help            show this help message and exit
       --log LOG             Path to the log file with benchmark statistics (if the directory doesn't exist, it will be created).
       --experiment EXPERIMENT
                             Name of the experiment (to be attached to the output)
       -v                    show program's version number and exit
-    
+
+
+Output
+------
+
+* ``experiment`` - Name of the experiment, if provided via ``-n``
+* ``real_s`` - Real time in seconds (wall clock time)
+* ``user_s`` - User CPU time in seconds (user mode, excluding system calls)
+* ``sys_s`` - System CPU time in seconds (kernel mode)
+* ``percent_cpu`` - CPU usage percentage
+* ``ram_kb`` - Maximum RAM usage in kilobytes
+* ``fs_inputs`` - File system read read operations count
+* ``fs_outputs`` - File system write operations count
+* ``python_real_s`` - Python-measured real time in seconds
+* ``command`` - Command executed, with tabs replaced by spaces
+
+
+
+
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/galitime/issues>`_.
```

### Comparing `galitime-0.1.1/galitime.egg-info/PKG-INFO` & `galitime-0.1.2/galitime.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galitime
-Version: 0.1.1
+Version: 0.1.2
 Summary: description
 Home-page: https://github.com/karel-brinda/galitime
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,15 +41,15 @@
 
 
 Quick example
 -------------
 
 .. code-block:: bash
 
-    # brew install gnu-time # on OS X
+    if [[ $(uname) == "Darwin" ]]; then brew install gnu-time; fi
     conda install -y -c bioconda -c conda-forge galitime
     galitime --log time.log ls
 
 
 
 Installation
 ------------
@@ -97,15 +97,33 @@
 
     options:
       -h, --help            show this help message and exit
       --log LOG             Path to the log file with benchmark statistics (if the directory doesn't exist, it will be created).
       --experiment EXPERIMENT
                             Name of the experiment (to be attached to the output)
       -v                    show program's version number and exit
-    
+
+
+Output
+------
+
+* ``experiment`` - Name of the experiment, if provided via ``-n``
+* ``real_s`` - Real time in seconds (wall clock time)
+* ``user_s`` - User CPU time in seconds (user mode, excluding system calls)
+* ``sys_s`` - System CPU time in seconds (kernel mode)
+* ``percent_cpu`` - CPU usage percentage
+* ``ram_kb`` - Maximum RAM usage in kilobytes
+* ``fs_inputs`` - File system read read operations count
+* ``fs_outputs`` - File system write operations count
+* ``python_real_s`` - Python-measured real time in seconds
+* ``command`` - Command executed, with tabs replaced by spaces
+
+
+
+
 
 Issues
 ------
 
 Please use `Github issues <https://github.com/karel-brinda/galitime/issues>`_.
```

### Comparing `galitime-0.1.1/setup.py` & `galitime-0.1.2/setup.py`

 * *Files identical despite different names*

