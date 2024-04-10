# Comparing `tmp/tsq-0.0.15.tar.gz` & `tmp/tsq-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsq-0.0.15.tar", last modified: Mon Apr  8 13:59:29 2024, max compression
+gzip compressed data, was "tsq-0.0.16.tar", last modified: Wed Apr 10 08:24:20 2024, max compression
```

## Comparing `tsq-0.0.15.tar` & `tsq-0.0.16.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.049893 tsq-0.0.15/
--rw-r--r--   0 ko         (501) staff       (20)     1061 2024-02-15 08:38:56.000000 tsq-0.0.15/LICENSE.md
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-08 13:59:29.049659 tsq-0.0.15/PKG-INFO
--rw-r--r--   0 ko         (501) staff       (20)      220 2024-02-21 13:05:14.000000 tsq-0.0.15/README.md
--rw-r--r--   0 ko         (501) staff       (20)      781 2024-04-08 13:59:23.000000 tsq-0.0.15/pyproject.toml
--rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-08 13:59:29.049934 tsq-0.0.15/setup.cfg
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.046458 tsq-0.0.15/taskq/
--rw-r--r--   0 ko         (501) staff       (20)       23 2024-03-27 07:03:11.000000 tsq-0.0.15/taskq/__init__.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.047582 tsq-0.0.15/taskq/actions/
--rw-r--r--   0 ko         (501) staff       (20)       92 2024-02-21 12:49:38.000000 tsq-0.0.15/taskq/actions/__init__.py
--rw-r--r--   0 ko         (501) staff       (20)     5141 2024-04-08 13:58:20.000000 tsq-0.0.15/taskq/actions/add.py
--rw-r--r--   0 ko         (501) staff       (20)     1522 2024-03-16 08:13:56.000000 tsq-0.0.15/taskq/actions/backend.py
--rw-r--r--   0 ko         (501) staff       (20)     2356 2024-03-27 06:54:37.000000 tsq-0.0.15/taskq/actions/base.py
--rw-r--r--   0 ko         (501) staff       (20)     1800 2024-03-25 17:22:30.000000 tsq-0.0.15/taskq/actions/config.py
--rw-r--r--   0 ko         (501) staff       (20)     2556 2024-02-21 12:59:28.000000 tsq-0.0.15/taskq/actions/filter.py
--rw-r--r--   0 ko         (501) staff       (20)    11868 2024-03-26 09:21:45.000000 tsq-0.0.15/taskq/actions/read.py
--rw-r--r--   0 ko         (501) staff       (20)     3067 2024-03-16 08:14:50.000000 tsq-0.0.15/taskq/actions/write.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.048280 tsq-0.0.15/taskq/backends/
--rw-r--r--   0 ko         (501) staff       (20)      106 2024-03-27 18:02:23.000000 tsq-0.0.15/taskq/backends/__init__.py
--rw-r--r--   0 ko         (501) staff       (20)     2671 2024-03-27 17:15:39.000000 tsq-0.0.15/taskq/backends/base.py
--rw-r--r--   0 ko         (501) staff       (20)     1087 2024-03-27 17:19:10.000000 tsq-0.0.15/taskq/backends/dummy.py
--rw-r--r--   0 ko         (501) staff       (20)     5690 2024-03-28 19:49:01.000000 tsq-0.0.15/taskq/backends/ts.py
--rw-r--r--   0 ko         (501) staff       (20)     3928 2024-03-27 18:07:00.000000 tsq-0.0.15/taskq/cli.py
--rw-r--r--   0 ko         (501) staff       (20)     1561 2024-02-21 12:17:48.000000 tsq-0.0.15/taskq/common.py
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-02-15 15:26:07.000000 tsq-0.0.15/taskq/utils.py
-drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-08 13:59:29.049297 tsq-0.0.15/tsq.egg-info/
--rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/PKG-INFO
--rw-r--r--   0 ko         (501) staff       (20)      543 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/SOURCES.txt
--rw-r--r--   0 ko         (501) staff       (20)        1 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/dependency_links.txt
--rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/entry_points.txt
--rw-r--r--   0 ko         (501) staff       (20)       45 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/requires.txt
--rw-r--r--   0 ko         (501) staff       (20)        6 2024-04-08 13:59:29.000000 tsq-0.0.15/tsq.egg-info/top_level.txt
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-10 08:24:20.321847 tsq-0.0.16/
+-rw-r--r--   0 ko         (501) staff       (20)     1061 2024-02-15 08:38:56.000000 tsq-0.0.16/LICENSE.md
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-10 08:24:20.321673 tsq-0.0.16/PKG-INFO
+-rw-r--r--   0 ko         (501) staff       (20)      220 2024-02-21 13:05:14.000000 tsq-0.0.16/README.md
+-rw-r--r--   0 ko         (501) staff       (20)      781 2024-04-10 08:23:14.000000 tsq-0.0.16/pyproject.toml
+-rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-10 08:24:20.321881 tsq-0.0.16/setup.cfg
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-10 08:24:20.316731 tsq-0.0.16/taskq/
+-rw-r--r--   0 ko         (501) staff       (20)       23 2024-04-10 08:24:15.000000 tsq-0.0.16/taskq/__init__.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-10 08:24:20.319270 tsq-0.0.16/taskq/actions/
+-rw-r--r--   0 ko         (501) staff       (20)       92 2024-02-21 12:49:38.000000 tsq-0.0.16/taskq/actions/__init__.py
+-rw-r--r--   0 ko         (501) staff       (20)     5141 2024-04-08 13:58:20.000000 tsq-0.0.16/taskq/actions/add.py
+-rw-r--r--   0 ko         (501) staff       (20)     1522 2024-03-16 08:13:56.000000 tsq-0.0.16/taskq/actions/backend.py
+-rw-r--r--   0 ko         (501) staff       (20)     2356 2024-03-27 06:54:37.000000 tsq-0.0.16/taskq/actions/base.py
+-rw-r--r--   0 ko         (501) staff       (20)     1800 2024-03-25 17:22:30.000000 tsq-0.0.16/taskq/actions/config.py
+-rw-r--r--   0 ko         (501) staff       (20)     2556 2024-02-21 12:59:28.000000 tsq-0.0.16/taskq/actions/filter.py
+-rw-r--r--   0 ko         (501) staff       (20)    11868 2024-03-26 09:21:45.000000 tsq-0.0.16/taskq/actions/read.py
+-rw-r--r--   0 ko         (501) staff       (20)     3067 2024-03-16 08:14:50.000000 tsq-0.0.16/taskq/actions/write.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-10 08:24:20.320498 tsq-0.0.16/taskq/backends/
+-rw-r--r--   0 ko         (501) staff       (20)      108 2024-04-09 14:06:58.000000 tsq-0.0.16/taskq/backends/__init__.py
+-rw-r--r--   0 ko         (501) staff       (20)     2671 2024-03-27 17:15:39.000000 tsq-0.0.16/taskq/backends/base.py
+-rw-r--r--   0 ko         (501) staff       (20)     1087 2024-03-27 17:19:10.000000 tsq-0.0.16/taskq/backends/dummy.py
+-rw-r--r--   0 ko         (501) staff       (20)     5690 2024-03-28 19:49:01.000000 tsq-0.0.16/taskq/backends/ts.py
+-rw-r--r--   0 ko         (501) staff       (20)     3928 2024-03-27 18:07:00.000000 tsq-0.0.16/taskq/cli.py
+-rw-r--r--   0 ko         (501) staff       (20)     1561 2024-02-21 12:17:48.000000 tsq-0.0.16/taskq/common.py
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-02-15 15:26:07.000000 tsq-0.0.16/taskq/utils.py
+drwxr-xr-x   0 ko         (501) staff       (20)        0 2024-04-10 08:24:20.321489 tsq-0.0.16/tsq.egg-info/
+-rw-r--r--   0 ko         (501) staff       (20)      770 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/PKG-INFO
+-rw-r--r--   0 ko         (501) staff       (20)      543 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/SOURCES.txt
+-rw-r--r--   0 ko         (501) staff       (20)        1 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/dependency_links.txt
+-rw-r--r--   0 ko         (501) staff       (20)       38 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/entry_points.txt
+-rw-r--r--   0 ko         (501) staff       (20)       45 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/requires.txt
+-rw-r--r--   0 ko         (501) staff       (20)        6 2024-04-10 08:24:20.000000 tsq-0.0.16/tsq.egg-info/top_level.txt
```

### Comparing `tsq-0.0.15/LICENSE.md` & `tsq-0.0.16/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/PKG-INFO` & `tsq-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsq
-Version: 0.0.15
+Version: 0.0.16
 Summary: A Friendly Task Scheduler Frontend
 Author: admk
 Project-URL: Homepage, https://github.com/admk/tu
 Project-URL: Issues, https://github.com/admk/tu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsq-0.0.15/pyproject.toml` & `tsq-0.0.16/pyproject.toml`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsq"
