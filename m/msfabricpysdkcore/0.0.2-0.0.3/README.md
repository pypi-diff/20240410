# Comparing `tmp/msfabricpysdkcore-0.0.2.tar.gz` & `tmp/msfabricpysdkcore-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.2.tar", last modified: Wed Apr  3 10:07:34 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.3.tar", last modified: Wed Apr 10 07:50:21 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.2.tar` & `msfabricpysdkcore-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:07:34.944567 msfabricpysdkcore-0.0.2/
--rw-rw-rw-   0        0        0     1156 2024-04-03 08:33:35.000000 msfabricpysdkcore-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    11319 2024-04-03 10:07:34.942563 msfabricpysdkcore-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    10799 2024-04-03 09:56:17.000000 msfabricpysdkcore-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 10:07:34.879469 msfabricpysdkcore-0.0.2/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       36 2024-04-03 05:52:03.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0    12536 2024-04-02 19:42:14.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    10188 2024-04-02 13:38:41.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2759 2024-04-02 13:32:39.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     3021 2024-04-02 12:46:53.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2033 2024-03-28 05:21:57.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/onelakeshortcut.py
--rw-rw-rw-   0        0        0    19796 2024-04-02 12:41:33.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:07:34.934292 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    11319 2024-04-03 10:07:34.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-04-03 10:07:34.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:07:34.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-03 10:07:34.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 10:07:34.000000 msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-03 10:07:26.000000 msfabricpysdkcore-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 10:07:34.945571 msfabricpysdkcore-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-03 08:30:56.000000 msfabricpysdkcore-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.701844 msfabricpysdkcore-0.0.3/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12511 2024-04-10 07:50:21.699851 msfabricpysdkcore-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11991 2024-04-10 05:54:29.000000 msfabricpysdkcore-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.607255 msfabricpysdkcore-0.0.3/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       36 2024-04-03 05:52:03.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1696 2024-04-09 16:57:48.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0    15047 2024-04-10 05:29:31.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    11086 2024-04-10 05:11:49.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2759 2024-04-02 13:32:39.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     4011 2024-04-09 16:58:34.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     3021 2024-04-02 12:46:53.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2033 2024-03-28 05:21:57.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/onelakeshortcut.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.692327 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2397 2024-04-02 10:23:19.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0     2940 2024-04-10 05:26:30.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1643 2024-04-02 13:24:07.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2389 2024-03-28 05:22:31.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6562 2024-04-10 05:15:10.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    21475 2024-04-10 05:31:51.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-10 07:50:21.696841 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    12511 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-10 07:50:21.000000 msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-04 12:17:39.000000 msfabricpysdkcore-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 07:50:21.701844 msfabricpysdkcore-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-10 07:48:09.000000 msfabricpysdkcore-0.0.3/setup.py
```

### Comparing `msfabricpysdkcore-0.0.2/LICENSE` & `msfabricpysdkcore-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.2/PKG-INFO` & `msfabricpysdkcore-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.30.0
 Requires-Dist: azure-identity>=1.15.0
 
 # A Python SDK for Microsoft Fabric
 
-This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs of Fabric*.
+This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs (v1) of Fabric*.
 
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
 - Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
-- Do bulk operations**
-- Pagination support**
+- Do bulk operations (see [Usage Patterns](usage_patterns.md))
+- Pagination support
 
