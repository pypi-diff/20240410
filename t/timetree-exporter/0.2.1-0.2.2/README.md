# Comparing `tmp/timetree-exporter-0.2.1.tar.gz` & `tmp/timetree-exporter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetree-exporter-0.2.1.tar", last modified: Tue Apr  9 15:27:49 2024, max compression
+gzip compressed data, was "timetree-exporter-0.2.2.tar", last modified: Tue Apr  9 18:13:37 2024, max compression
```

## Comparing `timetree-exporter-0.2.1.tar` & `timetree-exporter-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.github/workflows/release-please.yml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.978128 timetree-exporter-0.2.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/assets/images/copy-response.png
--rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/assets/images/prepare-for-signin.png
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/responses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.982128 timetree-exporter-0.2.1/timetree_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 15:27:45.000000 timetree-exporter-0.2.1/timetree_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:49.986128 timetree-exporter-0.2.1/timetree_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:27:49.000000 timetree-exporter-0.2.1/timetree_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.330505 timetree-exporter-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.326505 timetree-exporter-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.326505 timetree-exporter-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.github/workflows/release-please.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.326505 timetree-exporter-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-09 18:13:37.330505 timetree-exporter-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.322505 timetree-exporter-0.2.2/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.326505 timetree-exporter-0.2.2/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   574097 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/assets/images/copy-response.png
+-rw-r--r--   0 runner    (1001) docker     (127)   335580 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/assets/images/prepare-for-signin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.326505 timetree-exporter-0.2.2/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/responses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:13:37.330505 timetree-exporter-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.330505 timetree-exporter-0.2.2/timetree_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/timetree_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/timetree_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/timetree_exporter/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/timetree_exporter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 18:13:30.000000 timetree-exporter-0.2.2/timetree_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:13:37.330505 timetree-exporter-0.2.2/timetree_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 18:13:37.000000 timetree-exporter-0.2.2/timetree_exporter.egg-info/top_level.txt
```

### Comparing `timetree-exporter-0.2.1/.github/workflows/pylint.yml` & `timetree-exporter-0.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/.github/workflows/python-publish.yml` & `timetree-exporter-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/CHANGELOG.md` & `timetree-exporter-0.2.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [0.2.2](https://github.com/eoleedi/TimeTree-exporter/compare/v0.2.1...v0.2.2) (2024-04-09)
+
+
+### Bug Fixes
+
+* define main function in __main__.py to match the script ([#28](https://github.com/eoleedi/TimeTree-exporter/issues/28)) ([24cceba](https://github.com/eoleedi/TimeTree-exporter/commit/24ccebafee8198f8acb0862b722c0c63182bd845))
+
+
+### Documentation
+
+* update Changelog's URL ([05e9d58](https://github.com/eoleedi/TimeTree-exporter/commit/05e9d58282cd9657d749aaea542dc3b13554f401))
+
 ## [0.2.1](https://github.com/eoleedi/TimeTree-exporter/compare/v0.2.0...v0.2.1) (2024-04-09)
 
 
 ### Bug Fixes
 
 * use now as dtstamp ([#24](https://github.com/eoleedi/TimeTree-exporter/issues/24)) ([36c2d23](https://github.com/eoleedi/TimeTree-exporter/commit/36c2d2392bf964de9c8823b23b24f8802162923b))
```

### Comparing `timetree-exporter-0.2.1/LICENSE` & `timetree-exporter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/PKG-INFO` & `timetree-exporter-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
-Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
+Project-URL: Changelog, https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `timetree-exporter-0.2.1/README.md` & `timetree-exporter-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/assets/images/copy-response.png` & `timetree-exporter-0.2.2/assets/images/copy-response.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/assets/images/prepare-for-signin.png` & `timetree-exporter-0.2.2/assets/images/prepare-for-signin.png`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/pyproject.toml` & `timetree-exporter-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     "icalendar",
 ]
 
 [project.urls]
 Homepage = "https://github.com/eoleedi/TimeTree-Exporter"
 Repository = "https://github.com/eoleedi/TimeTree-Exporter"
 Issues = "https://github.com/eoleedi/TimeTree-Exporter/issues"
-Changelog = "https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md"
+Changelog = "https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md"
 
 [project.scripts]
 timetree-exporter = "timetree_exporter.__main__:main"
 
 [tool.setuptools_scm]
```

### Comparing `timetree-exporter-0.2.1/responses/README.md` & `timetree-exporter-0.2.2/responses/README.md`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/timetree_exporter/__main__.py` & `timetree-exporter-0.2.2/timetree_exporter/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,55 +5,61 @@
 """
 
 import argparse
 from icalendar import Calendar
 from timetree_exporter import TimeTreeEvent, ICalEventFormatter
 from timetree_exporter.utils import get_events_from_file, paths_to_filelist
 
-# Parse arguments
-parser = argparse.ArgumentParser(
-    description="Convert Timetree events to iCal format",
-    prog="timetree_exporter",
-)
-parser.add_argument(
-    "input",
-    type=str,
-    help="Path to the Timetree response file(s)/folder",
-    nargs="+",
-)
-parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    help="Path to the output iCal file",
-    default="timetree.ics",
-)
-args = parser.parse_args()
-
-
-cal = Calendar()
-filenames = paths_to_filelist(args.input)
-
-for filename in filenames:
-    # Skip non-JSON files
-    if not filename.endswith(".json"):
-        print(f"Skipping {filename} (Invalid file type, should be .json)")
-        continue
-    print(f"Parsing {filename}")
-
-    # Get events from file
-    events = get_events_from_file(filename)
-    if events is None:
-        continue
-
-    # Add events to calendar
-    for event in events:
-        time_tree_event = TimeTreeEvent.from_dict(event)
-        formatter = ICalEventFormatter(time_tree_event)
-        iCalEvent = formatter.to_ical()
-        if iCalEvent is None:
+
+def main():
+    """Main function for the Timetree Exporter."""
+    # Parse arguments
+    parser = argparse.ArgumentParser(
+        description="Convert Timetree events to iCal format",
+        prog="timetree_exporter",
+    )
+    parser.add_argument(
+        "input",
+        type=str,
+        help="Path to the Timetree response file(s)/folder",
+        nargs="+",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        help="Path to the output iCal file",
+        default="timetree.ics",
+    )
+    args = parser.parse_args()
+
+    cal = Calendar()
+    filenames = paths_to_filelist(args.input)
+
+    for filename in filenames:
+        # Skip non-JSON files
+        if not filename.endswith(".json"):
+            print(f"Skipping {filename} (Invalid file type, should be .json)")
+            continue
+        print(f"Parsing {filename}")
+
+        # Get events from file
+        events = get_events_from_file(filename)
+        if events is None:
             continue
-        cal.add_component(iCalEvent)
 
-# Write calendar to file
-with open(args.output, "wb") as f:  # Path Traversal Vulnerability if on a server
-    f.write(cal.to_ical())
+        # Add events to calendar
+        for event in events:
+            time_tree_event = TimeTreeEvent.from_dict(event)
+            formatter = ICalEventFormatter(time_tree_event)
+            ical_event = formatter.to_ical()
+            if ical_event is None:
+                continue
+            cal.add_component(ical_event)
+
+    # Write calendar to file
+    with open(args.output, "wb") as f:  # Path Traversal Vulnerability if on a server
+        f.write(cal.to_ical())
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `timetree-exporter-0.2.1/timetree_exporter/event.py` & `timetree-exporter-0.2.2/timetree_exporter/event.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/timetree_exporter/formatter.py` & `timetree-exporter-0.2.2/timetree_exporter/formatter.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/timetree_exporter/utils.py` & `timetree-exporter-0.2.2/timetree_exporter/utils.py`

 * *Files identical despite different names*

### Comparing `timetree-exporter-0.2.1/timetree_exporter.egg-info/PKG-INFO` & `timetree-exporter-0.2.2/timetree_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: timetree-exporter
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Tool for Exporting TimeTree Calendar and Convert to iCal format(.ics)
 Author-email: Fong-Chun Tsai <eoleedimin@gmail.com>
 Project-URL: Homepage, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Repository, https://github.com/eoleedi/TimeTree-Exporter
 Project-URL: Issues, https://github.com/eoleedi/TimeTree-Exporter/issues
-Project-URL: Changelog, https://github.com/eoleedi/TimeTree-Exporter/CHANGELOG.md
+Project-URL: Changelog, https://github.com/eoleedi/TimeTree-exporter/blob/main/CHANGELOG.md
 Keywords: timetree,exporter,icalendar,ics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `timetree-exporter-0.2.1/timetree_exporter.egg-info/SOURCES.txt` & `timetree-exporter-0.2.2/timetree_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

