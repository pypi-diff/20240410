# Comparing `tmp/gama_config-2.1.0.tar.gz` & `tmp/gama_config-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_config-2.1.0.tar", last modified: Mon Oct  9 10:18:52 2023, max compression
+gzip compressed data, was "gama_config-2.2.0.tar", last modified: Wed Apr 10 12:27:42 2024, max compression
```

## Comparing `gama_config-2.1.0.tar` & `gama_config-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:52.899750 gama_config-2.1.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1694 2023-10-09 10:18:52.899750 gama_config-2.1.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      957 2023-10-09 10:17:35.000000 gama_config-2.1.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:52.899750 gama_config-2.1.0/gama_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)      147 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1848 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3530 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/gama_vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      655 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1400 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:52.899750 gama_config-2.1.0/gama_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2239 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/schemas/gama_gs.schema.json
--rw-rw-r--   0 runner    (1000) runner    (1001)     4983 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/schemas/gama_vessel.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:52.899750 gama_config-2.1.0/gama_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)      314 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/test/helpers.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2626 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/test/test_read_gama_gs_config.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6866 2023-10-09 10:17:35.000000 gama_config-2.1.0/gama_config/test/test_read_gama_vessel_config.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-10-09 10:18:52.899750 gama_config-2.1.0/gama_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1694 2023-10-09 10:18:52.000000 gama_config-2.1.0/gama_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      567 2023-10-09 10:18:52.000000 gama_config-2.1.0/gama_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-10-09 10:18:52.000000 gama_config-2.1.0/gama_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       35 2023-10-09 10:18:52.000000 gama_config-2.1.0/gama_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2023-10-09 10:18:52.000000 gama_config-2.1.0/gama_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-10-09 10:18:23.000000 gama_config-2.1.0/gama_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      863 2023-10-09 10:18:52.903751 gama_config-2.1.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-10-09 10:17:35.000000 gama_config-2.1.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.296596 gama_config-2.2.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-10 12:27:42.292596 gama_config-2.2.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      957 2024-04-10 12:26:35.000000 gama_config-2.2.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      147 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2134 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2681 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/gama_vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    15464 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      655 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3732 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/generate_urdf.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1476 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1720 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/schemas/gama_gs.schema.json
+-rw-rw-r--   0 runner    (1000) runner    (1001)     7598 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/schemas/gama_vessel.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      314 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/helpers.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      463 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_generate_urdf.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1885 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_read_gama_gs_config.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4800 2024-04-10 12:26:35.000000 gama_config-2.2.0/gama_config/test/test_read_gama_vessel_config.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:27:42.292596 gama_config-2.2.0/gama_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1761 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      667 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2024-04-10 12:27:42.000000 gama_config-2.2.0/gama_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:27:26.000000 gama_config-2.2.0/gama_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      902 2024-04-10 12:27:42.296596 gama_config-2.2.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 12:26:35.000000 gama_config-2.2.0/setup.py
```

### Comparing `gama_config-2.1.0/PKG-INFO` & `gama_config-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_config
-Version: 2.1.0
+Version: 2.2.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: dacite
 Requires-Dist: PyYAML
 Requires-Dist: dc-schema
