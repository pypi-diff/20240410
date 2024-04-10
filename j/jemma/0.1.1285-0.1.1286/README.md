# Comparing `tmp/jemma-0.1.1285.tar.gz` & `tmp/jemma-0.1.1286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1285.tar", last modified: Tue Apr  9 19:56:04 2024, max compression
+gzip compressed data, was "jemma-0.1.1286.tar", last modified: Wed Apr 10 01:15:11 2024, max compression
```

## Comparing `jemma-0.1.1285.tar` & `jemma-0.1.1286.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.761820 jemma-0.1.1285/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:56:04.761368 jemma-0.1.1285/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      751 2024-04-09 19:09:59.000000 jemma-0.1.1285/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.739819 jemma-0.1.1285/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1285/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.744412 jemma-0.1.1285/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1285/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.746129 jemma-0.1.1285/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1285/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1285/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.749571 jemma-0.1.1285/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1285/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1285/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1285/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.751201 jemma-0.1.1285/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1285/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1285/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.753334 jemma-0.1.1285/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1285/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1285/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.758638 jemma-0.1.1285/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1285/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1285/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4889 2024-04-09 05:43:59.000000 jemma-0.1.1285/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1285/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1285/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1285/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1285/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.760336 jemma-0.1.1285/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1285/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1285/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 19:56:04.743548 jemma-0.1.1285/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-09 19:56:04.000000 jemma-0.1.1285/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 19:56:04.761957 jemma-0.1.1285/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 19:56:00.000000 jemma-0.1.1285/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.391343 jemma-0.1.1286/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:15:11.390709 jemma-0.1.1286/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1286/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.369434 jemma-0.1.1286/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1286/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.374882 jemma-0.1.1286/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1286/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.376236 jemma-0.1.1286/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1286/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1286/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.379060 jemma-0.1.1286/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1286/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1286/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1286/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.380673 jemma-0.1.1286/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1286/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1286/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.382460 jemma-0.1.1286/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1286/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1286/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.387778 jemma-0.1.1286/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1286/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1286/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4895 2024-04-10 01:12:33.000000 jemma-0.1.1286/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1286/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1286/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5375 2024-04-09 05:55:25.000000 jemma-0.1.1286/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1286/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.389536 jemma-0.1.1286/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1286/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1286/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:15:11.374092 jemma-0.1.1286/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:15:11.000000 jemma-0.1.1286/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:15:11.391528 jemma-0.1.1286/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:14:35.000000 jemma-0.1.1286/setup.py
```

### Comparing `jemma-0.1.1285/README.md` & `jemma-0.1.1286/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# jemma
+# <img src="docs/jemma-thumb.png" width="10px"> jemma
 
-<img src="docs/jemma.gif" width="800">
+<img src="docs/jemma.gif" width="850">
 
 ```bash
 $ python huddle.py --requirements /home/me/big-idea.txt --build-prototype --ollama
 ```
 
 ```bash
 Ollama 🧠 gemma:7b-instruct-v1.1-fp16 ✅
```

### Comparing `jemma-0.1.1285/jemma/prompt/business/owner.py` & `jemma-0.1.1286/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/prompt/engineer/clarify.py` & `jemma-0.1.1286/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/prompt/engineer/code.py` & `jemma-0.1.1286/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/prompt/tester/test.py` & `jemma-0.1.1286/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/requirements/feature.py` & `jemma-0.1.1286/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/team/business_owner.py` & `jemma-0.1.1286/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/team/engineer.py` & `jemma-0.1.1286/jemma/team/engineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
         self.implementation_approach = implementation_approach
 
     def create_prototype(self, thinker, requirements):
         say("Engineer", f"💫 creating a prototype based on the requirements...", message_color=color.DARKCYAN)
 
         css = thinker.think(code.create_css_file(requirements),
                             "Engineer",
-                            mute=True,
+                            # mute=True,
                             action="crafting css 🎨 (a.k.a. \"visual beauty\")")
 
         js = thinker.think(code.create_javascript_file(requirements, css),
                            "Engineer",
-                           mute=True,
+                           # mute=True,
                             action="cooking javascript 🎮 (a.k.a. \"master of interactions\")")
 
         html = thinker.think(code.create_html_file(requirements, css, js),
                              "Engineer",
-                             mute=True,
+                             # mute=True,
                              action="creating html 🕸️ (a.k.a. \"the skeleton of the web\")")
 
         return {"css": css, "js": js, "html": html}
 
     def record_prototype(self, path, prototype):
         # Create the directory if it doesn't exist
         os.makedirs(path, exist_ok=True)
```

### Comparing `jemma-0.1.1285/jemma/team/project_manager.py` & `jemma-0.1.1286/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/team/tester.py` & `jemma-0.1.1286/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/thinker.py` & `jemma-0.1.1286/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/tools.py` & `jemma-0.1.1286/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma/work/flow.py` & `jemma-0.1.1286/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1285/jemma.egg-info/SOURCES.txt` & `jemma-0.1.1286/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

