# Comparing `tmp/merakicat-0.1.8.tar.gz` & `tmp/merakicat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.1.8.tar", last modified: Wed Apr  3 15:45:12 2024, max compression
+gzip compressed data, was "merakicat-0.2.0.tar", last modified: Wed Apr 10 14:58:18 2024, max compression
```

## Comparing `merakicat-0.1.8.tar` & `merakicat-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.731782 merakicat-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 15:45:06.000000 merakicat-0.1.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-03 15:45:06.000000 merakicat-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-03 15:45:06.000000 merakicat-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 15:45:06.000000 merakicat-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 15:45:06.000000 merakicat-0.1.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 15:45:06.000000 merakicat-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 15:45:06.000000 merakicat-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-03 15:45:06.000000 merakicat-0.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-03 15:45:12.743782 merakicat-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-03 15:45:06.000000 merakicat-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 15:45:06.000000 merakicat-0.1.8/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.739782 merakicat-0.1.8/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-03 15:45:06.000000 merakicat-0.1.8/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 15:45:06.000000 merakicat-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-03 15:45:06.000000 merakicat-0.1.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:45:12.743782 merakicat-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-03 15:45:06.000000 merakicat-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.735782 merakicat-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_claim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8798 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/mc_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    84744 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 15:45:06.000000 merakicat-0.1.8/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:12.743782 merakicat-0.1.8/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 15:45:12.000000 merakicat-0.1.8/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 15:45:06.000000 merakicat-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.080835 merakicat-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 14:58:12.000000 merakicat-0.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 14:58:12.000000 merakicat-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 14:58:12.000000 merakicat-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 14:58:12.000000 merakicat-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 14:58:12.000000 merakicat-0.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 14:58:12.000000 merakicat-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 14:58:12.000000 merakicat-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 14:58:12.000000 merakicat-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-10 14:58:18.076835 merakicat-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-10 14:58:12.000000 merakicat-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 14:58:12.000000 merakicat-0.2.0/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.072835 merakicat-0.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 14:58:12.000000 merakicat-0.2.0/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 14:58:12.000000 merakicat-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 14:58:12.000000 merakicat-0.2.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:58:18.080835 merakicat-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 14:58:12.000000 merakicat-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.068835 merakicat-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54947 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34233 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93557 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 14:58:12.000000 merakicat-0.2.0/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:58:18.076835 merakicat-0.2.0/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:58:17.000000 merakicat-0.2.0/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 14:58:18.000000 merakicat-0.2.0/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 14:58:12.000000 merakicat-0.2.0/tox.ini
```

### Comparing `merakicat-0.1.8/.gitignore` & `merakicat-0.2.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# My own testing credentials
-src/merakicat/mc_user_info.py
-
 # Miscellaneous files
 src/merakicat/batch_helper_preview.json
 src/merakicat/test.txt
 
 # App-created files and logs
 files/*.cfg
 files/*.pdf
```

### Comparing `merakicat-0.1.8/CONTRIBUTING.rst` & `merakicat-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/HISTORY.md` & `merakicat-0.2.0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/LICENSE` & `merakicat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/Makefile` & `merakicat-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/PKG-INFO` & `merakicat-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.8
+Version: 0.2.0
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,22 +13,21 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: webexteamsbot==0.1.4.2
-Requires-Dist: webexteamssdk==1.0.3
+Requires-Dist: webex-bot-ecoen66==0.4.3
+Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
-Requires-Dist: ngrok==1.1.0
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
```

### Comparing `merakicat-0.1.8/README.md` & `merakicat-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/botcongrats.jpg` & `merakicat-0.2.0/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/cisco_meraki.png` & `merakicat-0.2.0/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/createbot.jpg` & `merakicat-0.2.0/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/mc_quick.gif` & `merakicat-0.2.0/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/merakicat.png` & `merakicat-0.2.0/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/newapp.jpg` & `merakicat-0.2.0/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/images/newbot.jpg` & `merakicat-0.2.0/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/setup.py` & `merakicat-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     history = history_file.read()
 
 requirements = [
-    "webexteamsbot==0.1.4.2",
-    "webexteamssdk==1.0.3",
+    "webex-bot-ecoen66==0.4.3",
+    "webexteamssdk==1.6.1",
     "Flask>=0.12.1",
     "netmiko==4.3.0",
     "tabulate==0.9.0",
     "ciscoconfparse2==0.5",
     "meraki==1.42.0",
-    "ngrok==1.1.0",
     "python-docx==1.1.0",
     "docx2pdf==0.1.8",
     "requests==2.31.0"
     ]
 
 setup_requirements = [ ]
```

### Comparing `merakicat-0.1.8/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.0/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/batch_helper/config.py` & `merakicat-0.2.0/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.0/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.0/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_claim.py` & `merakicat-0.2.0/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_file_exists.py` & `merakicat-0.2.0/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_get_config.py` & `merakicat-0.2.0/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_get_nms.py` & `merakicat-0.2.0/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_pedia.py` & `merakicat-0.2.0/src/merakicat/mc_pedia.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_ping.py` & `merakicat-0.2.0/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_register.py` & `merakicat-0.2.0/src/merakicat/mc_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         - A stack of 1-8 switches
         - The version of IOSXE
         - An ip name-server
         - A layer-3 interface that is operational
         - A default route
         - Succesful results of Meraki registration
     ** Need to add show meraki compatibility check. **
-    :param host: The switch or stack to SSH into
-    :param username: Username for SSH
-    :param password: Password for SSH
-    :param port: Port number for SSH
-    :param secret: IOSXE secret password for CLI escalation
+    :param host_id: The switch or stack to SSH into
+    :param ios_username: Username for SSH
+    :param ios_password: Password for SSH
+    :param ios_port: Port number for SSH
+    :param ios_secret: IOSXE secret password for CLI escalation
     :return: A string indicating success or failure to be used in reporting,
     :      : a list with any issues encountered, and lists of registered
     :      : switches, the Meraki serial numbers assigned, and a list of the
     :      : NM modules per switch for later.
     """
 
     debug = DEBUG or DEBUG_REGISTER
```

### Comparing `merakicat-0.1.8/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.0/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/mc_translate.py` & `merakicat-0.2.0/src/merakicat/mc_translate.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.1.8/src/merakicat/merakicat.py` & `merakicat-0.2.0/src/merakicat/merakicat.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 import shutil
 import docx
 import os
 import json
 import re
 import sys
 import time
-from webexteamsbot import TeamsBot
-from webexteamsbot.models import Response
+from webex_bot_ecoen66.webex_bot import WebexBot
+from webex_bot_ecoen66.models.response import Response
+from webex_bot_ecoen66.models.command import Command
 from netmiko import ConnectHandler
 from docx2pdf import convert
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 from docx.shared import Inches
 from docx.oxml import OxmlElement
 from docx.oxml.ns import qn
 from mc_cfg_check import CheckFeatures
 from mc_translate import Evaluate, MerakiConfig  # ,MerakiConfig_up
 from mc_claim import Claim
 from mc_register import Register
+from mc_cloud_mon import CloudSwitch
 from mc_get_nms import GetNmList
 from mc_splitcheck_serials import SplitCheckSerials
 from mc_ping import Ping
 from mc_file_exists import FileExists
 from mc_get_config import GetConfig
 from collections import defaultdict
 from functools import reduce
@@ -128,41 +130,123 @@
         ios_port = 22
 
 # If we were run without arguments, run as a BOT
 # Otherwise, we will attempt to use the args in batch mode
 BOT = False
 if len(sys.argv) == 1:
     BOT = True
+class RunCheck(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="check",
+            help_message="Check a Catalyst switch config for both translatable and possible \
+Meraki features",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        print(f"attachment_actions={attachment_actions}")
+        return greeting(attachment_actions)
+
+class RunRegister(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="register",
+            help_message="Register a Catalyst switch to the Meraki Dashboard",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
+class RunClaim(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="claim",
+            help_message="Claim Catalyst switches to a Meraki Network",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
+class RunTranslate(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="translate",
+            help_message="Translate a Catalyst switch config from a file or \
+host to claimed Meraki serial numbers",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
+class RunMigrate(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="migrate",
+            help_message="Migrate a Catalyst switch to a Meraki switch - \
+register, claim & translate",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
+class RunDemo(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="demo",
+            help_message="Create a demo report for all features currently in \
+the feature encyclopedia",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
+class RunHelp(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="help",
+            help_message="Get help",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
 
 teams_emails = list()
 if BOT:
     # Retrieve required details from environment variables
     bot_email = os.getenv("TEAMS_BOT_EMAIL")
     bot_app_name = os.getenv("TEAMS_BOT_APP_NAME")
     teams_token = os.getenv("TEAMS_BOT_TOKEN")
     if not os.getenv("TEAMS_EMAILS") is None:
         teams_emails = os.getenv("TEAMS_EMAILS")
-    ngrok_token = os.getenv("NGROK_AUTHTOKEN")
+    # ngrok_token = os.getenv("NGROK_AUTHTOKEN")
 
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
-    if ngrok_token is None:
-        ngrok_token = NGROK_AUTHTOKEN
-    listener = ngrok.forward("localhost:5000", authtoken=ngrok_token)
-    if debug:
-        print(f"Ingress established at: {listener.url()}")
-    bot_url = listener.url()
+    # if ngrok_token is None:
+    #     ngrok_token = NGROK_AUTHTOKEN
+    # listener = ngrok.forward("localhost:5000", authtoken=ngrok_token)
+    # if debug:
+    #     print(f"Ingress established at: {listener.url()}")
+    # bot_url = listener.url()
 
     # Either way, let's got the Bot's first name in case we are
     # directly addressed in room with multiple users
     bot_fname = bot_app_name.split()[0].strip()
 
 # Setup some global variables
 payload = {}
@@ -238,15 +322,16 @@
             meraki_net_name = meraki_networks[0]['name']
             if debug:
                 print(f"meraki_net = {meraki_net}")
                 print(f"meraki_net_name = {meraki_net_name}")
 
 if BOT:
     # If any of the required bot variables are missing, terminate the app
-    if not bot_email or not teams_token or not bot_url or not bot_app_name:
+    # if not bot_email or not teams_token or not bot_url or not bot_app_name:
+    if not bot_email or not teams_token or not bot_app_name:
         print(
             "merakicat.py - Missing Environment Variable. Please see" +
             " the 'Usage' section in the README."
         )
         if not bot_email:
             print("TEAMS_BOT_EMAIL")
         if not teams_token:
@@ -266,27 +351,43 @@
     # List of email accounts of approved users to talk with the bot
     # approved_users = [
     #     "josmith@demo.local",
     # ]
 
     if debug:
         print(f"teams_emails = {teams_emails}")
+
+    """
     bot = TeamsBot(
         bot_app_name,
         teams_bot_token=teams_token,
         teams_bot_url=bot_url,
         teams_bot_email=bot_email,
         debug=debug,
         # Comment out the approved_users lines if you don't care...
         approved_users=teams_emails,
         webhook_resource_event=[
             {"resource": "messages", "event": "created"},
             {"resource": "attachmentActions", "event": "created"},
         ],
     )
+    """
+    bot = WebexBot(
+        teams_token,
+        bot_name=bot_app_name,
+        # Comment out the approved_users lines if you don't care...
+        approved_users=teams_emails,
+        # approved_domains=[],
+        # approved_rooms=[],
+        threads=False,
+        help_command=RunHelp(),
+        log_level="ERROR"
+    )
+
+
 
 # Create a custom bot greeting function, returned when no /command is given.
 # The default behavior of the bot is to return the '/help' command response
 # If there is an English language command line, try to work with that.
 
 
 def greeting(incoming_msg):
@@ -331,21 +432,23 @@
         user_text = re.sub(regex, '', user_text, re.IGNORECASE)
         detailed = True
 
     # If the command is 'check' and the user attached any config files to
     # the bot message, we will try to use them
     if user_text.lower() == 'check' and (user_files is not None):
         x = 0
-        while x < len(user_files) - 1:
+        responses=list()
+        while x < len(user_files):
             config_file = save(user_files[x])
             response.markdown = check_switch(
                 incoming_msg,
                 config=config_file)
-            create_message(user_roomId, response.markdown)
+            create_message(user_roomId, response.markdown, type="html")
             x += 1
+        return
 
     # If the user asked for a report, we will try to give it to them
     if user_text.lower().startswith('check network '):
         # Now let's see if they specified target models...
         targets = ['C9300']
         regex = re.compile(r"\s*target\s *|\s*targets\s *", flags=re.I)
         if len(regex.split(user_text)) > 1:
@@ -395,26 +498,74 @@
         user_text = re.sub(regex, '', user_text, re.IGNORECASE)
         report = True
 
     serials = list()
 
     # Test if it is equivalent to a command.
     match command:
+        case "cloud":
+            # If the only thing the user typed was "cloud"...
+            if user_text.lower() == 'cloud':
+                if host_id == "":
+                    # Just missing the host
+                    r = "I'm sorry, but I don't have a host "
+                    r += "that we are working with."
+                    response.markdown = r
+                else:
+                    # We did, so mess with it!
+                    response.markdown = cloud_switch(
+                        incoming_msg,
+                        host=host_id)
+            elif not len(user_text.split()) >= 3:
+                r = "Syntax is **cloud (host <_fqdn or ip address_>**"
+                response.markdown = r
+            # Well, did they type "cloud host" ?
+            elif re.search('host ', user_text, re.IGNORECASE):
+                if not user_text.lower().split("host ", 1)[1] == "":
+                    host_id = user_text.lower().split("host ", 1)[1]
+                    if debug:
+                        print(f"Ping({host_id}) = {Ping(host_id)}")
+                    if not Ping(host_id):
+                        r = "I was unable to ping that host."
+                        response.markdown = r
+                        return (response)
+                    if BOT:
+                        response.html = cloud_switch(incoming_msg,
+                                                     host=host_id)
+                    else:
+                        response.markdown = cloud_switch(incoming_msg,
+                                                         host=host_id)
+                else:
+                    r = "I'm sorry, but I don't have a host that we are "
+                    r += "working with."
+                    response.markdown = r
+            else:
+                r = "Syntax is **check (host <_fqdn or ip address_>**"
+                response.markdown = r
+
         case "demo":
             # If the only thing the user typed was "demo report""...
             if user_text.lower() == 'demo report':
                 # It was so check it!
-                response.markdown = check_switch(incoming_msg, demo=True)
+                print("should be calling check_switch with demo")
+                response.markdown = check_switch(
+                    incoming_msg,
+                    demo=True)
+                if BOT:
+                    print(f"response.markdown={response.markdown}")
+                    create_message(user_roomId, response.markdown, type="html")
+                    return
+
             else:
                 # It was not...?!
                 response.markdown = "I'm sorry, but I don't know what "
                 response.markdown += "you mean."
 
         case "migrate":
-            # If the only thing the user typed was "migrate""...
+            # If the only thing the user typed was "migrate"...
             if user_text.lower() == 'migrate':
                 # Check and see if we have a global stateful
                 # host and network to work with
                 if host_id == "" and meraki_net == "":
                     # We did not...
                     r = "I'm sorry, but I don't have a host "
                     r += "or a Network that we are working with."
@@ -805,17 +956,15 @@
                 # Lookup details about sender for our default response
                 sender = bot.teams.people.get(incoming_msg.personId)
                 response.markdown = "Hello {}, I'm ".format(sender.firstName)
                 response.markdown += "really just a glorified chat bot. "
                 response.markdown += "See what I can do by asking for "
                 response.markdown += "**help**."
             else:
-                response.markdown = "Hello, I'm really just a glorified chat "
-                response.markdown += "bot. See what I can do by asking for "
-                response.markdown += "help."
+                response.markdown = "See what I can do by asking for help."
 
     # Whatever just happened up above, send our response back to the user.
     return response
 
 
 def save(file):
     """
@@ -996,14 +1145,15 @@
         config_file = config
 
         # Run the function in config_checker to get the list of
         # features configured on the switch (supported and not)
         host_name, the_list = CheckFeatures(config_file)
         switch_name = host_name
     else:
+        print("In check_switch in the demo area")
         # Prep for a demo report
         host_name = switch_name = "Demonstration"
         the_list = list()
         for k in mc_pedia['switch'].keys():
             value = mc_pedia['switch'][k]
             if not value['regex'] == '':
                 the_list.append([
@@ -1142,14 +1292,95 @@
                 mc_pedia['version'] + ", published on " + mc_pedia['dated'] +
                 ".\nIf you wish, I can translate or migrate the " +
                 "Translatable features to an existing switch in the Meraki " +
                 "Dashboard." +
                 timing + '\n')
 
 
+def cloud_switch(incoming_msg, host=""):
+    """
+    """
+
+    start_time = time.time()
+    timing = ""
+
+    # Import the global stateful variables
+    global host_id, times
+
+    # Since we weren't passed a config filespec, check for a hostname or 
+    # IP address
+    if host == "":
+        return ("You need to enter a host FQDN or IP address.")
+    else:
+        # We were passed a hostname or IP address...
+        # Update the global stateful variable for later
+        host_id = host
+
+    # SSH to the switch with netmiko, read the config, grab the hostname,
+    # write the config out to a file using the hostname as part of the
+    # filespec
+    sw_name, config_file = CloudSwitch(dashboard,
+                                       meraki_org,
+                                       host,
+                                       ios_username,
+                                       ios_password,
+                                       ios_port,
+                                       ios_secret)
+    '''
+    if debug:
+        print(f"In cloud_switch, status = {status}")
+    if status == "successfully":
+        meraki_serials = registered_serials
+        if debug:
+            for switch in registered_switches:
+                print(f"In register_switch status = {status}")
+                print(f"switch = {switch}")
+                print("switch['Migration Status'] = " +
+                      f"{switch['migration_status']}")
+    if debug:
+        print(f"After registering switches, meraki_serials = {meraki_serials}")
+    # Report back on what happened
+    if called == "":
+        timing = ""
+        if not len(registered_switches) == 0:
+            vals = reduce(lambda x, y: x + y, [list(dic.values())
+                          for dic in registered_switches])
+            header = registered_switches[0].keys()
+            rows = [x.values() for x in registered_switches]
+            thing = tabulate(rows, header)
+            if times:
+                t = "\n=== That registraion took "
+                t += "%s seconds" % str(round((time.time() - start_time), 2))
+                timing = t
+            if BOT:
+                payload = "```\n%s" % thing + "\n```" + timing
+                r = f"We **{status}** registered **{vals.count('Registered')}"
+                r += "** switch"
+                r += f"{'es' if (vals.count('Registered') > 1) else ''}"
+                return (r + f":\n{payload}")
+            else:
+                payload = "\n%s" % thing + timing
+                r = f"\n\nWe {status} registered {vals.count('Registered')}"
+                r += f"switch{'es' if (vals.count('Registered') > 1) else ''}"
+                return (r + f":\n{payload}")
+        else:
+            payload = ""
+            for issue in issues:
+                payload += issue + "\n"
+            r = f"We were unsuccessful registering {host}:\n\n{payload}"
+            return (r + timing)
+    else:
+        return (status, issues, registered_switches)
+    '''
+    if times:
+        t = "%s seconds!" % str(round((time.time() - start_time), 2))
+        timing = " And it only took " + t
+    return ("Well, that was fun!"+timing)
+
+
 def check_report_writer(switch_name, can_list_doc, not_list_doc):
 
     global detailed
 
     document = docx.Document()
     section = document.sections[0]
 
@@ -1861,24 +2092,28 @@
     if BOT:
         r += "```\nenable\nservice meraki start"
     else:
         r += "\n    enable\n    service meraki start"
     return (r)
 
 
-def create_message(rid, msgtxt):
+def create_message(rid, msgtxt, type="markdown"):
     headers = {
         "content-type": "application/json; charset=utf-8",
         "authorization": "Bearer " + teams_token,
     }
 
     url = "https://api.ciscospark.com/v1/messages"
-    data = {"roomId": rid, "markdown": msgtxt}
+    if type == "markdown":
+        data = {"roomId": rid, "markdown": msgtxt}
+    else:
+        data = {"roomId": rid, "html": msgtxt}
+    print(f"roomId={rid}")
     response = requests.post(url, json=data, headers=headers)
-    print(f"response from create_massage was: {response}")
+    print(f"response from create_message was: {response}")
     return response.json()
 
 
 # Temporary function to send a message with a card attachment (not yet
 # supported by webexteamssdk, but there are open PRs to add this
 # functionality)
 def create_message_with_attachment(rid, msgtxt, attachment):
@@ -1892,16 +2127,17 @@
     response = requests.post(url, json=data, headers=headers)
     return response.json()
 
 
 # If we are in BOT mode, set up some bot stuff
 if BOT:
 
+
     # Set the bot greeting.
-    bot.set_greeting(greeting)
+    # bot.set_greeting(greeting)
 
     # Add new commands to the bot.
     bot_commands = list(list())
     bot_commands.extend([
         ["* **help**", "Get help."],
 
         ["* **check [network _Meraki network name_] [with timing] \
@@ -1936,14 +2172,15 @@
          "Migrate a Catalyst switch to a Meraki switch - register, claim & \
 translate"],
 
         ["* **demo report**",
          "Create a demo report for all features currently in the feature \
 encyclopedia"]])
 
+    """
     bot.add_command("help", "This list of commands", greeting)
 
     bot.add_command("check [host _FQDN or IP address_ | file _filespec_] \
 [with timing] [with details]",
                     "Check a Catalyst switch config for both translatable \
 and possible Meraki features",
                     greeting)
@@ -1985,14 +2222,23 @@
                     "Create a demo report for all features currently in the \
 feature encyclopedia",
                     greeting)
 
     # Every bot includes a default "/echo" command.  You can remove it, or any
     # other command with the remove_command(command) method.
     bot.remove_command("/echo")
+    """
+    bot.add_command(RunHelp())
+    bot.add_command(RunCheck())
+    bot.add_command(RunRegister())
+    bot.add_command(RunClaim())
+    bot.add_command(RunTranslate())
+    bot.add_command(RunMigrate())
+    bot.add_command(RunDemo())
+
 else:
     command_list = list(list())
     command_list.extend([
         ["help", "This list of commands"],
 
         ["check network <Meraki network name> [with timing] [with details]",
          "Check the configs of cloud monitored Catalyst switches for both \
@@ -2026,15 +2272,16 @@
     ])
 
 
 # BOT or not?
 if __name__ == "__main__":
     if BOT:
         # Run Bot
-        bot.run(host="0.0.0.0", port=5000)
+        # bot.run(host="0.0.0.0", port=5000)
+        bot.run()
     else:
         if debug:
             print(f"The number of command line args is {len(sys.argv)-1}")
         args = sys.argv
         del args[0]
         if debug:
             print(f"The args are: {str(args)}")
```

### Comparing `merakicat-0.1.8/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.0/src/merakicat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.1.8
+Version: 0.2.0
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,22 +13,21 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: webexteamsbot==0.1.4.2
-Requires-Dist: webexteamssdk==1.0.3
+Requires-Dist: webex-bot-ecoen66==0.4.3
+Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
-Requires-Dist: ngrok==1.1.0
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
```

### Comparing `merakicat-0.1.8/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.0/src/merakicat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 images/newapp.jpg
 images/newbot.jpg
 src/merakicat/__init__.py
 src/merakicat/bulk_check.sh
 src/merakicat/bulk_migrate.sh
 src/merakicat/mc_cfg_check.py
 src/merakicat/mc_claim.py
+src/merakicat/mc_cloud_mon.py
 src/merakicat/mc_file_exists.py
 src/merakicat/mc_get_config.py
 src/merakicat/mc_get_nms.py
 src/merakicat/mc_pedia.py
 src/merakicat/mc_ping.py
 src/merakicat/mc_register.py
 src/merakicat/mc_splitcheck_serials.py
 src/merakicat/mc_translate.py
+src/merakicat/mc_user_info.py
 src/merakicat/merakicat.py
 src/merakicat/test.txt
 src/merakicat.egg-info/PKG-INFO
 src/merakicat.egg-info/SOURCES.txt
 src/merakicat.egg-info/dependency_links.txt
 src/merakicat.egg-info/not-zip-safe
 src/merakicat.egg-info/requires.txt
```

### Comparing `merakicat-0.1.8/tox.ini` & `merakicat-0.2.0/tox.ini`

 * *Files identical despite different names*

