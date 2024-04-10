# Comparing `tmp/train_route-0.6.3.tar.gz` & `tmp/train_route-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_route-0.6.3.tar", max compression
+gzip compressed data, was "train_route-1.0.0.tar", max compression
```

## Comparing `train_route-0.6.3.tar` & `train_route-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.6.3/LICENSE
--rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.6.3/README.md
--rw-r--r--   0        0        0      407 2024-04-04 15:40:18.526866 train_route-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.6.3/train_route/__init__.py
--rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.6.3/train_route/rotation.py
--rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.6.3/train_route/route.py
--rw-r--r--   0        0        0     5498 2024-04-04 15:39:58.936868 train_route-0.6.3/train_route/traveler.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-1.0.0/LICENSE
+-rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-1.0.0/README.md
+-rw-r--r--   0        0        0      443 2024-04-10 11:19:45.772098 train_route-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-1.0.0/train_route/__init__.py
+-rw-r--r--   0        0        0     1447 2024-04-09 11:56:48.086223 train_route-1.0.0/train_route/path.py
+-rw-r--r--   0        0        0     1827 2024-04-09 22:23:03.939153 train_route-1.0.0/train_route/schedule.py
+-rw-r--r--   0        0        0     2686 2024-04-09 23:25:04.468490 train_route-1.0.0/train_route/segment.py
+-rw-r--r--   0        0        0     1145 2024-04-09 23:42:26.468310 train_route-1.0.0/train_route/train.py
+-rw-r--r--   0        0        0     1573 2024-04-09 23:39:22.718337 train_route-1.0.0/train_route/train_render.py
+-rw-r--r--   0        0        0      892 2024-04-09 23:11:47.888634 train_route-1.0.0/train_route/train_system.py
+-rw-r--r--   0        0        0     1405 2024-04-09 23:17:03.118576 train_route-1.0.0/train_route/utils.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 train_route-1.0.0/PKG-INFO
```

### Comparing `train_route-0.6.3/LICENSE` & `train_route-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `train_route-0.6.3/PKG-INFO` & `train_route-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: train-route
-Version: 0.6.3
+Version: 1.0.0
 Summary: 
 Author: Samarin Aleksei
 Author-email: liotbiu1@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Train route
 
 Package provides classes for storing scheduled train routes and calculating current position of train.
 
 See [https://train-map.vercel.app/](https://train-map.vercel.app/)
```

