# Comparing `tmp/Drumpler-1.1.0.tar.gz` & `tmp/Drumpler-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.1.0.tar", last modified: Tue Apr  9 21:03:16 2024, max compression
+gzip compressed data, was "Drumpler-1.1.1.tar", last modified: Tue Apr  9 22:16:42 2024, max compression
```

## Comparing `Drumpler-1.1.0.tar` & `Drumpler-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.602467 Drumpler-1.1.0/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.601012 Drumpler-1.1.0/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.1.0/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 21:03:16.601885 Drumpler-1.1.0/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.1.0/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.594612 Drumpler-1.1.0/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.1.0/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-09 20:27:21.000000 Drumpler-1.1.0/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     7632 2024-04-09 21:02:54.000000 Drumpler-1.1.0/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6505 2024-04-09 21:02:58.000000 Drumpler-1.1.0/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3158 2024-04-09 21:02:56.000000 Drumpler-1.1.0/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 21:03:16.602595 Drumpler-1.1.0/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 21:03:07.000000 Drumpler-1.1.0/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.599939 Drumpler-1.1.0/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.1.0/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.286639 Drumpler-1.1.1/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.285356 Drumpler-1.1.1/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.1.1/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 22:16:42.286056 Drumpler-1.1.1/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 Drumpler-1.1.1/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.280271 Drumpler-1.1.1/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.1.1/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      804 2024-04-09 22:06:44.000000 Drumpler-1.1.1/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     7632 2024-04-09 22:01:45.000000 Drumpler-1.1.1/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6683 2024-04-09 22:05:32.000000 Drumpler-1.1.1/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3143 2024-04-09 21:57:52.000000 Drumpler-1.1.1/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 22:16:42.286753 Drumpler-1.1.1/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 22:16:26.000000 Drumpler-1.1.1/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.284438 Drumpler-1.1.1/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.1.1/test/test_drumpler.py
```

### Comparing `Drumpler-1.1.0/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.1.1/Drumpler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.1.0
+Version: 1.1.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.1.0/LICENSE` & `Drumpler-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.0/PKG-INFO` & `Drumpler-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.1.0
+Version: 1.1.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.1.0/README.md` & `Drumpler-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.0/drumpler/drumpler.py` & `Drumpler-1.1.1/drumpler/drumpler.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.0/drumpler/mammoth.py` & `Drumpler-1.1.1/drumpler/mammoth.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 from .request import Request
 import threading
 from datetime import datetime, timezone
 from sqlalchemy import create_engine, Column, Integer, String, DateTime, ForeignKey, Text
 from sqlalchemy.orm import sessionmaker, relationship
 from sqlalchemy.orm import declarative_base
-from .constants import DATABASE_URI, AUTHORIZATION_KEY, DRUMPLER_URL, MAMMOTH_WORKERS
+from .constants import DATABASE_URI, AUTHORIZATION_KEY, DRUMPLER_URL
 import signal
 
 Base = declarative_base()
 
 class Job(Base):
     __tablename__ = 'jobs'
     id = Column(Integer, primary_key=True)
@@ -34,31 +34,36 @@
 
 engine = create_engine(DATABASE_URI)
 Base.metadata.create_all(engine)
 
 Session = sessionmaker(bind=engine)
 
 class Mammoth:
-    def __init__(self, process_request_data, drumpler_url=DRUMPLER_URL, workers=MAMMOTH_WORKERS):
+    def __init__(self, process_request_data, drumpler_url=DRUMPLER_URL, workers=1, custom_value=None):
         self.drumpler_url = drumpler_url
         self.auth_key = AUTHORIZATION_KEY  # Default value if not set
         self.workers = workers if workers is not None else multiprocessing.cpu_count()
         self.stop_signal = threading.Event()  # Use an event to signal workers to stop
         self.user_process_request_data = process_request_data
+        self.custom_value = custom_value
 
     def insert_event(self, session, job_id, message):
         start_event = Event(job_id=job_id, message=message)
         session.add(start_event)
         session.commit()
         return True
 
-    def fetch_next_unhandled_request(self, session, drumpler_url):
+    def fetch_next_unhandled_request(self, session):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         try:
-            response = requests.get(f"{drumpler_url}/request/next-unhandled", headers=headers)
+            if self.custom_value:
+                response = requests.get(f"{DRUMPLER_URL}/request/next-unhandled?custom_value={self.custom_value}", headers=headers)
+            else:
+                response = requests.get(f"{DRUMPLER_URL}/request/next-unhandled", headers=headers)
+
             if response.status_code == 200:
                 data = response.json()
 
                 # Create a Job record
                 job = Job(request_id=data.get('id'), status='Pending')
                 session.add(job)
                 session.commit()
@@ -121,22 +126,22 @@
         # Factory method to create a new SQLAlchemy session
         return Session()
 
     def run(self):
         def worker_task(session_factory, drumpler_url, auth_key, stop_signal):
             session = session_factory()
             while not stop_signal.is_set():
-                request, job_id = self.fetch_next_unhandled_request(session, drumpler_url)
+                request, job_id = self.fetch_next_unhandled_request(session)
                 if request and job_id:
                     # Call the user-defined processing function
                     self.process_request_start(session, request, job_id)
                     process = self.user_process_request_data(session, request, job_id)
 
                     if process:
-                        request.mark_as_handled(drumpler_url)
+                        request.mark_as_handled()
                         self.process_request_complete(session, request, job_id)
 
             session.close()
 
         # Set up signal handling to catch CTRL+C
         original_sigint_handler = signal.getsignal(signal.SIGINT)
         signal.signal(signal.SIGINT, lambda sig, frame: self.stop_signal.set())
```

### Comparing `Drumpler-1.1.0/drumpler/request.py` & `Drumpler-1.1.1/drumpler/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,25 @@
         self._method = method
         self._request_url = request_url
         self._request_raw = request_raw
         self._request_json = json.loads(request_raw)
         self.custom_value = custom_value
         self._is_handled = is_handled
 
-    def mark_as_handled(self, drumpler_url):
+    def mark_as_handled(self):
         headers = {
             'Authorization': f'Bearer {AUTHORIZATION_KEY}',
             'Content-Type': 'application/json'  # Indicate JSON payload
         }
         payload = {
             'is_handled': 1  # Assuming setting `is_handled` to 1 marks it as handled
         }
 
         try:
-            response = requests.put(f"{drumpler_url}/request/{self.id}", json=payload, headers=headers)
+            response = requests.put(f"{DRUMPLER_URL}/request/{self.id}", json=payload, headers=headers)
             if response.status_code == 200:
                 return f"Request {self.id} marked as handled successfully."
             else:
                 # Attempt to extract and print a more descriptive error message
                 try:
                     error_message = response.json().get('message', 'No error message provided.')
                 except ValueError:  # If response is not in JSON format
@@ -104,8 +104,8 @@
 
     @property
     def is_handled(self):
         return self._is_handled
 
     @is_handled.setter
     def is_handled(self, value):
-        self._is_handled = value
+        self._is_handled = value
```

### Comparing `Drumpler-1.1.0/setup.py` & `Drumpler-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.1.0',
+    version='1.1.1',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.1.0/test/test_drumpler.py` & `Drumpler-1.1.1/test/test_drumpler.py`

 * *Files identical despite different names*

