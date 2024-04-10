# Comparing `tmp/redfish_utilities-3.2.7.tar.gz` & `tmp/redfish_utilities-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.2.7.tar", last modified: Fri Mar  1 20:37:48 2024, max compression
+gzip compressed data, was "redfish_utilities-3.2.8.tar", last modified: Wed Apr 10 18:56:26 2024, max compression
```

## Comparing `redfish_utilities-3.2.7.tar` & `redfish_utilities-3.2.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:37:48.282864 redfish_utilities-3.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-01 20:37:48.282864 redfish_utilities-3.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:37:48.278864 redfish_utilities-3.2.7/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24708 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/power_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:37:48.282864 redfish_utilities-3.2.7/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-01 20:37:47.000000 redfish_utilities-3.2.7/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-01 20:37:47.000000 redfish_utilities-3.2.7/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:37:47.000000 redfish_utilities-3.2.7/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-01 20:37:47.000000 redfish_utilities-3.2.7/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-01 20:37:47.000000 redfish_utilities-3.2.7/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:37:48.282864 redfish_utilities-3.2.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_power_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_test_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 20:37:48.282864 redfish_utilities-3.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-01 20:37:33.000000 redfish_utilities-3.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.685970 redfish_utilities-3.2.8/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24708 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/power_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24116 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_power_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_test_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/setup.py
```

### Comparing `redfish_utilities-3.2.7/LICENSE.md` & `redfish_utilities-3.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/PKG-INFO` & `redfish_utilities-3.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.2.7
+Version: 3.2.8
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.2.7/README.md` & `redfish_utilities-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/__init__.py` & `redfish_utilities-3.2.8/redfish_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/accounts.py` & `redfish_utilities-3.2.8/redfish_utilities/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/assembly.py` & `redfish_utilities-3.2.8/redfish_utilities/assembly.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/certificates.py` & `redfish_utilities-3.2.8/redfish_utilities/certificates.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/collections.py` & `redfish_utilities-3.2.8/redfish_utilities/collections.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/config.py` & `redfish_utilities-3.2.8/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/event_service.py` & `redfish_utilities-3.2.8/redfish_utilities/event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/inventory.py` & `redfish_utilities-3.2.8/redfish_utilities/inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/licenses.py` & `redfish_utilities-3.2.8/redfish_utilities/licenses.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/logs.py` & `redfish_utilities-3.2.8/redfish_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/managers.py` & `redfish_utilities-3.2.8/redfish_utilities/managers.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/messages.py` & `redfish_utilities-3.2.8/redfish_utilities/messages.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/misc.py` & `redfish_utilities-3.2.8/redfish_utilities/misc.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/power_equipment.py` & `redfish_utilities-3.2.8/redfish_utilities/power_equipment.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/resets.py` & `redfish_utilities-3.2.8/redfish_utilities/resets.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/sensors.py` & `redfish_utilities-3.2.8/redfish_utilities/sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             "ChassisName": chassis_name,
             "Readings": []
         }
         sensor_list.append( chassis_instance )
         get_discrete_status( "State", chassis.dict, chassis_instance["Readings"] )
 
         # If the chassis contains any of the newer power/thermal models, scan based on the common sensor model
-        if "EnvironmentMetrics" in chassis.dict or "PowerSubsystem" in chassis.dict or "ThermalSubsystem" in chassis.dict:
+        if "EnvironmentMetrics" in chassis.dict or "PowerSubsystem" in chassis.dict or "ThermalSubsystem" in chassis.dict or "Sensors" in chassis.dict:
             # Get readings from the EnvironmentMetrics resource if available
             if "EnvironmentMetrics" in chassis.dict:
                 environment = context.get( chassis.dict["EnvironmentMetrics"]["@odata.id"] )
                 get_excerpt_status( chassis_instance["ChassisName"], "TemperatureCelsius", "Cel", environment.dict, chassis_instance["Readings"] )
                 get_excerpt_status( chassis_instance["ChassisName"], "HumidityPercent", "%", environment.dict, chassis_instance["Readings"] )
                 get_excerpt_status( chassis_instance["ChassisName"], "PowerWatts", "W", environment.dict, chassis_instance["Readings"] )
                 get_excerpt_status( chassis_instance["ChassisName"], "EnergykWh", "kW.h", environment.dict, chassis_instance["Readings"] )
```

### Comparing `redfish_utilities-3.2.7/redfish_utilities/systems.py` & `redfish_utilities-3.2.8/redfish_utilities/systems.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/tasks.py` & `redfish_utilities-3.2.8/redfish_utilities/tasks.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities/update.py` & `redfish_utilities-3.2.8/redfish_utilities/update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.2.8/redfish_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.2.7
+Version: 3.2.8
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_utilities-3.2.7/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.2.8/redfish_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_accounts.py` & `redfish_utilities-3.2.8/scripts/rf_accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_assembly.py` & `redfish_utilities-3.2.8/scripts/rf_assembly.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_bios_settings.py` & `redfish_utilities-3.2.8/scripts/rf_bios_settings.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_boot_override.py` & `redfish_utilities-3.2.8/scripts/rf_boot_override.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_certificates.py` & `redfish_utilities-3.2.8/scripts/rf_certificates.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.2.8/scripts/rf_diagnostic_data.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_discover.py` & `redfish_utilities-3.2.8/scripts/rf_discover.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_event_service.py` & `redfish_utilities-3.2.8/scripts/rf_event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_licenses.py` & `redfish_utilities-3.2.8/scripts/rf_licenses.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_logs.py` & `redfish_utilities-3.2.8/scripts/rf_logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_manager_config.py` & `redfish_utilities-3.2.8/scripts/rf_manager_config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_power_equipment.py` & `redfish_utilities-3.2.8/scripts/rf_power_equipment.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_power_reset.py` & `redfish_utilities-3.2.8/scripts/rf_power_reset.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_raw_request.py` & `redfish_utilities-3.2.8/scripts/rf_raw_request.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_sensor_list.py` & `redfish_utilities-3.2.8/scripts/rf_sensor_list.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_sys_inventory.py` & `redfish_utilities-3.2.8/scripts/rf_sys_inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_test_event_listener.py` & `redfish_utilities-3.2.8/scripts/rf_test_event_listener.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_update.py` & `redfish_utilities-3.2.8/scripts/rf_update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/scripts/rf_virtual_media.py` & `redfish_utilities-3.2.8/scripts/rf_virtual_media.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.7/setup.py` & `redfish_utilities-3.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             self.pyinstaller(scripts)
 
 with open( "README.md", "r", "utf-8" ) as f:
     long_description = f.read()
 
 setup(
     name = "redfish_utilities",
-    version = "3.2.7",
+    version = "3.2.8",
     description = "Redfish Utilities",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "DMTF, https://www.dmtf.org/standards/feedback",
     license = "BSD 3-clause \"New\" or \"Revised License\"",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
```

