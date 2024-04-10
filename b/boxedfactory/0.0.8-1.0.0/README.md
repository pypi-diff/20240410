# Comparing `tmp/boxedfactory-0.0.8.tar.gz` & `tmp/boxedfactory-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxedfactory-0.0.8.tar", last modified: Sat Oct 21 14:55:27 2023, max compression
+gzip compressed data, was "boxedfactory-1.0.0.tar", last modified: Wed Apr 10 15:06:04 2024, max compression
```

## Comparing `boxedfactory-0.0.8.tar` & `boxedfactory-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       62 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        7 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/README.md
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       80 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/requirements.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-10-21 14:55:27.191866 boxedfactory-0.0.8/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1217 2023-10-21 12:59:33.000000 boxedfactory-0.0.8/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.179866 boxedfactory-0.0.8/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.183866 boxedfactory-0.0.8/src/boxedfactory/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory/core/common/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1791 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/configurations.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       54 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/cryptography.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1392 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/data.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       99 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/environment.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      643 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/http.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1512 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/queue.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3007 2023-10-21 14:30:35.000000 boxedfactory-0.0.8/src/boxedfactory/core/common/storage.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      348 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/test_worker.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-10-21 13:47:15.000000 boxedfactory-0.0.8/src/boxedfactory/core/worker.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1426 2023-10-21 12:55:50.000000 boxedfactory-0.0.8/src/boxedfactory/core/worker_manager.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-10-21 14:55:27.187866 boxedfactory-0.0.8/src/boxedfactory.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      977 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      782 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       81 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/requires.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2023-10-21 14:55:27.000000 boxedfactory-0.0.8/src/boxedfactory.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-10-21 14:54:58.000000 boxedfactory-0.0.8/version.txt
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.361392 boxedfactory-1.0.0/
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)    35148 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/LICENSE
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       62 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1059 2024-04-10 15:06:04.361392 boxedfactory-1.0.0/PKG-INFO
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       39 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/README.md
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       84 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/pyproject.toml
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       80 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/requirements.txt
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       38 2024-04-10 15:06:04.361392 boxedfactory-1.0.0/setup.cfg
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1267 2024-04-10 15:05:08.000000 boxedfactory-1.0.0/setup.py
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.349392 boxedfactory-1.0.0/src/
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.353392 boxedfactory-1.0.0/src/boxedfactory/
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/__init__.py
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.353392 boxedfactory-1.0.0/src/boxedfactory/core/
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/__init__.py
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.361392 boxedfactory-1.0.0/src/boxedfactory/core/common/
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/__init__.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1791 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/configurations.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       54 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/cryptography.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1392 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/data.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       99 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/environment.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)      663 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/http.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1530 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/queue.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     2875 2024-04-10 15:05:08.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/shared.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     3007 2024-04-01 17:40:03.000000 boxedfactory-1.0.0/src/boxedfactory/core/common/storage.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     2477 2024-04-10 15:05:08.000000 boxedfactory-1.0.0/src/boxedfactory/core/process_worker.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)      355 2024-04-08 21:56:50.000000 boxedfactory-1.0.0/src/boxedfactory/core/test_worker.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1369 2024-04-08 21:56:50.000000 boxedfactory-1.0.0/src/boxedfactory/core/thread_worker.py
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1960 2024-04-04 00:06:35.000000 boxedfactory-1.0.0/src/boxedfactory/core/worker_manager.py
+drwxr-xr-x   0 actions-runner  (1002) actions-runner  (1002)        0 2024-04-10 15:06:04.361392 boxedfactory-1.0.0/src/boxedfactory.egg-info/
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)     1059 2024-04-10 15:06:04.000000 boxedfactory-1.0.0/src/boxedfactory.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)      868 2024-04-10 15:06:04.000000 boxedfactory-1.0.0/src/boxedfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)        1 2024-04-10 15:06:04.000000 boxedfactory-1.0.0/src/boxedfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       81 2024-04-10 15:06:04.000000 boxedfactory-1.0.0/src/boxedfactory.egg-info/requires.txt
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)       13 2024-04-10 15:06:04.000000 boxedfactory-1.0.0/src/boxedfactory.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1002) actions-runner  (1002)        5 2024-04-10 15:05:08.000000 boxedfactory-1.0.0/version.txt
```

### Comparing `boxedfactory-0.0.8/LICENSE` & `boxedfactory-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.8/PKG-INFO` & `boxedfactory-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: boxedfactory
-Version: 0.0.8
-Summary: A library with rabbit, mongo and azure
+Version: 1.0.0
+Summary: A library for easy create and manage concurrent thread and process workers.
 Home-page: https://github.com/LostSavannah/boxed-factory
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/boxed-factory/issues
 Project-URL: Documentation, https://dev.moradev.dev/boxed-factory/documentation
 Project-URL: Examples, https://dev.moradev.dev/boxed-factory/examples
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: requests
 Requires-Dist: pymongo
 Requires-Dist: pika
 Requires-Dist: azure-storage-blob
 Requires-Dist: azure-identity
 