-Currently it supports all Core APIs, i.e.:
+See the latest release notes [here](releasenotes/release_notes.md).
+
+Currently it supports all Core APIs and Lakehouse APIs, i.e.:
 - [Capacities](#working-with-capacities)
 - [Git](#working-with-git)
 - [Items](#working-with-items)
 - [Job Scheduler](#working-with-job-scheduler)
 - Long Running Operations
 - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
 - [Workspaces](#working-with-workspaces)
+- [Lakehouse APIs](#lakehouse-apis)
 
-It is planned to support also the Admin and Lakehouse APIs and new APIs which are not released yet.
+It is planned to support also the Admin APIs and new APIs which are not released yet.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
-**These features are not yet implemented but are planned for the near future.
 
 
 
 ## Installation
 
 ```bash
 pip install msfabricpysdkcore
@@ -156,19 +158,24 @@
 
 ```
 
 ### Working with capacities
 
 ```python
 
+
+capacity_object = fc.get_capacity(capacity_id = "0129389012u8938491") 
+#or 
+capacity_object = fc.get_capacity(capacity_name = "sandboxcapacitygermanywc") 
+
 # Assign a capaycity to a workspace
 fc.assign_to_capacity(workspace_id=workspace_id,
-                      capacity_id="capacityid123123")
+                      capacity_id=capacity_object.id)
 # or
-ws.assign_to_capacity(capacity_id="capacityid123123")      
+ws.assign_to_capacity(capacity_id=capacity_object.id)      
 
 # Unassign from capacity
 fc.unassign_from_capacity(workspace_id=ws.id)
 # or
 ws.unassign_from_capacity()
 
 
@@ -355,11 +362,38 @@
 # or
 ws.cancel_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or 
 item.cancel_item_job_instance(job_instance_id="job_instance_id")
 
 ```
 
+## Lakehouse APIs
 
+# List tables in a Lakehouse
+
+```python
+from msfabricpysdkcore import FabricClientCore
+
+fc = FabricClientCore()
+ws = fc.get_workspace_by_name("testworkspace")
+lakehouse = ws.get_item_by_name(item_name="lakehouse1", item_type="Lakehouse")
+table_list = lakehouse.list_tables()
+# or
+table_list = ws.list_tables(item_id = "someitemid")
+# or
+table_list = fc.list_tables(workspace_id = "someworkspaceid", item_id = "someitemid")
+
+
+# Load a file (like a csv) into a Lakehouse table
+
+lakehouse.load_table(table_name="testtable", path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+ws.load_table(item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+fc.load_table(workspace_id = "someworkspaceid", item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+
+```
 
 Note: This SDK is not an official SDK from Microsoft. It is a community project and not supported by Microsoft. Use it at your own risk.
 Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
```

### Comparing `msfabricpysdkcore-0.0.2/README.md` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+Metadata-Version: 2.1
+Name: msfabricpysdkcore
+Version: 0.0.3
+Summary: A Python SDK for Microsoft Fabric
+Author: Andreas Rederer
+Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.30.0
+Requires-Dist: azure-identity>=1.15.0
+
 # A Python SDK for Microsoft Fabric
 
-This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs of Fabric*.
+This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs (v1) of Fabric*.
 
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
 - Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
-- Do bulk operations**
-- Pagination support**
+- Do bulk operations (see [Usage Patterns](usage_patterns.md))
+- Pagination support
+
+See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs, i.e.:
+Currently it supports all Core APIs and Lakehouse APIs, i.e.:
 - [Capacities](#working-with-capacities)
 - [Git](#working-with-git)
 - [Items](#working-with-items)
 - [Job Scheduler](#working-with-job-scheduler)
 - Long Running Operations
 - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
 - [Workspaces](#working-with-workspaces)
+- [Lakehouse APIs](#lakehouse-apis)
 
-It is planned to support also the Admin and Lakehouse APIs and new APIs which are not released yet.
+It is planned to support also the Admin APIs and new APIs which are not released yet.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
-**These features are not yet implemented but are planned for the near future.
 
 
 
 ## Installation
 
 ```bash
 pip install msfabricpysdkcore
@@ -141,19 +158,24 @@
 
 ```
 
 ### Working with capacities
 
 ```python
 
+
+capacity_object = fc.get_capacity(capacity_id = "0129389012u8938491") 
+#or 
+capacity_object = fc.get_capacity(capacity_name = "sandboxcapacitygermanywc") 
+
 # Assign a capaycity to a workspace
 fc.assign_to_capacity(workspace_id=workspace_id,
-                      capacity_id="capacityid123123")
+                      capacity_id=capacity_object.id)
 # or
-ws.assign_to_capacity(capacity_id="capacityid123123")      
+ws.assign_to_capacity(capacity_id=capacity_object.id)      
 
 # Unassign from capacity
 fc.unassign_from_capacity(workspace_id=ws.id)
 # or
 ws.unassign_from_capacity()
 
 
@@ -340,11 +362,38 @@
 # or
 ws.cancel_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or 
 item.cancel_item_job_instance(job_instance_id="job_instance_id")
 
 ```
 
+## Lakehouse APIs
+
+# List tables in a Lakehouse
+
+```python
+from msfabricpysdkcore import FabricClientCore
+
+fc = FabricClientCore()
+ws = fc.get_workspace_by_name("testworkspace")
+lakehouse = ws.get_item_by_name(item_name="lakehouse1", item_type="Lakehouse")
+table_list = lakehouse.list_tables()
+# or
+table_list = ws.list_tables(item_id = "someitemid")
+# or
+table_list = fc.list_tables(workspace_id = "someworkspaceid", item_id = "someitemid")
+
+
+# Load a file (like a csv) into a Lakehouse table
 
+lakehouse.load_table(table_name="testtable", path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+ws.load_table(item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+fc.load_table(workspace_id = "someworkspaceid", item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+
+```
 
 Note: This SDK is not an official SDK from Microsoft. It is a community project and not supported by Microsoft. Use it at your own risk.
-Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
+Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
```

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/auth.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/item.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests
 from time import sleep
 
 from msfabricpysdkcore.onelakeshortcut import OneLakeShortcut
 from msfabricpysdkcore.job_instance import JobInstance
 from msfabricpysdkcore.long_running_operation import check_long_running_operation
 
+
 class Item:
     """Class to represent a item in Microsoft Fabric"""
 
     def __init__(self, id, display_name, type, workspace_id, auth, properties = None, definition=None, description="") -> None:
         
         self.id = id
         self.display_name = display_name
@@ -32,14 +33,20 @@
             'workspace_id': self.workspace_id,
             'properties': self.properties
         }
         return json.dumps(dict_, indent=2)
     
     def from_dict(item_dict, auth):
         """Create Item object from dictionary"""
+        
+        if item_dict['type'] == "Lakehouse":
+            from msfabricpysdkcore.lakehouse import Lakehouse
+            return Lakehouse(id=item_dict['id'], display_name=item_dict['displayName'], type=item_dict['type'], workspace_id=item_dict['workspaceId'],
+                    properties=item_dict.get('properties', None),
+                    definition=item_dict.get('definition', None), description=item_dict.get('description', ""), auth=auth)
         return Item(id=item_dict['id'], display_name=item_dict['displayName'], type=item_dict['type'], workspace_id=item_dict['workspaceId'],
                     properties=item_dict.get('properties', None),
                     definition=item_dict.get('definition', None), description=item_dict.get('description', ""), auth=auth)
 
     def delete(self):
         """Delete the workspace item"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/items/{self.id}"
@@ -48,14 +55,15 @@
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
+                print(self)
                 raise Exception(f"Error deleting item: {response.text}")
             break
 
         return response.status_code
     
     def get_definition(self):
         """Get the definition of the item"""
@@ -239,8 +247,15 @@
         job_dict['workspaceId'] = self.workspace_id
         job_dict['itemId'] = self.id
         return JobInstance.from_dict(job_dict, auth=self.auth)
     
     def cancel_item_job_instance(self, job_instance_id):
         """Cancel a job instance ofjob the item"""
         return self.get_item_job_instance(job_instance_id=job_instance_id).cancel()
-        
+        
+    def list_tables(self):
+        raise NotImplementedError("List tables only works on Lakehouse Items")
+    
+    def load_table(self, table_name, path_type, relative_path,
+                    file_extension = None, format_options = None,
+                    mode = None, recursive = None, wait_for_completion = True):
+        raise NotImplementedError("Load table only works on Lakehouse Items")
```

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/job_instance.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.3/msfabricpysdkcore/workspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -236,60 +236,87 @@
             if response.status_code == 202:
                 check_long_running_operation( response.headers, self.auth)
             if response.status_code not in (201, 202, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error creating item: {response.text}")
             break
-        
+
         item_dict = json.loads(response.text)
+        if item_dict is None:
+            print("Item not returned by API, trying to get it by name")
+            return self.get_item_by_name(display_name, type)        
         return Item.from_dict(item_dict, auth=self.auth)
         
 
-    def get_item(self, item_id):
+    def get_item_by_name(self, item_name, item_type):
+        """Get an item from a workspace by name"""
+        ws_items = self.list_items()
+        for item in ws_items:
+            if item.display_name == item_name and item.type == item_type:
+                return item    
+
+    def get_item(self, item_id = None, item_name = None, item_type = None):
         # GET https://api.fabric.microsoft.com/v1/workspaces/{workspaceId}/items/{itemId}
         """Get an item from a workspace"""
+        if item_id is None and item_name is not None and item_type is not None:
+            return self.get_item_by_name(item_name, item_type)
+        elif item_id is None:
+            raise Exception("item_id or the combination item_name + item_type is required")
+        
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/items/{item_id}"
 
         for _ in range(10):
             response = requests.get(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
-                raise Exception(f"Error getting item capacity: {response.text}")
+                raise Exception(f"Error getting item: {response.text}")
             break
         
         item_dict = json.loads(response.text)
         return Item.from_dict(item_dict, auth=self.auth)
 
     def delete_item(self, item_id):
         """Delete an item from a workspace"""
         return self.get_item(item_id).delete()
+  
 
-    def list_items(self):
+    def list_items(self, continuationToken = None):
         """List items in a workspace"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.id}/items"
 
+        if continuationToken:
+            url = f"{url}?continuationToken={continuationToken}"
+
         for _ in range(10):
             response = requests.get(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error listing items: {response.text}")
             break
-        items = json.loads(response.text)["value"]
-        return [Item.from_dict(item, auth=self.auth) for item in items]
+        
+        resp_dict = json.loads(response.text)
+        items = resp_dict["value"]
+        items = [Item.from_dict(item, auth=self.auth) for item in items]
+
+        if "continuationToken" in resp_dict:
+            item_list_next = self.list_items(continuationToken=resp_dict["continuationToken"])
+            items.extend(item_list_next)
+
+        return items
     
     def get_item_definition(self, item_id):
         """Get the definition of an item from a workspace"""
         return self.get_item(item_id).get_definition()
     
     def update_item(self, item_id, display_name = None, description = None):
         """Update an item in a workspace"""
@@ -474,8 +501,18 @@
 
             if response.status_code not in (200, 202, 429):
                 print(response.status_code)
                 print(response.text)
                 raise Exception(f"Error updating from git: {response.text}")
             break
 
-        return response.status_code
+        return response.status_code
+    
+    def list_tables(self, item_id):
+        return self.get_item(item_id=item_id).list_tables()
+    
+    def load_table(self, item_id, table_name, path_type, relative_path,
+                    file_extension = None, format_options = None,
+                    mode = None, recursive = None, wait_for_completion = True):
+        return self.get_item(item_id).load_table(table_name, path_type, relative_path,
+                    file_extension, format_options,
+                    mode, recursive, wait_for_completion)
```

### Comparing `msfabricpysdkcore-0.0.2/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-Metadata-Version: 2.1
-Name: msfabricpysdkcore
-Version: 0.0.2
-Summary: A Python SDK for Microsoft Fabric
-Author: Andreas Rederer
-Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.30.0
-Requires-Dist: azure-identity>=1.15.0
-
 # A Python SDK for Microsoft Fabric
 
-This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs of Fabric*.
+This is a Python SDK for Microsoft Fabric. It is a wrapper around the REST APIs (v1) of Fabric*.
 
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
 - Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
-- Do bulk operations**
-- Pagination support**
+- Do bulk operations (see [Usage Patterns](usage_patterns.md))
+- Pagination support
+
+See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs, i.e.:
+Currently it supports all Core APIs and Lakehouse APIs, i.e.:
 - [Capacities](#working-with-capacities)
 - [Git](#working-with-git)
 - [Items](#working-with-items)
 - [Job Scheduler](#working-with-job-scheduler)
 - Long Running Operations
 - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
 - [Workspaces](#working-with-workspaces)
+- [Lakehouse APIs](#lakehouse-apis)
 
-It is planned to support also the Admin and Lakehouse APIs and new APIs which are not released yet.
+It is planned to support also the Admin APIs and new APIs which are not released yet.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
-**These features are not yet implemented but are planned for the near future.
 
 
 
 ## Installation
 
 ```bash
 pip install msfabricpysdkcore
@@ -156,19 +143,24 @@
 
 ```
 
 ### Working with capacities
 
 ```python
 
+
+capacity_object = fc.get_capacity(capacity_id = "0129389012u8938491") 
+#or 
+capacity_object = fc.get_capacity(capacity_name = "sandboxcapacitygermanywc") 
+
 # Assign a capaycity to a workspace
 fc.assign_to_capacity(workspace_id=workspace_id,
-                      capacity_id="capacityid123123")
+                      capacity_id=capacity_object.id)
 # or
-ws.assign_to_capacity(capacity_id="capacityid123123")      
+ws.assign_to_capacity(capacity_id=capacity_object.id)      
 
 # Unassign from capacity
 fc.unassign_from_capacity(workspace_id=ws.id)
 # or
 ws.unassign_from_capacity()
 
 
@@ -355,11 +347,38 @@
 # or
 ws.cancel_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or 
 item.cancel_item_job_instance(job_instance_id="job_instance_id")
 
 ```
 
+## Lakehouse APIs
+
+# List tables in a Lakehouse
+
+```python
+from msfabricpysdkcore import FabricClientCore
+
+fc = FabricClientCore()
+ws = fc.get_workspace_by_name("testworkspace")
+lakehouse = ws.get_item_by_name(item_name="lakehouse1", item_type="Lakehouse")
+table_list = lakehouse.list_tables()
+# or
+table_list = ws.list_tables(item_id = "someitemid")
+# or
+table_list = fc.list_tables(workspace_id = "someworkspaceid", item_id = "someitemid")
+
+
+# Load a file (like a csv) into a Lakehouse table
 
+lakehouse.load_table(table_name="testtable", path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+ws.load_table(item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+# or
+fc.load_table(workspace_id = "someworkspaceid", item_id = "someitemid", table_name="testtable",
+              path_type= "File", relative_path="Files/folder1/titanic.csv")
+
+```
 
 Note: This SDK is not an official SDK from Microsoft. It is a community project and not supported by Microsoft. Use it at your own risk.
-Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
+Also the API is still in preview and might change. This SDK is not yet feature complete and might not cover all APIs yet. Feel free to contribute to this project to make it better.
```

### Comparing `msfabricpysdkcore-0.0.2/pyproject.toml` & `msfabricpysdkcore-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.2"
+version = "0.0.3"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.11"
```

