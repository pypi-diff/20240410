# Comparing `tmp/clean_html_for_llm-1.2.0.tar.gz` & `tmp/clean_html_for_llm-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_html_for_llm-1.2.0.tar", last modified: Wed Apr 10 08:10:05 2024, max compression
+gzip compressed data, was "clean_html_for_llm-1.3.0.tar", last modified: Wed Apr 10 08:21:22 2024, max compression
```

## Comparing `clean_html_for_llm-1.2.0.tar` & `clean_html_for_llm-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:10:05.264615 clean_html_for_llm-1.2.0/
--rw-r--r--   0 shubhamraj   (502) staff       (20)     1073 2024-04-10 07:24:00.000000 clean_html_for_llm-1.2.0/LICENSE
--rw-r--r--   0 shubhamraj   (502) staff       (20)     2951 2024-04-10 08:10:05.264501 clean_html_for_llm-1.2.0/PKG-INFO
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:10:05.263648 clean_html_for_llm-1.2.0/clean_html_for_llm/
--rw-r--r--   0 shubhamraj   (502) staff       (20)       69 2024-04-10 07:57:46.000000 clean_html_for_llm-1.2.0/clean_html_for_llm/__init__.py
--rw-r--r--   0 shubhamraj   (502) staff       (20)     1228 2024-04-10 07:59:03.000000 clean_html_for_llm-1.2.0/clean_html_for_llm/clean_html_for_llm.py
-drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:10:05.264297 clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/
--rw-r--r--   0 shubhamraj   (502) staff       (20)     2951 2024-04-10 08:10:05.000000 clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/PKG-INFO
--rw-r--r--   0 shubhamraj   (502) staff       (20)      256 2024-04-10 08:10:05.000000 clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/SOURCES.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)        1 2024-04-10 08:10:05.000000 clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/dependency_links.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)       19 2024-04-10 08:10:05.000000 clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/top_level.txt
--rw-r--r--   0 shubhamraj   (502) staff       (20)       38 2024-04-10 08:10:05.264674 clean_html_for_llm-1.2.0/setup.cfg
--rw-r--r--   0 shubhamraj   (502) staff       (20)     1125 2024-04-10 08:10:02.000000 clean_html_for_llm-1.2.0/setup.py
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:21:22.040029 clean_html_for_llm-1.3.0/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     1073 2024-04-10 07:24:00.000000 clean_html_for_llm-1.3.0/LICENSE
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     2951 2024-04-10 08:21:22.039898 clean_html_for_llm-1.3.0/PKG-INFO
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:21:22.039066 clean_html_for_llm-1.3.0/clean_html_for_llm/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       69 2024-04-10 07:57:46.000000 clean_html_for_llm-1.3.0/clean_html_for_llm/__init__.py
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     1228 2024-04-10 07:59:03.000000 clean_html_for_llm-1.3.0/clean_html_for_llm/clean_html_for_llm.py
+drwxr-xr-x   0 shubhamraj   (502) staff       (20)        0 2024-04-10 08:21:22.039686 clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     2951 2024-04-10 08:21:22.000000 clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/PKG-INFO
+-rw-r--r--   0 shubhamraj   (502) staff       (20)      256 2024-04-10 08:21:22.000000 clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)        1 2024-04-10 08:21:22.000000 clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       19 2024-04-10 08:21:22.000000 clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/top_level.txt
+-rw-r--r--   0 shubhamraj   (502) staff       (20)       38 2024-04-10 08:21:22.040067 clean_html_for_llm-1.3.0/setup.cfg
+-rw-r--r--   0 shubhamraj   (502) staff       (20)     1125 2024-04-10 08:21:21.000000 clean_html_for_llm-1.3.0/setup.py
```

### Comparing `clean_html_for_llm-1.2.0/LICENSE` & `clean_html_for_llm-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_html_for_llm-1.2.0/PKG-INFO` & `clean_html_for_llm-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean_html_for_llm
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html
 Author: Shubham Raj
 Author-email: sraj13169@gmail.com
 License: MIT
 Keywords: html cleaning,html cleaning for llm,html denoise for llm,html denoising for llm,html cleaning for language model,html denoise for language model,html denoising for language model,html cleaning for nlp,html denoise for nlp,html denoising for nlp
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clean_html_for_llm Version: 1.2.0 Summary: A
+Metadata-Version: 2.1 Name: clean_html_for_llm Version: 1.3.0 Summary: A
 library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html Author: Shubham Raj
 Author-email: sraj13169@gmail.com License: MIT Keywords: html cleaning,html
 cleaning for llm,html denoise for llm,html denoising for llm,html cleaning for
 language model,html denoise for language model,html denoising for language
 model,html cleaning for nlp,html denoise for nlp,html denoising for nlp
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `clean_html_for_llm-1.2.0/clean_html_for_llm/clean_html_for_llm.py` & `clean_html_for_llm-1.3.0/clean_html_for_llm/clean_html_for_llm.py`

 * *Files identical despite different names*

### Comparing `clean_html_for_llm-1.2.0/clean_html_for_llm.egg-info/PKG-INFO` & `clean_html_for_llm-1.3.0/clean_html_for_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-html-for-llm
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html
 Author: Shubham Raj
 Author-email: sraj13169@gmail.com
 License: MIT
 Keywords: html cleaning,html cleaning for llm,html denoise for llm,html denoising for llm,html cleaning for language model,html denoise for language model,html denoising for language model,html cleaning for nlp,html denoise for nlp,html denoising for nlp
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clean-html-for-llm Version: 1.2.0 Summary: A
+Metadata-Version: 2.1 Name: clean-html-for-llm Version: 1.3.0 Summary: A
 library for cleaning HTML content by removing specified tags and attributes.
 Home-page: https://github.com/yourusername/clean_html Author: Shubham Raj
 Author-email: sraj13169@gmail.com License: MIT Keywords: html cleaning,html
 cleaning for llm,html denoise for llm,html denoising for llm,html cleaning for
 language model,html denoise for language model,html denoising for language
 model,html cleaning for nlp,html denoise for nlp,html denoising for nlp
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
```

### Comparing `clean_html_for_llm-1.2.0/setup.py` & `clean_html_for_llm-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clean_html_for_llm',
-    version='1.2.0',
+    version='1.3.0',
     description='A library for cleaning HTML content by removing specified tags and attributes.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/clean_html',
     author='Shubham Raj',
     author_email='sraj13169@gmail.com',
     license='MIT',
```

