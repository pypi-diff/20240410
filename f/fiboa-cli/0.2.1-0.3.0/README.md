# Comparing `tmp/fiboa-cli-0.2.1.tar.gz` & `tmp/fiboa-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.2.1.tar", last modified: Tue Apr  2 21:56:40 2024, max compression
+gzip compressed data, was "fiboa-cli-0.3.0.tar", last modified: Wed Apr 10 13:24:57 2024, max compression
```

## Comparing `fiboa-cli-0.2.1.tar` & `fiboa-cli-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:56:40.259917 fiboa-cli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 21:56:40.259917 fiboa-cli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:56:40.255917 fiboa-cli-0.2.1/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:56:40.259917 fiboa-cli-0.2.1/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 21:56:40.000000 fiboa-cli-0.2.1/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:56:40.259917 fiboa-cli-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-02 21:56:36.000000 fiboa-cli-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/tests/test_jsonschema.py
```

### Comparing `fiboa-cli-0.2.1/LICENSE` & `fiboa-cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.2.1/PKG-INFO` & `fiboa-cli-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,24 @@
-Metadata-Version: 2.1
-Name: fiboa-cli
-Version: 0.2.1
-Summary: CLI tools such as validation and file format conversion for fiboa.
-Home-page: https://github.com/fiboa/cli
-Author: Matthias Mohr
-License: Apache-2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: jsonschema>=4.20
-Requires-Dist: pyyaml>=6.0
-Requires-Dist: pyarrow>=14.0
-Requires-Dist: fsspec>=2024.0
-Requires-Dist: click>=8.1
-Requires-Dist: geopandas>=0.14
-Requires-Dist: requests>=2.30
-Requires-Dist: aiohttp>=3.9
-Requires-Dist: shapely>=2.0
-Provides-Extra: de-nrw
-
 # fiboa CLI
 
 CLI tools such as validation and file format conversion for fiboa.
 
 ## Installation
 
 You need **Python 3.9+** installed. 
 Run `pip install fiboa-cli` to install the validator.
 
