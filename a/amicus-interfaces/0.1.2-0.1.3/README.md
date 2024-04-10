# Comparing `tmp/amicus_interfaces-0.1.2.tar.gz` & `tmp/amicus_interfaces-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amicus_interfaces-0.1.2.tar", last modified: Wed Feb 14 11:22:12 2024, max compression
+gzip compressed data, was "amicus_interfaces-0.1.3.tar", last modified: Wed Apr 10 08:33:58 2024, max compression
```

## Comparing `amicus_interfaces-0.1.2.tar` & `amicus_interfaces-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-02-14 11:22:12.949671 amicus_interfaces-0.1.2/
--rw-r--r--   0 mauceric   (501) staff       (20)      351 2024-02-14 11:22:12.947675 amicus_interfaces-0.1.2/PKG-INFO
--rw-r--r--   0 mauceric   (501) staff       (20)      325 2024-02-10 14:49:17.000000 amicus_interfaces-0.1.2/README.md
-drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-02-14 11:22:12.894948 amicus_interfaces-0.1.2/amicus_interfaces/
--rw-r--r--   0 mauceric   (501) staff       (20)      264 2024-02-10 16:49:40.000000 amicus_interfaces-0.1.2/amicus_interfaces/__init__.py
--rw-r--r--   0 mauceric   (501) staff       (20)      786 2024-02-14 11:20:05.000000 amicus_interfaces-0.1.2/amicus_interfaces/interfaces.py
-drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-02-14 11:22:12.946106 amicus_interfaces-0.1.2/amicus_interfaces.egg-info/
--rw-r--r--   0 mauceric   (501) staff       (20)      351 2024-02-14 11:22:12.000000 amicus_interfaces-0.1.2/amicus_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 mauceric   (501) staff       (20)      244 2024-02-14 11:22:12.000000 amicus_interfaces-0.1.2/amicus_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 mauceric   (501) staff       (20)        1 2024-02-14 11:22:12.000000 amicus_interfaces-0.1.2/amicus_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 mauceric   (501) staff       (20)       18 2024-02-14 11:22:12.000000 amicus_interfaces-0.1.2/amicus_interfaces.egg-info/top_level.txt
--rw-r--r--   0 mauceric   (501) staff       (20)       38 2024-02-14 11:22:12.950058 amicus_interfaces-0.1.2/setup.cfg
--rw-r--r--   0 mauceric   (501) staff       (20)      475 2024-02-14 11:20:16.000000 amicus_interfaces-0.1.2/setup.py
+drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-04-10 08:33:58.192932 amicus_interfaces-0.1.3/
+-rw-r--r--   0 mauceric   (501) staff       (20)      351 2024-04-10 08:33:58.190944 amicus_interfaces-0.1.3/PKG-INFO
+-rw-r--r--   0 mauceric   (501) staff       (20)      325 2024-02-10 14:49:17.000000 amicus_interfaces-0.1.3/README.md
+drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-04-10 08:33:58.175641 amicus_interfaces-0.1.3/amicus_interfaces/
+-rw-r--r--   0 mauceric   (501) staff       (20)      264 2024-02-10 16:49:40.000000 amicus_interfaces-0.1.3/amicus_interfaces/__init__.py
+-rw-r--r--   0 mauceric   (501) staff       (20)      941 2024-04-10 08:12:57.000000 amicus_interfaces-0.1.3/amicus_interfaces/interfaces.py
+drwxr-xr-x   0 mauceric   (501) staff       (20)        0 2024-04-10 08:33:58.189902 amicus_interfaces-0.1.3/amicus_interfaces.egg-info/
+-rw-r--r--   0 mauceric   (501) staff       (20)      351 2024-04-10 08:33:58.000000 amicus_interfaces-0.1.3/amicus_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 mauceric   (501) staff       (20)      244 2024-04-10 08:33:58.000000 amicus_interfaces-0.1.3/amicus_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 mauceric   (501) staff       (20)        1 2024-04-10 08:33:58.000000 amicus_interfaces-0.1.3/amicus_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 mauceric   (501) staff       (20)       18 2024-04-10 08:33:58.000000 amicus_interfaces-0.1.3/amicus_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 mauceric   (501) staff       (20)       38 2024-04-10 08:33:58.193346 amicus_interfaces-0.1.3/setup.cfg
+-rw-r--r--   0 mauceric   (501) staff       (20)      475 2024-04-10 08:31:08.000000 amicus_interfaces-0.1.3/setup.py
```

### Comparing `amicus_interfaces-0.1.2/amicus_interfaces/interfaces.py` & `amicus_interfaces-0.1.3/amicus_interfaces/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
     @abstractmethod
     def notify(self, room:MatrixRoom, event:RoomMessageText, message: str, filepath: str= None, filename: str= None):
         pass
 
 
 class IPlugin(ABC):
+    def __init__(self, observable:IObservable, data_path:str="/data"):
+        self.data_path = data_path
+        self.__observable = observable
+        
+
     @abstractmethod
     def start(self):
         pass
 
     @abstractmethod
     def stop(self):
         pass
```

