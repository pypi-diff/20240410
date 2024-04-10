# Comparing `tmp/matplotlib_visual-0.9.3.tar.gz` & `tmp/matplotlib_visual-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_visual-0.9.3.tar", last modified: Tue Apr  9 14:53:39 2024, max compression
+gzip compressed data, was "matplotlib_visual-0.9.4.tar", last modified: Wed Apr 10 14:07:52 2024, max compression
```

## Comparing `matplotlib_visual-0.9.3.tar` & `matplotlib_visual-0.9.4.tar`

### file list

```diff
@@ -1,42 +1,30 @@
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-09 14:53:39.495811 matplotlib_visual-0.9.3/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.9.3/LICENSE
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-09 14:53:39.494811 matplotlib_visual-0.9.3/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.9.3/README.md
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-09 14:53:39.490811 matplotlib_visual-0.9.3/matplotlib_visual/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.9.3/matplotlib_visual/__init__.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-09 14:53:39.494811 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/__init__.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/god.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-02-04 07:14:39.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir1.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-02-04 07:15:04.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3301 2024-03-13 15:24:02.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir5full.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 15:03:11.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1627 2024-04-08 13:09:48.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml10.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1145 2024-04-08 13:13:22.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml11a.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      879 2024-04-08 13:13:05.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml11b.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1047 2024-04-08 13:12:53.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      952 2024-04-09 14:51:51.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1814 2024-04-09 14:51:55.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml33.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1303 2024-02-04 07:27:56.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      792 2024-04-09 14:51:35.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1153 2024-04-09 14:51:34.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml55.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1266 2024-04-09 14:52:19.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2967 2024-04-09 14:52:30.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml66.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      742 2024-03-25 16:15:35.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1195 2024-03-25 16:15:45.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1089 2024-04-08 13:09:25.000000 matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ml9.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      769 2024-04-08 13:57:55.000000 matplotlib_visual-0.9.3/matplotlib_visual/graph.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-04-08 13:57:54.000000 matplotlib_visual-0.9.3/matplotlib_visual/models.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      376 2024-04-08 13:57:53.000000 matplotlib_visual-0.9.3/matplotlib_visual/piechart.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-09 14:53:39.494811 matplotlib_visual-0.9.3/matplotlib_visual.egg-info/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-09 14:53:39.000000 matplotlib_visual-0.9.3/matplotlib_visual.egg-info/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1297 2024-04-09 14:53:39.000000 matplotlib_visual-0.9.3/matplotlib_visual.egg-info/SOURCES.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-09 14:53:39.000000 matplotlib_visual-0.9.3/matplotlib_visual.egg-info/dependency_links.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-09 14:53:39.000000 matplotlib_visual-0.9.3/matplotlib_visual.egg-info/top_level.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-09 14:53:39.496811 matplotlib_visual-0.9.3/setup.cfg
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-04-09 14:52:49.000000 matplotlib_visual-0.9.3/setup.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-10 14:07:52.745350 matplotlib_visual-0.9.4/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.9.4/LICENSE
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-10 14:07:52.744350 matplotlib_visual-0.9.4/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.9.4/README.md
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-10 14:07:52.741350 matplotlib_visual-0.9.4/matplotlib_visual/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.9.4/matplotlib_visual/__init__.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-10 14:07:52.743350 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/__init__.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/god.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-04-10 13:59:56.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir1.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-04-10 13:59:58.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1283 2024-04-10 14:05:44.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir5app.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1625 2024-04-10 14:06:38.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir5db.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1971 2024-04-10 14:06:23.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir5index.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-04-10 14:00:51.000000 matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      769 2024-04-08 13:57:55.000000 matplotlib_visual-0.9.4/matplotlib_visual/graph.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-04-08 13:57:54.000000 matplotlib_visual-0.9.4/matplotlib_visual/models.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      376 2024-04-08 13:57:53.000000 matplotlib_visual-0.9.4/matplotlib_visual/piechart.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-10 14:07:52.743350 matplotlib_visual-0.9.4/matplotlib_visual.egg-info/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-04-10 14:07:52.000000 matplotlib_visual-0.9.4/matplotlib_visual.egg-info/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      827 2024-04-10 14:07:52.000000 matplotlib_visual-0.9.4/matplotlib_visual.egg-info/SOURCES.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-10 14:07:52.000000 matplotlib_visual-0.9.4/matplotlib_visual.egg-info/dependency_links.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-10 14:07:52.000000 matplotlib_visual-0.9.4/matplotlib_visual.egg-info/top_level.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-10 14:07:52.745350 matplotlib_visual-0.9.4/setup.cfg
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-04-10 14:06:56.000000 matplotlib_visual-0.9.4/setup.py
```

### Comparing `matplotlib_visual-0.9.3/LICENSE` & `matplotlib_visual-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/README.md` & `matplotlib_visual-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/god.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/god.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir1.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir1.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir2.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir3.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir4.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir5.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir6.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir7.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/code_snippets/ir8.py` & `matplotlib_visual-0.9.4/matplotlib_visual/code_snippets/ir8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.9.3/matplotlib_visual/graph.py` & `matplotlib_visual-0.9.4/matplotlib_visual/graph.py`

 * *Files identical despite different names*

