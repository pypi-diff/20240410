# Comparing `tmp/simgui-1.5.0.tar.gz` & `tmp/simgui-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simgui-1.5.0.tar", last modified: Sun Mar 31 11:35:16 2024, max compression
+gzip compressed data, was "simgui-1.5.1.tar", last modified: Mon Apr  1 08:54:05 2024, max compression
```

## Comparing `simgui-1.5.0.tar` & `simgui-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-03-31 11:35:16.342642 simgui-1.5.0/
--rw-rw-r--   0 kent      (1000) kent      (1000)    35149 2022-03-11 08:18:45.000000 simgui-1.5.0/LICENSE
--rw-r--r--   0 kent      (1000) kent      (1000)     1960 2024-03-31 11:35:16.342642 simgui-1.5.0/PKG-INFO
--rw-rw-r--   0 kent      (1000) kent      (1000)     1330 2024-03-31 11:34:28.000000 simgui-1.5.0/README.md
--rw-rw-r--   0 kent      (1000) kent      (1000)      104 2022-03-11 08:18:45.000000 simgui-1.5.0/pyproject.toml
--rw-rw-r--   0 kent      (1000) kent      (1000)      762 2024-03-31 11:35:16.342642 simgui-1.5.0/setup.cfg
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-03-31 11:35:16.342642 simgui-1.5.0/src/
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-03-31 11:35:16.342642 simgui-1.5.0/src/simgui/
--rw-rw-r--   0 kent      (1000) kent      (1000)    19111 2024-03-31 11:34:28.000000 simgui-1.5.0/src/simgui/__init__.py
--rw-rw-r--   0 kent      (1000) kent      (1000)      113 2022-06-17 07:20:07.000000 simgui-1.5.0/src/simgui/mockaudio.py
--rw-rw-r--   0 kent      (1000) kent      (1000)     1342 2023-02-03 09:37:54.000000 simgui-1.5.0/src/simgui/transforms.py
-drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-03-31 11:35:16.342642 simgui-1.5.0/src/simgui.egg-info/
--rw-r--r--   0 kent      (1000) kent      (1000)     1960 2024-03-31 11:35:16.000000 simgui-1.5.0/src/simgui.egg-info/PKG-INFO
--rw-rw-r--   0 kent      (1000) kent      (1000)      283 2024-03-31 11:35:16.000000 simgui-1.5.0/src/simgui.egg-info/SOURCES.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)        1 2024-03-31 11:35:16.000000 simgui-1.5.0/src/simgui.egg-info/dependency_links.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)        8 2024-03-31 11:35:16.000000 simgui-1.5.0/src/simgui.egg-info/requires.txt
--rw-rw-r--   0 kent      (1000) kent      (1000)        7 2024-03-31 11:35:16.000000 simgui-1.5.0/src/simgui.egg-info/top_level.txt
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-04-01 08:54:05.274534 simgui-1.5.1/
+-rw-rw-r--   0 kent      (1000) kent      (1000)    35149 2022-03-11 08:18:45.000000 simgui-1.5.1/LICENSE
+-rw-r--r--   0 kent      (1000) kent      (1000)     1960 2024-04-01 08:54:05.274534 simgui-1.5.1/PKG-INFO
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1330 2024-03-31 11:34:28.000000 simgui-1.5.1/README.md
+-rw-rw-r--   0 kent      (1000) kent      (1000)      104 2022-03-11 08:18:45.000000 simgui-1.5.1/pyproject.toml
+-rw-rw-r--   0 kent      (1000) kent      (1000)      762 2024-04-01 08:54:05.274534 simgui-1.5.1/setup.cfg
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-04-01 08:54:05.270532 simgui-1.5.1/src/
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-04-01 08:54:05.274534 simgui-1.5.1/src/simgui/
+-rw-rw-r--   0 kent      (1000) kent      (1000)    19213 2024-04-01 08:52:55.000000 simgui-1.5.1/src/simgui/__init__.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)      113 2022-06-17 07:20:07.000000 simgui-1.5.1/src/simgui/mockaudio.py
+-rw-rw-r--   0 kent      (1000) kent      (1000)     1342 2023-02-03 09:37:54.000000 simgui-1.5.1/src/simgui/transforms.py
+drwxrwxr-x   0 kent      (1000) kent      (1000)        0 2024-04-01 08:54:05.274534 simgui-1.5.1/src/simgui.egg-info/
+-rw-r--r--   0 kent      (1000) kent      (1000)     1960 2024-04-01 08:54:05.000000 simgui-1.5.1/src/simgui.egg-info/PKG-INFO
+-rw-rw-r--   0 kent      (1000) kent      (1000)      283 2024-04-01 08:54:05.000000 simgui-1.5.1/src/simgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)        1 2024-04-01 08:54:05.000000 simgui-1.5.1/src/simgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)        8 2024-04-01 08:54:05.000000 simgui-1.5.1/src/simgui.egg-info/requires.txt
+-rw-rw-r--   0 kent      (1000) kent      (1000)        7 2024-04-01 08:54:05.000000 simgui-1.5.1/src/simgui.egg-info/top_level.txt
```

### Comparing `simgui-1.5.0/LICENSE` & `simgui-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simgui-1.5.0/PKG-INFO` & `simgui-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simgui
-Version: 1.5.0
+Version: 1.5.1
 Summary: A simple GUI API (wrapper around PySide6) for Python learners to build simple yet interesting event driven apps.
 Home-page: https://github.com/freemant2000/simgui
 Author: Kent Tong
 Author-email: kent.tong.mo@gmail.com
 Project-URL: Bug Tracker, https://github.com/freemant2000/simgui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simgui-1.5.0/README.md` & `simgui-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `simgui-1.5.0/setup.cfg` & `simgui-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simgui
