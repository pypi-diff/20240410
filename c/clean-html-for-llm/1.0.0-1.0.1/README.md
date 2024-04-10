# Comparing `tmp/clean_html_for_llm-1.0.0.tar.gz` & `tmp/clean_html_for_llm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_html_for_llm-1.0.0.tar", last modified: Wed Apr 10 07:38:44 2024, max compression
+gzip compressed data, was "clean_html_for_llm-1.0.1.tar", last modified: Wed Apr 10 07:52:55 2024, max compression
```

## Comparing `clean_html_for_llm-1.0.0.tar` & `clean_html_for_llm-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:38:44.577816 clean_html_for_llm-1.0.0/
--rw-r--r--   0 shubhamraj   (502) staff       (20)     1073 2024-04-10 07:24:00.000000 clean_html_for_llm-1.0.0/LICENSE
--rw-r--r--   0 shubhamraj   (502) staff       (20)      718 2024-04-10 07:38:44.577673 clean_html_for_llm-1.0.0/PKG-INFO
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:38:44.576884 clean_html_for_llm-1.0.0/clean_html_for_llm/
--rw-r--r--   0 shubhamraj   (502) staff       (20)      103 2024-04-10 07:37:34.000000 clean_html_for_llm-1.0.0/clean_html_for_llm/__init__.py
--rw-r--r--   0 shubhamraj   (502) staff       (20)      501 2024-04-10 07:37:18.000000 clean_html_for_llm-1.0.0/clean_html_for_llm/clean_html.py
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:38:44.577491 clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/
--rw-r--r--   0 shubhamraj   (502) staff       (20)      718 2024-04-10 07:38:44.000000 clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/PKG-INFO
--rw-r--r--   0 shubhamraj   (502) staff       (20)      248 2024-04-10 07:38:44.000000 clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/SOURCES.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)        1 2024-04-10 07:38:44.000000 clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/dependency_links.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)       19 2024-04-10 07:38:44.000000 clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/top_level.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)       38 2024-04-10 07:38:44.577859 clean_html_for_llm-1.0.0/setup.cfg
--rw-r--r--   0 shubhamraj   (502) staff       (20)      886 2024-04-10 07:36:58.000000 clean_html_for_llm-1.0.0/setup.py
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:52:55.337303 clean_html_for_llm-1.0.1/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     1073 2024-04-10 07:24:00.000000 clean_html_for_llm-1.0.1/LICENSE
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      718 2024-04-10 07:52:55.337187 clean_html_for_llm-1.0.1/PKG-INFO
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:52:55.336460 clean_html_for_llm-1.0.1/clean_html_for_llm/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       77 2024-04-10 07:52:00.000000 clean_html_for_llm-1.0.1/clean_html_for_llm/__init__.py
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      501 2024-04-10 07:37:18.000000 clean_html_for_llm-1.0.1/clean_html_for_llm/clean_html_for_llm.py
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 07:52:55.337037 clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      718 2024-04-10 07:52:55.000000 clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/PKG-INFO
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      256 2024-04-10 07:52:55.000000 clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)        1 2024-04-10 07:52:55.000000 clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       19 2024-04-10 07:52:55.000000 clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/top_level.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       38 2024-04-10 07:52:55.337341 clean_html_for_llm-1.0.1/setup.cfg
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      886 2024-04-10 07:52:49.000000 clean_html_for_llm-1.0.1/setup.py
```

### Comparing `clean_html_for_llm-1.0.0/LICENSE` & `clean_html_for_llm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_html_for_llm-1.0.0/PKG-INFO` & `clean_html_for_llm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean_html_for_llm
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html
 Author: Your Name
 Author-email: your.email@example.com
 License: MIT
 Keywords: html cleaning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clean_html_for_llm-1.0.0/clean_html_for_llm.egg-info/PKG-INFO` & `clean_html_for_llm-1.0.1/clean_html_for_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-html-for-llm
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html
 Author: Your Name
 Author-email: your.email@example.com
 License: MIT
 Keywords: html cleaning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clean_html_for_llm-1.0.0/setup.py` & `clean_html_for_llm-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clean_html_for_llm',
-    version='1.0.0',
+    version='1.0.1',
     description='A library for cleaning HTML content by removing specified tags and attributes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/clean_html',
     author='Your Name',
     author_email='your.email@example.com',
     license='MIT',
```

