# Comparing `tmp/merakicat-0.2.1.tar.gz` & `tmp/merakicat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.2.1.tar", last modified: Wed Apr 10 16:26:03 2024, max compression
+gzip compressed data, was "merakicat-0.2.2.tar", last modified: Wed Apr 10 19:24:02 2024, max compression
```

## Comparing `merakicat-0.2.1.tar` & `merakicat-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 16:25:57.000000 merakicat-0.2.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 16:25:57.000000 merakicat-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 16:25:57.000000 merakicat-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 16:25:57.000000 merakicat-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-10 16:25:57.000000 merakicat-0.2.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 16:25:57.000000 merakicat-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 16:25:57.000000 merakicat-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 16:25:57.000000 merakicat-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-10 16:26:03.213389 merakicat-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-10 16:25:57.000000 merakicat-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 16:25:57.000000 merakicat-0.2.1/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.209389 merakicat-0.2.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 16:25:57.000000 merakicat-0.2.1/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 16:25:57.000000 merakicat-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 16:25:57.000000 merakicat-0.2.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:26:03.213389 merakicat-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 16:25:57.000000 merakicat-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.205389 merakicat-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_cloud_mon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55397 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34364 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/mc_user_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    93245 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 16:25:57.000000 merakicat-0.2.1/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:26:03.213389 merakicat-0.2.1/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:26:02.000000 merakicat-0.2.1/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 16:26:03.000000 merakicat-0.2.1/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 16:25:57.000000 merakicat-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.779703 merakicat-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.767703 merakicat-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.771703 merakicat-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 19:23:56.000000 merakicat-0.2.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 19:23:56.000000 merakicat-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 19:23:56.000000 merakicat-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 19:23:56.000000 merakicat-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-10 19:23:56.000000 merakicat-0.2.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 19:23:56.000000 merakicat-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 19:23:56.000000 merakicat-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 19:23:56.000000 merakicat-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-04-10 19:24:02.779703 merakicat-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-10 19:23:56.000000 merakicat-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.771703 merakicat-0.2.2/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 19:23:56.000000 merakicat-0.2.2/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.771703 merakicat-0.2.2/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 19:23:56.000000 merakicat-0.2.2/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 19:23:56.000000 merakicat-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 19:23:56.000000 merakicat-0.2.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:24:02.779703 merakicat-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 19:23:56.000000 merakicat-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.767703 merakicat-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.775703 merakicat-0.2.2/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.779703 merakicat-0.2.2/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55397 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34364 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93515 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 19:23:56.000000 merakicat-0.2.2/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:24:02.779703 merakicat-0.2.2/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 19:24:02.000000 merakicat-0.2.2/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 19:23:56.000000 merakicat-0.2.2/tox.ini
```

### Comparing `merakicat-0.2.1/.gitignore` & `merakicat-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/CONTRIBUTING.rst` & `merakicat-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/HISTORY.md` & `merakicat-0.2.2/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 0.2.2 (04-10-2024)
+
+  - Added environment variable to specify a Meraki Oragnization name.
+
 ## 0.2.1 (04-10-2024)
 
   - Added support for ip default-gateway as a static route.
 
 ## 0.2.0 (04-10-2024)
 
   - Changed BOT libraries to enable websockets and remove ngrok for security.
```

### Comparing `merakicat-0.2.1/LICENSE` & `merakicat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/Makefile` & `merakicat-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/PKG-INFO` & `merakicat-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.1
+Version: 0.2.2
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -122,14 +122,15 @@
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
+    export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
 
@@ -240,14 +241,18 @@
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.2 (04-10-2024)
+
+  - Added environment variable to specify a Meraki Oragnization name.
+
 ## 0.2.1 (04-10-2024)
 
   - Added support for ip default-gateway as a static route.
 
 ## 0.2.0 (04-10-2024)
 
   - Changed BOT libraries to enable websockets and remove ngrok for security.
