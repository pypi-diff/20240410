# Comparing `tmp/merakicat-0.2.0.tar.gz` & `tmp/merakicat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.2.0.tar", last modified: Wed Apr 10 14:58:18 2024, max compression
+gzip compressed data, was "merakicat-0.2.1.tar", last modified: Wed Apr 10 16:26:03 2024, max compression
```

## Comparing `merakicat-0.2.0.tar` & `merakicat-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.080835 merakicat-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 14:58:12.000000 merakicat-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 14:58:12.000000 merakicat-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 14:58:12.000000 merakicat-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 14:58:12.000000 merakicat-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 14:58:12.000000 merakicat-0.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 14:58:12.000000 merakicat-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 14:58:12.000000 merakicat-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 14:58:12.000000 merakicat-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-10 14:58:18.076835 merakicat-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-10 14:58:12.000000 merakicat-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 14:58:12.000000 merakicat-0.2.0/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.072835 merakicat-0.2.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 14:58:12.000000 merakicat-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 14:58:12.000000 merakicat-0.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:58:18.080835 merakicat-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 14:58:12.000000 merakicat-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_cloud_mon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_user_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    93557 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:58:17.000000 merakicat-0.2.0/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 14:58:12.000000 merakicat-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 16:25:57.000000 merakicat-0.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 16:25:57.000000 merakicat-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 16:25:57.000000 merakicat-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 16:25:57.000000 merakicat-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-10 16:25:57.000000 merakicat-0.2.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 16:25:57.000000 merakicat-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 16:25:57.000000 merakicat-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 16:25:57.000000 merakicat-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-10 16:26:03.213389 merakicat-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-10 16:25:57.000000 merakicat-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 16:25:57.000000 merakicat-0.2.1/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.209389 merakicat-0.2.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 16:25:57.000000 merakicat-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 16:25:57.000000 merakicat-0.2.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:26:03.213389 merakicat-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 16:25:57.000000 merakicat-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55397 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34364 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93245 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:26:02.000000 merakicat-0.2.1/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 16:25:57.000000 merakicat-0.2.1/tox.ini
```

### Comparing `merakicat-0.2.0/.gitignore` & `merakicat-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/CONTRIBUTING.rst` & `merakicat-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/HISTORY.md` & `merakicat-0.2.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # History
 
+## 0.2.1 (04-10-2024)
+
+  - Added support for ip default-gateway as a static route.
+
+## 0.2.0 (04-10-2024)
+
+  - Changed BOT libraries to enable websockets and remove ngrok for security.
+  - Began adding logic for Catalyst Cloud Monitoring onboarding.
+
 ## 0.1.8 (04-03-2024)
 
   - Edited README.
   - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
   - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
 
 ## 0.1.7 (04-01-2024)
```

### Comparing `merakicat-0.2.0/LICENSE` & `merakicat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/Makefile` & `merakicat-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/PKG-INFO` & `merakicat-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.0
+Version: 0.2.1
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,19 +109,16 @@
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
     > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
