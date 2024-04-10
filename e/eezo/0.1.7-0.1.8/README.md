# Comparing `tmp/eezo-0.1.7.tar.gz` & `tmp/eezo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.1.7.tar", last modified: Sun Apr  7 18:36:10 2024, max compression
+gzip compressed data, was "eezo-0.1.8.tar", last modified: Wed Apr 10 19:48:11 2024, max compression
```

## Comparing `eezo-0.1.7.tar` & `eezo-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.626244 eezo-0.1.7/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-07 18:36:10.626134 eezo-0.1.7/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.7/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.622838 eezo-0.1.7/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.7/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.7/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    11110 2024-04-07 18:16:52.000000 eezo-0.1.7/eezo/connector.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.624104 eezo-0.1.7/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.625959 eezo-0.1.7/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3085 2024-04-07 18:22:55.000000 eezo-0.1.7/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.623530 eezo-0.1.7/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-07 18:36:10.626280 eezo-0.1.7/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-07 18:26:49.000000 eezo-0.1.7/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.251496 eezo-0.1.8/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-10 19:48:11.251389 eezo-0.1.8/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.8/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.249508 eezo-0.1.8/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.8/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-04-10 16:05:56.000000 eezo-0.1.8/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    11720 2024-04-10 18:30:47.000000 eezo-0.1.8/eezo/connector.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.250472 eezo-0.1.8/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.1.8/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.251239 eezo-0.1.8/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     5824 2024-04-10 18:29:33.000000 eezo-0.1.8/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     5974 2024-04-10 19:39:16.000000 eezo-0.1.8/eezo/interface/interface_async.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/message.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.250028 eezo-0.1.8/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      567 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-10 19:48:11.251532 eezo-0.1.8/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1946 2024-04-10 19:45:26.000000 eezo-0.1.8/setup.py
```

### Comparing `eezo-0.1.7/PKG-INFO` & `eezo-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.7/README.md` & `eezo-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.1.7/eezo/async_client.py` & `eezo-0.1.8/eezo/async_client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.7/eezo/client.py` & `eezo-0.1.8/eezo/client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.7/eezo/connector.py` & `eezo-0.1.8/eezo/connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 class AsyncConnector:
     def __init__(self, api_key, connector_id, connector_function, logger=False):
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
         self.job_responses = {}
+        self.user_id = None
         self.run_loop = True
 
         if logger:
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(asctime)s: %(message)s",
                 datefmt="%Y-%m-%d %H:%M:%S",
@@ -78,14 +79,15 @@
     async def __authenticate(self):
         async with aiohttp.ClientSession() as session:
             url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
             async with session.post(url, json={"api_key": self.api_key}) as response:
                 if response.status == 200:
                     resp_json = await response.json()
                     self.auth_token = resp_json.get("token")
+                    self.user_id = resp_json.get("user_id")
                 else:
                     resp_json = await response.json()
                     raise Exception(f"{response.status}: {resp_json['detail']}")
 
     async def __get_job_result(self, job_id):
         while job_id not in self.job_responses:
             await asyncio.sleep(0.1)
@@ -95,28 +97,36 @@
             self.__log(f" ✖ Sub Job {response['id']} failed:\n{response['traceback']}.")
             raise Exception(
                 f"Propagating error from sub job {job_id}: {response['error']}"
             )
         return response["result"]
 
     async def __execute_job(self, job_obj):
-        job_id, payload = job_obj["job_id"], job_obj["job_payload"]
-        self.__log(f"<< Job {job_id} received with payload: {payload}")
+        job_id, connector_id, payload = (
+            job_obj["job_id"],
+            job_obj["connector_id"],
+            job_obj["job_payload"],
+        )
+        self.__log(
+            f"<< Job for connector {connector_id} received with payload: {payload}"
+        )
         try:
             # Create an interface object that the connector function can use to interact with the Eezo server
             i = AsyncInterface(
                 job_id=job_id,
+                user_id=self.user_id,
+                api_key=self.api_key,
                 cb_send_message=lambda p: self.sio.emit("direct_message", p),
                 cb_invoke_connector=lambda p: self.sio.emit("invoke_skill", p),
                 cb_get_result=self.__get_job_result,
             )
             result = await self.func(i, **payload)
             await self.sio.emit("job_completed", JobCompleted(result, True).to_dict())
         except Exception as e:
