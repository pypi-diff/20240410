# Comparing `tmp/qualytics-cli-0.1.8.tar.gz` & `tmp/qualytics-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualytics-cli-0.1.8.tar", last modified: Mon Feb 19 16:06:55 2024, max compression
+gzip compressed data, was "qualytics-cli-0.1.9.tar", last modified: Mon Feb 19 16:15:12 2024, max compression
```

## Comparing `qualytics-cli-0.1.8.tar` & `qualytics-cli-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:06:55.473492 qualytics-cli-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-19 16:06:46.000000 qualytics-cli-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-02-19 16:06:55.473492 qualytics-cli-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-19 16:06:46.000000 qualytics-cli-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:06:55.469492 qualytics-cli-0.1.8/qualytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:06:46.000000 qualytics-cli-0.1.8/qualytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-02-19 16:06:46.000000 qualytics-cli-0.1.8/qualytics/qualytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:06:55.473492 qualytics-cli-0.1.8/qualytics_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 16:06:55.000000 qualytics-cli-0.1.8/qualytics_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-19 16:06:55.473492 qualytics-cli-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-19 16:06:46.000000 qualytics-cli-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:15:12.321727 qualytics-cli-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-19 16:15:04.000000 qualytics-cli-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-02-19 16:15:12.321727 qualytics-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-19 16:15:04.000000 qualytics-cli-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:15:12.321727 qualytics-cli-0.1.9/qualytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:15:04.000000 qualytics-cli-0.1.9/qualytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-02-19 16:15:04.000000 qualytics-cli-0.1.9/qualytics/qualytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:15:12.321727 qualytics-cli-0.1.9/qualytics_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 16:15:12.000000 qualytics-cli-0.1.9/qualytics_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-19 16:15:12.321727 qualytics-cli-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-19 16:15:04.000000 qualytics-cli-0.1.9/setup.py
```

### Comparing `qualytics-cli-0.1.8/LICENSE` & `qualytics-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qualytics-cli-0.1.8/PKG-INFO` & `qualytics-cli-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualytics-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Qualytics CLI
 Home-page: https://www.qualytics.co/
 Author: Qualytics
 Author-email: devops@qualytics.co
 License: MIT
 Project-URL: GitHub, https://github.com/Qualytics/qualytics-cli
 Project-URL: Userguide, https://qualytics.github.io/userguide/
@@ -97,15 +97,15 @@
 
 
 ### Export Check Templates
 
 Enables exporting check templates to the `_export_check_templates` table to an enrichment datastore.
 
 ```bash
-checks_app export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
+qualytics checks export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
 ```
 
 | Option        | Type     | Description                                                                | Default                            | Required |
 |---------------|----------|----------------------------------------------------------------------------|------------------------------------|----------|
 | `--enrichment_datastore_id` | INTEGER  | The ID of the enrichment datastore where check templates will be exported. | Yes      |
 | `--check_templates`    | TEXT     | Comma-separated list of check template IDs or array-like format. Example: "1, 2, 3" or "[1,2,3]".| No       |
```

### Comparing `qualytics-cli-0.1.8/README.md` & `qualytics-cli-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 ### Export Check Templates
 
 Enables exporting check templates to the `_export_check_templates` table to an enrichment datastore.
 
 ```bash
-checks_app export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
+qualytics checks export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
 ```
 
 | Option        | Type     | Description                                                                | Default                            | Required |
 |---------------|----------|----------------------------------------------------------------------------|------------------------------------|----------|
 | `--enrichment_datastore_id` | INTEGER  | The ID of the enrichment datastore where check templates will be exported. | Yes      |
 | `--check_templates`    | TEXT     | Comma-separated list of check template IDs or array-like format. Example: "1, 2, 3" or "[1,2,3]".| No       |
```

### Comparing `qualytics-cli-0.1.8/qualytics/qualytics.py` & `qualytics-cli-0.1.9/qualytics/qualytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from rich import print
 from rich.progress import track
 from itertools import product
 from typing import Optional
 from typing_extensions import Annotated
 from croniter import croniter
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 app = typer.Typer()
 
 # Create a new Typer instance for checks
 checks_app = typer.Typer(name="checks", help="Commands for handling checks")
 
 # Create a new Typer instance for operation
```

### Comparing `qualytics-cli-0.1.8/qualytics_cli.egg-info/PKG-INFO` & `qualytics-cli-0.1.9/qualytics_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualytics-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: Qualytics CLI
 Home-page: https://www.qualytics.co/
 Author: Qualytics
 Author-email: devops@qualytics.co
 License: MIT
 Project-URL: GitHub, https://github.com/Qualytics/qualytics-cli
 Project-URL: Userguide, https://qualytics.github.io/userguide/
@@ -97,15 +97,15 @@
 
 
 ### Export Check Templates
 
 Enables exporting check templates to the `_export_check_templates` table to an enrichment datastore.
 
 ```bash
-checks_app export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
+qualytics checks export-metadata --enrichment_datastore_id ENRICHMENT_DATASTORE_ID [--check_templates CHECK_TEMPLATE_IDS]
 ```
 
 | Option        | Type     | Description                                                                | Default                            | Required |
 |---------------|----------|----------------------------------------------------------------------------|------------------------------------|----------|
 | `--enrichment_datastore_id` | INTEGER  | The ID of the enrichment datastore where check templates will be exported. | Yes      |
 | `--check_templates`    | TEXT     | Comma-separated list of check template IDs or array-like format. Example: "1, 2, 3" or "[1,2,3]".| No       |
```

### Comparing `qualytics-cli-0.1.8/setup.py` & `qualytics-cli-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 project_urls = {
   'GitHub': 'https://github.com/Qualytics/qualytics-cli',
   'Userguide': 'https://qualytics.github.io/userguide/'
 }
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 setup(
     name="qualytics-cli",
     packages=find_packages(),
     version=__version__,
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

