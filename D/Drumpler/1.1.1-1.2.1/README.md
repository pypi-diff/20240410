# Comparing `tmp/Drumpler-1.1.1.tar.gz` & `tmp/Drumpler-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Drumpler-1.1.1.tar", last modified: Tue Apr  9 22:16:42 2024, max compression
+gzip compressed data, was "Drumpler-1.2.1.tar", last modified: Wed Apr 10 16:46:45 2024, max compression
```

## Comparing `Drumpler-1.1.1.tar` & `Drumpler-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.286639 Drumpler-1.1.1/
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.285356 Drumpler-1.1.1/Drumpler.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-09 22:16:42.000000 Drumpler-1.1.1/Drumpler.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.1.1/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-09 22:16:42.286056 Drumpler-1.1.1/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 Drumpler-1.1.1/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.280271 Drumpler-1.1.1/drumpler/
--rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.1.1/drumpler/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      804 2024-04-09 22:06:44.000000 Drumpler-1.1.1/drumpler/constants.py
--rw-r--r--   0 Karel      (503) staff       (20)     7632 2024-04-09 22:01:45.000000 Drumpler-1.1.1/drumpler/drumpler.py
--rw-r--r--   0 Karel      (503) staff       (20)     6683 2024-04-09 22:05:32.000000 Drumpler-1.1.1/drumpler/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)     3143 2024-04-09 21:57:52.000000 Drumpler-1.1.1/drumpler/request.py
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-09 22:16:42.286753 Drumpler-1.1.1/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-09 22:16:26.000000 Drumpler-1.1.1/setup.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-09 22:16:42.284438 Drumpler-1.1.1/test/
--rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.1.1/test/test_drumpler.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 16:46:45.065548 Drumpler-1.2.1/
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 16:46:45.063901 Drumpler-1.2.1/Drumpler.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-10 16:46:45.000000 Drumpler-1.2.1/Drumpler.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      470 2024-04-10 16:46:45.000000 Drumpler-1.2.1/Drumpler.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-10 16:46:45.000000 Drumpler-1.2.1/Drumpler.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       82 2024-04-10 16:46:45.000000 Drumpler-1.2.1/Drumpler.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        9 2024-04-10 16:46:45.000000 Drumpler-1.2.1/Drumpler.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 Drumpler-1.2.1/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4201 2024-04-10 16:46:45.064819 Drumpler-1.2.1/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 Drumpler-1.2.1/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 16:46:45.058612 Drumpler-1.2.1/drumpler/
+-rw-r--r--   0 Karel      (503) staff       (20)       32 2024-04-03 21:38:26.000000 Drumpler-1.2.1/drumpler/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)      804 2024-04-09 22:06:44.000000 Drumpler-1.2.1/drumpler/constants.py
+-rw-r--r--   0 Karel      (503) staff       (20)     7792 2024-04-10 16:46:17.000000 Drumpler-1.2.1/drumpler/drumpler.py
+-rw-r--r--   0 Karel      (503) staff       (20)     7906 2024-04-10 16:38:04.000000 Drumpler-1.2.1/drumpler/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3143 2024-04-09 21:57:52.000000 Drumpler-1.2.1/drumpler/request.py
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-10 16:46:45.065680 Drumpler-1.2.1/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      823 2024-04-10 16:46:29.000000 Drumpler-1.2.1/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-10 16:46:45.062877 Drumpler-1.2.1/test/
+-rw-r--r--   0 Karel      (503) staff       (20)     3729 2024-04-03 19:03:38.000000 Drumpler-1.2.1/test/test_drumpler.py
```

### Comparing `Drumpler-1.1.1/Drumpler.egg-info/PKG-INFO` & `Drumpler-1.2.1/Drumpler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.1.1
+Version: 1.2.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.1.1/LICENSE` & `Drumpler-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.1/PKG-INFO` & `Drumpler-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Drumpler
-Version: 1.1.1
+Version: 1.2.1
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Drumpler-1.1.1/README.md` & `Drumpler-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.1/drumpler/constants.py` & `Drumpler-1.2.1/drumpler/constants.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.1/drumpler/drumpler.py` & `Drumpler-1.2.1/drumpler/drumpler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 from flask import Flask, request, jsonify
 from .constants import DRUMPLER_HOST, DRUMPLER_PORT, DRUMPLER_DEBUG, DATABASE_URI, AUTHORIZATION_KEY
 import json
 from flask_sqlalchemy import SQLAlchemy
 from .request import Request as BaseRequest
+from sqlalchemy.exc import SQLAlchemyError
 
 app = Flask(__name__)
 app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 
 class Request(db.Model, BaseRequest):
