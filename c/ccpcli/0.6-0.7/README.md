# Comparing `tmp/ccpcli-0.6.tar.gz` & `tmp/ccpcli-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpcli-0.6.tar", last modified: Thu Apr  4 16:21:48 2024, max compression
+gzip compressed data, was "ccpcli-0.7.tar", last modified: Wed Apr 10 09:44:30 2024, max compression
```

## Comparing `ccpcli-0.6.tar` & `ccpcli-0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 16:21:48.756492 ccpcli-0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/ccpcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 16:21:48.000000 ccpcli-0.6/ccpcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.752493 ccpcli-0.6/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:21:48.760492 ccpcli-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-04 16:21:36.000000 ccpcli-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.752493 ccpcli-0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-04 16:21:36.000000 ccpcli-0.6/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-04 16:21:36.000000 ccpcli-0.6/src/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/resource_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-04 16:21:36.000000 ccpcli-0.6/src/resource_schemas/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/compute/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/network/security_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/service/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 16:21:36.000000 ccpcli-0.6/src/service/volume/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:48.756492 ccpcli-0.6/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/http_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-04 16:21:36.000000 ccpcli-0.6/src/util/utils.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.144260 ccpcli-0.7/
+-rw-r--r--   0 core      (1000) core      (1000)      181 2024-04-10 09:44:30.140260 ccpcli-0.7/PKG-INFO
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/ccpcli.egg-info/
+-rw-r--r--   0 core      (1000) core      (1000)      181 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/PKG-INFO
+-rw-rw-r--   0 core      (1000) core      (1000)      771 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 core      (1000) core      (1000)        1 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 core      (1000) core      (1000)       39 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/entry_points.txt
+-rw-rw-r--   0 core      (1000) core      (1000)       20 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/requires.txt
+-rw-rw-r--   0 core      (1000) core      (1000)       14 2024-04-10 09:44:30.000000 ccpcli-0.7/ccpcli.egg-info/top_level.txt
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.136260 ccpcli-0.7/resources/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/resources/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)       38 2024-04-10 09:44:30.144260 ccpcli-0.7/setup.cfg
+-rw-rw-r--   0 core      (1000) core      (1000)      944 2024-04-10 09:43:44.000000 ccpcli-0.7/setup.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.136260 ccpcli-0.7/src/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     5762 2024-04-10 09:43:44.000000 ccpcli-0.7/src/cli.py
+-rw-rw-r--   0 core      (1000) core      (1000)     5546 2024-04-10 09:43:44.000000 ccpcli-0.7/src/project.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/resource_schemas/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/resource_schemas/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     3049 2024-04-10 09:43:44.000000 ccpcli-0.7/src/resource_schemas/compute.py
+-rw-rw-r--   0 core      (1000) core      (1000)     2864 2024-04-10 09:43:44.000000 ccpcli-0.7/src/resource_schemas/network.py
+-rw-rw-r--   0 core      (1000) core      (1000)     1223 2024-04-10 09:43:44.000000 ccpcli-0.7/src/resource_schemas/project.py
+-rw-rw-r--   0 core      (1000) core      (1000)     1124 2024-04-10 09:43:44.000000 ccpcli-0.7/src/resource_schemas/volume.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/service/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/__init__.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/service/compute/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/compute/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     3686 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/compute/instance.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/service/network/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/network/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     4132 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/network/network.py
+-rw-rw-r--   0 core      (1000) core      (1000)     1669 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/network/security_group.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/service/volume/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/volume/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     5617 2024-04-10 09:43:44.000000 ccpcli-0.7/src/service/volume/volume.py
+drwxrwxr-x   0 core      (1000) core      (1000)        0 2024-04-10 09:44:30.140260 ccpcli-0.7/src/util/
+-rw-rw-r--   0 core      (1000) core      (1000)        0 2024-04-10 09:43:44.000000 ccpcli-0.7/src/util/__init__.py
+-rw-rw-r--   0 core      (1000) core      (1000)     6142 2024-04-10 09:43:44.000000 ccpcli-0.7/src/util/constants.py
+-rw-rw-r--   0 core      (1000) core      (1000)     1593 2024-04-10 09:43:44.000000 ccpcli-0.7/src/util/file_utils.py
+-rw-rw-r--   0 core      (1000) core      (1000)     3514 2024-04-10 09:43:44.000000 ccpcli-0.7/src/util/http_helper.py
+-rw-rw-r--   0 core      (1000) core      (1000)     5026 2024-04-10 09:43:44.000000 ccpcli-0.7/src/util/utils.py
```

### Comparing `ccpcli-0.6/ccpcli.egg-info/SOURCES.txt` & `ccpcli-0.7/ccpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/setup.py` & `ccpcli-0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='ccpcli',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     author='Mani Keshari',
-    author_email='mani@coredge.io',
+    author_email='info@coredge.io',
     description='CCP cli',
     install_requires=['click', 'halo', 'tabulate'],
     entry_points={
         'console_scripts': [
             'ccpcli=src.cli:cli'
         ]
     }
 )
