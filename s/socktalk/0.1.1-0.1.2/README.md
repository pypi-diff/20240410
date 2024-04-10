# Comparing `tmp/socktalk-0.1.1.tar.gz` & `tmp/socktalk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.1.tar", last modified: Wed Apr 10 10:53:06 2024, max compression
+gzip compressed data, was "socktalk-0.1.2.tar", last modified: Wed Apr 10 11:03:52 2024, max compression
```

## Comparing `socktalk-0.1.1.tar` & `socktalk-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.1/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     3721 2024-04-10 10:53:06.627013 socktalk-0.1.1/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3288 2024-04-10 09:26:06.000000 socktalk-0.1.1/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.1/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5408 2024-04-09 11:09:29.000000 socktalk-0.1.1/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.1/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.1/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     2527 2024-04-10 09:05:25.000000 socktalk-0.1.1/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-10 10:53:06.627013 socktalk-0.1.1/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)      922 2024-04-10 10:52:38.000000 socktalk-0.1.1/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 10:53:06.627013 socktalk-0.1.1/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     3721 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-10 10:53:06.000000 socktalk-0.1.1/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:03:52.295901 socktalk-0.1.2/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.2/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     3741 2024-04-10 11:03:52.295901 socktalk-0.1.2/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3308 2024-04-10 11:01:29.000000 socktalk-0.1.2/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:03:52.295901 socktalk-0.1.2/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.2/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5408 2024-04-09 11:09:29.000000 socktalk-0.1.2/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.2/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.2/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2527 2024-04-10 09:05:25.000000 socktalk-0.1.2/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-10 11:03:52.295901 socktalk-0.1.2/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)      922 2024-04-10 11:03:07.000000 socktalk-0.1.2/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-10 11:03:52.295901 socktalk-0.1.2/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     3741 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-10 11:03:52.000000 socktalk-0.1.2/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.1/LICENSE` & `socktalk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.1/PKG-INFO` & `socktalk-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Socket-based AI chat server and multi-user chat client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Requires-Dist: openai==1.14.2
 
 # Chat Server
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
-If running the code using the python library "chat_server":
+If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
 1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
```

### Comparing `socktalk-0.1.1/README.md` & `socktalk-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Chat Server
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
-If running the code using the python library "chat_server":
+If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
 1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
```

### Comparing `socktalk-0.1.1/server_client/ai_client.py` & `socktalk-0.1.2/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.1/server_client/client.py` & `socktalk-0.1.2/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.1/server_client/server.py` & `socktalk-0.1.2/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.1/server_client/start_server_with_ai_client.py` & `socktalk-0.1.2/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.1/setup.py` & `socktalk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'PyQt5==5.15.10',
         'openai==1.14.2'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `socktalk-0.1.1/socktalk.egg-info/PKG-INFO` & `socktalk-0.1.2/socktalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Socket-based AI chat server and multi-user chat client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 Requires-Dist: openai==1.14.2
 
 # Chat Server
 
 If running the code from the github repository:
 Please install the requirements into a virtual environment, then launch "start_server_with_ai_client.py" after adjusting the settings (send full chat history, ai client api key, enabling ai mode 1 or ai mode 2, editing mode1 or mode2 intervals), then launch "client.py" (can be launched multiple times, for multiple users)
 
-If running the code using the python library "chat_server":
+If running the code using the python library "socktalk" (pip install socktalk):
 You can use the following terminal commands:
 1) "ai_server": Runs the chat server with a connected AI client. Currently uses gpt-3.5-turbo model.
     You should create an environment file named ".env" in the working directory from which you execute the python
     commands for the library, in order to adjust the AI modes and chat server settings.
 
     Below is an example for your .env file. You will need to update the OpenAI chatgpt API key. In order for the API key to function you will need to load at least 5$ of credit on your OpenAI account.
     The AI client has two modes which can be toggled on or off using "True" or "False". AI response intervals can be adjusted. See below for more details.
```

