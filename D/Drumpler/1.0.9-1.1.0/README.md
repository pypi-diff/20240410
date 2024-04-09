# Comparing `tmp/Drumpler-1.0.9.tar.gz` & `tmp/Drumpler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.0.9.tar", last modified: Tue Apr  9 19:26:38 2024, max compression
+gzip compressed data, was "Drumpler-1.1.0.tar", last modified: Tue Apr  9 21:03:16 2024, max compression
```

## Comparing `Drumpler-1.0.9.tar` & `Drumpler-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.968396 Drumpler-1.0.9/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.966868 Drumpler-1.0.9/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 19:26:38.000000 Drumpler-1.0.9/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.0.9/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 19:26:38.967625 Drumpler-1.0.9/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.0.9/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.961568 Drumpler-1.0.9/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.0.9/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-05 19:22:33.000000 Drumpler-1.0.9/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     7118 2024-04-09 19:26:03.000000 Drumpler-1.0.9/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6434 2024-04-04 18:13:02.000000 Drumpler-1.0.9/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3089 2024-04-03 21:38:26.000000 Drumpler-1.0.9/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 19:26:38.968562 Drumpler-1.0.9/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 19:26:14.000000 Drumpler-1.0.9/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 19:26:38.965921 Drumpler-1.0.9/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.0.9/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.602467 Drumpler-1.1.0/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.601012 Drumpler-1.1.0/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 21:03:16.000000 Drumpler-1.1.0/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.1.0/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 21:03:16.601885 Drumpler-1.1.0/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-05 21:41:41.000000 Drumpler-1.1.0/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.594612 Drumpler-1.1.0/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.1.0/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      663 2024-04-09 20:27:21.000000 Drumpler-1.1.0/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     7632 2024-04-09 21:02:54.000000 Drumpler-1.1.0/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     6505 2024-04-09 21:02:58.000000 Drumpler-1.1.0/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3158 2024-04-09 21:02:56.000000 Drumpler-1.1.0/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 21:03:16.602595 Drumpler-1.1.0/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 21:03:07.000000 Drumpler-1.1.0/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 21:03:16.599939 Drumpler-1.1.0/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.1.0/test/test_drumpler.py
```

### Comparing `Drumpler-1.0.9/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.1.0/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.9
+Version: 1.1.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.9/LICENSE` & `Drumpler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.9/PKG-INFO` & `Drumpler-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.0.9
+Version: 1.1.0
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.0.9/README.md` & `Drumpler-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.9/drumpler/constants.py` & `Drumpler-1.1.0/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.0.9/drumpler/drumpler.py` & `Drumpler-1.1.0/drumpler/drumpler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 import sys
 from flask import Flask, request, jsonify
 from .constants import DRUMPLER_HOST, DRUMPLER_PORT, DRUMPLER_DEBUG, DATABASE_URI, AUTHORIZATION_KEY
 import json
 from flask_sqlalchemy import SQLAlchemy
 from .request import Request as BaseRequest
-from sqlalchemy import func
 
 app = Flask(__name__)
 app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 
 class Request(db.Model, BaseRequest):
     id = db.Column(db.Integer, primary_key=True)
     timestamp = db.Column(db.DateTime, default=db.func.current_timestamp())
     source_ip = db.Column(db.String(128))
     user_agent = db.Column(db.String(256))
     method = db.Column(db.String(8))
     request_url = db.Column(db.String(256))
     request_raw = db.Column(db.Text)
+    custom_value = db.Column(db.String(256))
     is_handled = db.Column(db.Integer, default=0)
     is_being_processed = db.Column(db.Boolean, default=False)
 
 class Drumpler:
     def __init__(self):
         self.__init_env()
         self.app = Flask(__name__)
@@ -66,50 +66,59 @@
         return "Hello World"
 
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
         data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
+        custom_value = request.args.get('custom_value', None)
+
         new_request = Request(
             source_ip=request.remote_addr,
             user_agent=request.user_agent.string,
             method=request.method,
             request_url=request.url,
-            request_raw=json.dumps(data)
+            request_raw=json.dumps(data),
+            custom_value=custom_value
         )
         db.session.add(new_request)
         db.session.commit()
         return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
     
     def __get_next_unhandled_request(self):
         with db.session.begin():