```

### Comparing `merakicat-0.2.1/README.md` & `merakicat-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
+    export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
```

### Comparing `merakicat-0.2.1/images/botcongrats.jpg` & `merakicat-0.2.2/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/cisco_meraki.png` & `merakicat-0.2.2/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/createbot.jpg` & `merakicat-0.2.2/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/mc_quick.gif` & `merakicat-0.2.2/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/merakicat.png` & `merakicat-0.2.2/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/newapp.jpg` & `merakicat-0.2.2/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/images/newbot.jpg` & `merakicat-0.2.2/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/setup.py` & `merakicat-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.2/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/batch_helper/config.py` & `merakicat-0.2.2/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.2/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.2/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_claim.py` & `merakicat-0.2.2/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_cloud_mon.py` & `merakicat-0.2.2/src/merakicat/mc_cloud_mon.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_file_exists.py` & `merakicat-0.2.2/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_get_config.py` & `merakicat-0.2.2/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_get_nms.py` & `merakicat-0.2.2/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_pedia.py` & `merakicat-0.2.2/src/merakicat/mc_pedia.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_ping.py` & `merakicat-0.2.2/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_register.py` & `merakicat-0.2.2/src/merakicat/mc_register.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.2/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_translate.py` & `merakicat-0.2.2/src/merakicat/mc_translate.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/src/merakicat/mc_user_info.py` & `merakicat-0.2.2/src/merakicat/mc_user_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 DEBUG_SPLIT = False
 DEBUG_FILE = False
 
 # So you want a PDF report generated from the DOCX report (requires MS Word)
 PDF = False
 
 # For netmiko to connect to a switch directly
-# IOS_USERNAME = 'admin'
-# IOS_PASSWORD = 'password'
-# IOS_SECRET = 'secret'
+# IOS_USERNAME = "admin"
+# IOS_PASSWORD = "password"
+# IOS_SECRET = "secret"
 # IOS_PORT = 22
 
 # Webex Teams Bot Access Token for this Bot 
 # TEAMS_BOT_TOKEN = "ZTZjMDc5ZTUtN2Q5NS00NzNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN2_PF84_1eb65fdf-9643-417f-9974-ad72cae0e10f"
 
 # Webex Teams Bot email address for this Bot 
 # TEAMS_BOT_EMAIL = "mybot@webex.bot"
@@ -26,8 +26,9 @@
 # Webex Teams Bot email address for this Bot 
 # TEAMS_BOT_APP_NAME = "My Bot"
 
 # Webex Teams user email who can access our bot
 # TEAMS_EMAILS = ["somebody@google.com"]
 
 # For meraki SDK to connect to a Dahsboard account
-# MERAKI_API_KEY = '99NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN90'
+# MERAKI_API_KEY = "99NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN90"
+# MERAKI_ORG_NAME = "My Organization"
```

### Comparing `merakicat-0.2.1/src/merakicat/merakicat.py` & `merakicat-0.2.2/src/merakicat/merakicat.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 except ImportError:
     TEAMS_BOT_TOKEN = TEAMS_BOT_EMAIL = None
 try:
     from mc_user_info import TEAMS_BOT_APP_NAME, TEAMS_EMAILS
 except ImportError:
     TEAMS_BOT_APP_NAME = TEAMS_EMAILS = None
 try:
-    from mc_user_info import NGROK_AUTHTOKEN
-except ImportError:
-    NGROK_AUTHTOKEN = None
-try:
     from mc_user_info import MERAKI_API_KEY
 except ImportError:
     MERAKI_API_KEY = None
 try:
+    from mc_user_info import MERAKI_ORG_NAME
+except ImportError:
+    MERAKI_ORG_NAME = None
+try:
     from mc_user_info import DEBUG, DEBUG_MAIN, PDF
 except ImportError:
     DEBUG = DEBUG_MAIN = PDF = False
 debug = DEBUG or DEBUG_MAIN
 
 # Check to see if we have the most recent encyclopedia
 # and update it if not
@@ -97,41 +97,14 @@
         print("Request timed out")
 else:
     if debug:
         print("Not old enough to update.")
 
 from mc_pedia import mc_pedia
 
-# Retrieve required Meraki details from environment variables
-meraki_api_key = os.getenv("MERAKI_API_KEY")
-# If the required details were not in the environment variables
-# grab them from the mc_user_info.py file
-if meraki_api_key is None:
-    meraki_api_key = MERAKI_API_KEY
-
-# Retrieve required SSH details from environment variables
-ios_username = os.getenv("IOS_USERNAME")
-ios_password = os.getenv("IOS_PASSWORD")
-ios_secret = os.getenv("IOS_SECRET")
-ios_port = os.getenv("IOS_PORT")
-# If the required details were not in the environment variables
-# grab them from the mc_user_info.py file
-if ios_username is None:
-    ios_username = IOS_USERNAME
-if ios_username is None:
-    ios_username = IOS_USERNAME
-if ios_password is None:
-    ios_password = IOS_PASSWORD
-if ios_secret is None:
-    ios_secret = IOS_SECRET
-if ios_port is None:
-    ios_port = IOS_PORT
-    if ios_port is None:
-        ios_port = 22
-
 # If we were run without arguments, run as a BOT
 # Otherwise, we will attempt to use the args in batch mode
 BOT = False
 if len(sys.argv) == 1:
     BOT = True
 class RunCheck(Command):
 
