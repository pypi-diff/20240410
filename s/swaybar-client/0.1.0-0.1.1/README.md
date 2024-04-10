# Comparing `tmp/swaybar-client-0.1.0.tar.gz` & `tmp/swaybar-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swaybar-client-0.1.0.tar", last modified: Wed Mar 27 21:12:48 2024, max compression
+gzip compressed data, was "swaybar-client-0.1.1.tar", last modified: Wed Apr 10 08:36:20 2024, max compression
```

## Comparing `swaybar-client-0.1.0.tar` & `swaybar-client-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/
--rw-r--r--   0 elliem    (1000) elliem    (1000)    34260 2024-03-27 16:29:32.000000 swaybar-client-0.1.0/LICENSE
--rw-r--r--   0 elliem    (1000) elliem    (1000)    39882 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/PKG-INFO
--rw-r--r--   0 elliem    (1000) elliem    (1000)      602 2024-03-27 21:10:41.000000 swaybar-client-0.1.0/pyproject.toml
--rw-r--r--   0 elliem    (1000) elliem    (1000)       38 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/setup.cfg
-drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/swaybar_client.egg-info/
--rw-r--r--   0 elliem    (1000) elliem    (1000)    39882 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/PKG-INFO
--rw-r--r--   0 elliem    (1000) elliem    (1000)      401 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/SOURCES.txt
--rw-r--r--   0 elliem    (1000) elliem    (1000)        1 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/dependency_links.txt
--rw-r--r--   0 elliem    (1000) elliem    (1000)       53 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/entry_points.txt
--rw-r--r--   0 elliem    (1000) elliem    (1000)       17 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/requires.txt
--rw-r--r--   0 elliem    (1000) elliem    (1000)       14 2024-03-27 21:12:48.000000 swaybar-client-0.1.0/swaybar_client.egg-info/top_level.txt
-drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/swaybarclient/
--rw-r--r--   0 elliem    (1000) elliem    (1000)       41 2024-03-27 20:08:30.000000 swaybar-client-0.1.0/swaybarclient/__init__.py
-drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-03-27 21:12:48.924289 swaybar-client-0.1.0/swaybarclient/modules/
--rw-r--r--   0 elliem    (1000) elliem    (1000)     2095 2024-03-27 03:02:37.000000 swaybar-client-0.1.0/swaybarclient/modules/battery.py
--rw-r--r--   0 elliem    (1000) elliem    (1000)      442 2024-03-26 22:59:49.000000 swaybar-client-0.1.0/swaybarclient/modules/cpu.py
--rw-r--r--   0 elliem    (1000) elliem    (1000)      556 2024-03-26 23:00:13.000000 swaybar-client-0.1.0/swaybarclient/modules/time.py
--rw-r--r--   0 elliem    (1000) elliem    (1000)     6761 2024-03-27 20:33:01.000000 swaybar-client-0.1.0/swaybarclient/swaybarclient.py
+drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/
+-rw-r--r--   0 elliem    (1000) elliem    (1000)    34260 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/LICENSE
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       54 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/MANIFEST.in
+-rw-r--r--   0 elliem    (1000) elliem    (1000)    39882 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/PKG-INFO
+-rw-r--r--   0 elliem    (1000) elliem    (1000)      602 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/pyproject.toml
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       38 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/setup.cfg
+drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/swaybar_client.egg-info/
+-rw-r--r--   0 elliem    (1000) elliem    (1000)    39882 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/PKG-INFO
+-rw-r--r--   0 elliem    (1000) elliem    (1000)      460 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/SOURCES.txt
+-rw-r--r--   0 elliem    (1000) elliem    (1000)        1 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/dependency_links.txt
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       53 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/entry_points.txt
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       17 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/requires.txt
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       14 2024-04-10 08:36:20.000000 swaybar-client-0.1.1/swaybar_client.egg-info/top_level.txt
+drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/swaybarclient/
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       41 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/__init__.py
+drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/swaybarclient/data/
+-rw-r--r--   0 elliem    (1000) elliem    (1000)       89 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/data/swaybar-client-default.json
+drwxr-xr-x   0 elliem    (1000) elliem    (1000)        0 2024-04-10 08:36:20.183357 swaybar-client-0.1.1/swaybarclient/modules/
+-rw-r--r--   0 elliem    (1000) elliem    (1000)     2095 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/modules/battery.py
+-rw-r--r--   0 elliem    (1000) elliem    (1000)      442 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/modules/cpu.py
+-rw-r--r--   0 elliem    (1000) elliem    (1000)      556 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/modules/time.py
+-rw-r--r--   0 elliem    (1000) elliem    (1000)     6761 2024-04-10 08:36:06.000000 swaybar-client-0.1.1/swaybarclient/swaybarclient.py
```

### Comparing `swaybar-client-0.1.0/LICENSE` & `swaybar-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swaybar-client-0.1.0/PKG-INFO` & `swaybar-client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swaybar-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A swaybar client
 Author-email: Ellie Lapanje <ellie.lapanje@gmail.com>
 Maintainer-email: Ellie Lapanje <ellie.lapanje@gmail.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