-
     ```
     # These exports are used for Webex bot mode:
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
@@ -231,49 +228,34 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
-# ngrok
-
-[ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
-
-You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
-
-1. After you've created an `ngrok` account, you will need to get your Authtoken.  Click on `Your Authtoken` on the ngrok dashboard and copy it.
-
-
-1. You can now export it to the OS environment variables like this:
-
-    ```
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
-    ```
-
-1. Now launch the bot!!
-
-    ```
-    python merakicat.py
-    ```
-
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webexteamsbot` project by [Hank Preston](https://github.com/hpreston).
+The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
-The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
+# History
 
+## 0.2.1 (04-10-2024)
 
-# History
+  - Added support for ip default-gateway as a static route.
+
+## 0.2.0 (04-10-2024)
+
+  - Changed BOT libraries to enable websockets and remove ngrok for security.
+  - Began adding logic for Catalyst Cloud Monitoring onboarding.
 
 ## 0.1.8 (04-03-2024)
 
   - Edited README.
   - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
   - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
```

### Comparing `merakicat-0.2.0/README.md` & `merakicat-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -79,19 +79,16 @@
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
     > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
-
     ```
     # These exports are used for Webex bot mode:
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
@@ -201,39 +198,15 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
-# ngrok
-
-[ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
-
-You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
-
-1. After you've created an `ngrok` account, you will need to get your Authtoken.  Click on `Your Authtoken` on the ngrok dashboard and copy it.
-
-
-1. You can now export it to the OS environment variables like this:
-
-    ```
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
-    ```
-
-1. Now launch the bot!!
-
-    ```
-    python merakicat.py
-    ```
-
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webexteamsbot` project by [Hank Preston](https://github.com/hpreston).
-
-The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
-
+The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
```

### Comparing `merakicat-0.2.0/images/botcongrats.jpg` & `merakicat-0.2.1/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/cisco_meraki.png` & `merakicat-0.2.1/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/createbot.jpg` & `merakicat-0.2.1/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/mc_quick.gif` & `merakicat-0.2.1/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/merakicat.png` & `merakicat-0.2.1/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/newapp.jpg` & `merakicat-0.2.1/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/images/newbot.jpg` & `merakicat-0.2.1/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/setup.py` & `merakicat-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.1/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/batch_helper/config.py` & `merakicat-0.2.1/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.1/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.1/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_claim.py` & `merakicat-0.2.1/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_cloud_mon.py` & `merakicat-0.2.1/src/merakicat/mc_cloud_mon.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_file_exists.py` & `merakicat-0.2.1/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_get_config.py` & `merakicat-0.2.1/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_get_nms.py` & `merakicat-0.2.1/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_pedia.py` & `merakicat-0.2.1/src/merakicat/mc_pedia.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
 #####################################################################################
 '''
 
 
 mc_pedia = {
 
-    'version': "v0.1.5",
-    'dated': "03/28/2024",
+    'version': "v0.1.6",
+    'dated': "04/10/2024",
 
     'switch': {
         
         'switch_name': {
             'name': "Hostname",
             'support':"✓",
             'translatable':"✓",
@@ -585,25 +585,31 @@
             'iosxe': "multicast_pim = parse.find_objects('^ip\spim')\n"
         },
         
         'static_routing':{
             'name': "Static routing",
             'support':"✓",
             'translatable':"✓",
-            'regex': '^ip\sroute',
+            'regex': '^ip\sroute|^ip\sdefault-gateway',
             'iosxe': "\
 static_routing = list()\n\
 route_obj_list = parse.find_objects('^ip\sroute\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})')\n\
 for route_obj in route_obj_list:\n\
     net = route_obj.re_match_typed('^ip\sroute\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}')\n\
     mask = route_obj.re_match_typed('^ip\sroute\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}')\n\
     gw = route_obj.re_match_typed('^ip\sroute\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})')\n\
     import ipaddress\n\
     subnet = str(ipaddress.ip_network(net + '/' + mask, strict=False))\n\
-    static_routing.append({'net': net, 'mask': mask, 'gw': gw, 'subnet': subnet})\n",
+    static_routing.append({'net': net, 'mask': mask, 'gw': gw, 'subnet': subnet})\n\
+route_obj_list = parse.find_objects('^ip\sdefault-gateway\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})')\n\
+if len(route_obj_list) == 1:\n\
+    import ipaddress\n\
+    subnet = str(ipaddress.ip_network('0.0.0.0/0', strict=False))\n\
+    gw = route_obj_list[0].re_match_typed('^ip\sdefault-gateway\s(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})')\n\
+    static_routing.append({'net': '0.0.0.0', 'mask': '0.0.0.0', 'gw': gw, 'subnet': subnet})\n",
             'meraki': {
                 'skip': 'post_ports',
                 'post_process': "\
 for route in switch_dict['static_routing']:\n\
     if route['subnet'] == '0.0.0.0/0':\n\
         default_route = route\n\
         return_vals = ['default_route']\n",
```

### Comparing `merakicat-0.2.0/src/merakicat/mc_ping.py` & `merakicat-0.2.1/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_register.py` & `merakicat-0.2.1/src/merakicat/mc_register.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.1/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/mc_translate.py` & `merakicat-0.2.1/src/merakicat/mc_translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,36 +351,37 @@
         """
 
         # Create a place to hold the Dashboard URL for each switch
         # Configure the switch_name in the Dashboard
         if debug:
             print(f"switch_dict = {switch_dict}")
         for key, val in mc_pedia['switch'].items():
-            if (val['translatable'] == "✓" and
-                val['meraki']['skip'] == "post_process") or \
-                 val['meraki']['skip'] == "post_ports":
-                if debug:
-                    print(f"key = {key}, val = {val}")
-                if val['meraki']['skip'] == "post_ports":
-                    post_ports_list.append([key, True])
-                newvals = {}
-                exec(val['meraki'].get('post_process'), locals(), newvals)
-                if debug:
-                    print(f"newvals = {newvals}")
-                return_vals = newvals['return_vals']
-                if debug:
-                    print(f"newvals['return_vals'] = " +
-                          f"{newvals['return_vals']}")
-                n = 0
-                while n < len(return_vals):
-                    switch_dict[return_vals[n]] = newvals[return_vals[n]]
-                    returns_dict[return_vals[n]] = newvals[return_vals[n]]
-                    n += 1
-                if debug:
-                    print(f"switch_dict = {switch_dict}")
+            if not switch_dict[key] == []:
+                if (val['translatable'] == "✓" and
+                    val['meraki']['skip'] == "post_process") or \
+                     val['meraki']['skip'] == "post_ports":
+                    if debug:
+                        print(f"key = {key}, val = {val}")
+                    if val['meraki']['skip'] == "post_ports":
+                        post_ports_list.append([key, True])
+                    newvals = {}
+                    exec(val['meraki'].get('post_process'), locals(), newvals)
+                    if debug:
+                        print(f"newvals = {newvals}")
+                    return_vals = newvals['return_vals']
+                    if debug:
+                        print(f"newvals['return_vals'] = " +
+                              f"{newvals['return_vals']}")
+                    n = 0
+                    while n < len(return_vals):
+                        switch_dict[return_vals[n]] = newvals[return_vals[n]]
+                        returns_dict[return_vals[n]] = newvals[return_vals[n]]
+                        n += 1
+                    if debug:
+                        print(f"switch_dict = {switch_dict}")
 
         # Loop to get all the interfaces in the port_dict
         y = 0
         while y <= len(Intf_list)-1:
             interface_descriptor = Intf_list[y]
             intf_settings = port_dict[interface_descriptor]
             if debug:
```

### Comparing `merakicat-0.2.0/src/merakicat/mc_user_info.py` & `merakicat-0.2.1/src/merakicat/mc_user_info.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/src/merakicat/merakicat.py` & `merakicat-0.2.1/src/merakicat/merakicat.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 Meraki Cat webexteamsbot is a chat bot with a swiss army knife
 of functions for checking & translating Catalyst IOSXE to Meraki
 switch configs, registering Catalyst switches to Dashboard and
 claiming them.  It can also be run from the command line or in
 batch from a shell script.
 """
-import ngrok
 import meraki
 import urllib.request
 import requests
 import shutil
 import docx
 import os
 import json
@@ -221,32 +220,25 @@
 if BOT:
     # Retrieve required details from environment variables
     bot_email = os.getenv("TEAMS_BOT_EMAIL")
     bot_app_name = os.getenv("TEAMS_BOT_APP_NAME")
     teams_token = os.getenv("TEAMS_BOT_TOKEN")
     if not os.getenv("TEAMS_EMAILS") is None:
         teams_emails = os.getenv("TEAMS_EMAILS")
-    # ngrok_token = os.getenv("NGROK_AUTHTOKEN")
 
     # If the required details were not in the environment variables
     # grab them from the mc_user_info.py file
     if bot_email is None:
         bot_email = TEAMS_BOT_EMAIL
     if bot_app_name is None:
         bot_app_name = TEAMS_BOT_APP_NAME
     if teams_token is None:
         teams_token = TEAMS_BOT_TOKEN
     if len(teams_emails) == 0:
         teams_emails = TEAMS_EMAILS
-    # if ngrok_token is None:
-    #     ngrok_token = NGROK_AUTHTOKEN
-    # listener = ngrok.forward("localhost:5000", authtoken=ngrok_token)
-    # if debug:
-    #     print(f"Ingress established at: {listener.url()}")
-    # bot_url = listener.url()
 
     # Either way, let's got the Bot's first name in case we are
     # directly addressed in room with multiple users
     bot_fname = bot_app_name.split()[0].strip()
 
 # Setup some global variables
 payload = {}
```

### Comparing `merakicat-0.2.0/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.1/src/merakicat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.0
+Version: 0.2.1
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,19 +109,16 @@
 
 # Usage
 
  - The easiest way to use this module is to set a few environment variables
 
     > Note: As an alternative, you may edit the variables in mc_user_info.py.  Although more convenient, it is less secure.
 
-    > Note: See [ngrok](#ngrok) for details on setting up an easy HTTP tunnel for webhooks callbacks for Bot mode.
-
     ```
     # These exports are used for Webex bot mode:
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
@@ -231,49 +228,34 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
-# ngrok
-
-[ngrok](http://ngrok.com) will make it easy for you to interact with merakicat as a bot.
-
-You can find account instructions here under `Sign up for free!`: [https://dashboard.ngrok.com/login](https://dashboard.ngrok.com/login)
-
-1. After you've created an `ngrok` account, you will need to get your Authtoken.  Click on `Your Authtoken` on the ngrok dashboard and copy it.
-
-
-1. You can now export it to the OS environment variables like this:
-
-    ```
-    export NGROK_AUTHTOKEN=<your ngrok Authtoken>
-    ```
-
-1. Now launch the bot!!
-
-    ```
-    python merakicat.py
-    ```
-
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
-The bot functionality is based on the `webexteamsbot` project by [Hank Preston](https://github.com/hpreston).
+The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
-The initial packaging of the original `ciscosparkbot` project was done by [Kevin Corbin](https://github.com/kecorbin).
 
+# History
 
+## 0.2.1 (04-10-2024)
 
-# History
+  - Added support for ip default-gateway as a static route.
+
+## 0.2.0 (04-10-2024)
+
+  - Changed BOT libraries to enable websockets and remove ngrok for security.
+  - Began adding logic for Catalyst Cloud Monitoring onboarding.
 
 ## 0.1.8 (04-03-2024)
 
   - Edited README.
   - Renamed mc_user_sample.py to mc_user_info.py and commented out possible environment variables.
   - Added logic to merakicat.py to handle missing variables on import from mc_user_info.py.
```

### Comparing `merakicat-0.2.0/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.1/src/merakicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.0/tox.ini` & `merakicat-0.2.1/tox.ini`

 * *Files identical despite different names*

