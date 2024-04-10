# Comparing `tmp/palworld-api-1.0.0.tar.gz` & `tmp/palworld-api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palworld-api-1.0.0.tar", last modified: Fri Apr  5 00:12:29 2024, max compression
+gzip compressed data, was "palworld-api-1.0.1.tar", last modified: Wed Apr 10 13:09:10 2024, max compression
```

## Comparing `palworld-api-1.0.0.tar` & `palworld-api-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 00:12:29.296349 palworld-api-1.0.0/
--rw-rw-rw-   0        0        0     1262 2024-04-05 00:12:29.295349 palworld-api-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      952 2024-04-05 00:05:26.000000 palworld-api-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 00:12:29.288350 palworld-api-1.0.0/palworld_api/
--rw-rw-rw-   0        0        0       27 2024-04-04 23:38:01.000000 palworld-api-1.0.0/palworld_api/__init__.py
--rw-rw-rw-   0        0        0     6755 2024-04-04 23:49:20.000000 palworld-api-1.0.0/palworld_api/palworld_api.py
-drwxrwxrwx   0        0        0        0 2024-04-05 00:12:29.294348 palworld-api-1.0.0/palworld_api.egg-info/
--rw-rw-rw-   0        0        0     1262 2024-04-05 00:12:29.000000 palworld-api-1.0.0/palworld_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-05 00:12:29.000000 palworld-api-1.0.0/palworld_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 00:12:29.000000 palworld-api-1.0.0/palworld_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 00:12:29.000000 palworld-api-1.0.0/palworld_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 00:12:29.000000 palworld-api-1.0.0/palworld_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 00:12:29.297351 palworld-api-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2024-04-05 00:12:27.000000 palworld-api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.282538 palworld-api-1.0.1/
+-rw-rw-rw-   0        0        0     1378 2024-04-10 13:09:10.282538 palworld-api-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2024-04-10 13:08:35.000000 palworld-api-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.258539 palworld-api-1.0.1/palworld_api/
+-rw-rw-rw-   0        0        0       27 2024-04-04 23:38:01.000000 palworld-api-1.0.1/palworld_api/__init__.py
+-rw-rw-rw-   0        0        0     7168 2024-04-10 13:05:01.000000 palworld-api-1.0.1/palworld_api/palworld_api.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:09:10.281537 palworld-api-1.0.1/palworld_api.egg-info/
+-rw-rw-rw-   0        0        0     1378 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-10 13:09:10.000000 palworld-api-1.0.1/palworld_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 13:09:10.282538 palworld-api-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2024-04-10 13:08:29.000000 palworld-api-1.0.1/setup.py
```

### Comparing `palworld-api-1.0.0/PKG-INFO` & `palworld-api-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: palworld-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python API wrapper for the Palworld Rest API.
 Home-page: https://github.com/dkoz/palworld-api
 Author: dkoz
 Author-email: koz@beskor.net
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp==3.9.3
 
 # Palworld REST API Wrapper
- `palworld-api` is an API wrapper for the new Palworld Rest API. This supports all endpoints of the API and has been thoroughly tested.
+ This is a simple Palworld REST API Wrapper for Python project. This supports all API endpoints for Palworld.
 
 ## Version
-> v1.0.0
+> v1.0.1
 
 ## Installation
 1. Install `palworld-api` using pip:
    ```bash
    pip install palworld-api
    ```
+2. Import into your project.
+   ```python
+   import asyncio
+   from palworld_api import PalworldAPI
+   ```
 
 ## Requirements
 - Python 3.8+
 - RestAPI Enabled
 
 ## Usage
  Refer to example files to get an idea of how this works. Here is a basic usage:
- ```
- async def main():
+ ```python
+import asyncio
+from palworld_api import PalworldAPI
+
+async def main():
     server_url = "http://localhost:8212"
     username = "admin"
     password = "admin password"
     api = PalworldAPI(server_url, username, password)
 
     server_info = await api.get_server_info()
     print("Server Info:", server_info)
```

### Comparing `palworld-api-1.0.0/README.md` & `palworld-api-1.0.1/palworld_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+Metadata-Version: 2.1
+Name: palworld-api
+Version: 1.0.1
+Summary: A Python API wrapper for the Palworld Rest API.
+Home-page: https://github.com/dkoz/palworld-api
+Author: dkoz
+Author-email: koz@beskor.net
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Palworld REST API Wrapper
- `palworld-api` is an API wrapper for the new Palworld Rest API. This supports all endpoints of the API and has been thoroughly tested.
+ This is a simple Palworld REST API Wrapper for Python project. This supports all API endpoints for Palworld.
 
 ## Version
-> v1.0.0
+> v1.0.1
 
 ## Installation
 1. Install `palworld-api` using pip:
    ```bash
    pip install palworld-api
    ```
+2. Import into your project.
+   ```python
+   import asyncio
+   from palworld_api import PalworldAPI
+   ```
 
 ## Requirements
 - Python 3.8+
 - RestAPI Enabled
 
 ## Usage
  Refer to example files to get an idea of how this works. Here is a basic usage:
- ```
- async def main():
+ ```python
+import asyncio
+from palworld_api import PalworldAPI
+
+async def main():
     server_url = "http://localhost:8212"
     username = "admin"
     password = "admin password"
     api = PalworldAPI(server_url, username, password)
 
     server_info = await api.get_server_info()
     print("Server Info:", server_info)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Resources
- For detailed documentation on the Palworld REST API, check out the official [REST API Documentation](https://tech.palworldgame.com/api/rest-api/palwold-rest-api/).
+ For detailed documentation on the Palworld REST API, check out the official [REST API Documentation](https://tech.palworldgame.com/api/rest-api/palwold-rest-api/).
```

### Comparing `palworld-api-1.0.0/palworld_api/palworld_api.py` & `palworld-api-1.0.1/palworld_api/palworld_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,29 @@
         self.auth = aiohttp.BasicAuth(login=username, password=password)
         self.headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
 
     async def fetch(self, session, url):
         """
         General method for fetching data from a given URL.
         """
-        async with session.get(url, headers=self.headers, auth=self.auth) as response:
-            response.raise_for_status()
-            if 'application/json' in response.headers.get('Content-Type', ''):
-                return await response.json()
-            else:
-                return await response.text()
+        try:
+            async with session.get(url, headers=self.headers, auth=self.auth) as response:
+                response.raise_for_status()
+                if 'application/json' in response.headers.get('Content-Type', ''):
+                    return await response.json()
+                else:
+                    return await response.text()
+        except aiohttp.ClientResponseError as e:
+            return {'error': f'Client error {e.status}: {e.message}'}
+        except aiohttp.ClientConnectionError:
+            return {'error': 'Connection error'}
+        except asyncio.TimeoutError:
+            return {'error': 'Request timeout'}
+        except Exception as e:
+            return {'error': str(e)}
 
     async def get_server_info(self):
         """
         Retrieves server information.
         """
         async with aiohttp.ClientSession() as session:
             url = f"{self.server_url}/v1/api/info"
```