-            self.__log(f" ✖ Job {job_id} failed:\n{traceback.format_exc()}")
+            self.__log(f" ✖ Connector {connector_id} failed:\n{traceback.format_exc()}")
             job_completed = JobCompleted(
                 result=None,
                 success=False,
                 error=str(e),
                 traceback=traceback.format_exc(),
                 error_tag="Connector error",
             )
@@ -173,14 +183,15 @@
 class Connector:
     def __init__(self, api_key, connector_id, connector_function, logger=False):
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
         self.job_responses = {}
+        self.user_id = None
         self.run_loop = True
 
         if logger:
             logging.basicConfig(
                 level=logging.INFO,
                 format="%(asctime)s: %(message)s",
                 datefmt="%Y-%m-%d %H:%M:%S",
@@ -211,14 +222,15 @@
             logging.info(message)
 
     def __authenticate(self):
         url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
         response = requests.post(url, json={"api_key": self.api_key})
         if response.status_code == 200:
             self.auth_token = response.json().get("token")
+            self.user_id = response.json().get("user_id")
         else:
             raise Exception(f"{response.status_code}: {response.json()['detail']}")
 
     def __get_job_result(self, job_id):
         while True:
             if job_id in self.job_responses:
                 response = self.job_responses.pop(job_id)
@@ -231,29 +243,37 @@
                     raise Exception(response["error"])
 
                 return response["result"]
             else:
                 time.sleep(0.1)
 
     def __execute_job(self, job_obj):
-        job_id, payload = job_obj["job_id"], job_obj["job_payload"]
-        self.__log(f"<< Job {job_id} received with payload: {payload}")
+        job_id, connector_id, payload = (
+            job_obj["job_id"],
+            job_obj["connector_id"],
+            job_obj["job_payload"],
+        )
+        self.__log(
+            f"<< Job for connector {connector_id} received with payload: {payload}"
+        )
         try:
             # Create an interface object that the connector function can use to interact with the Eezo server
             i = Interface(
                 job_id=job_id,
+                user_id=self.user_id,
+                api_key=self.api_key,
                 cb_send_message=lambda p: self.sio.emit("direct_message", p),
                 cb_invoke_connector=lambda p: self.sio.emit("invoke_skill", p),
                 cb_get_result=self.__get_job_result,
             )
             # Call the connector function with the interface object and the job payload
             result = self.func(i, **payload)
             self.sio.emit("job_completed", JobCompleted(result, True).to_dict())
         except Exception as e:
-            self.__log(f" ✖ Job {job_id} failed:\n{traceback.format_exc()}")
+            self.__log(f" ✖ Connector {connector_id} failed:\n{traceback.format_exc()}")
             job_completed = JobCompleted(
                 result=None,
                 success=False,
                 error=str(e),
                 traceback=str(traceback.format_exc()),
                 error_tag="Connector error",
             )
```

### Comparing `eezo-0.1.7/eezo/interface/components/chart.py` & `eezo-0.1.8/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.7/eezo/interface/message.py` & `eezo-0.1.8/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.7/eezo.egg-info/PKG-INFO` & `eezo-0.1.8/eezo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.7
+Version: 0.1.8
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.7/eezo.egg-info/SOURCES.txt` & `eezo-0.1.8/eezo.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 eezo.egg-info/PKG-INFO
 eezo.egg-info/SOURCES.txt
 eezo.egg-info/dependency_links.txt
 eezo.egg-info/requires.txt
 eezo.egg-info/top_level.txt
 eezo/interface/__init__.py
 eezo/interface/interface.py
+eezo/interface/interface_async.py
 eezo/interface/message.py
 eezo/interface/components/__init__.py
 eezo/interface/components/chart.py
 eezo/interface/components/component.py
 eezo/interface/components/image.py
 eezo/interface/components/text.py
 eezo/interface/components/youtube_video.py
```

### Comparing `eezo-0.1.7/setup.py` & `eezo-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.1.7",
+    version="0.1.8",
     description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
@@ -24,14 +24,15 @@
         "requests==2.31.0",
         "simple-websocket==1.0.0",
         "urllib3==2.2.1",
         "watchdog==4.0.0",
         "wsproto==1.2.0",
         "yarl==1.9.4",
         "websocket-client==1.7.0",
+        "httpx==0.27.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",  # Alpha status
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