+To install additional dependencies for specific [converters](#converter-for-existing-datasets),
+you can for example run: `pip install fiboa-cli[xyz]` with xyz being the converter name.
+
+## fiboa versions
+
+- fiboa CLI >= 0.3.0 works with fiboa version > 0.2.0
+- fiboa CLI < 0.3.0 works with fiboa version = 0.1.0
+
 ## Validation
 
 To validate a fiboa GeoParquet or GeoJSON file, you can for example run:
 
 - GeoJSON: `fiboa validate example.json --collection collection.json`
 - GeoParquet: `fiboa validate example.parquet --data`
 
@@ -47,17 +33,29 @@
   By default, `gcsfs` will attempt to use your default gcloud credentials or, attempt to get credentials from the google metadata service, or fall back to anonymous access.
 
 ## Create fiboa GeoParquet from GeoJSON
 
 To create a fiboa-compliant GeoParquet for a fiboa-compliant set of GeoJSON files containing Features or FeatureCollections,
 you can for example run:
 
-- `fiboa create geojson/example.json -o test.parquet -c geojson/collection.json`
+- `fiboa create-geoparquet geojson/example.json -o example.parquet -c geojson/collection.json`
+
+Check `fiboa create-geoparquet --help` for more details.
+
+## Create fiboa GeoJSON from GeoParquet
+
+To create one or multiple fiboa-compliant GeoJSON file(s) for a fiboa-compliant GeoParquet file,
+you can for example run:
+
+- GeoJSON FeatureCollection:
+  `fiboa create-geojson example.parquet -o dest-folder`
+- GeoJSON Features (with indentation and max. 100 features):
+  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f TRUE`
 
-Check `fiboa create --help` for more details.
+Check `fiboa create-geoparquet --help` for more details.
 
 ## Inspect fiboa GeoParquet file
 
 To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
 
 - `fiboa describe example.parquet`
 
@@ -67,27 +65,42 @@
 
 To create a JSON Schema for a fiboa Schema YAML file, you can for example run:
 
 - `fiboa jsonschema example.json --id=https://fiboa.github.io/specification/v0.1.0/geojson/schema.json -o schema.json`
 
 Check `fiboa jsonschema --help` for more details.
 
+## Validate a fiboa Schema
+
+To validate a fiboa Schema YAML file, you can for example run:
+
+- `fiboa validate-schema schema/schema.yaml`
+
+Check `fiboa validate-schema --help` for more details.
+
 ## Converter for existing datasets
 
 To convert an existing dataset to fiboa using the pre-defined converters:
 
 - `fiboa convert de_nrw`
 
 Available converters:
-- `de_nrw` (Germany, NRW from Shapefile)
+- `at` (Austria)
+- `de_bb` (Berlin/Brandenburh, Germany)
+- `de_nds` (Lowe Saxony, Germany)
+- `de_nrw` (North Rhine-Westphalia, Germany)
+- `de_sh` (Schleswig-Holstein, Germany)
 
 ### Implement a converter
 
 1. Create a new file in `fiboa_cli/datasets` based on the `template.py`
 2. Implement the `convert()` function
 3. Add missing dependencies into a separate dependency group in `setup.py`
 4. Add the converter to the list above
 5. Create a PR to submit your converter for review
 
 ## Development
 
 To install in development mode run `pip install -e .` in this folder.
+
+For the tests first run `pip install -r requirements-dev.txt` to install pytest.
+Then you can run `pytest` to execute the tests.
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/__init__.py` & `fiboa-cli-0.3.0/fiboa_cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import click
 import sys
+import json
+import os
 
 from .convert import convert as convert_
-from .create import create as create_
+from .create_geoparquet import create_geoparquet as create_geoparquet_
+from .create_geojson import create_geojson as create_geojson_
 from .describe import describe as describe_
 from .jsonschema import jsonschema as jsonschema_
 from .validate import validate as validate_
-from .version import __version__, fiboa_version
+from .validate_schema import validate_schema as validate_schema_
+from .version import __version__, fiboa_version as fiboa_version_
 from .util import log, check_ext_schema_for_cli, valid_file_for_cli, valid_file_for_cli_with_ext, valid_files_folders_for_cli
 
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     """
     The fiboa CLI.
@@ -95,54 +99,122 @@
             else:
                 log("\n  => INVALID\n", "error")
                 sys.exit(1)
         except Exception as e:
             log(f"\n  => UNKNOWN: {e}\n", "error")
             sys.exit(2)
 
-## CREATE
+
+## VALIDATE SCHEMA
+@click.command()
+@click.argument('files', nargs=-1, callback=lambda ctx, param, value: valid_files_folders_for_cli(value, ["yaml", "yml"]))
+@click.option(
+    '--metaschema', '-m',
+    callback=valid_file_for_cli,
+    help=f'A fiboa schema metaschema to validate against.',
+    default=None
+)
+def validate_schema(files, metaschema):
+    """
+    Validates a fiboa schema file.
+    """
+    log(f"fiboa CLI {__version__} - Schema Validator\n", "success")
+    config = {
+        "metaschema": metaschema
+    }
+    for file in files:
+        log(f"Validating {file}", "info")
+        result = validate_schema_(file, config)
+        if result:
+            sys.exit(0)
+        else:
+            sys.exit(1)
+
+
+## CREATE PARQUET
 @click.command()
 @click.argument('files', nargs=-1, callback=lambda ctx, param, value: valid_files_folders_for_cli(value, ["json", "geojson"]))
 @click.option(
     '--out', '-o',
     type=click.Path(exists=False),
     help='File to write the file to.',
     required=True
 )
 @click.option(
     '--collection', '-c',
     callback=valid_file_for_cli,
     help='Points to the STAC collection that defines the fiboa version and extensions.',
-    required=True
+    default=None
 )
 @click.option(
     '--schema', '-s',
     type=click.Path(exists=True),
     help='fiboa Schema to work against. If not provided, uses the fiboa version from the collection to load the schema for the released version.'
 )
 @click.option(
     '--ext-schema', '-e',
     multiple=True,
     callback=check_ext_schema_for_cli,
     help='Maps a remote fiboa extension schema url to a local file. First the URL, then the local file path. Separated with a comma character. Example: https://example.com/schema.json,/path/to/schema.json',
 )
-def create(files, out, collection, schema, ext_schema):
+def create_geoparquet(files, out, collection, schema, ext_schema):
     """
-    Create a fiboa file from GeoJSON file(s).
+    Create a fiboa GeoParquet file from GeoJSON file(s).
     """
     log(f"fiboa CLI {__version__} - Create GeoParquet\n", "success")
     config = {
         "files": files,
         "out": out,
         "schema": schema,
         "collection": collection,
         "extension_schemas": ext_schema,
     }
     try:
-        create_(config)
+        create_geoparquet_(config)
+    except Exception as e:
+        log(e, "error")
+        sys.exit(1)
+
+
+## CREATE GEOJSON
+@click.command()
+@click.argument('file', nargs=1, callback=lambda ctx, param, value: valid_file_for_cli_with_ext(value, ["parquet", "geoparquet"]))
+@click.option(
+    '--out', '-o',
+    type=click.Path(exists=False),
+    help='Folder to write the files to.',
+    required=True
+)
+@click.option(
+    '--features', '-f',
+    type=click.BOOL,
+    help='Create seperate GeoJSON Feature files.',
+    default=False
+)
+@click.option(
+    '--num', '-n',
+    type=click.IntRange(min=1),
+    help='Number of features to export. Defaults to all.',
+    default=None
+)
+@click.option(
+    '--indent', '-i',
+    type=click.IntRange(min=0, max=8),
+    help='Indentation for JSON files. Defaults to no indentation.',
+    default=None
+)
+def create_geojson(file, out, features = False, num = None, indent = None):
+    """
+    Create a fiboa GeoJSON file(s) from a fiboa GeoParquet file
+    """
+    log(f"fiboa CLI {__version__} - Create GeoJSON\n", "success")
+    try:
+        create_geojson_(file, out, features, num, indent)
+        abs_path = os.path.abspath(out)
+        log(f"Files written to {abs_path}", "success")
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
 ## JSON SCHEMA
 @click.command()
@@ -157,62 +229,87 @@
     type=click.Path(exists=False),
     help='File to write the file to. If not provided, prints the file to the STDOUT.',
     default=None
 )
 @click.option(
     '--fiboa-version', '-f',
     type=click.STRING,
-    help=f'The fiboa version to validate against. Defaults to {fiboa_version}.',
-    default=fiboa_version
+    help=f'The fiboa version to validate against. Defaults to {fiboa_version_}.',
+    default=fiboa_version_
 )
 @click.option(
-    '--id',
+    '--id', '-i', 'id_',
     type=click.STRING,
     help='The JSON Schema $id to use for the schema. If not provided, the $id will be omitted.',
 )
-def jsonschema(schema, out, fiboa_version, id):
+def jsonschema(schema, out, fiboa_version, id_):
     """
     Create a JSON Schema for a fiboa Schema
     """
     log(f"fiboa CLI {__version__} - Create JSON Schema\n", "success")
     config = {
         "schema": schema,
-        "out": out,
         "fiboa_version": fiboa_version,
-        "id": id,
+        "id": id_,
     }
     try:
-        jsonschema_(config)
+        schema = jsonschema_(config)
+        if out:
+            with open(out, 'w', encoding='utf-8') as f:
+                json.dump(schema, f, indent=2)
+        else:
+            print(schema)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
 ## CONVERT
 @click.command()
 @click.argument('dataset', nargs=1)
 @click.option(
     '--out', '-o',
     type=click.Path(exists=False),
     help='File to write the GeoParquet file to.',
     required=True
 )
-def convert(dataset, out):
+@click.option(
+    '--cache', '-c',
+    type=click.Path(exists=False),
+    help='For network requests: Local cache file to store the downloaded file to avoid multiple downloads.',
+    default=None
+)
+@click.option(
+    '--source-coop', '-h',
+    type=click.STRING,
+    help='(Future) URL to the source cooperative repository, will be added to the Collection metadata.',
+    default=None
+)
+@click.option(
+    '--collection',
+    is_flag=True,
+    type=click.BOOL,
+    help='Export a Collection JSON alongside the data file.',
+    default=False
+)
+def convert(dataset, out, cache, source_coop, collection):
     """
     Converts existing field boundary datasets to fiboa.
     """
-    log(f"fiboa CLI {__version__} - Convert {dataset}\n", "success")
+    log(f"fiboa CLI {__version__} - Convert '{dataset}'\n", "success")
     try:
-        convert_(dataset, out)
+        convert_(dataset, out, cache, source_coop, collection)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
 cli.add_command(describe)
 cli.add_command(validate)
-cli.add_command(create)
+cli.add_command(validate_schema)
+cli.add_command(create_geoparquet)
+cli.add_command(create_geojson)
 cli.add_command(jsonschema)
 cli.add_command(convert)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/const.py` & `fiboa-cli-0.3.0/fiboa_cli/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 import pyarrow as pa
 import pyarrow.types as pat
 import pandas as pd
 
 # fiboa datatypes to geopandas datatypes
 GP_TYPE_MAP = {
     "boolean": "bool",
-    "int8": "int8",
+    "int8": "int8", # todo add enum support - start
     "uint8": "uint8",
     "int16": "int16",
     "uint16": "uint16",
     "int32": "int32",
     "uint32": "uint32",
     "int64": "int64",
-    "uint64": "uint64",
+    "uint64": "uint64", # todo add enum support - end
     "float": "float32",
     "double": "float64",
     "binary": "bytearray", # todo: check
-    "string": "str",
+    "string": "str", # todo: support enum
     "array": None, # todo: object?
     "object": "object",
-    "enum": "category", # todo: check
     "date": "datetime64[D]",
     "date-time": lambda x: pd.to_datetime(x),
     "geometry": None, # not a column, don't convert geometry
     "bounding-box": None # todo
 }
 
 # fiboa datatypes to pyarrow datatypes
 PA_TYPE_MAP = {
     "boolean": pa.bool_(),
-    "int8": pa.int8(),
+    "int8": pa.int8(), # todo add enum support - start
     "uint8": pa.uint8(),
     "int16": pa.int16(),
     "uint16": pa.uint16(),
     "int32": pa.int32(),
     "uint32": pa.uint32(),
     "int64": pa.int64(),
-    "uint64": pa.uint64(),
+    "uint64": pa.uint64(), # todo add enum support - end
     "float": pa.float32(),
     "double": pa.float64(),
     "binary": pa.binary(),
-    "string": pa.string(),
+    "string": pa.string(), # todo add enum support
     "array": lambda type: pa.list_(type),
     "object": None, # todo: lambda type: pa.map_(pa.string(), type)
-    "enum": pa.string(), # todo: support other data types [ENUM (BYTE_ARRAY)]
     "date": pa.date32(),
     "date-time": pa.timestamp("ms", tz="UTC"),
     "geometry": pa.binary(),
     "bounding-box": None # todo
 }
 
 # geopandas datatypes to pyarrow datatypes
 GP_TO_PA_TYPE_MAP = {
-    "string": pa.string(),
+    "string": pa.string(), # todo add enum support
     "|S0": pa.string(), # todo
     "<U0": pa.string(), # todo
     "bool": pa.bool_(),
-    "int8": pa.int8(),
+    "int8": pa.int8(), # todo add enum support - start
     "uint8": pa.uint8(),
     "int16": pa.int16(),
     "uint16": pa.uint16(),
     "int32": pa.int32(),
     "uint32": pa.uint32(),
     "int64": pa.int64(),
-    "uint64": pa.uint64(),
+    "uint64": pa.uint64(), # todo add enum support - end
     "float16": pa.float16(),
     "float32": pa.float32(),
     "float64": pa.float64(),
     "float128": None, # todo
     "complex64": None, # todo
     "complex128": None, # todo
     "complex256": None, # todo
@@ -90,22 +88,23 @@
     "uint64": pat.is_uint64,
     "float": pat.is_float32,
     "double": pat.is_float64,
     "binary": pat.is_binary,
     "string": pat.is_string,
     "array": pat.is_list,
     "object": pat.is_map,
-    "enum": None, # ENUM (BYTE_ARRAY)
     "date": pat.is_date32,
     "date-time": pat.is_timestamp,
     "geometry": pat.is_binary, # todo: check more?
     "bounding-box": None # todo
 }
 
 LOG_STATUS_COLOR = {
     "info": "white",
     "warning": "yellow",
     "error": "red",
     "success": "green"
 }
 
 SUPPORTED_PROTOCOLS = ["http", "https", "s3", "gs"]
+
+STAC_COLLECTION_SCHEMA = "http://schemas.stacspec.org/v1.0.0/collection-spec/json-schema/collection.json"
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/create.py` & `fiboa-cli-0.3.0/fiboa_cli/create_geoparquet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import os
 
 from .parquet import create_parquet
-from .util import log, load_file
+from .util import get_collection, log, load_file
 
-def create(config):
+def create_geoparquet(config):
     output_file = config.get("out")
 
-    # Add a STAC collection to the fiboa property to the Parquet metadata
-    collection = load_file(config.get("collection"))
-    if "id" not in collection or not collection["id"]:
-        collection["id"] = os.path.basename(output_file)
-    if "fiboa_version" not in collection:
-        raise Exception("No fiboa_version found in collection metadata")
-    else:
-        config["fiboa_version"] = collection["fiboa_version"]
-    # todo: fill with more/better metadata
-
     # Load all features from the GeoJSON files
     features = []
+    geojson = {}
+    file = None
     files = config.get("files")
     for file in files:
         geojson = load_file(file)
         if geojson["type"] == "Feature":
             features.append(geojson)
         elif geojson["type"] == "FeatureCollection":
             features += geojson["features"]
         else:
             log(f"{file}: Skipped - Unsupported GeoJSON type, must be Feature or FeatureCollection")
 
     if len(features) == 0:
         raise Exception("No valid features provided as input files")
 
+    # Add a STAC collection to the fiboa property to the Parquet metadata
+    # todo: for features this loads the collection of the last feature only if not provided specifically
+    collection = get_collection(geojson, config.get("collection"), file)
+    if "id" not in collection or not collection["id"]:
+        collection["id"] = os.path.basename(output_file)
+    if "fiboa_version" not in collection:
+        raise Exception("No fiboa_version found in collection metadata")
+    else:
+        config["fiboa_version"] = collection["fiboa_version"]
+    # todo: fill with more/better metadata
+
     # Get a list of the properties/columns (without duplicates)
     columns = set(["id", "geometry"])
     for feature in features:
         keys = feature["properties"].keys()
         columns.update(keys)
 
     columns = list(columns)
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/geopandas.py` & `fiboa-cli-0.3.0/fiboa_cli/geopandas.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pandas import DataFrame, Series
 
 import shapely
 
 from geopandas._compat import import_optional_dependency
 import geopandas
 from geopandas.io.file import _expand_user
+from geopandas.array import GeometryArray
 
 METADATA_VERSION = "1.0.0"
 SUPPORTED_VERSIONS = ["0.1.0", "0.4.0", "1.0.0-beta.1", "1.0.0"]
 
 def _remove_id_from_member_of_ensembles(json_dict):
     """
     Older PROJ versions will not recognize IDs of datum ensemble members that
@@ -185,7 +186,100 @@
     parquet = import_optional_dependency(
         "pyarrow.parquet", extra="pyarrow is required for Parquet support."
     )
 
     path = _expand_user(path)
     table = _geopandas_to_arrow(df, schema = schema, index=index, schema_version=schema_version)
     parquet.write_table(table, path, compression=compression, **kwargs)
+
+
+def decode_metadata(metadata_str):
+    """Decode a UTF-8 encoded JSON string to dict
+
+    Parameters
+    ----------
+    metadata_str : string (UTF-8 encoded)
+
+    Returns
+    -------
+    dict
+    """
+    if metadata_str is None:
+        return None
+
+    return json.loads(metadata_str.decode("utf-8"))
+
+
+def arrow_to_geopandas(table):
+    """
+    Helper function with main, shared logic for read_parquet/read_feather.
+    """
+    df = table.to_pandas()
+
+    metadata = table.schema.metadata
+
+    if metadata is None or b"geo" not in metadata:
+        raise ValueError(
+            """Missing geo metadata in Parquet/Feather file.
+            Use pandas.read_parquet/read_feather() instead."""
+        )
+
+    try:
+        metadata = decode_metadata(metadata.get(b"geo", b""))
+    except (TypeError, json.decoder.JSONDecodeError):
+        raise ValueError("Missing or malformed geo metadata in Parquet/Feather file")
+
+    # Find all geometry columns that were read from the file.  May
+    # be a subset if 'columns' parameter is used.
+    geometry_columns = df.columns.intersection(metadata["columns"])
+
+    if not len(geometry_columns):
+        raise ValueError(
+            """No geometry columns are included in the columns read from
+            the Parquet/Feather file. To read this file without geometry columns,
+            use pandas.read_parquet/read_feather() instead."""
+        )
+
+    geometry = metadata["primary_column"]
+
+    # Missing geometry likely indicates a subset of columns was read;
+    # promote the first available geometry to the primary geometry.
+    if len(geometry_columns) and geometry not in geometry_columns:
+        geometry = geometry_columns[0]
+
+    # Convert the WKB columns that are present back to geometry.
+    for col in geometry_columns:
+        col_metadata = metadata["columns"][col]
+        if "crs" in col_metadata:
+            crs = col_metadata["crs"]
+            if isinstance(crs, dict):
+                _remove_id_from_member_of_ensembles(crs)
+        else:
+            # per the GeoParquet spec, missing CRS is to be interpreted as
+            # OGC:CRS84
+            crs = "OGC:CRS84"
+
+        df[col] = from_wkb(df[col].values, crs=crs)
+
+    return geopandas.GeoDataFrame(df, geometry=geometry)
+
+
+def from_wkb(data, crs=None, on_invalid="raise"):
+    """
+    Convert a list or array of WKB objects to a GeometryArray.
+
+    Parameters
+    ----------
+    data : array-like
+        list or array of WKB objects
+    crs : value, optional
+        Coordinate Reference System of the geometry objects. Can be anything accepted by
+        :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
+        such as an authority string (eg "EPSG:4326") or a WKT string.
+    on_invalid: {"raise", "warn", "ignore"}, default "raise"
+        - raise: an exception will be raised if a WKB input geometry is invalid.
+        - warn: a warning will be raised and invalid WKB geometries will be returned as
+          None.
+        - ignore: invalid WKB geometries will be returned as None without a warning.
+
+    """
+    return GeometryArray(shapely.from_wkb(data, on_invalid=on_invalid), crs=crs)
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/jsonschema.py` & `fiboa-cli-0.3.0/fiboa_cli/jsonschema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import json
 from .util import load_datatypes, load_fiboa_schema
 from .jsonschema_template import jsonschema_template
 
 def jsonschema(config):
     core_schema = load_fiboa_schema(config)
     datatypes = load_datatypes(config['fiboa_version'])
-    schema = create_jsonschema(core_schema, datatypes, config.get('id'))
-    if config['out']:
-        with open(config['out'], 'w') as f:
-            json.dump(schema, f, indent=2)
-    else:
-        print(schema)
+    return create_jsonschema(core_schema, datatypes, config.get('id'))
+
 
 def create_jsonschema(core_schema, datatypes, id=None):
     geojson_root_properties = ['id', 'geometry', 'bbox', 'properties']
 
     geojson = {
         'root': {
             'required': [],
@@ -22,19 +18,20 @@
         },
         'properties': {
             'required': [],
             'properties': {}
         }
     }
 
-    for key, prop_schema in core_schema['properties'].items():
-        result = convert_schema(prop_schema, datatypes)
+    for key, prop_schema in core_schema.get('properties', {}).items():
+        required = key in core_schema.get('required',[])
+        result = convert_schema(prop_schema, datatypes, required)
 
         place = 'root' if key in geojson_root_properties else 'properties'
-        if result['required']:
+        if required:
             geojson[place]['required'].append(key)
         geojson[place]['properties'][key] = result['schema']
 
     schema = jsonschema_template()
     if id:
         schema['$id'] = id
     else:
@@ -53,23 +50,22 @@
             target['properties'] = source['properties']
 
     merge(schema, geojson['root'])
     merge(schema['properties']['properties'], geojson['properties'])
 
     return schema
 
-def convert_schema(prop_schema, datatypes):
+def convert_schema(prop_schema, datatypes, required = False):
     if not isinstance(prop_schema, dict) or 'type' not in prop_schema:
         return prop_schema
     elif prop_schema['type'] not in datatypes:
         raise ValueError(f"Unknown datatype {prop_schema['type']}")
 
     datatype_schema = datatypes[prop_schema['type']].copy()
 
-    required = prop_schema.get('required')
     if required:
         if '$ref' in datatype_schema:
             datatype_schema = {
                 "allOf": [
                     datatype_schema,
                     {
                         "not": {
@@ -116,17 +112,18 @@
             datatype_schema['items'] = {**datatype_schema.get('items', {}), **result['schema']}
         elif key == 'properties' and isinstance(value, dict):
             if not isinstance(datatype_schema.get('properties'), dict):
                 datatype_schema['properties'] = {}
             if not isinstance(datatype_schema.get('required'), list):
                 datatype_schema['required'] = []
             for prop_name, prop_value in value.items():
-                result = convert_schema(prop_value, datatypes)
+                required = key in value.get('required', [])
+                result = convert_schema(prop_value, datatypes, required)
                 datatype_schema['properties'][prop_name] = {**datatype_schema['properties'].get(prop_name, {}), **result['schema']}
-                if result['required']:
+                if required:
                     datatype_schema['required'].append(prop_name)
         elif key not in ['type', 'required']:
             datatype_schema[key] = value
 
     return {
         'required': required,
         'schema': datatype_schema
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/jsonschema_template.py` & `fiboa-cli-0.3.0/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.2.1/fiboa_cli/parquet.py` & `fiboa-cli-0.3.0/fiboa_cli/parquet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import json
 import pyarrow as pa
 
-from .const import PA_TYPE_MAP, GP_TYPE_MAP, GP_TO_PA_TYPE_MAP
-from .util import log, load_fiboa_schema, load_file
-from .geopandas import to_parquet
 from geopandas import GeoDataFrame
 from shapely.geometry import shape
 
-def create_parquet(data, columns, collection, output_file, config):
+from .const import PA_TYPE_MAP, GP_TYPE_MAP, GP_TO_PA_TYPE_MAP
+from .util import log, load_fiboa_schema, load_file, merge_schemas
+from .geopandas import to_parquet
+
+def create_parquet(data, columns, collection, output_file, config, missing_schemas = {}, compression = "brotli"):
     # Load the data schema
     fiboa_schema = load_fiboa_schema(config)
-    properties = {}
-    properties.update(fiboa_schema["properties"])
+    schemas = merge_schemas(missing_schemas, fiboa_schema)
 
     # Load all extension schemas
     extensions = {}
     if "fiboa_extensions" in collection and isinstance(collection["fiboa_extensions"], list):
         ext_map = config.get("extension_schemas", [])
         for ext in collection["fiboa_extensions"]:
             try:
                 if ext in ext_map:
                     path = ext_map[ext]
                     log(f"Redirecting {ext} to {path}", "info")
                 else:
                     path = ext
                 extensions[ext] = load_file(path)
-                properties.update(extensions[ext]["properties"])
+                schemas = merge_schemas(schemas, extensions[ext])
             except Exception as e:
                 log(f"Extension schema for {ext} can't be loaded: {e}", "warning")
 
     # Create GeoDataFrame from the features
     if not isinstance(data, GeoDataFrame):
         data = features_to_dataframe(data, columns)
 
     # Update the GeoDataFrame with the correct types etc.
-    data = update_dataframe(data, columns, properties)
+    data = update_dataframe(data, columns, schemas)
 
     # Define the fields for the schema
     pq_fields = []
     for name in columns:
+        properties = schemas.get("properties", {})
         if name in properties:
             prop_schema = properties[name]
             pa_type = create_type(prop_schema)
-            nullable = not prop_schema.get("required", False)
+            nullable = name not in schemas.get("required", [])
             field = pa.field(name, pa_type, nullable = nullable)
         else:
             pd_type = str(data[name].dtype) # pandas data type
-            pa_type = GP_TO_PA_TYPE_MAP.get(pd_type, None) # pyarrow data type
+            pa_type = GP_TO_PA_TYPE_MAP.get(pd_type) # pyarrow data type
             if pa_type is not None:
                 log(f"{name}: No schema defined, converting {pd_type} to nullable {pa_type}", "warning")
                 field = pa.field(name, pa_type, nullable = True)
             else:
                 log(f"{name}: No schema defined and converter doesn't support {pd_type}, skipping field", "warning")
                 continue
 
@@ -64,17 +65,20 @@
     # Proprietary function exported from geopandas to solve
     # https://github.com/geopandas/geopandas/issues/3182
     to_parquet(
         data,
         output_file,
         schema = pq_schema,
         index = False,
-        coerce_timestamps = "ms"
+        coerce_timestamps = "ms",
+        compression = compression
     )
 
+    return pq_fields
+
 
 def features_to_dataframe(features, columns):
     # Create a list of shapes
     rows = []
     for feature in features:
         id = feature["id"] if "id" in feature else None
         geometry = shape(feature["geometry"]) if "geometry" in feature else None
@@ -89,36 +93,36 @@
     # Create the GeoDataFrame
     return GeoDataFrame(rows, columns=columns, geometry="geometry", crs="EPSG:4326")
 
 
 def update_dataframe(data, columns, schema):
     # Convert the data to the correct types
     for column in columns:
-        if column not in schema:
+        if column not in schema["properties"]:
             continue
-        dtype = schema[column].get("type", None)
+        dtype = schema["properties"][column].get("type")
         if dtype == "geometry":
             continue
 
-        gp_type = GP_TYPE_MAP.get(dtype, None)
+        gp_type = GP_TYPE_MAP.get(dtype)
         if gp_type is None:
             log(f"{column}: No type conversion available for {dtype}")
         elif callable(gp_type):
             data[column] = gp_type(data[column])
         else:
             data[column] = data[column].astype(gp_type)
 
     return data
 
 def create_type(schema):
-    dtype = schema.get("type", None)
+    dtype = schema.get("type")
     if dtype is None:
         raise Exception("No type specified")
 
-    pa_type = PA_TYPE_MAP.get(dtype, None)
+    pa_type = PA_TYPE_MAP.get(dtype)
     if pa_type is None:
         raise Exception(f"{dtype} is not supported yet")
     elif callable(pa_type):
         if dtype == "array":
             pa_subtype = create_type(schema["items"])
             pa_type = pa_type(pa_subtype)
         elif dtype == "object":
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/validate.py` & `fiboa-cli-0.3.0/fiboa_cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import json
 import pyarrow.types as pat
-import geopandas as gpd
 
 from jsonschema.validators import Draft7Validator
-from .const import PA_TYPE_CHECK
+from .const import PA_TYPE_CHECK, STAC_COLLECTION_SCHEMA
 from .jsonschema import create_jsonschema
-from .util import log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema
+from .util import get_collection, log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema, merge_schemas
 from .validate_data import validate_column
 
-STAC_COLLECTION_SCHEMA = "http://schemas.stacspec.org/v1.0.0/collection-spec/json-schema/collection.json"
-
 def log(text: str, status="info"):
     # Indent logs
-    log_("  - " + text, status)
+    log_("  - " + str(text), status)
 
 
 def validate(file, config):
     if file.endswith(".json") or file.endswith(".geojson"):
         return validate_geojson(file, config)
     else:
         return validate_parquet(file, config)
@@ -28,15 +25,15 @@
     # Check fiboa version
     if "fiboa_version" not in collection:
         log("No fiboa_version found in collection metadata", "error")
         valid = False
     elif config.get("fiboa_version") is None:
         config["fiboa_version"] = collection["fiboa_version"]
 
-    log("fiboa extensions: " + collection["fiboa_version"])
+    log("fiboa version: " + collection["fiboa_version"])
 
     if collection["fiboa_version"] != config["fiboa_version"]:
         log(f"fiboa versions differs: Collection is {collection['fiboa_version']} and requested specification version is {config['fiboa_version']}", "warning")
 
     # Check STAC Collection
     if not validate_colletion_schema(collection):
         valid = False
@@ -64,54 +61,50 @@
     extension_info = ", ".join(collection["fiboa_extensions"]) or "none"
     log("fiboa extensions: " + extension_info)
 
     return valid, extensions
 
 
 def validate_geojson(file, config):
-    if not config.get("collection"):
-        log("No collection specified", "error")
+    try:
+        data = load_file(file)
+    except Exception as error:
+        log(error, "error")
         return False
 
-    collection = load_file(config.get("collection"))
+    collection = get_collection(data, config.get("collection"), file)
+    if collection is None:
+        log("No collection specified", "error")
+        return False
 
     valid, extensions = validate_collection(collection, config)
-
     core_schema = load_fiboa_schema(config)
-
     datatypes = load_datatypes(config["fiboa_version"])
-
     schema = create_jsonschema(core_schema, datatypes)
 
     # Load extensions
     ext_errors = []
     for ext in extensions:
         try:
             uri = ext
-            if ext in config["ext_schema"]:
-                uri = config["ext_schema"][ext]
+            if ext in config["extension_schemas"]:
+                uri = config["extension_schemas"][ext]
             ext_schema = load_file(uri)
             json_schema = create_jsonschema(ext_schema, datatypes)
             extensions[ext] = lambda obj: validate_json_schema(obj, json_schema)
         except Exception as error:
             extensions[ext] = None
             ext_errors.append(f"Failed to load extension {ext}: {str(error)}")
 
     for error in ext_errors:
         log(error, "error")
 
     # Validate
-    try:
-        data = load_file(file)
-    except Exception as error:
-        log(error, "error")
-        return False
-
     if not isinstance(data, dict):
-        log("Must be a JSON object")
+        log("Must be a JSON object", "error")
         return False
 
     if data["type"] == "Feature":
         features = [data]
     elif data["type"] == "FeatureCollection":
         features = data["features"]
     elif data["type"] == "Collection":
@@ -177,59 +170,59 @@
     # Validate Collection
     valid, extensions = validate_collection(collection, config)
 
     # load the actual fiboa schema
     fiboa_schema = load_fiboa_schema(config)
 
     # Load data if needed
-    df = None
+    gdf = None
     if config.get("data"):
         try:
-            df = load_parquet_data(file)
+            gdf = load_parquet_data(file)
         except Exception as e:
             log(f"Data could not be read: {e}", "error")
             valid = False
 
     # Compile all properties from the schemas
-    properties = fiboa_schema["properties"]
+    schemas = fiboa_schema
     for ext in extensions.values():
-        properties.update(ext["properties"])
+        schemas = merge_schemas(schemas, ext)
 
     # Check that all required fields are present
-    for key, schema in properties.items():
-        required = schema.get("required", False)
-        if required and key not in parquet_schema.names:
+    for key in schemas.get("required", []):
+        if key not in parquet_schema.names:
             log(f"{key}: Required field is missing", "error")
             valid = False
 
     # Validate whether the Parquet schema complies with the property schemas
+    properties = schemas.get("properties", {})
     for key in parquet_schema.names:
         # Ignore fields without a schema
         if key not in properties:
             log(f"{key}: No schema defined")
             continue
 
         prop_schema = properties[key]
         # Make sure the schema has a data type assigned
-        dtype = prop_schema.get("type", None)
+        dtype = prop_schema.get("type")
         if dtype is None:
             log(f"{key}: No type specified", "warning")
             continue
 
         pq_field = parquet_schema.field(key)
         pq_type = pq_field.type
 
         # Does the field (dis)allow null?
-        nullable = not prop_schema.get("required", False)
+        nullable = key not in schemas.get("required", [])
         if nullable != pq_field.nullable:
             log(f"{key}: Nullability differs, is {pq_field.nullable} but must be {nullable}", "error")
             valid = False
 
         # Is the data type of the field correct?
-        pa_check = PA_TYPE_CHECK.get(dtype, None)
+        pa_check = PA_TYPE_CHECK.get(dtype)
         if pa_check is None:
             log(f"{key}: Validating {dtype} is not supported yet", "warning")
             continue
         elif not pa_check(pq_type):
             log(f"{key}: Data type invalid, is {pq_type} but must be {dtype}", "error")
             valid = False
             continue
@@ -243,36 +236,43 @@
                 valid = False
         elif dtype == "object":
             if not pat.is_string(pq_field.key_type):
                 log(f"{key}: Map key datatype is not string", "error")
                 valid = False
 
         # Validate data of the column
-        if df is not None:
-            issues = validate_column(df[key], prop_schema)
+        if gdf is not None:
+            issues = validate_column(gdf[key], prop_schema)
             if len(issues) > 0:
                 for issue in issues:
                     log(f"{key}: {issue}")
                 valid = False
 
     # Show a note once if data was not validated
     if not config.get("data"):
         log("Data was not validated as the --data parameter was not provided", "info")
 
     return valid
 
 
 # todo: use stac_validator instead of our own validation routine
 def validate_colletion_schema(obj):
-    schema = load_file(STAC_COLLECTION_SCHEMA)
-    errors = validate_json_schema(obj, schema)
-    for error in errors:
-        log(f"Collection: {error.path}: {error.message}", "error")
+    if "stac_version" in obj:
+        try:
+            schema = load_file(STAC_COLLECTION_SCHEMA)
+            errors = validate_json_schema(obj, schema)
+            for error in errors:
+                log(f"Collection: {error.path}: {error.message}", "error")
+
+            return len(errors) == 0
+        except:
+            log("Failed to validate STAC Collection", "warning")
+            return False
 
-    return len(errors) == 0
+    return True
 
 
 def validate_json_schema(obj, schema):
     if isinstance(obj, (bytearray, bytes, str)):
         obj = json.loads(obj)
 
     validator = Draft7Validator(schema)
```

### Comparing `fiboa-cli-0.2.1/fiboa_cli/validate_data.py` & `fiboa-cli-0.3.0/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.2.1/setup.py` & `fiboa-cli-0.3.0/setup.py`

 * *Files identical despite different names*

