# Comparing `tmp/jemma-0.1.1286.tar.gz` & `tmp/jemma-0.1.1287.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1286.tar", last modified: Wed Apr 10 01:15:11 2024, max compression
+gzip compressed data, was "jemma-0.1.1287.tar", last modified: Wed Apr 10 01:18:37 2024, max compression
```

## Comparing `jemma-0.1.1286.tar` & `jemma-0.1.1287.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.391343 jemma-0.1.1286/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:15:11.390709 jemma-0.1.1286/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1286/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.369434 jemma-0.1.1286/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1286/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.374882 jemma-0.1.1286/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1286/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.376236 jemma-0.1.1286/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1286/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1286/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.379060 jemma-0.1.1286/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1286/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1286/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1286/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.380673 jemma-0.1.1286/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1286/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1286/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.382460 jemma-0.1.1286/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1286/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1286/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.387778 jemma-0.1.1286/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1286/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1286/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4895 2024-04-10 01:12:33.000000 jemma-0.1.1286/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1286/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1286/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1286/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1286/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.389536 jemma-0.1.1286/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1286/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1286/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.374092 jemma-0.1.1286/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:15:11.391528 jemma-0.1.1286/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:14:35.000000 jemma-0.1.1286/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.827574 jemma-0.1.1287/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:18:37.826770 jemma-0.1.1287/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1287/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.783325 jemma-0.1.1287/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1287/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.789003 jemma-0.1.1287/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1287/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.790460 jemma-0.1.1287/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1287/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1287/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.794564 jemma-0.1.1287/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1287/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1287/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1287/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.797407 jemma-0.1.1287/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1287/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1287/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.800155 jemma-0.1.1287/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1287/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1287/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.821176 jemma-0.1.1287/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1287/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1287/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.1287/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1287/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1287/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5392 2024-04-10 01:18:25.000000 jemma-0.1.1287/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1287/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.824981 jemma-0.1.1287/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1287/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1287/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:18:37.788114 jemma-0.1.1287/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:18:37.000000 jemma-0.1.1287/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:18:37.827788 jemma-0.1.1287/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:18:33.000000 jemma-0.1.1287/setup.py
```

### Comparing `jemma-0.1.1286/README.md` & `jemma-0.1.1287/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/prompt/business/owner.py` & `jemma-0.1.1287/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/prompt/engineer/clarify.py` & `jemma-0.1.1287/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/prompt/engineer/code.py` & `jemma-0.1.1287/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/prompt/tester/test.py` & `jemma-0.1.1287/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/requirements/feature.py` & `jemma-0.1.1287/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/team/business_owner.py` & `jemma-0.1.1287/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/team/engineer.py` & `jemma-0.1.1287/jemma/team/engineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
         self.implementation_approach = implementation_approach
 
     def create_prototype(self, thinker, requirements):
         say("Engineer", f"💫 creating a prototype based on the requirements...", message_color=color.DARKCYAN)
 
         css = thinker.think(code.create_css_file(requirements),
                             "Engineer",
-                            # mute=True,
+                            mute=True,
                             action="crafting css 🎨 (a.k.a. \"visual beauty\")")
 
         js = thinker.think(code.create_javascript_file(requirements, css),
                            "Engineer",
-                           # mute=True,
-                            action="cooking javascript 🎮 (a.k.a. \"master of interactions\")")
+                           mute=True,
+                           action="cooking javascript 🎮 (a.k.a. \"master of interactions\")")
 
         html = thinker.think(code.create_html_file(requirements, css, js),
                              "Engineer",
-                             # mute=True,
+                             mute=True,
                              action="creating html 🕸️ (a.k.a. \"the skeleton of the web\")")
 
         return {"css": css, "js": js, "html": html}
 
     def record_prototype(self, path, prototype):
         # Create the directory if it doesn't exist
         os.makedirs(path, exist_ok=True)
```

### Comparing `jemma-0.1.1286/jemma/team/project_manager.py` & `jemma-0.1.1287/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/team/tester.py` & `jemma-0.1.1287/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/thinker.py` & `jemma-0.1.1287/jemma/thinker.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         super().__init__(model_name)
 
     def think(self, prompt, who="user", action="", mute=False, sleep_time=0):
         thinking = ollama.generate(model=self.model_name,
                                    prompt=prompt,
                                    options={'num_predict': 4096},
                                    stream=True)
-        if not mute:
+        if not mute and action != "":
             say(who, action)
 
         response = ""
         for word in thinking:
             response += word['response']
             if not mute:
                 print(word['response'], end="")
```

### Comparing `jemma-0.1.1286/jemma/tools.py` & `jemma-0.1.1287/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma/work/flow.py` & `jemma-0.1.1287/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1286/jemma.egg-info/SOURCES.txt` & `jemma-0.1.1287/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

