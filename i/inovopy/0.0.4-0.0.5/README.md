# Comparing `tmp/inovopy-0.0.4.tar.gz` & `tmp/inovopy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inovopy-0.0.4.tar", last modified: Tue Apr  9 05:29:37 2024, max compression
+gzip compressed data, was "inovopy-0.0.5.tar", last modified: Wed Apr 10 03:07:26 2024, max compression
```

## Comparing `inovopy-0.0.4.tar` & `inovopy-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 05:29:37.259289 inovopy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 05:29:20.000000 inovopy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.255289 inovopy-0.0.4/inovopy/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.255289 inovopy-0.0.4/inovopy/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/geometry/jointcoord.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/geometry/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/inovopy/iva/
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/iva/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/inovopy/logger/
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/inovopy/robot/
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/robridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/inovopy/socket/
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/socket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/socket/tcp_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/socket/tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/socket/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 05:29:20.000000 inovopy-0.0.4/inovopy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:37.259289 inovopy-0.0.4/inovopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 05:29:37.000000 inovopy-0.0.4/inovopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 05:29:37.000000 inovopy-0.0.4/inovopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:29:37.000000 inovopy-0.0.4/inovopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:29:37.000000 inovopy-0.0.4/inovopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 05:29:37.000000 inovopy-0.0.4/inovopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:29:37.259289 inovopy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 05:29:20.000000 inovopy-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 03:07:26.411643 inovopy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 03:07:02.000000 inovopy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.407643 inovopy-0.0.5/inovopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/geometry/jointcoord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/geometry/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy/iva/
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/iva/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy/robot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/robridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/socket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/socket/tcp_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/socket/tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/socket/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 03:07:02.000000 inovopy-0.0.5/inovopy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:07:26.411643 inovopy-0.0.5/inovopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 03:07:26.000000 inovopy-0.0.5/inovopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 03:07:26.000000 inovopy-0.0.5/inovopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:07:26.000000 inovopy-0.0.5/inovopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:07:26.000000 inovopy-0.0.5/inovopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 03:07:26.000000 inovopy-0.0.5/inovopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:07:26.411643 inovopy-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-10 03:07:02.000000 inovopy-0.0.5/setup.py
```

### Comparing `inovopy-0.0.4/PKG-INFO` & `inovopy-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: inovopy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Inovo Robot Arm API
 Author: Alan Chung
 Author-email: deeralan827@gmail.com
 Keywords: python,robotics,inovo robotics,inovo robot arm,motion,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: websockets
-Requires-Dist: asyncio
-Requires-Dist: nest-asyncio
 
 
 A package that provide a simple python socket based api for controlling inovo robot arms.
```

### Comparing `inovopy-0.0.4/inovopy/geometry/__init__.py` & `inovopy-0.0.5/inovopy/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/geometry/jointcoord.py` & `inovopy-0.0.5/inovopy/geometry/jointcoord.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/geometry/transform.py` & `inovopy-0.0.5/inovopy/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/iva/__init__.py` & `inovopy-0.0.5/inovopy/iva/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/logger/__init__.py` & `inovopy-0.0.5/inovopy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/robot/__init__.py` & `inovopy-0.0.5/inovopy/robot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,36 +256,40 @@
         ## Parameter
         - `port: int`: output port to set, default `0-7`
         - `state: bool`: target state of the output
         """
         res = self.io(IOCommand.set_digital(target="wrist", port=port, state=state))
         assert res == "OK"
 
+    def gripper(self, gripper_command: GripperCommand):
+        self.write(gripper(gripper_command))
+
     def gipper_activate(self):
         """activate the gripper"""
-        self.write(GripperCommand.activate())
+        self.gripper(GripperCommand.activate())
         self.assert_res_ok()
     def gripper_get(self)->float:
         """
         get the gripper width
         
         ## Return
         `float` in percentage
         """
-        self.write(GripperCommand.get())
+        self.gripper(GripperCommand.get())
         return float(self.read()) * 100
+    
     def gripper_set(self, label: str):
         """
         set a gripper to a predefine label
         
 
         #Parameter
         - `label: str`: the label to set to 
         """
-        self.write(GripperCommand.set(label=label))
+        self.gripper(GripperCommand.set(label=label))
         self.assert_res_ok()
 
     def get_current_transform(self) -> Transform:
         """
         get the current transform
 
         ## Return:
```

### Comparing `inovopy-0.0.4/inovopy/robridge.py` & `inovopy-0.0.5/inovopy/robridge.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/socket/__init__.py` & `inovopy-0.0.5/inovopy/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/socket/tcp_listener.py` & `inovopy-0.0.5/inovopy/socket/tcp_listener.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/socket/tcp_stream.py` & `inovopy-0.0.5/inovopy/socket/tcp_stream.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/socket/utils.py` & `inovopy-0.0.5/inovopy/socket/utils.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy/utils.py` & `inovopy-0.0.5/inovopy/utils.py`

 * *Files identical despite different names*

### Comparing `inovopy-0.0.4/inovopy.egg-info/PKG-INFO` & `inovopy-0.0.5/inovopy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: inovopy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Inovo Robot Arm API
 Author: Alan Chung
 Author-email: deeralan827@gmail.com
 Keywords: python,robotics,inovo robotics,inovo robot arm,motion,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: websockets
-Requires-Dist: asyncio
-Requires-Dist: nest-asyncio
 
 
 A package that provide a simple python socket based api for controlling inovo robot arms.
```

### Comparing `inovopy-0.0.4/setup.py` & `inovopy-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 setup script for inovopy
 """
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Inovo Robot Arm API'
 LONG_DESCRIPTION = \
 """
 A package that provide a simple python socket based api for controlling inovo robot arms.
 """
 
 # Setting up
```

