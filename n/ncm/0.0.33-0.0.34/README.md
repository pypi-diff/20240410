# Comparing `tmp/ncm-0.0.33.tar.gz` & `tmp/ncm-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.33.tar", last modified: Tue Apr  9 15:51:41 2024, max compression
+gzip compressed data, was "ncm-0.0.34.tar", last modified: Wed Apr 10 19:46:00 2024, max compression
```

## Comparing `ncm-0.0.33.tar` & `ncm-0.0.34.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.222190 ncm-0.0.33/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.33/LICENSE
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-09 15:51:41.221190 ncm-0.0.33/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.33/README.md
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.221190 ncm-0.0.33/ncm/
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.33/ncm/__init__.py
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   148254 2024-04-08 23:21:43.000000 ncm-0.0.33/ncm/ncm.py
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-09 15:51:41.221190 ncm-0.0.33/ncm.egg-info/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/requires.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-09 15:51:41.000000 ncm-0.0.33/ncm.egg-info/top_level.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-09 15:51:41.222190 ncm-0.0.33/setup.cfg
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-09 15:49:48.000000 ncm-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.207752 ncm-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:45:46.000000 ncm-0.0.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-10 19:46:00.203752 ncm-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-10 19:45:46.000000 ncm-0.0.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.203752 ncm-0.0.34/ncm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:45:46.000000 ncm-0.0.34/ncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148216 2024-04-10 19:45:46.000000 ncm-0.0.34/ncm/ncm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.203752 ncm-0.0.34/ncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:46:00.207752 ncm-0.0.34/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-04-10 19:45:46.000000 ncm-0.0.34/setup.py
```

### Comparing `ncm-0.0.33/LICENSE` & `ncm-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.33/PKG-INFO` & `ncm-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.33
+Version: 0.0.34
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.33/README.md` & `ncm-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.33/ncm/ncm.py` & `ncm-0.0.34/ncm/ncm.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     You can also return the full list of records in a single array without
     the need for paging by passing limit='all':
        n.get_accounts(limit='all')
 
     It also has native support for handling any number of "__in" filters
     beyond Cradlepoint's limit of 100. The script automatically chunks
-    the list into groups of 100 and combines the results into a single array.
+    the list into groups of 100 and combines the results into a single array
 """
 
 from requests import Session
 from requests.adapters import HTTPAdapter
 from http import HTTPStatus
 from urllib3.util.retry import Retry
 from datetime import datetime, timedelta
@@ -2447,61 +2447,61 @@
                           'fields',
                           'limit',
                           'sort']
 
         params = self.__parse_kwargs(kwargs, allowed_params)
         return self.__get_json(get_url, call_type, params=params)
     
-    def regrade(self, subscription_id, mac_or_serial_number=None):
+    def regrade(self, subscription_id, mac_or_serial_number, action="UPGRADE"):
         """ 
         Applies a subscription to an asset.
-        :param subscription_id: ID of the subscription to apply. (see https://developer.cradlepoint.com/ for list of subscriptions)
-        :param asset_id: ID of the asset to apply the subscription to. If not provided, the MAC address must be provided. Can also be a list
-        :param mac: MAC address of the asset to apply the subscription to. If not provided, the asset_id must be provided. Can also be a list.
+        :param subscription_id: ID of the subscription to apply. See https://developer.cradlepoint.com/ for list of subscriptions.
+        :param mac_or_serial_number: MAC address or serial number of the asset to apply the subscription to. Can also be a list.
+        :param action: Action to take. Default is "UPGRADE". Can also be "DOWNGRADE".
         """
 
         call_type = 'Subscription'
-        post_url = f'{self.base_url}/asset_endpoints/regrade'
+        post_url = f'{self.base_url}/asset_endpoints/regrades'
 
         payload = {
             "atomic:operations": []
         }
         mac_or_serial_number = mac_or_serial_number if isinstance(mac_or_serial_number, list) else [mac_or_serial_number]
         for smac in mac_or_serial_number:
             data = {
                 "op": "add",
                 "data": {
                     "type": "regrades",
                     "attributes": {
-                        "action": "UPGRADE",
+                        "action": action,
                         "subscription_type": subscription_id
                     }
                 }
             }
             if len(smac) == 17:
                 data['data']['attributes']['mac_address'] = smac.replace(':','')
             elif len(smac) == 12:
                 data['data']['attributes']['mac_address'] = smac
             else:
                 data['data']['attributes']['serial_number'] = smac
-            payload.append(data)
+            payload["atomic:operations"].append(data)
 
         ncm = self.session.post(post_url, json=payload)
         result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def get_regrades(self, **kwargs):
         """
         Returns regrade jobs with details.
         :param kwargs: A set of zero or more allowed parameters
           in the allowed_params list.
         :return: A list of regrades with details.
         """
         call_type = 'Subscription'
-        get_url = f'{self.base_url}/asset_endpoints/regrade'
+        get_url = f'{self.base_url}/asset_endpoints/regrades'
 
         allowed_params = ["id", 
                     "action_id", 
                     "mac_address", 
                     "created_at", 
                     "action", 
                     "subcription_type",
```

### Comparing `ncm-0.0.33/ncm.egg-info/PKG-INFO` & `ncm-0.0.34/ncm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.33
+Version: 0.0.34
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.33/setup.py` & `ncm-0.0.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.33",
+    version="0.0.34",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

