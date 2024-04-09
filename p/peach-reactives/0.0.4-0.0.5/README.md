# Comparing `tmp/peach-reactives-0.0.4.tar.gz` & `tmp/peach-reactives-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peach-reactives-0.0.4.tar", last modified: Mon Apr  1 08:26:22 2024, max compression
+gzip compressed data, was "peach-reactives-0.0.5.tar", last modified: Tue Apr  9 22:38:40 2024, max compression
```

## Comparing `peach-reactives-0.0.4.tar` & `peach-reactives-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-01 08:26:22.086689 peach-reactives-0.0.4/
--rw-rw-r--   0 jahall    (1001) jahall    (1001)      439 2024-03-29 09:32:37.000000 peach-reactives-0.0.4/LICENSE
--rw-r--r--   0 jahall    (1001) jahall    (1001)     6628 2024-04-01 08:26:22.086689 peach-reactives-0.0.4/PKG-INFO
--rw-rw-r--   0 jahall    (1001) jahall    (1001)     6370 2024-03-29 07:59:19.000000 peach-reactives-0.0.4/README.md
-drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-01 08:26:22.082689 peach-reactives-0.0.4/peach_reactives.egg-info/
--rw-r--r--   0 jahall    (1001) jahall    (1001)     6628 2024-04-01 08:26:22.000000 peach-reactives-0.0.4/peach_reactives.egg-info/PKG-INFO
--rw-rw-r--   0 jahall    (1001) jahall    (1001)      524 2024-04-01 08:26:22.000000 peach-reactives-0.0.4/peach_reactives.egg-info/SOURCES.txt
--rw-rw-r--   0 jahall    (1001) jahall    (1001)        1 2024-04-01 08:26:22.000000 peach-reactives-0.0.4/peach_reactives.egg-info/dependency_links.txt
--rw-rw-r--   0 jahall    (1001) jahall    (1001)       26 2024-04-01 08:26:22.000000 peach-reactives-0.0.4/peach_reactives.egg-info/top_level.txt
--rw-rw-r--   0 jahall    (1001) jahall    (1001)      366 2024-04-01 08:25:45.000000 peach-reactives-0.0.4/pyproject.toml
-drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-01 08:26:22.082689 peach-reactives-0.0.4/reactives/
--rw-rw-r--   0 jahall    (1001) jahall    (1001)       64 2024-03-29 09:28:26.000000 peach-reactives-0.0.4/reactives/__init__.py
--rw-rw-r--   0 jahall    (1001) jahall    (1001)     6664 2024-04-01 08:22:08.000000 peach-reactives-0.0.4/reactives/messenger.py
--rw-rw-r--   0 jahall    (1001) jahall    (1001)     4154 2024-03-29 09:43:00.000000 peach-reactives-0.0.4/reactives/reactive.py
--rw-rw-r--   0 jahall    (1001) jahall    (1001)       38 2024-04-01 08:26:22.086689 peach-reactives-0.0.4/setup.cfg
-drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-01 08:26:22.082689 peach-reactives-0.0.4/venv/
-drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-01 08:26:22.082689 peach-reactives-0.0.4/venv/bin/
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      629 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2html.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      751 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2html4.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)     1086 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2html5.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      828 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2latex.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      651 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2man.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      817 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2odt.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      623 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      636 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      672 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2s5.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      908 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2xetex.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      637 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rst2xml.py
--rwxrwxr-x   0 jahall    (1001) jahall    (1001)      705 2024-03-29 22:07:25.000000 peach-reactives-0.0.4/venv/bin/rstpep2html.py
+drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)      439 2024-03-29 09:32:37.000000 peach-reactives-0.0.5/LICENSE
+-rw-r--r--   0 jahall    (1001) jahall    (1001)     6628 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/PKG-INFO
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)     6370 2024-03-29 07:59:19.000000 peach-reactives-0.0.5/README.md
+drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/peach_reactives.egg-info/
+-rw-r--r--   0 jahall    (1001) jahall    (1001)     6628 2024-04-09 22:38:40.000000 peach-reactives-0.0.5/peach_reactives.egg-info/PKG-INFO
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)      524 2024-04-09 22:38:40.000000 peach-reactives-0.0.5/peach_reactives.egg-info/SOURCES.txt
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)        1 2024-04-09 22:38:40.000000 peach-reactives-0.0.5/peach_reactives.egg-info/dependency_links.txt
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)       26 2024-04-09 22:38:40.000000 peach-reactives-0.0.5/peach_reactives.egg-info/top_level.txt
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)      366 2024-04-09 22:36:45.000000 peach-reactives-0.0.5/pyproject.toml
+drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/reactives/
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)       64 2024-03-29 09:28:26.000000 peach-reactives-0.0.5/reactives/__init__.py
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)     7130 2024-04-09 22:31:11.000000 peach-reactives-0.0.5/reactives/messenger.py
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)     4154 2024-03-29 09:43:00.000000 peach-reactives-0.0.5/reactives/reactive.py
+-rw-rw-r--   0 jahall    (1001) jahall    (1001)       38 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/setup.cfg
+drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/venv/
+drwxrwxr-x   0 jahall    (1001) jahall    (1001)        0 2024-04-09 22:38:40.646648 peach-reactives-0.0.5/venv/bin/
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      629 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2html.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      751 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2html4.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)     1086 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2html5.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      828 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2latex.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      651 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2man.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      817 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2odt.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      623 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      636 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      672 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2s5.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      908 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      637 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rst2xml.py
+-rwxrwxr-x   0 jahall    (1001) jahall    (1001)      705 2024-03-29 22:07:25.000000 peach-reactives-0.0.5/venv/bin/rstpep2html.py
```

### Comparing `peach-reactives-0.0.4/PKG-INFO` & `peach-reactives-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peach-reactives
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Peach <james@christhall.us>
 Project-URL: Homepage, https://gitlab.com/peach_experiments/reactives
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Reactives
```

### Comparing `peach-reactives-0.0.4/README.md` & `peach-reactives-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/peach_reactives.egg-info/PKG-INFO` & `peach-reactives-0.0.5/peach_reactives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peach-reactives
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Peach <james@christhall.us>
 Project-URL: Homepage, https://gitlab.com/peach_experiments/reactives
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Reactives
```

### Comparing `peach-reactives-0.0.4/peach_reactives.egg-info/SOURCES.txt` & `peach-reactives-0.0.5/peach_reactives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/reactives/messenger.py` & `peach-reactives-0.0.5/reactives/messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import inspect
+import uuid
 from dataclasses import dataclass
 from queue import Queue
 
 
 @dataclass(frozen=True)
 class Message:
