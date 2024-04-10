# Comparing `tmp/wiliot-api-4.8.1.tar.gz` & `tmp/wiliot-api-4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.8.1.tar", last modified: Mon Apr  8 11:06:06 2024, max compression
+gzip compressed data, was "wiliot-api-4.8.2.tar", last modified: Wed Apr 10 06:56:06 2024, max compression
```

## Comparing `wiliot-api-4.8.1.tar` & `wiliot-api-4.8.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10719 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.631605 wiliot-api-4.8.1/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20455 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52463 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.635605 wiliot-api-4.8.1/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-08 11:05:47.000000 wiliot-api-4.8.1/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:06:06.631605 wiliot-api-4.8.1/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11225 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-08 11:06:06.000000 wiliot-api-4.8.1/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10787 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.382493 wiliot-api-4.8.2/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13768 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20618 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    23403 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52463 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7096 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2024-04-10 06:55:48.000000 wiliot-api-4.8.2/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 06:56:06.386493 wiliot-api-4.8.2/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2024-04-10 06:56:06.000000 wiliot-api-4.8.2/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.8.1/LICENSE` & `wiliot-api-4.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/PKG-INFO` & `wiliot-api-4.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.1
+Version: 4.8.2
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.2:
+
+* Fixed a bug in updating bridge configuration
+
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
 
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
```

### Comparing `wiliot-api-4.8.1/README.md` & `wiliot-api-4.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.2:
+
+* Fixed a bug in updating bridge configuration
+
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
 
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
```

### Comparing `wiliot-api-4.8.1/bitbucket-pipelines.yml` & `wiliot-api-4.8.2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/setup.py` & `wiliot-api-4.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/__init__.py` & `wiliot-api-4.8.2/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/api_client.py` & `wiliot-api-4.8.2/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/edge/edge.py` & `wiliot-api-4.8.2/wiliot_api/edge/edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,31 +338,34 @@
                     payload["config"][key] = config[key]
                 else:
                     print(f"Key {key} does not exist in bridge {bridge_info['id']} config")
         # Bridge configuration has a "modules" key - hierarchical configuration structure
         elif len(bridge_info.get("modules", {}).keys()):
             payload["modules"] = {}
             # If the provided config is already arranged in the required hierarchy
-            if set(config).issubset(bridge_info["modules"].keys()):
+            if set(config.keys()).issubset(bridge_info["modules"].keys()):
                 # Use the provided config as is
                 payload["modules"] = config
             else:
-                # Provided config dictionary contains leaf keys of modules - find each one's parent key and
-                # construct the payload accordingly
+                payload['modules'] = {}
                 for key in config.keys():
-                    payload['modules'] = {}
-                    try:
-                        parent_module = [m for m in bridge_info['modules'].keys() if key in list(bridge_info['modules'][m]['config'].keys())][0]
+                    if key in bridge_info["modules"].keys():
+                        payload['modules'][key] = config[key]
+                    elif key == 'version' or key == 'desiredVersion':
+                        payload['desiredVersion'] = config[key]
+                    else:
                         try:
-                            payload["modules"][parent_module][key] = config[key]
-                        except KeyError:
-                            payload["modules"][parent_module] = {key: config[key]}
-                    except IndexError:
-                        print(f"Could not find parent module for config key {key}. Will not apply it")
-                        continue
+                            parent_module = [m for m in bridge_info['modules'].keys() if key in list(bridge_info['modules'][m]['config'].keys())][0]
+                            try:
+                                payload["modules"][parent_module][key] = config[key]
+                            except KeyError:
+                                payload["modules"][parent_module] = {key: config[key]}
+                        except IndexError:
+                            print(f"Could not find parent module for config key {key}. Will not apply it")
+                            continue
         # Neither keys exist - error state
         else:
             raise Exception("Returned bridge info does not contain configuration values")
         return payload
 
     def update_bridge_configuration(self, bridge_id, config={}, name=None):
         """
@@ -426,8 +429,9 @@
         }
         try:
             res = self._post(path, payload)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to send action to bridge")
             raise WiliotCloudError(
-                "Failed to send action to bridge. Recevied the following error: {}".format(e.args[0]))
+                "Failed to send action to bridge. Received the following error: {}".format(e.args[0]))
+
```

### Comparing `wiliot-api-4.8.1/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.8.2/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.8.2/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.8.2/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.8.2/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/platform/platform.py` & `wiliot-api-4.8.2/wiliot_api/platform/platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/platform/platform_models.py` & `wiliot-api-4.8.2/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/security/security.py` & `wiliot-api-4.8.2/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api/utils/get_version.py` & `wiliot-api-4.8.2/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.8.1/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.8.2/wiliot_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.8.1
+Version: 4.8.2
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -38,14 +38,18 @@
 
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+### Version 4.8.2:
+
+* Fixed a bug in updating bridge configuration
+
 ### Version 4.8.1:
 
 * Fixed a bug in setting multiple key value pairs in a single call
 
 ### Version 4.8.0:
 
 * Added support for new labels (key:value pairs for platform entities)
```

### Comparing `wiliot-api-4.8.1/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.8.2/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