@@ -34,20 +35,21 @@
         self.host = os.environ.get("DRUMPLER_HOST", DRUMPLER_HOST)
         self.port = os.environ.get("DRUMPLER_PORT", DRUMPLER_PORT)
         self.debug = os.environ.get("DRUMPLER_DEBUG",DRUMPLER_DEBUG)
         
         self.app.config['SQLALCHEMY_DATABASE_URI'] = DATABASE_URI
         self.app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 
-        # Initialize SQLAlchemy with the Flask app here instead of global scope
         db.init_app(self.app)
-
         with self.app.app_context():
-            db.create_all()  # Move database initialization here
-        
+            try:
+                db.create_all()  # Attempt to create all tables
+            except SQLAlchemyError as e:
+                sys.exit(f"Failed to initialize database: {e}")
+
         self.__setup_routes()
 
     def __setup_routes(self):
         self.app.add_url_rule('/', view_func=self.hello_world, methods=['GET'])
         self.app.add_url_rule('/request', view_func=self.__process_request, methods=['POST'])
         self.app.add_url_rule('/request/<int:request_id>', view_func=self.__get_request, methods=['GET'])
         self.app.add_url_rule('/request/next-unhandled', view_func=self.__get_next_unhandled_request, methods=['GET'])
@@ -65,114 +67,112 @@
     def hello_world(self):
         return "Hello World"
 
     def __process_request(self):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
-        data = request.get_json() or {}  # Fallback to an empty dict if no JSON is provided
-        custom_value = request.args.get('custom_value', None)
-
-        new_request = Request(
-            source_ip=request.remote_addr,
-            user_agent=request.user_agent.string,
-            method=request.method,
-            request_url=request.url,
-            request_raw=json.dumps(data),
-            custom_value=custom_value
-        )
-        db.session.add(new_request)
-        db.session.commit()
-        return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
+        try:
+            data = request.get_json() or {}
+            custom_value = request.args.get('custom_value', None)
+            new_request = Request(
+                source_ip=request.remote_addr,
+                user_agent=request.user_agent.string,
+                method=request.method,
+                request_url=request.url,
+                request_raw=json.dumps(data),
+                custom_value=custom_value
+            )
+            db.session.add(new_request)
+            db.session.commit()
+            return jsonify({"message": "Request processed successfully", "id": new_request.id}), 200
+        except SQLAlchemyError as e:
+            return jsonify({"message": f"Failed to process request: {e}"}), 500
     
     def __get_next_unhandled_request(self):
-        with db.session.begin():
-            # Start with a base query
-            query = db.session.query(Request)\
-                .filter(Request.is_handled == 0, 
-                        Request.is_being_processed == False)
-
-            # Conditionally add the custom_value filter if it is provided
-            custom_value = request.args.get('custom_value', None)
-            if custom_value is not None:
-                query = query.filter(Request.custom_value == custom_value)
-
-            # Execute the query with ordering and locking
-            unhandled_request = query.order_by(Request.id)\
-                .with_for_update(skip_locked=True).first()
-
+        try:
+            with db.session.begin():
+                query = db.session.query(Request)\
+                    .filter(Request.is_handhandled == 0, 
+                            Request.is_being_processed == False)
+                custom_value = request.args.get('custom_value', None)
+                if custom_value:
+                    query = query.filter(Request.custom_value == custom_value)
+                unhandled_request = query.order_by(Request.id)\
+                    .with_for_update(skip_locked=True).first()
+
+                if unhandled_request:
+                    unhandled_request.is_being_processed = True
+                    request_data = {
+                        "id": unhandled_request.id,
+                        # Remainder of your field assignments remain unchanged
+                    }
             if unhandled_request:
-                # Prepare data before committing the transaction
-                request_data = {
-                    "id": unhandled_request.id,
-                    "timestamp": unhandled_request.timestamp.isoformat(),
-                    "source_ip": unhandled_request.source_ip,
-                    "user_agent": unhandled_request.user_agent,
-                    "method": unhandled_request.method,
-                    "request_url": unhandled_request.request_url,
-                    "request_raw": unhandled_request.request_raw,
-                    "custom_value": unhandled_request.custom_value,  # Include the custom field in the response
-                    "is_handled": unhandled_request.is_handled
-                }
-
-                # Mark the request as being processed
-                unhandled_request.is_being_processed = True
-                # Commit is done by the context manager upon exit
-
-        # Return outside the context manager to avoid accessing the session
-        if unhandled_request:
-            return jsonify(request_data), 200
-        else:
-            return jsonify({"message": "No unhandled requests found."}), 404
+                return jsonify(request_data), 200
+            else:
+                return jsonify({"message": "No unhandled requests found."}), 404
+        except SQLAlchemyError as e:
+            return jsonify({"message": f"Database error: {e}"}), 500
 
     def __get_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