+dynamic = ["version"]
 authors = [
   { name="admk" },
 ]
 description = "A Friendly Task Scheduler Frontend"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -17,15 +18,14 @@
     "blessed >= 1.20.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dynamic = ["version"]
 
 [project.scripts]
 tq = "taskq.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/admk/tu"
 Issues = "https://github.com/admk/tu/issues"
```

### Comparing `tsq-0.0.15/taskq/actions/add.py` & `tsq-0.0.16/taskq/actions/add.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/backend.py` & `tsq-0.0.16/taskq/actions/backend.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/base.py` & `tsq-0.0.16/taskq/actions/base.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/config.py` & `tsq-0.0.16/taskq/actions/config.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/filter.py` & `tsq-0.0.16/taskq/actions/filter.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/read.py` & `tsq-0.0.16/taskq/actions/read.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/actions/write.py` & `tsq-0.0.16/taskq/actions/write.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/backends/base.py` & `tsq-0.0.16/taskq/backends/base.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/backends/dummy.py` & `tsq-0.0.16/taskq/backends/dummy.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/backends/ts.py` & `tsq-0.0.16/taskq/backends/ts.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/cli.py` & `tsq-0.0.16/taskq/cli.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/common.py` & `tsq-0.0.16/taskq/common.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/taskq/utils.py` & `tsq-0.0.16/taskq/utils.py`

 * *Files identical despite different names*

### Comparing `tsq-0.0.15/tsq.egg-info/PKG-INFO` & `tsq-0.0.16/tsq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsq
-Version: 0.0.15
+Version: 0.0.16
 Summary: A Friendly Task Scheduler Frontend
 Author: admk
 Project-URL: Homepage, https://github.com/admk/tu
 Project-URL: Issues, https://github.com/admk/tu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tsq-0.0.15/tsq.egg-info/SOURCES.txt` & `tsq-0.0.16/tsq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

