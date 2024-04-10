# Comparing `tmp/cloud_orbit_api-1.1.18.tar.gz` & `tmp/cloud_orbit_api-1.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_orbit_api-1.1.18.tar", max compression
+gzip compressed data, was "cloud_orbit_api-1.1.19.tar", max compression
```

## Comparing `cloud_orbit_api-1.1.18.tar` & `cloud_orbit_api-1.1.19.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-04-09 17:31:14.544275 cloud_orbit_api-1.1.18/README.md
--rw-r--r--   0        0        0        0 2024-04-09 17:31:14.544275 cloud_orbit_api-1.1.18/cloud_orbit_api/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-09 17:31:14.544275 cloud_orbit_api-1.1.18/cloud_orbit_api/db_factory.py
--rw-r--r--   0        0        0     1670 2024-04-09 17:31:14.544275 cloud_orbit_api-1.1.18/cloud_orbit_api/main.py
--rw-r--r--   0        0        0       90 2024-04-09 17:31:14.544275 cloud_orbit_api-1.1.18/cloud_orbit_api/models.py
--rw-r--r--   0        0        0      494 2024-04-09 17:31:27.596397 cloud_orbit_api-1.1.18/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.18/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-09 19:45:39.608920 cloud_orbit_api-1.1.19/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 19:45:39.608920 cloud_orbit_api-1.1.19/cloud_orbit_api/__init__.py
+-rw-r--r--   0        0        0     1123 2024-04-09 19:45:39.608920 cloud_orbit_api-1.1.19/cloud_orbit_api/db_factory.py
+-rw-r--r--   0        0        0     2092 2024-04-09 19:45:39.608920 cloud_orbit_api-1.1.19/cloud_orbit_api/main.py
+-rw-r--r--   0        0        0       90 2024-04-09 19:45:39.608920 cloud_orbit_api-1.1.19/cloud_orbit_api/models.py
+-rw-r--r--   0        0        0      494 2024-04-09 19:45:52.993034 cloud_orbit_api-1.1.19/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 cloud_orbit_api-1.1.19/PKG-INFO
```

### Comparing `cloud_orbit_api-1.1.18/cloud_orbit_api/db_factory.py` & `cloud_orbit_api-1.1.19/cloud_orbit_api/db_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-1.1.18/cloud_orbit_api/main.py` & `cloud_orbit_api-1.1.19/cloud_orbit_api/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from fastapi import FastAPI, HTTPException
 import os
 from cloud_orbit_api.models import item
 from cloud_orbit_api.db_factory import SQLiteSingleton
 from fastapi.middleware.cors import CORSMiddleware
 
 # Define the FastAPI app
-app = FastAPI(root_path="backend")
+app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
@@ -23,14 +23,25 @@
 # Endpoint to create an item
 @app.post("/items/")
 async def create_item(item: item):
     SQLiteSingleton._instance.cursor.execute(''' INSERT INTO items (name, description) VALUES (?, ?)''', (item.name, item.description))
     SQLiteSingleton._instance.conn.commit()
     return {"name": item.name, "description": item.description}
 
+# Delete item by index
+@app.delete("/items/{item_index}")
+async def delete_item(item_index: int):
+    try:
+        # Delete the item from the database
+        SQLiteSingleton._instance.cursor.execute('''DELETE FROM items WHERE id = ?''', (item_index,))
+        SQLiteSingleton._instance.conn.commit()
+        return {"message": f"Item at index {item_index} deleted successfully"}
+    except Exception as e:
+        return {"error": str(e)}
+
 # Endpoint to retrieve an item by ID
 @app.get("/items/all")
 async def read_all_items():
     SQLiteSingleton._instance.cursor.execute('''SELECT id, name, description FROM items''')
     items = SQLiteSingleton._instance.cursor.fetchall()
     for item in items:
         print(item)
```

### Comparing `cloud_orbit_api-1.1.18/PKG-INFO` & `cloud_orbit_api-1.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-orbit-api
-Version: 1.1.18
+Version: 1.1.19
 Summary: This a demo project
 Author: sukruth grandhi
 Author-email: sukruthgrandhi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