-        request_entry = Request.query.get(request_id)
-        if request_entry:
-            return jsonify({
-                "id": request_entry.id,
-                "timestamp": request_entry.timestamp.isoformat(),
-                "source_ip": request_entry.source_ip,
-                "user_agent": request_entry.user_agent,
-                "method": request_entry.method,
-                "request_url": request_entry.request_url,
-                "request_raw": json.loads(request_entry.request_raw),
-                "custom_value": request_entry.custom_value,
-                "is_handled": request_entry.is_handled
-            }), 200
-        else:
-            return jsonify({"message": "Request not found"}), 404
+        try:
+            request_entry = Request.query.get(request_id)
+            if request_entry:
+                return jsonify({
+                    "id": request_entry.id,
+                    "timestamp": request_entry.timestamp.isoformat(),
+                    "source_ip": request_entry.source_ip,
+                    "user_agent": request_entry.user_agent,
+                    "method": request_entry.method,
+                    "request_url": request_entry.request_url,
+                    "request_raw": json.loads(request_entry.request_raw),
+                    "custom_value": request_entry.custom_value,
+                    "is_handled": request_entry.is_handled
+                }), 200
+            else:
+                return jsonify({"message": "Request not found"}), 404
+        except SQLAlchemyError as e:
+            return jsonify({"message": f"Database error: {e}"}), 500
 
     def __update_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
-        data = request.get_json()
-        request_entry = Request.query.get(request_id)
-        if request_entry:
-            if 'is_handled' in data:
-                request_entry.is_handled = data['is_handled']
-            db.session.commit()
-            return jsonify({"message": "Request updated successfully"}), 200
-        else:
-            return jsonify({"message": "Request not found"}), 404
+        try:
+            data = request.get_json()
+            request_entry = Request.query.get(request_id)
+            if request_entry:
+                if 'is_handled' in data:
+                    request_entry.is_handled = data['is_handled']
+                db.session.commit()
+                return jsonify({"message": "Request updated successfully"}), 200
+            else:
+                return jsonify({"message": "Request not found"}), 404
+        except SQLAlchemyError as e:
+            db.session.rollback()  # Ensure that the session is rolled back in case of error
+            return jsonify({"message": f"Failed to update request: {e}"}), 500
 
     def __delete_request(self, request_id):
         if not self.__authorize_request():
             return jsonify({"message": "Invalid or missing authorization"}), 401
 
-        request_entry = Request.query.get(request_id)
-        if request_entry:
-            db.session.delete(request_entry)
-            db.session.commit()
-            return jsonify({"message": "Request deleted successfully"}), 200
-        else:
-            return jsonify({"message": "Request not found"}), 404
+        try:
+            request_entry = Request.query.get(request_id)
+            if request_entry:
+                db.session.delete(request_entry)
+                db.session.commit()
+                return jsonify({"message": "Request deleted successfully"}), 200
+            else:
+                return jsonify({"message": "Request not found"}), 404
+        except SQLAlchemyError as e:
+            db.session.rollback()  # It's good practice to roll back the session in case of error
+            return jsonify({"message": f"Failed to delete request: {e}"}), 500
 
     def run(self):
         app.run(host=self.host, port=self.port, debug=self.debug)
 
 if __name__ == '__main__':
     drumpler = Drumpler()
     drumpler.run()
```

### Comparing `Drumpler-1.1.1/drumpler/mammoth.py` & `Drumpler-1.2.1/drumpler/mammoth.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,18 +43,23 @@
         self.auth_key = AUTHORIZATION_KEY  # Default value if not set
         self.workers = workers if workers is not None else multiprocessing.cpu_count()
         self.stop_signal = threading.Event()  # Use an event to signal workers to stop
         self.user_process_request_data = process_request_data
         self.custom_value = custom_value
 
     def insert_event(self, session, job_id, message):
-        start_event = Event(job_id=job_id, message=message)
-        session.add(start_event)
-        session.commit()
-        return True
+        try:
+            start_event = Event(job_id=job_id, message=message)
+            session.add(start_event)
+            session.commit()
+            return True
+        except Exception as e:
+            print(f"Exception inserting event for job {job_id}: {e}")
+            session.rollback()  # Ensure the session is rolled back on error
+            return False
 
     def fetch_next_unhandled_request(self, session):
         headers = {"Authorization": f"Bearer {self.auth_key}"}
         try:
             if self.custom_value:
                 response = requests.get(f"{DRUMPLER_URL}/request/next-unhandled?custom_value={self.custom_value}", headers=headers)
             else:
@@ -83,68 +88,83 @@
             else:
                 print("Failed to fetch unhandled request:", response.status_code)
                 time.sleep(5)
                 return None, None
         except requests.exceptions.RequestException as e:
             print("Error fetching unhandled request:", e)
             return None, None
