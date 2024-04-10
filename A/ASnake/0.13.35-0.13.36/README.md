# Comparing `tmp/ASnake-0.13.35.tar.gz` & `tmp/ASnake-0.13.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASnake-0.13.35.tar", last modified: Fri Apr  5 08:11:42 2024, max compression
+gzip compressed data, was "ASnake-0.13.36.tar", last modified: Wed Apr 10 15:49:43 2024, max compression
```

## Comparing `ASnake-0.13.35.tar` & `ASnake-0.13.36.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-05 08:11:42.079517 ASnake-0.13.35/
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-05 08:11:42.079517 ASnake-0.13.35/ASnake.egg-info/
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1133 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      263 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/SOURCES.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/dependency_links.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       39 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/entry_points.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/requires.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       19 2024-04-05 08:11:42.000000 ASnake-0.13.35/ASnake.egg-info/top_level.txt
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)   536080 2024-04-03 17:22:37.000000 ASnake-0.13.35/ASnake.py
--rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.35/LICENSE.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1133 2024-04-05 08:11:42.079517 ASnake-0.13.35/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.35/README.md
--rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-05 08:11:22.000000 ASnake-0.13.35/__version__.py
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8889 2024-03-31 14:25:37.000000 ASnake-0.13.35/megaTest.asnake
--rw-r--r--   0 ahri      (1002) ahri      (1002)      454 2024-04-05 08:11:42.079517 ASnake-0.13.35/setup.cfg
--rw-r--r--   0 ahri      (1002) ahri      (1002)      750 2024-04-05 08:11:22.000000 ASnake-0.13.35/setup.py
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/ASnake.egg-info/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    14968 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      237 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/SOURCES.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/dependency_links.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       11 2024-04-10 15:49:43.000000 ASnake-0.13.36/ASnake.egg-info/top_level.txt
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-10 15:49:43.164333 ASnake-0.13.36/ASnakeData/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-09 12:51:58.000000 ASnake-0.13.36/ASnakeData/ASnakeAlias.bat
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 15:43:29.000000 ASnake-0.13.36/ASnakeData/megaTest.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-09 14:58:35.000000 ASnake-0.13.36/ASnakeData/setAlias.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 ASnake-0.13.36/LICENSE.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    14968 2024-04-10 15:49:43.164333 ASnake-0.13.36/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 ASnake-0.13.36/README.md
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1611 2024-04-10 15:35:00.000000 ASnake-0.13.36/pyproject.toml
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-10 15:49:43.164333 ASnake-0.13.36/setup.cfg
```

### Comparing `ASnake-0.13.35/LICENSE.txt` & `ASnake-0.13.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.35/README.md` & `ASnake-0.13.36/README.md`

 * *Files identical despite different names*

### Comparing `ASnake-0.13.35/megaTest.asnake` & `ASnake-0.13.36/ASnakeData/megaTest.asnake`

 * *Files 1% similar despite different names*

```diff
@@ -183,21 +183,21 @@
 a is 5
 for xx in a do xx
 if result is 4 $worked
 else 'int to range' $failed
 
 
 $start
-ฯ€ is 3.14
-if ฯ€ is 3.14 $worked
+π is 3.14
+if π is 3.14 $worked
 else 'non-ascii variable' $failed
 
 $start
-๐ค๐’๐งก is 'love'
-if ๐ค๐’๐งก is 'love' $worked
+🤍💚🧡 is 'love'
+if 🤍💚🧡 is 'love' $worked
 else '(multi) emoji variable' $failed
 
 
 $start
 x is 12
 if f"{x+2}" is '14' $worked
 else 'basic f-string parsing' $failed
@@ -459,8 +459,8 @@
 $functionPass = off
 test2
 if result is 2 do $worked
 else 'functionPass meta off' $failed
 
 
 
-f"Failed={failed} Working={working} out of {max}" to print
+f"Failed={failed} Working={working} out of {max}" to print
```