+
+# Note:- While changing version, make sure to change version in cli methhod too.
```

### Comparing `ccpcli-0.6/src/cli.py` & `ccpcli-0.7/src/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 urllib3.disable_warnings()
 
 __CLOUD_API_BASE_PREFIX = 'api/v1'
 
 
 @click.group()
 @click.pass_context
+@click.version_option(version='0.7', message='ccpcli %(version)s')
 def cli(ctx):
     if not ctx.obj:
         ctx.obj = {}
 
 
 def setup(ctx):
     try:
```

### Comparing `ccpcli-0.6/src/project.py` & `ccpcli-0.7/src/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/resource_schemas/compute.py` & `ccpcli-0.7/src/resource_schemas/compute.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/resource_schemas/network.py` & `ccpcli-0.7/src/resource_schemas/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/resource_schemas/project.py` & `ccpcli-0.7/src/resource_schemas/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/resource_schemas/volume.py` & `ccpcli-0.7/src/resource_schemas/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/service/compute/instance.py` & `ccpcli-0.7/src/service/compute/instance.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/service/network/network.py` & `ccpcli-0.7/src/service/network/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/service/network/security_group.py` & `ccpcli-0.7/src/service/network/security_group.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/util/constants.py` & `ccpcli-0.7/src/util/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     TABLE_HEADER_PROJECTS_DESCRIBE = COMMON_TABLE_HEADERS + ["ORGANISATION_ID", "ORGANISATION_NAME", "ACTION"]
 
     # Network Table Headers
     TABLE_HEADER_NETWORKS = replace_field(COMMON_TABLE_HEADERS, "NAME", "NETWORK_NAME") + ["MANAGED_BY"]
     TABLE_HEADER_NETWORK_DESCRIBE = TABLE_HEADER_NETWORKS + ["SUBNET_NAME", "NETWORK_ADDRESS", "GATEWAY_IP", "IP_VERSION"]
 
     # Volume Table Headers
-    TABLE_HEADER_VOLUME = replace_field(COMMON_TABLE_HEADERS, "NAME", "VOLUME_NAME") + ["VOLUME_TYPE"]
+    TABLE_HEADER_VOLUME = replace_field(COMMON_TABLE_HEADERS, "NAME", "VOLUME_NAME") + ["VOLUME_TYPE", "VOLUME_SIZE",
+                                                                                        "ACTION"]
 
     # Security Group Table Headers
     SECURITY_GROUP_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "SECURITY_GROUP_NAME") + [
         "TYPE", "MANAGED_BY", "LAST_UPDATED_AT"]
 
     # Instance Table Headers
     INSTANCE_TABLE_HEADERS = replace_field(COMMON_TABLE_HEADERS, "NAME", "INSTANCE_NAME") + [
@@ -132,19 +133,27 @@
     COMMAND_SET_DEFAULT_PROJECT = 'set-default-project'
 
 
     # Billing unit
     HOURLY_BILLING_UNIT = "HRC"
     MONTHLY_BILLING_UNIT = "MRC"
 
+    VOLUME_TYPES = {"encrypted-storage":"Encrypted Storage",
+                         "hdd-storage":"HDD Storage",
+                         "ssd-storage":"SSD Storage"}
+
+    MIN_VOLUME_SIZE = 50
+    VOLUME_STEP_SIZE = 50
+
 
 class HttpStatus:
     # Status Codes
     OK: int = 200
     CREATED: int = 201
+    ACCEPTED : int = 202
     BAD_REQUEST: int = 400
     UNAUTHORIZED: int = 401
     NO_CONTENT: int = 204
     NOT_FOUND: int = 404
     INTERNAL_SERVER_ERROR: int = 500
```

### Comparing `ccpcli-0.6/src/util/file_utils.py` & `ccpcli-0.7/src/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/util/http_helper.py` & `ccpcli-0.7/src/util/http_helper.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.6/src/util/utils.py` & `ccpcli-0.7/src/util/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,7 +176,13 @@
 
     # Format the datetime object as a string
     formatted_date_time = dt_object.strftime('%Y-%m-%d %H:%M:%S')
 
     return formatted_date_time
 
 
+def validate_size(ctx, param, value):
+    if value < Constants.MIN_VOLUME_SIZE:
+        raise click.BadParameter(f'Size must be at least {Constants.MIN_VOLUME_SIZE} GB.')
+    if value % Constants.VOLUME_STEP_SIZE != 0:
+        raise click.BadParameter(f'Size must be a multiple of {Constants.VOLUME_STEP_SIZE}.')
+    return value
```