-
+        
     def process_request_start(self, session, request, job_id):
         if request.request_raw:
-            payload = json.loads(request.request_raw)
-            thread_id = threading.get_ident()  # Get the current thread's identifier
-            
-            # Log the start of processing as an event
-            start_event = Event(job_id=job_id, message=f'Started processing job:{job_id}, originated from request {request.id}.')
-            session.add(start_event)
-            session.commit()
+            try:
+                payload = json.loads(request.request_raw)
+                thread_id = threading.get_ident()  # Get the current thread's identifier
+                
+                # Log the start of processing as an event
+                start_event = Event(job_id=job_id, message=f'Started processing job:{job_id}, originated from request {request.id}.')
+                session.add(start_event)
+                session.commit()
             
-            return True
+                return True
+            except Exception as e:
+                print(f"Exception in process_request_start for job {job_id}: {e}")
+                self.insert_event(session, job_id, f"Exception in process_request_start: {e}")
+        
         return False
     
     def process_request_complete(self, session, request, job_id):
         if request.request_raw:
-            payload = json.loads(request.request_raw)
-            thread_id = threading.get_ident()  # Get the current thread's identifier
-            
-            # Mark job as completed
-            job = session.query(Job).filter(Job.id == job_id).first()
-            if job:
-                job.status = 'Completed'
-                job.finished_date = datetime.now(timezone.utc)
-                session.add(job)
-            
-            # Log the completion of processing as an event
-            completion_event = Event(job_id=job_id, message=f'Completed processing job:{job_id}, originated from request {request.id}.')
-            session.add(completion_event)
+            try:
+                payload = json.loads(request.request_raw)
+                thread_id = threading.get_ident()  # Get the current thread's identifier
+                
+                # Mark job as completed
+                job = session.query(Job).filter(Job.id == job_id).first()
+                if job:
+                    job.status = 'Completed'
+                    job.finished_date = datetime.now(timezone.utc)
+                    session.add(job)
+                
+                # Log the completion of processing as an event
+                completion_event = Event(job_id=job_id, message=f'Completed processing job:{job_id}, originated from request {request.id}.')
+                session.add(completion_event)
 
-            session.commit()
-            
-            return True
+                session.commit()
+                
+                return True
+            except Exception as e:
+                print(f"Exception in process_request_complete for job {job_id}: {e}")
+                self.insert_event(session, job_id, f"Exception in process_request_complete: {e}")
+        
         return False
 
     def session_factory(self):
         # Factory method to create a new SQLAlchemy session
         return Session()
 
     def run(self):
         def worker_task(session_factory, drumpler_url, auth_key, stop_signal):
             session = session_factory()
-            while not stop_signal.is_set():
-                request, job_id = self.fetch_next_unhandled_request(session)
-                if request and job_id:
-                    # Call the user-defined processing function
-                    self.process_request_start(session, request, job_id)
-                    process = self.user_process_request_data(session, request, job_id)
-
-                    if process:
-                        request.mark_as_handled()
-                        self.process_request_complete(session, request, job_id)
-
-            session.close()
+            try:
+                while not stop_signal.is_set():
+                    request, job_id = self.fetch_next_unhandled_request(session)
+                    if request and job_id:
+                        # Additional logging here
+                        print(f"Processing request {request.id}, job {job_id}")
+                        self.process_request_start(session, request, job_id)
+                        process = self.user_process_request_data(session, request, job_id)
+                        if process:
+                            request.mark_as_handled()
+                            self.process_request_complete(session, request, job_id)
+            except Exception as e:
+                print(f"Exception in worker_task: {e}")
+                # Consider setting stop_signal here if you want to stop all workers on error
+                self.insert_event(session, -1, f"Exception in worker_task: {e}")
+            finally:
+                session.close()
 
         # Set up signal handling to catch CTRL+C
         original_sigint_handler = signal.getsignal(signal.SIGINT)
         signal.signal(signal.SIGINT, lambda sig, frame: self.stop_signal.set())
 
         with ThreadPoolExecutor(max_workers=self.workers) as executor:
             for _ in range(self.workers):
```

### Comparing `Drumpler-1.1.1/drumpler/request.py` & `Drumpler-1.2.1/drumpler/request.py`

 * *Files identical despite different names*

### Comparing `Drumpler-1.1.1/setup.py` & `Drumpler-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Drumpler',
-    version='1.1.1',
+    version='1.2.1',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler',
     packages=find_packages(),
```

### Comparing `Drumpler-1.1.1/test/test_drumpler.py` & `Drumpler-1.2.1/test/test_drumpler.py`

 * *Files identical despite different names*