@@ -661,11 +661,11 @@
         the specific requirements.
         
         You should also get your employer (if you work as a programmer) or
         school, if any, to sign a "copyright disclaimer" for the program, if
         necessary. For more information on this, and how to apply and follow
         the GNU AGPL, see <https://www.gnu.org/licenses/>.
         
-Project-URL: Repository, https://github.com/Elliiem/SwayBar-Client
+Project-URL: Repository, https://github.com/Elliiem/swaybar-client
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: importlib
```

### Comparing `swaybar-client-0.1.0/pyproject.toml` & `swaybar-client-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'swaybar-client'
-version = '0.1.0'
+version = '0.1.1'
 
 description = 'A swaybar client'
 
 authors = [{ name = 'Ellie Lapanje', email = 'ellie.lapanje@gmail.com' }]
 maintainers = [{ name = 'Ellie Lapanje', email = 'ellie.lapanje@gmail.com' }]
 
 dependencies = ['psutil', 'importlib']
 
 license = { file = 'LICENSE' }
 
 [project.scripts]
 swaybarclient = 'swaybarclient:Main'
 
 [project.urls]
-Repository = 'https://github.com/Elliiem/SwayBar-Client'
+Repository = 'https://github.com/Elliiem/swaybar-client'
 
 [tool.setuptools.package-data]
 swaybarclient = ['swaybar-client-default.json']
```

### Comparing `swaybar-client-0.1.0/swaybar_client.egg-info/PKG-INFO` & `swaybar-client-0.1.1/swaybar_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swaybar-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A swaybar client
 Author-email: Ellie Lapanje <ellie.lapanje@gmail.com>
 Maintainer-email: Ellie Lapanje <ellie.lapanje@gmail.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
@@ -661,11 +661,11 @@
         the specific requirements.
         
         You should also get your employer (if you work as a programmer) or
         school, if any, to sign a "copyright disclaimer" for the program, if
         necessary. For more information on this, and how to apply and follow
         the GNU AGPL, see <https://www.gnu.org/licenses/>.
         
-Project-URL: Repository, https://github.com/Elliiem/SwayBar-Client
+Project-URL: Repository, https://github.com/Elliiem/swaybar-client
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: importlib
```

### Comparing `swaybar-client-0.1.0/swaybarclient/modules/battery.py` & `swaybar-client-0.1.1/swaybarclient/modules/battery.py`

 * *Files identical despite different names*

### Comparing `swaybar-client-0.1.0/swaybarclient/modules/time.py` & `swaybar-client-0.1.1/swaybarclient/modules/time.py`

 * *Files identical despite different names*

### Comparing `swaybar-client-0.1.0/swaybarclient/swaybarclient.py` & `swaybar-client-0.1.1/swaybarclient/swaybarclient.py`

 * *Files identical despite different names*

