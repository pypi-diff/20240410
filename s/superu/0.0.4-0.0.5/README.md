# Comparing `tmp/superu-0.0.4.tar.gz` & `tmp/superu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superu-0.0.4.tar", last modified: Wed Apr 10 14:10:57 2024, max compression
+gzip compressed data, was "superu-0.0.5.tar", last modified: Wed Apr 10 14:14:43 2024, max compression
```

## Comparing `superu-0.0.4.tar` & `superu-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.482615 superu-0.0.4/
--rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:10:57.479363 superu-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-10 12:32:15.000000 superu-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 14:10:57.482615 superu-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1250 2024-04-10 14:08:25.000000 superu-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.441940 superu-0.0.4/superu/
--rw-rw-rw-   0        0        0      446 2024-04-10 14:10:26.000000 superu-0.0.4/superu/__init__.py
--rw-rw-rw-   0        0        0     1109 2024-04-10 11:54:09.000000 superu-0.0.4/superu/superU.py
--rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.4/superu/superU_Intent_Classification.py
--rw-rw-rw-   0        0        0     4210 2024-04-10 11:44:10.000000 superu-0.0.4/superu/superU_LLM_Analytics.py
--rw-rw-rw-   0        0        0     4402 2024-04-09 10:37:00.000000 superu-0.0.4/superu/superU_User_Persona.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:10:57.471140 superu-0.0.4/superu.egg-info/
--rw-rw-rw-   0        0        0     4165 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 14:10:57.000000 superu-0.0.4/superu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 14:14:43.943439 superu-0.0.5/
+-rw-rw-rw-   0        0        0     1084 2024-04-09 12:12:26.000000 superu-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4165 2024-04-10 14:14:43.943439 superu-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-10 12:32:15.000000 superu-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:14:43.943439 superu-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2024-04-10 14:14:36.000000 superu-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:14:43.887796 superu-0.0.5/superu/
+-rw-rw-rw-   0        0        0      425 2024-04-10 14:14:13.000000 superu-0.0.5/superu/__init__.py
+-rw-rw-rw-   0        0        0     1030 2024-04-09 11:04:22.000000 superu-0.0.5/superu/datetime_util.py
+-rw-rw-rw-   0        0        0     1299 2024-04-06 10:19:57.000000 superu-0.0.5/superu/download_models.py
+-rw-rw-rw-   0        0        0     1926 2024-04-10 14:13:00.000000 superu-0.0.5/superu/serializer.py
+-rw-rw-rw-   0        0        0     1103 2024-04-10 14:13:21.000000 superu-0.0.5/superu/superU.py
+-rw-rw-rw-   0        0        0     2253 2024-04-10 14:13:27.000000 superu-0.0.5/superu/superUClient.py
+-rw-rw-rw-   0        0        0     3061 2024-04-06 07:39:35.000000 superu-0.0.5/superu/superU_Intent_Classification.py
+-rw-rw-rw-   0        0        0     4204 2024-04-10 14:13:09.000000 superu-0.0.5/superu/superU_LLM_Analytics.py
+-rw-rw-rw-   0        0        0     4402 2024-04-09 10:37:00.000000 superu-0.0.5/superu/superU_User_Persona.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:14:43.934321 superu-0.0.5/superu.egg-info/
+-rw-rw-rw-   0        0        0     4165 2024-04-10 14:14:43.000000 superu-0.0.5/superu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-10 14:14:43.000000 superu-0.0.5/superu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:14:43.000000 superu-0.0.5/superu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-10 14:14:43.000000 superu-0.0.5/superu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 14:14:43.000000 superu-0.0.5/superu.egg-info/top_level.txt
```

### Comparing `superu-0.0.4/LICENSE` & `superu-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `superu-0.0.4/PKG-INFO` & `superu-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `superu-0.0.4/README.md` & `superu-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `superu-0.0.4/setup.py` & `superu-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A package that helps optimize your chatbot response'
 # LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="superu",
     version=VERSION,
```

### Comparing `superu-0.0.4/superu/superU.py` & `superu-0.0.5/superu/superU.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from utils.download_models import FileDownloader
+from download_models import FileDownloader
 from superU_User_Persona import User_Persona
 from superU_Intent_Classification import Intent_Classifier
 from superU_LLM_Analytics import llm_analytics
 
 class Build_User_Persona:
     def __init__(self, openai, llm_deploymentname):
         self.user_persona = User_Persona(openai, llm_deploymentname)
```

### Comparing `superu-0.0.4/superu/superU_Intent_Classification.py` & `superu-0.0.5/superu/superU_Intent_Classification.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.4/superu/superU_LLM_Analytics.py` & `superu-0.0.5/superu/superU_LLM_Analytics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import httpx
 import uuid
 import datetime
-from utils.superUClient import SuperUClient
+from superUClient import SuperUClient
 
 class llm_analytics:
 
     def __init__(self, public_key: str, secret_key: str , version: str = "latest", timeout: int = 10):
         self.public_key = public_key
         self.secret_key = secret_key
         self.host = "https://analytics.superu.ai"
```

### Comparing `superu-0.0.4/superu/superU_User_Persona.py` & `superu-0.0.5/superu/superU_User_Persona.py`

 * *Files identical despite different names*

### Comparing `superu-0.0.4/superu.egg-info/PKG-INFO` & `superu-0.0.5/superu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superu
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that helps optimize your chatbot response
 Author: SuperU
 Author-email: <adi@superu.ai>
 Keywords: python,chatbot,ecommerce,tag generation,semantic search,openai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

