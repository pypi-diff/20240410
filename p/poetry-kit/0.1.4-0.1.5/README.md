# Comparing `tmp/poetry_kit-0.1.4.tar.gz` & `tmp/poetry_kit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_kit-0.1.4.tar", max compression
+gzip compressed data, was "poetry_kit-0.1.5.tar", max compression
```

## Comparing `poetry_kit-0.1.4.tar` & `poetry_kit-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       31 2023-12-11 06:18:44.494983 poetry_kit-0.1.4/poetry_kit/__init__.py
--rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 poetry_kit-0.1.4/poetry_kit/__itinerary/later.S.HTML
--rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 poetry_kit-0.1.4/poetry_kit/_clique/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 poetry_kit-0.1.4/poetry_kit/_clique/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 poetry_kit-0.1.4/poetry_kit/_clique/group/__init__.py
--rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 poetry_kit-0.1.4/poetry_kit/_clique/group/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 poetry_kit-0.1.4/poetry_kit/_licenses/gpl-3.0-standalone.html
--rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 poetry_kit-0.1.4/poetry_kit/_status/DB/records.json
--rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 poetry_kit-0.1.4/poetry_kit/_status/monitors/status_1.py
--rw-r--r--   0        0        0     1381 2024-03-23 19:57:06.935925 poetry_kit-0.1.4/poetry_kit/_status/status.proc.py
--rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 poetry_kit-0.1.4/poetry_kit/license.S.HTML
--rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 poetry_kit-0.1.4/poetry_kit/mixer.MD
--rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 poetry_kit-0.1.4/poetry_kit/mixer.S.HTML
--rwxr-xr-x   0        0        0      254 2024-04-09 23:13:03.129410 poetry_kit-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0      314 2024-04-09 23:04:48.126709 poetry_kit-0.1.4/readme.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 poetry_kit-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      325 2024-04-09 23:17:29.338550 poetry_kit-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0      314 2024-04-09 23:04:48.126709 poetry_kit-0.1.5/readme.md
+-rw-r--r--   0        0        0       31 2023-12-11 06:18:44.494983 poetry_kit-0.1.5/venues/stages/poetry_kit/__init__.py
+-rw-r--r--   0        0        0       77 2024-03-23 20:03:57.719484 poetry_kit-0.1.5/venues/stages/poetry_kit/__itinerary/later.S.HTML
+-rw-r--r--   0        0        0      297 2023-12-11 06:07:46.193124 poetry_kit-0.1.5/venues/stages/poetry_kit/_clique/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.907926 poetry_kit-0.1.5/venues/stages/poetry_kit/_clique/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      294 2023-12-01 19:53:30.939388 poetry_kit-0.1.5/venues/stages/poetry_kit/_clique/group/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-23 19:57:06.923925 poetry_kit-0.1.5/venues/stages/poetry_kit/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 poetry_kit-0.1.5/venues/stages/poetry_kit/_licenses/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0      627 2024-03-23 19:56:41.932187 poetry_kit-0.1.5/venues/stages/poetry_kit/_status/DB/records.json
+-rw-r--r--   0        0        0       62 2024-03-23 19:55:58.252641 poetry_kit-0.1.5/venues/stages/poetry_kit/_status/monitors/status_1.py
+-rw-r--r--   0        0        0     1375 2024-04-09 23:13:50.708900 poetry_kit-0.1.5/venues/stages/poetry_kit/_status/status.proc.py
+-rw-r--r--   0        0        0      227 2024-03-23 19:57:06.947925 poetry_kit-0.1.5/venues/stages/poetry_kit/license.S.HTML
+-rw-r--r--   0        0        0      304 2024-03-23 19:57:06.955925 poetry_kit-0.1.5/venues/stages/poetry_kit/mixer.MD
+-rw-r--r--   0        0        0      154 2024-03-23 19:57:06.959925 poetry_kit-0.1.5/venues/stages/poetry_kit/mixer.S.HTML
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 poetry_kit-0.1.5/PKG-INFO
```

### Comparing `poetry_kit-0.1.4/poetry_kit/_licenses/gpl-3.0-standalone.html` & `poetry_kit-0.1.5/venues/stages/poetry_kit/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `poetry_kit-0.1.4/poetry_kit/_status/DB/records.json` & `poetry_kit-0.1.5/venues/stages/poetry_kit/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `poetry_kit-0.1.4/poetry_kit/_status/status.proc.py` & `poetry_kit-0.1.5/venues/stages/poetry_kit/_status/status.proc.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 	db_directory = False
 else:
 	glob_string = status_assurances_path + '/**/status_*.py'
 	db_directory = normpath (join (this_directory_path, "DB"))
 
 print ("glob string:", glob_string)
 
-import bracelet
-scan = bracelet.start (
+import volts
+scan = volts.start (
 	glob_string = glob_string,
 	simultaneous = True,
 	mixer_paths = [
 		normpath (join (structures_path, "mixers")),
 		normpath (join (structures_path, "mixers_pip"))
 	],
 	relative_path = status_assurances_path,
```

### Comparing `poetry_kit-0.1.4/PKG-INFO` & `poetry_kit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-kit
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: volts (>=1.0.9,<2.0.0)
```