-### IDK
+### Boxed-factory
+
+Easy managed workers
```

### Comparing `boxedfactory-0.0.8/setup.py` & `boxedfactory-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
         return f.read()
 
 setuptools.setup(    
     name="boxedfactory",
     version=readfile('version.txt'),
     author="Erick Fernando Mora Ramirez",
     author_email="erickfernandomoraramirez@gmail.com",
-    description="A library with rabbit, mongo and azure",
+    description="A library for easy create and manage concurrent thread and process workers.",
     long_description=readfile('README.md'),
     long_description_content_type="text/markdown",
     url="https://github.com/LostSavannah/boxed-factory",
     project_urls={
         "Bug Tracker": "https://dev.moradev.dev/boxed-factory/issues",
         "Documentation": "https://dev.moradev.dev/boxed-factory/documentation",
         "Examples": "https://dev.moradev.dev/boxed-factory/examples",
     },
     package_data={
         "":["*.txt"]
     },
     classifiers=[
     "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     install_requires=[i.strip() for i in open("requirements.txt").readlines()]
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/common/configurations.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/configurations.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/common/data.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/data.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/common/http.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 def http_error(code:int, detail:str=''):
     raise HTTPException(code, detail)
 
 def configure_cors(api:FastAPI) -> FastAPI:
     async def inner(request:Request, call_next):
         response:Response = Response() if request.method == "OPTIONS" else await call_next(request)
         response.headers["Access-Control-Allow-Origin"] = '*'
-        response.headers["Access-Control-Allow-Methods"] = 'GET, POST, OPTIONS'
+        response.headers["Access-Control-Allow-Methods"] = 'GET, POST, OPTIONS, PUT, DELETE, PATCH'
         response.headers["Access-Control-Allow-Headers"] = '*'
         return response
     api.middleware("http")(inner)
     return api
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/common/queue.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         host, user, password = self.get_rabbit_parameters()
         creds = pika.PlainCredentials(user, password)
         with pika.BlockingConnection(pika.ConnectionParameters(host, credentials=creds)) as c:
             channel = c.channel()
             channel.queue_declare(queue_name, durable=True, auto_delete=False)
             method, properties, body = channel.basic_get(queue_name, True)
             c.close()
-            return json.loads(body)
+            return json.loads(body) if body else None
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/common/storage.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/storage.py`

 * *Files identical despite different names*

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/worker.py` & `boxedfactory-1.0.0/src/boxedfactory/core/common/shared.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,94 @@
 import time
-from threading import Thread
-from enum import IntEnum, StrEnum
+from enum import IntEnum, Enum
+from typing import Callable
+import uuid
 
-class LogKind(StrEnum):
+class LogKind(str, Enum):
     Information = "Information"
     Alert = "Alert"
     Error = "Error"
     Warning = "Warning"
     Success = "Success"
 
 class WorkerLog:
     def __init__(self, title:str, kind:LogKind = LogKind.Information, detail:str = None) -> None:
+        self.id = str(uuid.uuid4())
         self.epoch:float = time.time()
         self.kind = kind
         self.title = title
         self.detail = detail or ''
 
 class WorkerStatus(IntEnum):
     Stopped = 1
     Stopping = 2
     Paused = 3
     Active = 4
 
-class Worker(Thread):
-    def __init__(self, interval:float = 1000, log_size:int = 100) -> None:
-        Thread.__init__(self)
+class OperationState():
+    def __init__(self, log_size:int = 100) -> None:       
         self.log_size = log_size
-        self.logs:list[WorkerLog] = []
         self.status:WorkerStatus = WorkerStatus.Stopped
-        self.interval = self.set_interval(interval)
+        self.logs:list[WorkerLog] = []
         self.current:str = ''
         self.steps = 0
         self.step = 0
         self.meta:dict = dict()
 
     def log(self, title, kind:LogKind = LogKind.Information, detail:str = None):
         while len(self.logs) > self.log_size:
             self.logs.pop()
         self.logs.append(WorkerLog(title, kind, detail))
 
-    def start(self) -> None:
-        if self.status == WorkerStatus.Stopped:
-            self.status = WorkerStatus.Active
-            self.log("Started", LogKind.Success)
-            return super().start()
+    def get_snapshot(self):
+        return self.__dict__
+
+class WorkerBase:
+    def __init__(self, interval:float = 1000, log_size:int = 100) -> None:
+        self.state = OperationState(log_size)
+        self.interval = self.set_interval(interval)
+
+    def try_start(self, on_start:Callable[[],None]):
+        if self.state.status == WorkerStatus.Stopped:
+            self.state.status = WorkerStatus.Active
+            self.state.log("Started", LogKind.Success)
+            return on_start()
 
     def set_interval(self, interval:float):
         self.interval = max(10, min(0.1, interval))
         return self.interval
 
-    def run(self) -> None:
-        while self.status not in [WorkerStatus.Stopped, WorkerStatus.Stopping]:
-            if self.status != WorkerStatus.Paused:
+    def main_control(self):
+        while self.state.status not in [WorkerStatus.Stopped, WorkerStatus.Stopping]:
+            if self.state.status != WorkerStatus.Paused:
                 self.main_event_loop()
             time.sleep(self.interval)
-        self.status = WorkerStatus.Stopped
-
-    def main_event_loop(self):
-        raise NotImplemented()
+        self.state.status = WorkerStatus.Stopped
 
     def set_pause(self, paused:bool = True):
-        if paused and self.status != WorkerStatus.Paused:
-            self.status = WorkerStatus.Paused
-            self.log("Paused", LogKind.Success)
-        elif not paused and self.status == WorkerStatus.Paused:
-            self.status = WorkerStatus.Active
-            self.log("Resumed", LogKind.Success)
+        if paused and self.state.status != WorkerStatus.Paused:
+            self.state.status = WorkerStatus.Paused
+            self.state.log("Paused", LogKind.Success)
+        elif not paused and self.state.status == WorkerStatus.Paused:
+            self.state.status = WorkerStatus.Active
+            self.state.log("Resumed", LogKind.Success)
 
     def pause(self):
         return self.set_pause(True)
 
     def resume(self):
         return self.set_pause(False)
 
     def stop(self, retries:int = 3):
-        if self.status in [WorkerStatus.Stopped, WorkerStatus.Stopping]:
-            return
-        self.status = WorkerStatus.Stopping
-        while self.is_alive() and retries > 0:
-            self.join(1000)
-            retries -= 1
-        if self.is_alive():
-            self.log("Failed stop", LogKind.Error)
-            self.status = WorkerStatus.Active
-        else:
-            self.log("Success stop", LogKind.Success)
-            self.status = WorkerStatus.Stopped
+        raise NotImplemented()
+    
+    def start(self):
+        raise NotImplemented()
+    
+    def run(self):
+        raise NotImplemented()
+    
+    def get_state(self) -> dict:
+        raise NotImplemented()
+
+    def main_event_loop(self):
+        raise NotImplemented()
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory/core/worker_manager.py` & `boxedfactory-1.0.0/src/boxedfactory/core/worker_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from .worker import Worker
+from .common.shared import WorkerBase
 from .common.cryptography import newid
 from typing import Callable
 
-WorkerFactory = dict[str, Callable[[], Worker]]
-WorkerPool = dict[str, dict[str, Worker]]
+WorkerFactory = dict[str, Callable[[], WorkerBase]]
+WorkerPool = dict[str, dict[str, WorkerBase]]
 
 class WorkerManager:
     def __init__(self, factory:WorkerFactory) -> None:
         self.factory:WorkerFactory = factory
         self.pool:WorkerPool = {i:dict() for i in self.factory}
 
-    def create(self, kind:str) -> str:
+    def create(self, kind:str, id:str = None) -> str:
+        id = id or newid()
         if kind in self.factory:
-            id = newid()
-            self.pool[kind][id] = self.factory[kind]()
+            if id in self.pool[kind]:
+                self.recycle(kind, id)
+            else:
+                self.pool[kind][id] = self.factory[kind]()
             return id
         else:
             raise Exception(f"Worker type {kind} not found")
         
-    def get_worker(self, kind:str, id:str) -> Worker:
+    def get_worker(self, kind:str, id:str) -> WorkerBase:
         if kind in self.pool:
             if id in self.pool[kind]:
                 return self.pool[kind][id]
             else:
                 raise Exception(f"Worker type {kind} with id {id} not found")
         else:
             raise Exception(f"Worker type {kind} not found")
@@ -32,12 +35,25 @@
     
     def get_worker_ids(self, kind:str) -> list[str]:
         if kind in self.pool:
             return [i for i in self.pool[kind]]
         else:
             raise Exception(f"Worker type {kind} not found")
         
-    def recicle(self, kind:str, id:str) -> str:
+    def recycle(self, kind:str, id:str) -> str:
+        self.remove(kind, id)
+        print(f'recycle: {id}')
+        self.pool[kind][id] = self.factory[kind]()
+        return id
+    
+    def remove(self, kind:str, id:str) -> str:
         w = self.get_worker(kind, id)
+        print(f'remove: {id}')
         w.stop()
         del self.pool[kind][id]
-        return id
+        return id
+    
+    def __del__(self):
+        for kind in self.pool:
+            kind_ids = [i for i in self.pool[kind]]
+            for id in kind_ids:
+                self.remove(kind, id)
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory.egg-info/PKG-INFO` & `boxedfactory-1.0.0/src/boxedfactory.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: boxedfactory
-Version: 0.0.8
-Summary: A library with rabbit, mongo and azure
+Version: 1.0.0
+Summary: A library for easy create and manage concurrent thread and process workers.
 Home-page: https://github.com/LostSavannah/boxed-factory
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/boxed-factory/issues
 Project-URL: Documentation, https://dev.moradev.dev/boxed-factory/documentation
 Project-URL: Examples, https://dev.moradev.dev/boxed-factory/examples
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
 Requires-Dist: requests
 Requires-Dist: pymongo
 Requires-Dist: pika
 Requires-Dist: azure-storage-blob
 Requires-Dist: azure-identity
 
-### IDK
+### Boxed-factory
+
+Easy managed workers
```

### Comparing `boxedfactory-0.0.8/src/boxedfactory.egg-info/SOURCES.txt` & `boxedfactory-1.0.0/src/boxedfactory.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 src/boxedfactory/__init__.py
 src/boxedfactory.egg-info/PKG-INFO
 src/boxedfactory.egg-info/SOURCES.txt
 src/boxedfactory.egg-info/dependency_links.txt
 src/boxedfactory.egg-info/requires.txt
 src/boxedfactory.egg-info/top_level.txt
 src/boxedfactory/core/__init__.py
+src/boxedfactory/core/process_worker.py
 src/boxedfactory/core/test_worker.py
-src/boxedfactory/core/worker.py
+src/boxedfactory/core/thread_worker.py
 src/boxedfactory/core/worker_manager.py
 src/boxedfactory/core/common/__init__.py
 src/boxedfactory/core/common/configurations.py
 src/boxedfactory/core/common/cryptography.py
 src/boxedfactory/core/common/data.py
 src/boxedfactory/core/common/environment.py
 src/boxedfactory/core/common/http.py
 src/boxedfactory/core/common/queue.py
+src/boxedfactory/core/common/shared.py
 src/boxedfactory/core/common/storage.py
```

