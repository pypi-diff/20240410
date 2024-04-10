# Comparing `tmp/superu-0.0.3.tar.gz` & `tmp/superu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superu-0.0.3.tar", last modified: Wed Apr 10 14:03:53 2024, max compression
+gzip compressed data, was "superu-0.0.4.tar", last modified: Wed Apr 10 14:10:57 2024, max compression
```

## Comparing `superu-0.0.3.tar` & `superu-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:03:53.883749 superu-0.0.3/
--rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:03:53.875971 superu-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-10 12:32:15.000000 superu-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 14:03:53.884405 superu-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1250 2024-04-10 14:03:46.000000 superu-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:03:53.824333 superu-0.0.3/superu/
--rw-rw-rw-   0        0        0      449 2024-04-10 14:03:13.000000 superu-0.0.3/superu/__init__.py
--rw-rw-rw-   0        0        0     1109 2024-04-10 11:54:09.000000 superu-0.0.3/superu/superU.py
--rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.3/superu/superU_Intent_Classification.py
--rw-rw-rw-   0        0        0     4210 2024-04-10 11:44:10.000000 superu-0.0.3/superu/superU_LLM_Analytics.py
--rw-rw-rw-   0        0        0     4402 2024-04-09 10:37:00.000000 superu-0.0.3/superu/superU_User_Persona.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:03:53.875971 superu-0.0.3/superu.egg-info/
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:03:53.000000 superu-0.0.3/superu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-10 14:03:53.000000 superu-0.0.3/superu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:03:53.000000 superu-0.0.3/superu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-10 14:03:53.000000 superu-0.0.3/superu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 14:03:53.000000 superu-0.0.3/superu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.482615 superu-0.0.4/
+-rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4165 2024-04-10 14:10:57.479363 superu-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-10 12:32:15.000000 superu-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:10:57.482615 superu-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2024-04-10 14:08:25.000000 superu-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.441940 superu-0.0.4/superu/
+-rw-rw-rw-   0        0        0      446 2024-04-10 14:10:26.000000 superu-0.0.4/superu/__init__.py
+-rw-rw-rw-   0        0        0     1109 2024-04-10 11:54:09.000000 superu-0.0.4/superu/superU.py
+-rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.4/superu/superU_Intent_Classification.py
+-rw-rw-rw-   0        0        0     4210 2024-04-10 11:44:10.000000 superu-0.0.4/superu/superU_LLM_Analytics.py
+-rw-rw-rw-   0        0        0     4402 2024-04-09 10:37:00.000000 superu-0.0.4/superu/superU_User_Persona.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.471140 superu-0.0.4/superu.egg-info/
+-rw-rw-rw-   0        0        0     4165 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/top_level.txt
```

### Comparing `superu-0.0.3/LICENSE` & `superu-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/PKG-INFO` & `superu-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `superu-0.0.3/README.md` & `superu-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/setup.py` & `superu-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A package that helps optimize your chatbot response'
 # LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="superu",
     version=VERSION,
```

### Comparing `superu-0.0.3/superu/superU.py` & `superu-0.0.4/superu/superU.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/superu/superU_Intent_Classification.py` & `superu-0.0.4/superu/superU_Intent_Classification.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/superu/superU_LLM_Analytics.py` & `superu-0.0.4/superu/superU_LLM_Analytics.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/superu/superU_User_Persona.py` & `superu-0.0.4/superu/superU_User_Persona.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.3/superu.egg-info/PKG-INFO` & `superu-0.0.4/superu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