-version = 1.5.0
+version = 1.5.1
 author = Kent Tong
 author_email = kent.tong.mo@gmail.com
 description = A simple GUI API (wrapper around PySide6) for Python learners to build simple yet interesting event driven apps.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/freemant2000/simgui
 project_urls =
```

### Comparing `simgui-1.5.0/src/simgui/__init__.py` & `simgui-1.5.1/src/simgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,21 +156,24 @@
       if ev.type()==QEvent.Type.User:
         self.call_handler("on_ready")  
       return super().event(ev)
     def make_opener(self):
       self.op=build_opener()
       self.op.addheaders=[("User-agent", "Mozilla/5.0 (X11; U; Linux i686) Gecko/20071127 Firefox/2.0.0.11")]
       self.op.cache={}
-    def call_handler(self, fn, data=None):
+    def call_handler(self, fn, data=None)->bool:
         handler=self.mod.get(fn)
         if handler:
           if data:
             handler(data)
           else:
             handler()
+          return True
+        else:
+          return False
     def add_label(self, name, text, **kwargs):
         lbl=QLabel(str(text))
         ww=WidgetWrapper(lbl, self)
         self.add_wid(name, ww, **kwargs)
         return ww
     def add_button(self, name, text, **kwargs):
         btn=QPushButton(str(text))
@@ -271,19 +274,20 @@
       evt=event.type()
       if evt==QEvent.KeyPress:
         self.key_ev=event
         self.call_handler("on_key")
       elif evt==QEvent.KeyRelease:
         self.key_ev=event
         self.call_handler("on_key_up")
-    def on_mouse(self, event):
+    def on_mouse(self, event: QEvent):
       evt=event.type()
       if evt==QEvent.MouseButtonPress:
         self.mouse_ev=event
-        self.call_handler("on_mouse")
+        if self.call_handler("on_mouse"):
+          event.accept()
     def add_graphics_view(self, min_w, min_h, scene_w=None, scene_h=None):
         if self.gs:
           raise ValueError("Only one graphics view can be added")
         self.gs=QGraphicsScene()
         self.gv=SimGraphicsView(self.gs, self.on_key, self.on_mouse)
         self.gv.setMinimumSize(min_w, min_h)
         if scene_w and scene_h:
```

### Comparing `simgui-1.5.0/src/simgui/transforms.py` & `simgui-1.5.1/src/simgui/transforms.py`

 * *Files identical despite different names*

### Comparing `simgui-1.5.0/src/simgui.egg-info/PKG-INFO` & `simgui-1.5.1/src/simgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simgui
-Version: 1.5.0
+Version: 1.5.1
 Summary: A simple GUI API (wrapper around PySide6) for Python learners to build simple yet interesting event driven apps.
 Home-page: https://github.com/freemant2000/simgui
 Author: Kent Tong
 Author-email: kent.tong.mo@gmail.com
 Project-URL: Bug Tracker, https://github.com/freemant2000/simgui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