-            unhandled_request = db.session.query(Request)\
-                .filter(
-                    Request.is_handled == 0, 
-                    Request.is_being_processed == False,
-                    Request.request_url.like(func.concat(self.host, '%'))
-                )\
-            .order_by(Request.id)\
-            .with_for_update(skip_locked=True).first()
+            # Start with a base query
+            query = db.session.query(Request)\
+                .filter(Request.is_handled == 0, 
+                        Request.is_being_processed == False)
+
+            # Conditionally add the custom_value filter if it is provided
+            custom_value = request.args.get('custom_value', None)
+            if custom_value is not None:
+                query = query.filter(Request.custom_value == custom_value)
+
+            # Execute the query with ordering and locking
+            unhandled_request = query.order_by(Request.id)\
+                .with_for_update(skip_locked=True).first()
 
             if unhandled_request:
                 # Prepare data before committing the transaction
                 request_data = {
                     "id": unhandled_request.id,
                     "timestamp": unhandled_request.timestamp.isoformat(),
                     "source_ip": unhandled_request.source_ip,
                     "user_agent": unhandled_request.user_agent,
                     "method": unhandled_request.method,
                     "request_url": unhandled_request.request_url,
                     "request_raw": unhandled_request.request_raw,
+                    "custom_value": unhandled_request.custom_value,  # Include the custom field in the response
                     "is_handled": unhandled_request.is_handled
                 }
-                
-                # Now that we have all needed data, mark as being processed
+
+                # Mark the request as being processed
                 unhandled_request.is_being_processed = True
                 # Commit is done by the context manager upon exit
 
         # Return outside the context manager to avoid accessing the session
         if unhandled_request:
             return jsonify(request_data), 200
         else:
@@ -125,14 +134,15 @@
                 "id": request_entry.id,
                 "timestamp": request_entry.timestamp.isoformat(),
                 "source_ip": request_entry.source_ip,
                 "user_agent": request_entry.user_agent,
                 "method": request_entry.method,
                 "request_url": request_entry.request_url,
                 "request_raw": json.loads(request_entry.request_raw),
+                "custom_value": request_entry.custom_value,
                 "is_handled": request_entry.is_handled
             }), 200
         else:
             return jsonify({"message": "Request not found"}), 404
 
     def __update_request(self, request_id):
         if not self.__authorize_request():
```

### Comparing `Drumpler-1.0.9/drumpler/mammoth.py` & `Drumpler-1.1.0/drumpler/mammoth.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                     id=data.get('id'),
                     timestamp=data.get('timestamp'),  
                     source_ip=data.get('source_ip'),
                     user_agent=data.get('user_agent'),
                     method=data.get('method'),
                     request_url=data.get('request_url'),
                     request_raw=data.get('request_raw'),
+                    custom_value=data.get('custom_value'),
                     is_handled=data.get('is_handled')
                 ), job.id
             else:
                 print("Failed to fetch unhandled request:", response.status_code)
                 time.sleep(5)
                 return None, None
         except requests.exceptions.RequestException as e:
@@ -127,15 +128,15 @@
                 request, job_id = self.fetch_next_unhandled_request(session, drumpler_url)
                 if request and job_id:
                     # Call the user-defined processing function
                     self.process_request_start(session, request, job_id)
                     process = self.user_process_request_data(session, request, job_id)
 
                     if process:
-                        request.mark_as_handled()
+                        request.mark_as_handled(drumpler_url)
                         self.process_request_complete(session, request, job_id)
 
             session.close()
 
         # Set up signal handling to catch CTRL+C
         original_sigint_handler = signal.getsignal(signal.SIGINT)
         signal.signal(signal.SIGINT, lambda sig, frame: self.stop_signal.set())
```

### Comparing `Drumpler-1.0.9/drumpler/request.py` & `Drumpler-1.1.0/drumpler/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import requests
 import json
 from .constants import DRUMPLER_URL, AUTHORIZATION_KEY
 
 class Request:
-    def __init__(self, id, timestamp, source_ip, user_agent, method, request_url, request_raw, is_handled):
+    def __init__(self, id, timestamp, source_ip, user_agent, method, request_url, request_raw, custom_value, is_handled):
         self._id = id
         self._timestamp = timestamp
         self._source_ip = source_ip
         self._user_agent = user_agent
         self._method = method
         self._request_url = request_url
         self._request_raw = request_raw
         self._request_json = json.loads(request_raw)
+        self.custom_value = custom_value
         self._is_handled = is_handled
 
-    def mark_as_handled(self):
+    def mark_as_handled(self, drumpler_url):
         headers = {
             'Authorization': f'Bearer {AUTHORIZATION_KEY}',
             'Content-Type': 'application/json'  # Indicate JSON payload
         }
         payload = {
             'is_handled': 1  # Assuming setting `is_handled` to 1 marks it as handled
         }
 
         try:
-            response = requests.put(f"{DRUMPLER_URL}/request/{self.id}", json=payload, headers=headers)
+            response = requests.put(f"{drumpler_url}/request/{self.id}", json=payload, headers=headers)
             if response.status_code == 200:
                 return f"Request {self.id} marked as handled successfully."
             else:
                 # Attempt to extract and print a more descriptive error message
                 try:
                     error_message = response.json().get('message', 'No error message provided.')
                 except ValueError:  # If response is not in JSON format
```

### Comparing `Drumpler-1.0.9/setup.py` & `Drumpler-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.0.9',
+    version='1.1.0',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.0.9/test/test_drumpler.py` & `Drumpler-1.1.0/test/test_drumpler.py`

 * *Files identical despite different names*