+Requires-Dist: greenstream-config==2.12.0
+Requires-Dist: gr-urchin
 
 # GAMA Config
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
```

### Comparing `gama_config-2.1.0/README.md` & `gama_config-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_config-2.1.0/gama_config/generate_schemas.py` & `gama_config-2.2.0/gama_config/generate_schemas.py`

 * *Files identical despite different names*

### Comparing `gama_config-2.1.0/gama_config/schemas/gama_gs.schema.json` & `gama_config-2.2.0/gama_config/schemas/gama_gs.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9610780423280423%*

 * *Differences: {"'$defs'": "{'Mode': {'enum': {insert: [(7, 'single_unknown'), (8, 'dual_unknown')]}}, 'Network': "*

 * *            "{'enum': {delete: [1]}}}",*

 * * "'properties'": "{'namespace_vessel': {'default': 'vessel_1'}, 'static_peers': "*

 * *                 "OrderedDict([('anyOf', [OrderedDict([('type', 'string')]), OrderedDict([('type', "*

 * *                 "'null')])]), ('default', None)]), delete: ['ddsrouter_groundstation_ip', "*

 * *                 "'ddsrouter_groundstation_port', 'ddsrouter_vessel_ip', 'ddsrouter_vessel_port […]*

```diff
@@ -14,77 +14,34 @@
             "enum": [
                 "none",
                 "xbox",
                 "thrustmaster",
                 "thrustmaster_combo",
                 "warthog",
                 "warthog_combo",
-                "aeronav"
+                "aeronav",
+                "single_unknown",
+                "dual_unknown"
             ],
             "title": "Mode"
         },
         "Network": {
             "enum": [
                 "shared",
-                "vpn",
                 "host"
             ],
             "title": "Network"
         }
     },
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "properties": {
         "buttons": {
             "default": false,
             "type": "boolean"
         },
-        "ddsrouter_groundstation_ip": {
-            "anyOf": [
-                {
-                    "type": "string"
-                },
-                {
-                    "type": "null"
-                }
-            ],
-            "default": null
-        },
-        "ddsrouter_groundstation_port": {
-            "anyOf": [
-                {
-                    "type": "string"
-                },
-                {
-                    "type": "null"
-                }
-            ],
-            "default": null
-        },
-        "ddsrouter_vessel_ip": {
-            "anyOf": [
-                {
-                    "type": "string"
-                },
-                {
-                    "type": "null"
-                }
-            ],
-            "default": null
-        },
-        "ddsrouter_vessel_port": {
-            "anyOf": [
-                {
-                    "type": "string"
-                },
-                {
-                    "type": "null"
-                }
-            ],
-            "default": null
-        },
         "log_level": {
             "allOf": [
                 {
                     "$ref": "#/$defs/LogLevel"
                 }
             ],
             "default": "info"
@@ -98,15 +55,15 @@
             "default": "none"
         },
         "namespace_groundstation": {
             "default": "groundstation",
             "type": "string"
         },
         "namespace_vessel": {
-            "default": "vessel",
+            "default": "vessel_1",
             "type": "string"
         },
         "network": {
             "allOf": [
                 {
                     "$ref": "#/$defs/Network"
                 }
@@ -120,12 +77,23 @@
         "remote_cmd_override": {
             "default": false,
             "type": "boolean"
         },
         "ros_domain_id": {
             "default": 0,
             "type": "integer"
+        },
+        "static_peers": {
+            "anyOf": [
+                {
+                    "type": "string"
+                },
+                {
+                    "type": "null"
+                }
+            ],
+            "default": null
         }
     },
     "title": "GamaGsConfig",
     "type": "object"
 }
```

### Comparing `gama_config-2.1.0/gama_config.egg-info/PKG-INFO` & `gama_config-2.2.0/gama_config.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama-config
-Version: 2.1.0
+Name: gama_config
+Version: 2.2.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: dacite
 Requires-Dist: PyYAML
 Requires-Dist: dc-schema
+Requires-Dist: greenstream-config==2.12.0
+Requires-Dist: gr-urchin
 
 # GAMA Config
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
```

### Comparing `gama_config-2.1.0/gama_config.egg-info/SOURCES.txt` & `gama_config-2.2.0/gama_config.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 README.md
 setup.cfg
 setup.py
 gama_config/__init__.py
 gama_config/gama_gs.py
 gama_config/gama_vessel.py
+gama_config/generate_cameras.py
 gama_config/generate_schemas.py
+gama_config/generate_urdf.py
 gama_config/helpers.py
 gama_config.egg-info/PKG-INFO
 gama_config.egg-info/SOURCES.txt
 gama_config.egg-info/dependency_links.txt
 gama_config.egg-info/requires.txt
 gama_config.egg-info/top_level.txt
 gama_config.egg-info/zip-safe
 gama_config/schemas/gama_gs.schema.json
 gama_config/schemas/gama_vessel.schema.json
 gama_config/test/helpers.py
+gama_config/test/test_generate_urdf.py
 gama_config/test/test_read_gama_gs_config.py
 gama_config/test/test_read_gama_vessel_config.py
```

### Comparing `gama_config-2.1.0/setup.cfg` & `gama_config-2.2.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_config
-version = 2.1.0
+version = 2.2.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -22,14 +22,16 @@
 [options]
 packages = find:
 install_requires = 
 	setuptools
 	dacite
 	PyYAML
 	dc-schema
+	greenstream-config==2.12.0
+	gr-urchin
 zip_safe = true
 
 [options.package_data]
 gama_config = 
 	**/*.json
 	**/*.py
```