@@ -261,16 +234,46 @@
 meraki_networks = list()
 meraki_org = ""
 meraki_org_name = ""
 meraki_net = ""
 meraki_net_name = ""
 meraki_urls = list()
 
+# Retrieve required Meraki details from environment variables
+meraki_api_key = os.getenv("MERAKI_API_KEY")
+meraki_org_name = os.getenv("MERAKI_ORG_NAME")
+# If the required details were not in the environment variables
+# grab them from the mc_user_info.py file
+if meraki_api_key is None:
+    meraki_api_key = MERAKI_API_KEY
+if meraki_org_name is None:
+    meraki_org_name = MERAKI_ORG_NAME
+
+# Retrieve required SSH details from environment variables
+ios_username = os.getenv("IOS_USERNAME")
+ios_password = os.getenv("IOS_PASSWORD")
+ios_secret = os.getenv("IOS_SECRET")
+ios_port = os.getenv("IOS_PORT")
+# If the required details were not in the environment variables
+# grab them from the mc_user_info.py file
+if ios_username is None:
+    ios_username = IOS_USERNAME
+if ios_username is None:
+    ios_username = IOS_USERNAME
+if ios_password is None:
+    ios_password = IOS_PASSWORD
+if ios_secret is None:
+    ios_secret = IOS_SECRET
+if ios_port is None:
+    ios_port = IOS_PORT
+    if ios_port is None:
+        ios_port = 22
+
 # Request the lists of Organizations and their Networks from Dashboard
-if not meraki_api_key == "":
+if not meraki_api_key == "" and not meraki_org_name =="":
     if debug:
         print("Trying to setup a dashboard instance")
     dashboard = meraki.DashboardAPI(
         api_key=meraki_api_key,
         output_log=False,
         suppress_logging=True)
 
@@ -282,28 +285,30 @@
     except meraki.exceptions.APIError:
         print("We were unable to get the list of Orgs.")
         sys.exit()
     if debug:
         print(f"meraki_orgs = {meraki_orgs}")
     x = 0
     while x <= len(meraki_orgs) - 1:
-        try:
-            raw_nets = dashboard.organizations.getOrganizationNetworks(
-                organizationId=meraki_orgs[x]['id'])
-
-        except meraki.exceptions.APIError:
-            print("We were unable to get the list of networks" +
-                  f" for {meraki_orgs[x]['name']}.")
-            sys.exit()
-        if debug:
-            print(raw_nets)
-        y = 0
-        while y <= len(raw_nets) - 1:
-            meraki_networks.append(raw_nets[y])
-            y += 1
+        if meraki_orgs[x]['name'] == meraki_org_name:
+            try:
+                raw_nets = dashboard.organizations.getOrganizationNetworks(
+                    organizationId=meraki_orgs[x]['id'])
+    
+            except meraki.exceptions.APIError:
+                print("We were unable to get the list of networks" +
+                      f" for {meraki_orgs[x]['name']}.")
+                sys.exit()
+            if debug:
+                print(raw_nets)
+            y = 0
+            while y <= len(raw_nets) - 1:
+                meraki_networks.append(raw_nets[y])
+                y += 1
+            break
         x += 1
     if debug:
         print(f"meraki_networks = {meraki_networks}")
     if len(meraki_orgs) == 1:
         meraki_org = meraki_orgs[0]['id']
         meraki_org_name = meraki_orgs[0]['name']
         if debug:
```

### Comparing `merakicat-0.2.1/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.2/src/merakicat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.1
+Version: 0.2.2
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -122,14 +122,15 @@
     
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
+    export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
 
@@ -240,14 +241,18 @@
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.2 (04-10-2024)
+
+  - Added environment variable to specify a Meraki Oragnization name.
+
 ## 0.2.1 (04-10-2024)
 
   - Added support for ip default-gateway as a static route.
 
 ## 0.2.0 (04-10-2024)
 
   - Changed BOT libraries to enable websockets and remove ngrok for security.
```

### Comparing `merakicat-0.2.1/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.2/src/merakicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.1/tox.ini` & `merakicat-0.2.2/tox.ini`

 * *Files identical despite different names*

