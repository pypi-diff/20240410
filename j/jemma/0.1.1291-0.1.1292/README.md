# Comparing `tmp/jemma-0.1.1291.tar.gz` & `tmp/jemma-0.1.1292.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1291.tar", last modified: Wed Apr 10 01:42:22 2024, max compression
+gzip compressed data, was "jemma-0.1.1292.tar", last modified: Wed Apr 10 01:45:42 2024, max compression
```

## Comparing `jemma-0.1.1291.tar` & `jemma-0.1.1292.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.971976 jemma-0.1.1291/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:42:22.971554 jemma-0.1.1291/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1291/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.954894 jemma-0.1.1291/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1291/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.959994 jemma-0.1.1291/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1291/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.961087 jemma-0.1.1291/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1291/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1291/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.963050 jemma-0.1.1291/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1291/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1291/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1291/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.964319 jemma-0.1.1291/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1291/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1291/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.965736 jemma-0.1.1291/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1291/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1291/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.969403 jemma-0.1.1291/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1291/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1291/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.1291/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1291/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1291/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5391 2024-04-10 01:42:03.000000 jemma-0.1.1291/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1291/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.970821 jemma-0.1.1291/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1291/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1291/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:42:22.959345 jemma-0.1.1291/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:42:22.000000 jemma-0.1.1291/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:42:22.972143 jemma-0.1.1291/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:42:19.000000 jemma-0.1.1291/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.886420 jemma-0.1.1292/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:45:42.886040 jemma-0.1.1292/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1292/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.870072 jemma-0.1.1292/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1292/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.874730 jemma-0.1.1292/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1292/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.876198 jemma-0.1.1292/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1292/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1292/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.878277 jemma-0.1.1292/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1292/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1292/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1292/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.879765 jemma-0.1.1292/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1292/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1292/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.881099 jemma-0.1.1292/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1292/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1292/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.884247 jemma-0.1.1292/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1292/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1292/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.1292/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1292/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1292/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 01:45:32.000000 jemma-0.1.1292/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1292/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.885452 jemma-0.1.1292/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1292/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1292/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.873613 jemma-0.1.1292/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:45:42.886536 jemma-0.1.1292/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:45:39.000000 jemma-0.1.1292/setup.py
```

### Comparing `jemma-0.1.1291/README.md` & `jemma-0.1.1292/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/prompt/business/owner.py` & `jemma-0.1.1292/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/prompt/engineer/clarify.py` & `jemma-0.1.1292/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/prompt/engineer/code.py` & `jemma-0.1.1292/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/prompt/tester/test.py` & `jemma-0.1.1292/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/requirements/feature.py` & `jemma-0.1.1292/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/team/business_owner.py` & `jemma-0.1.1292/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/team/engineer.py` & `jemma-0.1.1292/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/team/project_manager.py` & `jemma-0.1.1292/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/team/tester.py` & `jemma-0.1.1292/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/thinker.py` & `jemma-0.1.1292/jemma/thinker.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 class Replicate(Thinker):
 
     def __init__(self, model_name):
         super().__init__(model_name)
 
     def think(self, prompt, who="user", action="", mute=False, sleep_time=0):
 
-        if not mute:
+        if action != "" or not mute:
             say(who, action)
 
         response = ""
         for event in replicate.stream(
             self.model_name,
             input={
                 "prompt": prompt,
@@ -73,15 +73,15 @@
 
         ## make sure ANTHROPIC_API_KEY is exported in shell
         ## or it is exported in a .env file
         self.client = client = Anthropic()
 
     def think(self, prompt, who="user", action="", mute=False, sleep_time=1): # sleep not to exceed the rate limit
 
-        if not mute:
+        if action != "" or not mute:
             say(who, action)
 
         time.sleep(sleep_time)
 
         response = ""
         with self.client.messages.stream(max_tokens=4096,
                                          messages=[{"role": "user",
@@ -104,15 +104,15 @@
 
         ## make sure OPENAI_API_KEY is exported in shell
         ## or it is exported in a .env file
         self.client = client = OpenAI()
 
     def think(self, prompt, who="user", action="", mute=False, sleep_time=2): # sleep not to exceed the rate limit
 
-        if not mute:
+        if action != "" or not mute:
             say(who, action)
 
         time.sleep(sleep_time)
 
         response = ""
         stream = self.client.chat.completions.create(
             model=self.model_name,
```

### Comparing `jemma-0.1.1291/jemma/tools.py` & `jemma-0.1.1292/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma/work/flow.py` & `jemma-0.1.1292/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1291/jemma.egg-info/SOURCES.txt` & `jemma-0.1.1292/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