+    uuid: str
     sender: str
     receiver: str
     message: any
 
 
 class Messenger:
     class UnknownReactive(Exception):
@@ -35,15 +37,14 @@
 
         # Set flag to indicate already initialized
         self.init = True
 
         # Dict to hold reactive queue
         self.r_queues = {}
         self.r_queues['main'] = Queue()
-        self.r_queues['block'] = Queue()
 
         # Dict to hold subject subscribers
         self.r_subjects = {}
 
         # Dict to hold reactive start function
         self.r_start = {}
         # Dict to hold reactive stop function
@@ -111,45 +112,58 @@
         # Find sender of message
         try:
             sender = inspect.stack()[1][0].f_locals['self'].name
         except:
             # Default to 'main'
             sender = 'main'
 
+        # Generate uuid for messenger
+        m_uuid = str(uuid.uuid4())
+
         # Override sender if call is blocking
         if blocking:
-            sender = 'block'
+            # Create new queue for unique message
+            self.r_queues[m_uuid] = Queue()
+            sender = m_uuid
 
         # Check if receiver is direct message to reactive
         if receiver in self.r_queues.keys():
-            message = Message(sender,
+            message = Message(m_uuid,
+                              sender,
                               receiver,
                               msg)
             self.r_queues[receiver].put(message)
 
             # if blocking, wait for response
             if blocking:
-                return self.get(name='block',
-                                timeout=timeout)
+                retVal = self.get(name=m_uuid,
+                                  timeout=timeout)
+                # Delete unique message queue
+                del self.r_queues[m_uuid]
+                # Return message
+                return retVal
 
             return
 
         # Check if receiver is subscribed subject
         if receiver in self.r_subjects.keys():
             for r in self.r_subjects[receiver]:
                 message = Message(sender,
                                   r,
                                   msg)
                 self.r_queues[r].put(message)
 
-                # if blocking, wait for response
+                # if blocking, wait for responses
                 if blocking:
-                    retVal.append(self.get(name='block',
+                    retVal.append(self.get(name=m_uuid,
                                            timeout=timeout))
             if blocking:
+                # Delete unique message queue
+                del self.r_queues[m_uuid]
+                # Return messages
                 return retVal
 
             return
 
         # No Reactive or Subject found
         raise self.UnknownReceiver(f"{receiver} not registered")
```

### Comparing `peach-reactives-0.0.4/reactives/reactive.py` & `peach-reactives-0.0.5/reactives/reactive.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2html.py` & `peach-reactives-0.0.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2html4.py` & `peach-reactives-0.0.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2html5.py` & `peach-reactives-0.0.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2latex.py` & `peach-reactives-0.0.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2man.py` & `peach-reactives-0.0.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2odt.py` & `peach-reactives-0.0.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2odt_prepstyles.py` & `peach-reactives-0.0.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2pseudoxml.py` & `peach-reactives-0.0.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2s5.py` & `peach-reactives-0.0.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2xetex.py` & `peach-reactives-0.0.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rst2xml.py` & `peach-reactives-0.0.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `peach-reactives-0.0.4/venv/bin/rstpep2html.py` & `peach-reactives-0.0.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

