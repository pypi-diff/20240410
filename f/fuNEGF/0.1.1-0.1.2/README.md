# Comparing `tmp/fuNEGF-0.1.1.tar.gz` & `tmp/fuNEGF-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuNEGF-0.1.1.tar", last modified: Tue Apr  9 07:01:18 2024, max compression
+gzip compressed data, was "fuNEGF-0.1.2.tar", last modified: Wed Apr 10 09:26:41 2024, max compression
```

## Comparing `fuNEGF-0.1.1.tar` & `fuNEGF-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:18.362473 fuNEGF-0.1.1/
--rw-rw-rw-   0        0        0     1524 2024-03-09 08:17:51.000000 fuNEGF-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       22 2024-04-09 07:01:04.000000 fuNEGF-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2075 2024-04-09 07:01:18.361473 fuNEGF-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-03-10 07:38:33.000000 fuNEGF-0.1.1/README.md
--rw-rw-rw-   0        0        0       82 2024-04-08 14:48:16.000000 fuNEGF-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      449 2024-04-09 07:01:18.364473 fuNEGF-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:18.301875 fuNEGF-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:18.341475 fuNEGF-0.1.1/src/examples/
--rw-rw-rw-   0        0        0   796090 2024-03-11 16:29:42.000000 fuNEGF-0.1.1/src/examples/one-dimensional_channel.html
--rw-rw-rw-   0        0        0   480745 2024-03-10 07:17:45.000000 fuNEGF-0.1.1/src/examples/one-dimensional_channel.ipynb
--rw-rw-rw-   0        0        0   846545 2024-04-08 15:14:10.000000 fuNEGF-0.1.1/src/examples/one-dimensional_channel.pdf
--rw-rw-rw-   0        0        0   344658 2024-03-11 16:37:06.000000 fuNEGF-0.1.1/src/examples/time_complexity.html
--rw-rw-rw-   0        0        0    52670 2024-03-15 18:18:08.000000 fuNEGF-0.1.1/src/examples/time_complexity.ipynb
--rw-rw-rw-   0        0        0   296053 2024-03-11 16:37:31.000000 fuNEGF-0.1.1/src/examples/time_complexity.pdf
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:18.359474 fuNEGF-0.1.1/src/fuNEGF.egg-info/
--rw-rw-rw-   0        0        0     2075 2024-04-09 07:01:18.000000 fuNEGF-0.1.1/src/fuNEGF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-04-09 07:01:18.000000 fuNEGF-0.1.1/src/fuNEGF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:01:18.000000 fuNEGF-0.1.1/src/fuNEGF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-09 07:01:18.000000 fuNEGF-0.1.1/src/fuNEGF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:01:18.000000 fuNEGF-0.1.1/src/fuNEGF.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 09:26:41.137811 fuNEGF-0.1.2/
+-rw-rw-rw-   0        0        0     1524 2024-03-09 08:17:51.000000 fuNEGF-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-10 09:22:33.000000 fuNEGF-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3295 2024-04-10 09:26:41.136810 fuNEGF-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2024-04-10 08:02:01.000000 fuNEGF-0.1.2/README.md
+-rw-rw-rw-   0        0        0       82 2024-04-08 14:48:16.000000 fuNEGF-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      449 2024-04-10 09:26:41.139806 fuNEGF-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 09:26:41.083805 fuNEGF-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-10 09:26:41.112803 fuNEGF-0.1.2/src/examples/
+-rw-rw-rw-   0        0        0   796090 2024-03-11 16:29:42.000000 fuNEGF-0.1.2/src/examples/one-dimensional_channel.html
+-rw-rw-rw-   0        0        0   480745 2024-03-10 07:17:45.000000 fuNEGF-0.1.2/src/examples/one-dimensional_channel.ipynb
+-rw-rw-rw-   0        0        0   846545 2024-04-08 15:14:10.000000 fuNEGF-0.1.2/src/examples/one-dimensional_channel.pdf
+-rw-rw-rw-   0        0        0   344658 2024-03-11 16:37:06.000000 fuNEGF-0.1.2/src/examples/time_complexity.html
+-rw-rw-rw-   0        0        0    52670 2024-03-15 18:18:08.000000 fuNEGF-0.1.2/src/examples/time_complexity.ipynb
+-rw-rw-rw-   0        0        0   296053 2024-03-11 16:37:31.000000 fuNEGF-0.1.2/src/examples/time_complexity.pdf
+drwxrwxrwx   0        0        0        0 2024-04-10 09:26:41.120812 fuNEGF-0.1.2/src/fuNEGF/
+-rw-rw-rw-   0        0        0        0 2024-03-09 08:17:51.000000 fuNEGF-0.1.2/src/fuNEGF/__init.py__
+-rw-rw-rw-   0        0        0    12092 2024-04-09 16:06:28.000000 fuNEGF-0.1.2/src/fuNEGF/models.py
+-rw-rw-rw-   0        0        0      381 2024-04-09 11:27:41.000000 fuNEGF-0.1.2/src/fuNEGF/physical_models.py
+drwxrwxrwx   0        0        0        0 2024-04-10 09:26:41.134805 fuNEGF-0.1.2/src/fuNEGF.egg-info/
+-rw-rw-rw-   0        0        0     3295 2024-04-10 09:26:41.000000 fuNEGF-0.1.2/src/fuNEGF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-10 09:26:41.000000 fuNEGF-0.1.2/src/fuNEGF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 09:26:41.000000 fuNEGF-0.1.2/src/fuNEGF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-10 09:26:41.000000 fuNEGF-0.1.2/src/fuNEGF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 09:26:41.000000 fuNEGF-0.1.2/src/fuNEGF.egg-info/top_level.txt
```

### Comparing `fuNEGF-0.1.1/LICENSE` & `fuNEGF-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/one-dimensional_channel.html` & `fuNEGF-0.1.2/src/examples/one-dimensional_channel.html`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/one-dimensional_channel.ipynb` & `fuNEGF-0.1.2/src/examples/one-dimensional_channel.ipynb`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/one-dimensional_channel.pdf` & `fuNEGF-0.1.2/src/examples/one-dimensional_channel.pdf`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/time_complexity.html` & `fuNEGF-0.1.2/src/examples/time_complexity.html`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/time_complexity.ipynb` & `fuNEGF-0.1.2/src/examples/time_complexity.ipynb`

 * *Files identical despite different names*

### Comparing `fuNEGF-0.1.1/src/examples/time_complexity.pdf` & `fuNEGF-0.1.2/src/examples/time_complexity.pdf`

 * *Files identical despite different names*

