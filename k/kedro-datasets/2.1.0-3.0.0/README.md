# Comparing `tmp/kedro-datasets-2.1.0.tar.gz` & `tmp/kedro-datasets-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-2.1.0.tar", last modified: Wed Feb 28 11:18:46 2024, max compression
+gzip compressed data, was "kedro-datasets-3.0.0.tar", last modified: Wed Apr 10 14:53:32 2024, max compression
```

## Comparing `kedro-datasets-2.1.0.tar` & `kedro-datasets-3.0.0.tar`

### file list

```diff
@@ -1,119 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.428443 kedro-datasets-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-02-28 11:18:46.428443 kedro-datasets-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.380442 kedro-datasets-2.1.0/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.380442 kedro-datasets-2.1.0/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.380442 kedro-datasets-2.1.0/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/huggingface/hugging_face_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/matlab/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/matlab/matlab_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.384442 kedro-datasets-2.1.0/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.388442 kedro-datasets-2.1.0/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.388442 kedro-datasets-2.1.0/kedro_datasets/partitions/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/partitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/partitions/incremental_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/partitions/partitioned_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.388442 kedro-datasets-2.1.0/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.388442 kedro-datasets-2.1.0/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.388442 kedro-datasets-2.1.0/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/polars/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/polars/eager_polars_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/polars/lazy_polars_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.392442 kedro-datasets-2.1.0/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.396442 kedro-datasets-2.1.0/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 11:18:46.396442 kedro-datasets-2.1.0/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-02-28 11:18:46.000000 kedro-datasets-2.1.0/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-28 11:18:46.000000 kedro-datasets-2.1.0/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 11:18:46.000000 kedro-datasets-2.1.0/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-02-28 11:18:46.000000 kedro-datasets-2.1.0/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-28 11:18:46.000000 kedro-datasets-2.1.0/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 11:18:46.428443 kedro-datasets-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-02-28 11:18:29.000000 kedro-datasets-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20534 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17369 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.304596 kedro-datasets-3.0.0/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/hugging_face_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/ibis/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/ibis/table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/matlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matlab/matlab_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/netcdf/netcdf_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.308596 kedro-datasets-3.0.0/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10244 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22978 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/partitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/incremental_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/partitions/partitioned_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.312596 kedro-datasets-3.0.0/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/eager_polars_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/polars/lazy_polars_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.316596 kedro-datasets-3.0.0/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:53:32.320596 kedro-datasets-3.0.0/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20534 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 14:53:32.000000 kedro-datasets-3.0.0/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-04-10 14:53:26.000000 kedro-datasets-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:53:32.348596 kedro-datasets-3.0.0/setup.cfg
```

### Comparing `kedro-datasets-2.1.0/PKG-INFO` & `kedro-datasets-3.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,246 +1,254 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 2.1.0
+Version: 3.0.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: kedro>=0.19
 Requires-Dist: lazy_loader
-Provides-Extra: api
-Requires-Dist: requests~=2.20; extra == "api"
-Provides-Extra: biosequence
-Requires-Dist: biopython~=1.73; extra == "biosequence"
-Provides-Extra: dask
-Requires-Dist: dask[complete]>=2021.10; extra == "dask"
-Requires-Dist: triad<1.0,>=0.6.7; extra == "dask"
-Provides-Extra: databricks
-Requires-Dist: delta-spark~=1.2.1; extra == "databricks"
-Requires-Dist: pandas<3.0,>=1.3; extra == "databricks"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "databricks"
-Provides-Extra: geopandas
-Requires-Dist: geopandas<1.0,>=0.6.0; extra == "geopandas"
-Requires-Dist: pyproj~=3.0; extra == "geopandas"
-Provides-Extra: holoviews
-Requires-Dist: holoviews~=1.13.0; extra == "holoviews"
-Provides-Extra: huggingface
-Requires-Dist: datasets; extra == "huggingface"
-Requires-Dist: huggingface_hub; extra == "huggingface"
-Requires-Dist: transformers; extra == "huggingface"
-Provides-Extra: matlab
-Requires-Dist: scipy; extra == "matlab"
-Provides-Extra: matplotlib
-Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "matplotlib"
-Provides-Extra: networkx
-Requires-Dist: networkx~=2.4; extra == "networkx"
-Provides-Extra: pandas
-Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas"
-Requires-Dist: deltalake>=0.10.0; extra == "pandas"
-Requires-Dist: lxml~=4.6; extra == "pandas"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas"
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas"
-Requires-Dist: pyarrow>=6.0; extra == "pandas"
-Requires-Dist: pyodbc~=4.0; extra == "pandas"
-Requires-Dist: tables~=3.6; extra == "pandas"
-Provides-Extra: pickle
-Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "pickle"
-Provides-Extra: pillow
-Requires-Dist: Pillow~=9.0; extra == "pillow"
-Provides-Extra: plotly
-Requires-Dist: pandas<3.0,>=1.3; extra == "plotly"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly"
-Provides-Extra: polars
-Requires-Dist: deltalake>=0.6.2; extra == "polars"
-Requires-Dist: polars>=0.18.0; extra == "polars"
-Requires-Dist: pyarrow>=4.0; extra == "polars"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "polars"
-Provides-Extra: redis
-Requires-Dist: redis~=4.1; extra == "redis"
-Provides-Extra: snowflake
-Requires-Dist: snowflake-snowpark-python~=1.0; extra == "snowflake"
-Provides-Extra: spark
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark"
-Provides-Extra: svmlight
-Requires-Dist: scikit-learn>=1.0.2; extra == "svmlight"
-Requires-Dist: scipy~=1.7.3; extra == "svmlight"
-Provides-Extra: tensorflow
-Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "tensorflow"
-Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "tensorflow"
-Provides-Extra: video
-Requires-Dist: opencv-python~=4.5.5.64; extra == "video"
-Provides-Extra: yaml
-Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml"
-Requires-Dist: pandas<3.0,>=1.3; extra == "yaml"
+Provides-Extra: pandas-base
+Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-base"
+Provides-Extra: spark-base
+Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-base"
+Provides-Extra: hdfs-base
+Requires-Dist: hdfs<3.0,>=2.5.8; extra == "hdfs-base"
+Provides-Extra: s3fs-base
+Requires-Dist: s3fs<2024.1,>=2021.4; extra == "s3fs-base"
+Provides-Extra: polars-base
+Requires-Dist: polars>=0.18.0; extra == "polars-base"
+Provides-Extra: plotly-base
+Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-base"
+Provides-Extra: delta-base
+Requires-Dist: delta-spark~=1.2.1; extra == "delta-base"
+Provides-Extra: networkx-base
+Requires-Dist: networkx~=2.4; extra == "networkx-base"
 Provides-Extra: api-apidataset
 Requires-Dist: requests~=2.20; extra == "api-apidataset"
+Provides-Extra: api
+Requires-Dist: kedro-datasets[api-apidataset]; extra == "api"
 Provides-Extra: biosequence-biosequencedataset
 Requires-Dist: biopython~=1.73; extra == "biosequence-biosequencedataset"
+Provides-Extra: biosequence
+Requires-Dist: kedro-datasets[biosequence-biosequencedataset]; extra == "biosequence"
 Provides-Extra: dask-parquetdataset
 Requires-Dist: dask[complete]>=2021.10; extra == "dask-parquetdataset"
 Requires-Dist: triad<1.0,>=0.6.7; extra == "dask-parquetdataset"
+Provides-Extra: dask
+Requires-Dist: kedro-datasets[dask-parquetdataset]; extra == "dask"
 Provides-Extra: databricks-managedtabledataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "databricks-managedtabledataset"
-Requires-Dist: pandas<3.0,>=1.3; extra == "databricks-managedtabledataset"
-Requires-Dist: delta-spark~=1.2.1; extra == "databricks-managedtabledataset"
+Requires-Dist: kedro-datasets[delta-base,pandas-base,spark-base]; extra == "databricks-managedtabledataset"
+Provides-Extra: databricks
+Requires-Dist: kedro-datasets[databricks-managedtabledataset]; extra == "databricks"
 Provides-Extra: geopandas-geojsondataset
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "geopandas-geojsondataset"
 Requires-Dist: pyproj~=3.0; extra == "geopandas-geojsondataset"
+Provides-Extra: geopandas
+Requires-Dist: kedro-datasets[geopandas-geojsondataset]; extra == "geopandas"
 Provides-Extra: holoviews-holoviewswriter
 Requires-Dist: holoviews~=1.13.0; extra == "holoviews-holoviewswriter"
+Provides-Extra: holoviews
+Requires-Dist: kedro-datasets[holoviews-holoviewswriter]; extra == "holoviews"
+Provides-Extra: huggingface-hfdataset
+Requires-Dist: datasets; extra == "huggingface-hfdataset"
+Requires-Dist: huggingface_hub; extra == "huggingface-hfdataset"
+Provides-Extra: huggingface-hftransformerpipelinedataset
+Requires-Dist: transformers; extra == "huggingface-hftransformerpipelinedataset"
+Provides-Extra: huggingface
+Requires-Dist: kedro-datasets[huggingface-hfdataset,huggingface-hftransformerpipelinedataset]; extra == "huggingface"
+Provides-Extra: ibis-bigquery
+Requires-Dist: ibis-framework[bigquery]; extra == "ibis-bigquery"
+Provides-Extra: ibis-clickhouse
+Requires-Dist: ibis-framework[clickhouse]; extra == "ibis-clickhouse"
+Provides-Extra: ibis-dask
+Requires-Dist: ibis-framework[dask]; extra == "ibis-dask"
+Provides-Extra: ibis-datafusion
+Requires-Dist: ibis-framework[datafusion]; extra == "ibis-datafusion"
+Provides-Extra: ibis-druid
+Requires-Dist: ibis-framework[druid]; extra == "ibis-druid"
+Provides-Extra: ibis-duckdb
+Requires-Dist: ibis-framework[duckdb]; extra == "ibis-duckdb"
+Provides-Extra: ibis-exasol
+Requires-Dist: ibis-framework[exasol]; extra == "ibis-exasol"
+Provides-Extra: ibis-flink
+Requires-Dist: ibis-framework; extra == "ibis-flink"
+Requires-Dist: apache-flink; extra == "ibis-flink"
+Provides-Extra: ibis-impala
+Requires-Dist: ibis-framework[impala]; extra == "ibis-impala"
+Provides-Extra: ibis-mssql
+Requires-Dist: ibis-framework[mssql]; extra == "ibis-mssql"
+Provides-Extra: ibis-mysql
+Requires-Dist: ibis-framework[mysql]; extra == "ibis-mysql"
+Provides-Extra: ibis-oracle
+Requires-Dist: ibis-framework[oracle]; extra == "ibis-oracle"
+Provides-Extra: ibis-pandas
+Requires-Dist: ibis-framework[pandas]; extra == "ibis-pandas"
+Provides-Extra: ibis-polars
+Requires-Dist: ibis-framework[polars]; extra == "ibis-polars"
+Provides-Extra: ibis-postgres
+Requires-Dist: ibis-framework[postgres]; extra == "ibis-postgres"
+Provides-Extra: ibis-pyspark
+Requires-Dist: ibis-framework[pyspark]; extra == "ibis-pyspark"
+Provides-Extra: ibis-risingwave
+Requires-Dist: ibis-framework[risingwave]; extra == "ibis-risingwave"
+Provides-Extra: ibis-snowflake
+Requires-Dist: ibis-framework[snowflake]; extra == "ibis-snowflake"
+Provides-Extra: ibis-sqlite
+Requires-Dist: ibis-framework[sqlite]; extra == "ibis-sqlite"
+Provides-Extra: ibis-trino
+Requires-Dist: ibis-framework[trino]; extra == "ibis-trino"
+Provides-Extra: ibis
+Requires-Dist: ibis-framework; extra == "ibis"
+Provides-Extra: json-jsondataset
+Provides-Extra: json
+Requires-Dist: kedro-datasets[json-jsondataset]; extra == "json"
+Provides-Extra: matlab-matlabdataset
+Requires-Dist: scipy; extra == "matlab-matlabdataset"
+Provides-Extra: matlab
+Requires-Dist: kedro-datasets[matlab-matlabdataset]; extra == "matlab"
 Provides-Extra: matplotlib-matplotlibwriter
 Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "matplotlib-matplotlibwriter"
-Provides-Extra: networkx-networkxdataset
-Requires-Dist: networkx~=2.4; extra == "networkx-networkxdataset"
+Provides-Extra: matplotlib
+Requires-Dist: kedro-datasets[matplotlib-matplotlibwriter]; extra == "matplotlib"
+Provides-Extra: netcdf-netcdfdataset
+Requires-Dist: h5netcdf>=1.2.0; extra == "netcdf-netcdfdataset"
+Requires-Dist: netcdf4>=1.6.4; extra == "netcdf-netcdfdataset"
+Requires-Dist: xarray>=2023.1.0; extra == "netcdf-netcdfdataset"
+Provides-Extra: netcdf
+Requires-Dist: kedro-datasets[netcdf-netcdfdataset]; extra == "netcdf"
+Provides-Extra: networkx-gmldataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-gmldataset"
+Provides-Extra: networkx-graphmldataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-graphmldataset"
+Provides-Extra: networkx-jsondataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-jsondataset"
+Provides-Extra: networkx
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx"
 Provides-Extra: pandas-csvdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-csvdataset"
-Provides-Extra: pandas-exceldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-exceldataset"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas-exceldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-csvdataset"
 Provides-Extra: pandas-deltatabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-deltatabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-deltatabledataset"
 Requires-Dist: deltalake>=0.10.0; extra == "pandas-deltatabledataset"
+Provides-Extra: pandas-exceldataset
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-exceldataset"
+Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas-exceldataset"
 Provides-Extra: pandas-featherdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-featherdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-featherdataset"
 Provides-Extra: pandas-gbqtabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-gbqtabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-gbqtabledataset"
 Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas-gbqtabledataset"
 Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas-gbqtabledataset"
 Provides-Extra: pandas-gbqquerydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-gbqquerydataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-gbqquerydataset"
 Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas-gbqquerydataset"
 Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas-gbqquerydataset"
+Provides-Extra: pandas-genericdataset
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-genericdataset"
 Provides-Extra: pandas-hdfdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-hdfdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-hdfdataset"
 Requires-Dist: tables~=3.6; extra == "pandas-hdfdataset"
 Provides-Extra: pandas-jsondataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-jsondataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-jsondataset"
 Provides-Extra: pandas-parquetdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-parquetdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-parquetdataset"
 Requires-Dist: pyarrow>=6.0; extra == "pandas-parquetdataset"
 Provides-Extra: pandas-sqltabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-sqltabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-sqltabledataset"
 Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas-sqltabledataset"
 Provides-Extra: pandas-sqlquerydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-sqlquerydataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-sqlquerydataset"
 Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas-sqlquerydataset"
-Requires-Dist: pyodbc~=4.0; extra == "pandas-sqlquerydataset"
+Requires-Dist: pyodbc>=4.0; extra == "pandas-sqlquerydataset"
 Provides-Extra: pandas-xmldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-xmldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-xmldataset"
 Requires-Dist: lxml~=4.6; extra == "pandas-xmldataset"
-Provides-Extra: pandas-genericdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-genericdataset"
+Provides-Extra: pandas
+Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-deltatabledataset,pandas-exceldataset,pandas-featherdataset,pandas-gbqquerydataset,pandas-gbqtabledataset.pandas-genericdataset,pandas-hdfdataset,pandas-jsondataset,pandas-parquetdataset,pandas-sqlquerydataset,pandas-sqltabledataset,pandas-xmldataset]; extra == "pandas"
 Provides-Extra: pickle-pickledataset
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "pickle-pickledataset"
+Provides-Extra: pickle
+Requires-Dist: kedro-datasets[pickle-pickledataset]; extra == "pickle"
 Provides-Extra: pillow-imagedataset
 Requires-Dist: Pillow~=9.0; extra == "pillow-imagedataset"
-Provides-Extra: plotly-plotlydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "plotly-plotlydataset"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-plotlydataset"
+Provides-Extra: pillow
+Requires-Dist: kedro-datasets[pillow-imagedataset]; extra == "pillow"
 Provides-Extra: plotly-jsondataset
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-jsondataset"
+Requires-Dist: kedro-datasets[plotly-base]; extra == "plotly-jsondataset"
+Provides-Extra: plotly-plotlydataset
+Requires-Dist: kedro-datasets[pandas-base,plotly-base]; extra == "plotly-plotlydataset"
+Provides-Extra: plotly
+Requires-Dist: kedro-datasets[plotly-jsondataset,plotly-plotlydataset]; extra == "plotly"
 Provides-Extra: polars-csvdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-csvdataset"
-Provides-Extra: polars-genericdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-genericdataset"
-Requires-Dist: pyarrow>=4.0; extra == "polars-genericdataset"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-genericdataset"
-Requires-Dist: deltalake>=0.6.2; extra == "polars-genericdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-csvdataset"
 Provides-Extra: polars-eagerpolarsdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-eagerpolarsdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-eagerpolarsdataset"
 Requires-Dist: pyarrow>=4.0; extra == "polars-eagerpolarsdataset"
 Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-eagerpolarsdataset"
 Requires-Dist: deltalake>=0.6.2; extra == "polars-eagerpolarsdataset"
+Provides-Extra: polars-genericdataset
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-genericdataset"
+Requires-Dist: pyarrow>=4.0; extra == "polars-genericdataset"
+Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-genericdataset"
+Requires-Dist: deltalake>=0.6.2; extra == "polars-genericdataset"
 Provides-Extra: polars-lazypolarsdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-lazypolarsdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-lazypolarsdataset"
 Requires-Dist: pyarrow>=4.0; extra == "polars-lazypolarsdataset"
 Requires-Dist: deltalake>=0.6.2; extra == "polars-lazypolarsdataset"
+Provides-Extra: polars
+Requires-Dist: kedro-datasets[polars-genericdataset]; extra == "polars"
+Provides-Extra: redis-pickledataset
+Requires-Dist: redis~=4.1; extra == "redis-pickledataset"
+Provides-Extra: redis
+Requires-Dist: kedro-datasets[redis-pickledataset]; extra == "redis"
 Provides-Extra: snowflake-snowparktabledataset
 Requires-Dist: snowflake-snowpark-python~=1.0; extra == "snowflake-snowparktabledataset"
+Provides-Extra: snowflake
+Requires-Dist: kedro-datasets[snowflake-snowparktabledataset]; extra == "snowflake"
+Provides-Extra: spark-deltatabledataset
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-deltatabledataset"
+Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark-deltatabledataset"
 Provides-Extra: spark-sparkdataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkdataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkdataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkdataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkdataset"
 Provides-Extra: spark-sparkhivedataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkhivedataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkhivedataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkhivedataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkhivedataset"
 Provides-Extra: spark-sparkjdbcdataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkjdbcdataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkjdbcdataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkjdbcdataset"
-Provides-Extra: spark-deltatabledataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-deltatabledataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-deltatabledataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-deltatabledataset"
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark-deltatabledataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkjdbcdataset"
+Provides-Extra: spark
+Requires-Dist: kedro-datasets[spark-deltatabledataset]; extra == "spark"
 Provides-Extra: svmlight-svmlightdataset
 Requires-Dist: scikit-learn>=1.0.2; extra == "svmlight-svmlightdataset"
 Requires-Dist: scipy~=1.7.3; extra == "svmlight-svmlightdataset"
+Provides-Extra: svmlight
+Requires-Dist: kedro-datasets[svmlight-svmlightdataset]; extra == "svmlight"
 Provides-Extra: tensorflow-tensorflowmodeldataset
 Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "tensorflow-tensorflowmodeldataset"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "tensorflow-tensorflowmodeldataset"
+Provides-Extra: tensorflow
+Requires-Dist: kedro-datasets[tensorflow-tensorflowmodeldataset]; extra == "tensorflow"
+Provides-Extra: text-textdataset
+Provides-Extra: text
+Requires-Dist: kedro-datasets[text-textdataset]; extra == "text"
+Provides-Extra: tracking-jsondataset
+Provides-Extra: tracking-metricsdataset
+Provides-Extra: tracking
+Requires-Dist: kedro-datasets[tracking-jsondataset,tracking-metricsdataset]; extra == "tracking"
 Provides-Extra: video-videodataset
 Requires-Dist: opencv-python~=4.5.5.64; extra == "video-videodataset"
+Provides-Extra: video
+Requires-Dist: kedro-datasets[video-videodataset]; extra == "video"
 Provides-Extra: yaml-yamldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "yaml-yamldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "yaml-yamldataset"
 Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml-yamldataset"
-Provides-Extra: all
-Requires-Dist: Pillow~=9.0; extra == "all"
-Requires-Dist: PyYAML<7.0,>=4.2; extra == "all"
-Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "all"
-Requires-Dist: biopython~=1.73; extra == "all"
-Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "all"
-Requires-Dist: dask[complete]>=2021.10; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "all"
-Requires-Dist: delta-spark~=1.2.1; extra == "all"
-Requires-Dist: deltalake>=0.6.2; extra == "all"
-Requires-Dist: deltalake>=0.10.0; extra == "all"
-Requires-Dist: geopandas<1.0,>=0.6.0; extra == "all"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "all"
-Requires-Dist: holoviews~=1.13.0; extra == "all"
-Requires-Dist: huggingface_hub; extra == "all"
-Requires-Dist: lxml~=4.6; extra == "all"
-Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "all"
-Requires-Dist: networkx~=2.4; extra == "all"
-Requires-Dist: opencv-python~=4.5.5.64; extra == "all"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "all"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "all"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "all"
-Requires-Dist: pandas<3.0,>=1.3; extra == "all"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "all"
-Requires-Dist: polars>=0.18.0; extra == "all"
-Requires-Dist: pyarrow>=4.0; extra == "all"
-Requires-Dist: pyarrow>=6.0; extra == "all"
-Requires-Dist: pyodbc~=4.0; extra == "all"
-Requires-Dist: pyproj~=3.0; extra == "all"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "all"
-Requires-Dist: redis~=4.1; extra == "all"
-Requires-Dist: requests~=2.20; extra == "all"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "all"
-Requires-Dist: scikit-learn>=1.0.2; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: scipy~=1.7.3; extra == "all"
-Requires-Dist: snowflake-snowpark-python~=1.0; extra == "all"
-Requires-Dist: tables~=3.6; extra == "all"
-Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "all"
-Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "all"
-Requires-Dist: transformers; extra == "all"
-Requires-Dist: triad<1.0,>=0.6.7; extra == "all"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "all"
+Provides-Extra: yaml
+Requires-Dist: kedro-datasets[yaml-yamldataset]; extra == "yaml"
 Provides-Extra: docs
 Requires-Dist: docutils==0.16; extra == "docs"
 Requires-Dist: sphinx~=5.3.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme==1.2.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
 Requires-Dist: sphinx_copybutton==0.3.1; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
@@ -256,72 +264,75 @@
 Requires-Dist: blacken-docs==1.9.2; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: cloudpickle<=2.0.0; extra == "test"
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: dask[complete]>=2021.10; extra == "test"
 Requires-Dist: delta-spark<3.0,>=1.0; extra == "test"
-Requires-Dist: deltalake<0.15.2,>=0.10.0; extra == "test"
+Requires-Dist: deltalake>=0.10.0; extra == "test"
 Requires-Dist: dill~=0.3.1; extra == "test"
 Requires-Dist: filelock<4.0,>=3.4.0; extra == "test"
 Requires-Dist: gcsfs<2023.3,>=2023.1; extra == "test"
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "test"
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "test"
 Requires-Dist: holoviews>=1.13.0; extra == "test"
+Requires-Dist: ibis-framework[duckdb,examples]; extra == "test"
 Requires-Dist: import-linter[toml]==1.2.6; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; extra == "test"
 Requires-Dist: Jinja2<3.1.0; extra == "test"
 Requires-Dist: joblib>=0.14; extra == "test"
-Requires-Dist: jupyterlab~=3.0; extra == "test"
+Requires-Dist: jupyterlab>=3.0; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: lxml~=4.6; extra == "test"
 Requires-Dist: matplotlib<3.4,>=3.0.3; python_version < "3.10" and extra == "test"
 Requires-Dist: matplotlib<3.6,>=3.5; python_version >= "3.10" and extra == "test"
 Requires-Dist: memory_profiler<1.0,>=0.50.0; extra == "test"
 Requires-Dist: moto==5.0.0; extra == "test"
 Requires-Dist: networkx~=2.4; extra == "test"
 Requires-Dist: opencv-python~=4.5.5.64; extra == "test"
 Requires-Dist: openpyxl<4.0,>=3.0.3; extra == "test"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "test"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "test"
-Requires-Dist: pandas~=1.3; extra == "test"
+Requires-Dist: pandas-gbq>=0.12.0; extra == "test"
+Requires-Dist: pandas>=2.0; extra == "test"
 Requires-Dist: Pillow~=9.0; extra == "test"
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "test"
 Requires-Dist: polars[deltalake,xlsx2csv]~=0.18.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pyarrow>=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyarrow>=7.0; python_version >= "3.11" and extra == "test"
-Requires-Dist: pyodbc~=4.0.35; extra == "test"
+Requires-Dist: pyodbc~=5.0; extra == "test"
 Requires-Dist: pyproj~=3.0; extra == "test"
-Requires-Dist: pyspark<3.4,>=2.2; python_version < "3.11" and extra == "test"
+Requires-Dist: pyspark<3.4,>=3.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyspark>=3.4; python_version >= "3.11" and extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<2.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest~=7.2; extra == "test"
 Requires-Dist: redis~=4.1; extra == "test"
 Requires-Dist: requests-mock~=1.6; extra == "test"
 Requires-Dist: requests~=2.20; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: s3fs<2024.1,>=2021.04; extra == "test"
 Requires-Dist: snowflake-snowpark-python~=1.0; python_version == "3.9" and extra == "test"
 Requires-Dist: scikit-learn<2,>=1.0.2; extra == "test"
 Requires-Dist: scipy>=1.7.3; extra == "test"
 Requires-Dist: packaging; extra == "test"
-Requires-Dist: SQLAlchemy~=1.2; extra == "test"
-Requires-Dist: tables~=3.8.0; platform_system == "Windows" and extra == "test"
+Requires-Dist: SQLAlchemy>=1.2; extra == "test"
+Requires-Dist: tables>=3.8.0; platform_system == "Windows" and extra == "test"
 Requires-Dist: tables~=3.6; platform_system != "Windows" and extra == "test"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "test"
 Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "test"
 Requires-Dist: triad<1.0,>=0.6.7; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
+Requires-Dist: xarray>=2023.1.0; extra == "test"
 Requires-Dist: xlsxwriter~=1.0; extra == "test"
 Requires-Dist: datasets; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
-Requires-Dist: transformers; extra == "test"
+Requires-Dist: transformers[torch]; extra == "test"
+Provides-Extra: all
+Requires-Dist: kedro-datasets[docs,test]; extra == "all"
 
 # Kedro-Datasets
 
 <!-- Note that the contents of this file are also used in the documentation, see docs/source/index.md -->
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-datasets/)
```

### Comparing `kedro-datasets-2.1.0/README.md` & `kedro-datasets-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-2.1.0/kedro_datasets/__init__.py` & `kedro-datasets-3.0.0/kedro_datasets/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """``kedro_datasets`` is where you can find all of Kedro's data connectors."""
 
 __all__ = ["KedroDeprecationWarning"]
-__version__ = "2.1.0"
+__version__ = "3.0.0"
 
 import sys
 import warnings
 
 try:
     # Custom `KedroDeprecationWarning` class was added in Kedro 0.18.14.
     from kedro import KedroDeprecationWarning
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/_typing.py` & `kedro-datasets-3.0.0/kedro_datasets/_typing.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-2.1.0/kedro_datasets/api/api_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/api/api_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``APIDataset`` loads the data from HTTP(S) APIs.
 It uses the python requests library: https://requests.readthedocs.io/en/latest/
 """
+
 import json as json_  # make pylint happy
 from copy import deepcopy
 from typing import Any, Union
 
 import requests
 from kedro.io.core import AbstractDataset, DatasetError
 from requests import Session, sessions
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """BioSequenceDataset loads and saves data to/from bio-sequence objects to
 file.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from Bio import SeqIO
 from kedro.io.core import AbstractDataset, get_filepath_str, get_protocol_and_path
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/dask/parquet_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``ParquetDataset`` is a data set used to load and save data to parquet files using Dask
 dataframe"""
+
 from copy import deepcopy
 from typing import Any
 
 import dask.dataframe as dd
 import fsspec
 import triad
 from kedro.io.core import AbstractDataset, get_protocol_and_path
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ManagedTableDataset`` implementation to access managed delta tables
 in Databricks.
 """
+
 import logging
 import re
 from dataclasses import dataclass
 from typing import Any, Optional, Union
 
 import pandas as pd
 from kedro.io.core import (
@@ -184,15 +185,26 @@
         >>> import importlib_metadata
         >>>
         >>> DELTA_VERSION = importlib_metadata.version("delta-spark")
         >>> schema = StructType(
         ...     [StructField("name", StringType(), True), StructField("age", IntegerType(), True)]
         ... )
         >>> data = [("Alex", 31), ("Bob", 12), ("Clarke", 65), ("Dave", 29)]
-        >>> spark_df = SparkSession.builder.config("spark.jars.packages", f"io.delta:delta-core_2.12:{DELTA_VERSION}").config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension").config("spark.sql.catalog.spark_catalog","org.apache.spark.sql.delta.catalog.DeltaCatalog",).getOrCreate().createDataFrame(data, schema)
+        >>> spark_df = (
+        ...     SparkSession.builder.config(
+        ...         "spark.jars.packages", f"io.delta:delta-core_2.12:{DELTA_VERSION}"
+        ...     )
+        ...     .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
+        ...     .config(
+        ...         "spark.sql.catalog.spark_catalog",
+        ...         "org.apache.spark.sql.delta.catalog.DeltaCatalog",
+        ...     )
+        ...     .getOrCreate()
+        ...     .createDataFrame(data, schema)
+        ... )
         >>> dataset = ManagedTableDataset(table="names_and_ages", write_mode="overwrite")
         >>> dataset.save(spark_df)
         >>> reloaded = dataset.load()
         >>> assert Row(name="Bob", age=12) in reloaded.take(4)
     """
 
     # this dataset cannot be used with ``ParallelRunner``,
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/email/message_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/email/message_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``EmailMessageDataset`` loads/saves an email message from/to a file
 using an underlying filesystem (e.g.: local, S3, GCS). It uses the
 ``email`` package in the standard library to manage email messages.
 """
+
 from copy import deepcopy
 from email.generator import Generator
 from email.message import Message
 from email.parser import Parser
 from email.policy import default
 from pathlib import PurePosixPath
 from typing import Any
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """GeoJSONDataset loads and saves data to a local geojson file. The
 underlying functionality is supported by geopandas, so it supports all
 allowed geopandas (pandas) options for loading and saving geosjon files.
 """
+
 import copy
 from pathlib import PurePosixPath
 from typing import Any, Union
 
 import fsspec
 import geopandas as gpd
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-3.0.0/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-2.1.0/kedro_datasets/huggingface/hugging_face_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/huggingface/hugging_face_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,28 +19,38 @@
          type: kedro_hf_datasets.HFDataset
          dataset_name: yelp_review_full
 
     Example usage for the :doc:`Python API <kedro:data/advanced_data_catalog_usage>`:
 
     .. code-block:: pycon
 
+       >>> from datasets.utils.logging import disable_progress_bar, set_verbosity, ERROR
+       >>> disable_progress_bar()  # for doctest to pass
+       >>> set_verbosity(ERROR)  # for doctest to pass
        >>> from kedro_datasets.huggingface import HFDataset
-       >>> dataset = HFDataset(dataset_name="yelp_review_full")
-       >>> yelp_review_full = dataset.load()
-       >>> assert "train" in yelp_review_full
-       >>> assert "test" in yelp_review_full
-       >>> assert len(yelp_review_full["train"]) == 650000
+       >>> dataset = HFDataset(dataset_name="openai_humaneval")
+       >>> ds = dataset.load()  # doctest: +ELLIPSIS
+       Downloading and preparing dataset ...
+       Dataset ...
+       >>> assert "test" in ds
+       >>> assert len(ds["test"]) == 164
 
     """
 
-    def __init__(self, *, dataset_name: str):
+    def __init__(
+        self,
+        *,
+        dataset_name: str,
+        dataset_kwargs: dict[Any] | None = None,
+    ):
         self.dataset_name = dataset_name
+        self._dataset_kwargs = dataset_kwargs or {}
 
     def _load(self):
-        return load_dataset(self.dataset_name)
+        return load_dataset(self.dataset_name, **self._dataset_kwargs)
 
     def _save(self):
         raise NotImplementedError("Not yet implemented")
 
     def _describe(self) -> dict[str, Any]:
         api = HfApi()
         dataset_info = list(api.list_datasets(search=self.dataset_name))[0]
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/huggingface/transformer_pipeline_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,17 +25,17 @@
          model_name: Twitter/twhin-bert-base
 
     Example usage for the :doc:`Python API <kedro:data/advanced_data_catalog_usage>`:
 
     .. code-block:: pycon
 
        >>> from kedro_datasets.huggingface import HFTransformerPipelineDataset
-       >>> dataset = HFTransformerPipelineDataset(task="text-classification", model_name="papluca/xlm-roberta-base-language-detection")
-       >>> detector = dataset.load()
-       >>> assert detector("Ceci n'est pas une pipe")[0]["label"] == "fr"
+       >>> dataset = HFTransformerPipelineDataset(task="text-classification", model_name="prajjwal1/bert-tiny")
+       >>> model = dataset.load()
+       >>> assert model("Hello world")[0]["label"].startswith("LABEL_")
 
     """
 
     def __init__(
         self,
         *,
         task: str | None = None,
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/json/json_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/json/json_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """``JSONDataset`` loads/saves data from/to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 """
+
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
     AbstractVersionedDataset,
     DatasetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from kedro_datasets._typing import JSONPreview
+
 
 class JSONDataset(AbstractVersionedDataset[Any, Any]):
     """``JSONDataset`` loads/saves data from/to a JSON file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -155,7 +158,18 @@
         super()._release()
         self._invalidate_cache()
 
     def _invalidate_cache(self) -> None:
         """Invalidate underlying filesystem caches."""
         filepath = get_filepath_str(self._filepath, self._protocol)
         self._fs.invalidate_cache(filepath)
+
+    def preview(self) -> JSONPreview:
+        """
+        Generate a preview of the JSON dataset with a specified number of items.
+
+        Returns:
+            A string representing the JSON data for previewing.
+        """
+        data = self._load()
+
+        return json.dumps(data)
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/matlab/matlab_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/matlab/matlab_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``MatlabDataset`` loads/saves data from/to a Matlab file using an underlying
 filesystem ?(e.g.: local, S3, GCS)?. The underlying functionality is supported by
 the specified backend library passed in (defaults to the ``matlab`` library), so it
 supports all allowed options for loading and saving matlab files.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import numpy as np
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-3.0.0/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-2.1.0/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/networkx/gml_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """NetworkX ``GMLDataset`` loads and saves graphs to a graph modelling language (GML)
 file using an underlying filesystem (e.g.: local, S3, GCS). NetworkX is used to
 create GML data.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import networkx
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/networkx/graphml_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """NetworkX ``GraphMLDataset`` loads and saves graphs to a GraphML file using an underlying
 filesystem (e.g.: local, S3, GCS). NetworkX is used to create GraphML data.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import networkx
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/networkx/json_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads and saves graphs to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). NetworkX is used to create JSON data.
 """
+
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import networkx
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/__init__.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """``AbstractDataset`` implementations that produce pandas DataFrames."""
+
 from typing import Any
 
 import lazy_loader as lazy
 
 # https://github.com/pylint-dev/pylint/issues/4300#issuecomment-1043601901
 CSVDataset: Any
 DeltaTableDataset: Any
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/csv_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``CSVDataset`` loads/saves data from/to a CSV file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the CSV file.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/deltatable_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/deltatable_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``DeltaTableDataset`` loads/saves delta tables from/to a filesystem (e.g.: local,
 S3, GCS), Databricks unity catalog and AWS Glue catalog respectively. It handles
 load and save using a pandas dataframe.
 """
+
 from copy import deepcopy
 from typing import Any, Optional
 
 import pandas as pd
 from deltalake import DataCatalog, DeltaTable, Metadata
 from deltalake.exceptions import TableNotFoundError
 from deltalake.writer import write_deltalake
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/excel_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ExcelDataset`` loads/saves data from/to a Excel file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Excel file.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any, Union
 
 import fsspec
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/feather_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``FeatherDataset`` is a data set used to load and save data to feather files
 using an underlying filesystem (e.g.: local, S3, GCS). The underlying functionality
 is supported by pandas, so it supports all operations the pandas supports.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/gbq_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``GBQTableDataset`` loads and saves data from/to Google BigQuery. It uses pandas-gbq
 to read and write from/to BigQuery table.
 """
+
 import copy
 from pathlib import PurePosixPath
 from typing import Any, NoReturn, Union
 
 import fsspec
 import pandas as pd
 from google.cloud import bigquery
@@ -47,15 +48,17 @@
     .. code-block:: pycon
 
         >>> from kedro_datasets.pandas import GBQTableDataset
         >>> import pandas as pd
         >>>
         >>> data = pd.DataFrame({"col1": [1, 2], "col2": [4, 5], "col3": [5, 6]})
         >>>
-        >>> dataset = GBQTableDataset(dataset="dataset", table_name="table_name", project="my-project")
+        >>> dataset = GBQTableDataset(
+        ...     dataset="dataset", table_name="table_name", project="my-project"
+        ... )
         >>> dataset.save(data)
         >>> reloaded = dataset.load()
         >>>
         >>> assert data.equals(reloaded)
 
     """
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/generic_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``GenericDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the
 type of read/write target.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/hdf_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``HDFDataset`` loads/saves data from/to a hdf file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from threading import Lock
 from typing import Any
 
 import fsspec
 import pandas as pd
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/xml_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""``JSONDataset`` loads/saves data from/to a JSON file using an underlying
-filesystem (e.g.: local, S3, GCS). It uses pandas to handle the JSON file.
+"""``XMLDataset`` loads/saves data from/to a XML file using an underlying
+filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
@@ -17,96 +18,80 @@
     get_filepath_str,
     get_protocol_and_path,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class JSONDataset(AbstractVersionedDataset[pd.DataFrame, pd.DataFrame]):
-    """``JSONDataset`` loads/saves data from/to a JSON file using an underlying
-    filesystem (e.g.: local, S3, GCS). It uses pandas to handle the json file.
-
-    Example usage for the
-    `YAML API <https://kedro.readthedocs.io/en/stable/data/\
-    data_catalog_yaml_examples.html>`_:
-
-    .. code-block:: yaml
-
-        clickstream_dataset:
-          type: pandas.JSONDataset
-          filepath: abfs://landing_area/primary/click_stream.json
-          credentials: abfs_creds
-
-        json_dataset:
-          type: pandas.JSONDataset
-          filepath: data/01_raw/Video_Games.json
-          load_args:
-            lines: True
+class XMLDataset(AbstractVersionedDataset[pd.DataFrame, pd.DataFrame]):
+    """``XMLDataset`` loads/saves data from/to a XML file using an underlying
+    filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
 
     Example usage for the
     `Python API <https://kedro.readthedocs.io/en/stable/data/\
     advanced_data_catalog_usage.html>`_:
 
     .. code-block:: pycon
 
-        >>> from kedro_datasets.pandas import JSONDataset
+        >>> from kedro_datasets.pandas import XMLDataset
         >>> import pandas as pd
         >>>
         >>> data = pd.DataFrame({"col1": [1, 2], "col2": [4, 5], "col3": [5, 6]})
         >>>
-        >>> dataset = JSONDataset(filepath=tmp_path / "test.json")
+        >>> dataset = XMLDataset(filepath=tmp_path / "test.xml")
         >>> dataset.save(data)
         >>> reloaded = dataset.load()
         >>> assert data.equals(reloaded)
 
     """
 
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
-    DEFAULT_SAVE_ARGS: dict[str, Any] = {}
+    DEFAULT_SAVE_ARGS: dict[str, Any] = {"index": False}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         load_args: dict[str, Any] = None,
         save_args: dict[str, Any] = None,
         version: Version = None,
         credentials: dict[str, Any] = None,
         fs_args: dict[str, Any] = None,
         metadata: dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``JSONDataset`` pointing to a concrete JSON file
+        """Creates a new instance of ``XMLDataset`` pointing to a concrete XML file
         on a specific filesystem.
 
         Args:
-            filepath: Filepath in POSIX format to a JSON file prefixed with a protocol like `s3://`.
-                If prefix is not provided `file` protocol (local filesystem) will be used.
+            filepath: Filepath in POSIX format to a XML file prefixed with a protocol like `s3://`.
+                If prefix is not provided, `file` protocol (local filesystem) will be used.
                 The prefix should be any protocol supported by ``fsspec``.
                 Note: `http(s)` doesn't support versioning.
-            load_args: Pandas options for loading JSON files.
+            load_args: Pandas options for loading XML files.
                 Here you can find all available arguments:
-                https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_json.html
+                https://pandas.pydata.org/docs/reference/api/pandas.read_xml.html
                 All defaults are preserved.
-            save_args: Pandas options for saving JSON files.
+            save_args: Pandas options for saving XML files.
                 Here you can find all available arguments:
-                https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.to_json.html
+                https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_xml.html
                 All defaults are preserved, but "index", which is set to False.
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
-                E.g. for ``GCSFileSystem`` it should look like `{'token': None}`.
+                E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
             metadata: Any arbitrary metadata.
                 This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _credentials = deepcopy(credentials) or {}
+
         protocol, path = get_protocol_and_path(filepath, version)
         if protocol == "file":
             _fs_args.setdefault("auto_mkdir", True)
 
         self._protocol = protocol
         self._storage_options = {**_credentials, **_fs_args}
         self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
@@ -149,26 +134,26 @@
     def _load(self) -> pd.DataFrame:
         load_path = str(self._get_load_path())
         if self._protocol == "file":
             # file:// protocol seems to misbehave on Windows
             # (<urlopen error file not on local host>),
             # so we don't join that back to the filepath;
             # storage_options also don't work with local paths
-            return pd.read_json(load_path, **self._load_args)
+            return pd.read_xml(load_path, **self._load_args)
 
         load_path = f"{self._protocol}{PROTOCOL_DELIMITER}{load_path}"
-        return pd.read_json(
+        return pd.read_xml(
             load_path, storage_options=self._storage_options, **self._load_args
         )
 
     def _save(self, data: pd.DataFrame) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
 
         buf = BytesIO()
-        data.to_json(path_or_buf=buf, **self._save_args)
+        data.to_xml(path_or_buffer=buf, **self._save_args)
 
         with self._fs.open(save_path, mode="wb") as fs_file:
             fs_file.write(buf.getvalue())
 
         self._invalidate_cache()
 
     def _exists(self) -> bool:
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/parquet_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ParquetDataset`` loads/saves data from/to a Parquet file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Parquet file.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import Path, PurePosixPath
 from typing import Any
 
 import fsspec
@@ -14,14 +15,16 @@
     AbstractVersionedDataset,
     DatasetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from kedro_datasets._typing import TablePreview
+
 logger = logging.getLogger(__name__)
 
 
 class ParquetDataset(AbstractVersionedDataset[pd.DataFrame, pd.DataFrame]):
     """``ParquetDataset`` loads/saves data from/to a Parquet file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Parquet file.
 
@@ -209,7 +212,28 @@
         super()._release()
         self._invalidate_cache()
 
     def _invalidate_cache(self) -> None:
         """Invalidate underlying filesystem caches."""
         filepath = get_filepath_str(self._filepath, self._protocol)
         self._fs.invalidate_cache(filepath)
+
+    def preview(self, nrows: int = 5) -> TablePreview:
+        """
+        Generate a preview of the dataset with a specified number of rows.
+
+        Args:
+            nrows: The number of rows to include in the preview. Defaults to 5.
+
+        Returns:
+            dict: A dictionary containing the data in a split format.
+        """
+        import pyarrow.parquet as pq
+
+        load_path = str(self._get_load_path())
+
+        table = pq.read_table(
+            load_path, columns=self._load_args.get("columns"), use_threads=True
+        )[:nrows]
+        data_preview = table.to_pandas()
+
+        return data_preview.to_dict(orient="split")
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pandas/sql_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """``SQLDataset`` to load and save data to a SQL backend."""
+
 from __future__ import annotations
 
 import copy
 import datetime as dt
 import re
 from pathlib import PurePosixPath
 from typing import Any, NoReturn
@@ -11,17 +12,19 @@
 import pandas as pd
 from kedro.io.core import (
     AbstractDataset,
     DatasetError,
     get_filepath_str,
     get_protocol_and_path,
 )
-from sqlalchemy import create_engine, inspect
+from sqlalchemy import MetaData, Table, create_engine, inspect, select
 from sqlalchemy.exc import NoSuchModuleError
 
+from kedro_datasets._typing import TablePreview
+
 __all__ = ["SQLTableDataset", "SQLQueryDataset"]
 
 KNOWN_PIP_INSTALL = {
     "psycopg2": "psycopg2",
     "mysqldb": "mysqlclient",
     "cx_Oracle": "cx_Oracle",
     "mssql": "pyodbc",
@@ -221,19 +224,22 @@
         self._connection_args = {
             k: credentials[k] for k in credentials.keys() if k != "con"
         }
 
         self.metadata = metadata
 
     @classmethod
-    def create_connection(cls, connection_str: str, connection_args: dict) -> None:
+    def create_connection(
+        cls, connection_str: str, connection_args: dict | None = None
+    ) -> None:
         """Given a connection string, create singleton connection
         to be used across all instances of ``SQLTableDataset`` that
         need to connect to the same source.
         """
+        connection_args = connection_args or {}
         try:
             engine = create_engine(connection_str, **connection_args)
         except ImportError as import_error:
             raise _get_missing_module_error(import_error) from import_error
         except NoSuchModuleError as exc:
             raise _get_sql_alchemy_missing_error() from exc
 
@@ -267,14 +273,39 @@
         data.to_sql(con=self.engine, **self._save_args)
 
     def _exists(self) -> bool:
         insp = inspect(self.engine)
         schema = self._load_args.get("schema", None)
         return insp.has_table(self._load_args["table_name"], schema)
 
+    def preview(self, nrows: int = 5) -> TablePreview:
+        """
+        Generate a preview of the dataset with a specified number of rows.
+
+        Args:
+            nrows: The number of rows to include in the preview. Defaults to 5.
+
+        Returns:
+            dict: A dictionary containing the data in a split format.
+        """
+
+        table_name = self._load_args["table_name"]
+
+        metadata = MetaData()
+        table_ref = Table(table_name, metadata, autoload_with=self.engine)
+
+        query = select(table_ref).limit(nrows)
+
+        with self.engine.connect() as conn:
+            result = conn.execute(query)
+            data_preview = pd.DataFrame(result.fetchall(), columns=result.keys())
+
+        preview_data = data_preview.to_dict(orient="split")
+        return preview_data
+
 
 class SQLQueryDataset(AbstractDataset[None, pd.DataFrame]):
     """``SQLQueryDataset`` loads data from a provided SQL query. It
     uses ``pandas.DataFrame`` internally, so it supports all allowed
     pandas options on ``read_sql_query``. Since Pandas uses SQLAlchemy behind
     the scenes, when instantiating ``SQLQueryDataset`` one needs to pass
     a compatible connection string either in ``credentials`` (see the example
@@ -493,19 +524,22 @@
             k: credentials[k] for k in credentials.keys() if k != "con"
         }
         self._execution_options = execution_options or {}
         if "mssql" in self._connection_str:
             self.adapt_mssql_date_params()
 
     @classmethod
-    def create_connection(cls, connection_str: str, connection_args: dict) -> None:
+    def create_connection(
+        cls, connection_str: str, connection_args: dict | None = None
+    ) -> None:
         """Given a connection string, create singleton connection
         to be used across all instances of `SQLQueryDataset` that
         need to connect to the same source.
         """
+        connection_args = connection_args or {}
         try:
             engine = create_engine(connection_str, **connection_args)
         except ImportError as import_error:
             raise _get_missing_module_error(import_error) from import_error
         except NoSuchModuleError as exc:
             raise _get_sql_alchemy_missing_error() from exc
 
@@ -562,8 +596,8 @@
             try:
                 as_date = dt.date.fromisoformat(value)
                 new_val = dt.datetime.combine(as_date, dt.time.min)
                 new_load_args.append(new_val.strftime("%Y-%m-%dT%H:%M:%S"))
             except (TypeError, ValueError):
                 new_load_args.append(value)
         if new_load_args:
-            self._load_args["params"] = new_load_args
+            self._load_args["params"] = tuple(new_load_args)
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,158 @@
-"""``XMLDataset`` loads/saves data from/to a XML file using an underlying
-filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
-"""
-import logging
+"""SparkStreamingDataset to load and save a PySpark Streaming DataFrame."""
+
 from copy import deepcopy
-from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
-import fsspec
-import pandas as pd
-from kedro.io.core import (
-    PROTOCOL_DELIMITER,
-    AbstractVersionedDataset,
-    DatasetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
+from kedro.io.core import AbstractDataset
+from pyspark.sql import DataFrame
+from pyspark.sql.utils import AnalysisException
+
+from kedro_datasets.spark.spark_dataset import (
+    SparkDataset,
+    _get_spark,
+    _split_filepath,
+    _strip_dbfs_prefix,
 )
 
-logger = logging.getLogger(__name__)
-
 
-class XMLDataset(AbstractVersionedDataset[pd.DataFrame, pd.DataFrame]):
-    """``XMLDataset`` loads/saves data from/to a XML file using an underlying
-    filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
+class SparkStreamingDataset(AbstractDataset):
+    """``SparkStreamingDataset`` loads data to Spark Streaming Dataframe objects.
 
     Example usage for the
-    `Python API <https://kedro.readthedocs.io/en/stable/data/\
-    advanced_data_catalog_usage.html>`_:
-
-    .. code-block:: pycon
+    `YAML API <https://kedro.readthedocs.io/en/stable/data/\
+    data_catalog_yaml_examples.html>`_:
 
-        >>> from kedro_datasets.pandas import XMLDataset
-        >>> import pandas as pd
-        >>>
-        >>> data = pd.DataFrame({"col1": [1, 2], "col2": [4, 5], "col3": [5, 6]})
-        >>>
-        >>> dataset = XMLDataset(filepath=tmp_path / "test.xml")
-        >>> dataset.save(data)
-        >>> reloaded = dataset.load()
-        >>> assert data.equals(reloaded)
+    .. code-block:: yaml
 
+        raw.new_inventory:
+          type: spark.SparkStreamingDataset
+          filepath: data/01_raw/stream/inventory/
+          file_format: json
+          save_args:
+            output_mode: append
+            checkpoint: data/04_checkpoint/raw_new_inventory
+            header: True
+          load_args:
+            schema:
+                filepath: data/01_raw/schema/inventory_schema.json
     """
 
-    DEFAULT_LOAD_ARGS: dict[str, Any] = {}
-    DEFAULT_SAVE_ARGS: dict[str, Any] = {"index": False}
+    DEFAULT_LOAD_ARGS = {}  # type: Dict[str, Any]
+    DEFAULT_SAVE_ARGS = {}  # type: Dict[str, Any]
 
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         *,
-        filepath: str,
-        load_args: dict[str, Any] = None,
+        filepath: str = "",
+        file_format: str = "",
         save_args: dict[str, Any] = None,
-        version: Version = None,
-        credentials: dict[str, Any] = None,
-        fs_args: dict[str, Any] = None,
-        metadata: dict[str, Any] = None,
+        load_args: dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``XMLDataset`` pointing to a concrete XML file
-        on a specific filesystem.
+        """Creates a new instance of SparkStreamingDataset.
 
         Args:
-            filepath: Filepath in POSIX format to a XML file prefixed with a protocol like `s3://`.
-                If prefix is not provided, `file` protocol (local filesystem) will be used.
-                The prefix should be any protocol supported by ``fsspec``.
-                Note: `http(s)` doesn't support versioning.
-            load_args: Pandas options for loading XML files.
-                Here you can find all available arguments:
-                https://pandas.pydata.org/docs/reference/api/pandas.read_xml.html
-                All defaults are preserved.
-            save_args: Pandas options for saving XML files.
-                Here you can find all available arguments:
-                https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_xml.html
-                All defaults are preserved, but "index", which is set to False.
-            version: If specified, should be an instance of
-                ``kedro.io.core.Version``. If its ``load`` attribute is
-                None, the latest version will be loaded. If its ``save``
-                attribute is None, save version will be autogenerated.
-            credentials: Credentials required to get access to the underlying filesystem.
-                E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
-            fs_args: Extra arguments to pass into underlying filesystem class constructor
-                (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
-            metadata: Any arbitrary metadata.
-                This is ignored by Kedro, but may be consumed by users or external plugins.
+            filepath: Filepath in POSIX format to a Spark dataframe. When using Databricks
+                specify ``filepath``s starting with ``/dbfs/``. For message brokers such as
+                Kafka and all filepath is not required.
+            file_format: File format used during load and save operations.
+                These are formats supported by the running SparkContext including parquet,
+                csv, and delta. For a list of supported formats please refer to the Apache
+                Spark documentation at
+                https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html
+            load_args: Load args passed to Spark DataFrameReader load method.
+                It is dependent on the selected file format. You can find a list of read options
+                for each selected format in Spark DataFrame read documentation, see
+                https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html.
+                Please note that a schema is mandatory for a streaming DataFrame
+                if ``schemaInference`` is not True.
+            save_args: Save args passed to Spark DataFrameReader write options.
+                Similar to load_args, this is dependent on the selected file format. You can pass
+                ``mode`` and ``partitionBy`` to specify your overwrite mode and partitioning
+                respectively. You can find a list of options for each selected format in
+                Spark DataFrame write documentation, see
+                https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html
         """
-        _fs_args = deepcopy(fs_args) or {}
-        _credentials = deepcopy(credentials) or {}
+        self._file_format = file_format
+        self._save_args = save_args
+        self._load_args = load_args
 
-        protocol, path = get_protocol_and_path(filepath, version)
-        if protocol == "file":
-            _fs_args.setdefault("auto_mkdir", True)
-
-        self._protocol = protocol
-        self._storage_options = {**_credentials, **_fs_args}
-        self._fs = fsspec.filesystem(self._protocol, **self._storage_options)
-
-        self.metadata = metadata
-
-        super().__init__(
-            filepath=PurePosixPath(path),
-            version=version,
-            exists_function=self._fs.exists,
-            glob_function=self._fs.glob,
-        )
+        fs_prefix, filepath = _split_filepath(filepath)
+
+        self._fs_prefix = fs_prefix
+        self._filepath = PurePosixPath(filepath)
 
         # Handle default load and save arguments
         self._load_args = deepcopy(self.DEFAULT_LOAD_ARGS)
         if load_args is not None:
             self._load_args.update(load_args)
         self._save_args = deepcopy(self.DEFAULT_SAVE_ARGS)
         if save_args is not None:
             self._save_args.update(save_args)
 
-        if "storage_options" in self._save_args or "storage_options" in self._load_args:
-            logger.warning(
-                "Dropping 'storage_options' for %s, "
-                "please specify them under 'fs_args' or 'credentials'.",
-                self._filepath,
-            )
-            self._save_args.pop("storage_options", None)
-            self._load_args.pop("storage_options", None)
+        # Handle schema load argument
+        self._schema = self._load_args.pop("schema", None)
+        if self._schema is not None:
+            if isinstance(self._schema, dict):
+                self._schema = SparkDataset._load_schema_from_file(self._schema)
 
     def _describe(self) -> dict[str, Any]:
+        """Returns a dict that describes attributes of the dataset."""
         return {
-            "filepath": self._filepath,
-            "protocol": self._protocol,
+            "filepath": self._fs_prefix + str(self._filepath),
+            "file_format": self._file_format,
             "load_args": self._load_args,
             "save_args": self._save_args,
-            "version": self._version,
         }
 
-    def _load(self) -> pd.DataFrame:
-        load_path = str(self._get_load_path())
-        if self._protocol == "file":
-            # file:// protocol seems to misbehave on Windows
-            # (<urlopen error file not on local host>),
-            # so we don't join that back to the filepath;
-            # storage_options also don't work with local paths
-            return pd.read_xml(load_path, **self._load_args)
-
-        load_path = f"{self._protocol}{PROTOCOL_DELIMITER}{load_path}"
-        return pd.read_xml(
-            load_path, storage_options=self._storage_options, **self._load_args
+    def _load(self) -> DataFrame:
+        """Loads data from filepath.
+        If the connector type is kafka then no file_path is required, schema needs to be
+        seperated from load_args.
+        Returns:
+            Data from filepath as pyspark dataframe.
+        """
+        load_path = _strip_dbfs_prefix(self._fs_prefix + str(self._filepath))
+        data_stream_reader = (
+            _get_spark()
+            .readStream.schema(self._schema)
+            .format(self._file_format)
+            .options(**self._load_args)
         )
+        return data_stream_reader.load(load_path)
 
-    def _save(self, data: pd.DataFrame) -> None:
-        save_path = get_filepath_str(self._get_save_path(), self._protocol)
-
-        buf = BytesIO()
-        data.to_xml(path_or_buffer=buf, **self._save_args)
-
-        with self._fs.open(save_path, mode="wb") as fs_file:
-            fs_file.write(buf.getvalue())
+    def _save(self, data: DataFrame) -> None:
+        """Saves pyspark dataframe.
+        Args:
+            data: PySpark streaming dataframe for saving
+        """
+        save_path = _strip_dbfs_prefix(self._fs_prefix + str(self._filepath))
+        output_constructor = data.writeStream.format(self._file_format)
 
-        self._invalidate_cache()
+        (
+            output_constructor.option(
+                "checkpointLocation", self._save_args.pop("checkpoint")
+            )
+            .option("path", save_path)
+            .outputMode(self._save_args.pop("output_mode"))
+            .options(**self._save_args)
+            .start()
+        )
 
     def _exists(self) -> bool:
+        load_path = _strip_dbfs_prefix(self._fs_prefix + str(self._filepath))
+
         try:
-            load_path = get_filepath_str(self._get_load_path(), self._protocol)
-        except DatasetError:
-            return False
-
-        return self._fs.exists(load_path)
-
-    def _release(self) -> None:
-        super()._release()
-        self._invalidate_cache()
-
-    def _invalidate_cache(self) -> None:
-        """Invalidate underlying filesystem caches."""
-        filepath = get_filepath_str(self._filepath, self._protocol)
-        self._fs.invalidate_cache(filepath)
+            _get_spark().readStream.schema(self._schema).load(
+                load_path, self._file_format
+            )
+        except AnalysisException as exception:
+            # `AnalysisException.desc` is deprecated with pyspark >= 3.4
+            message = exception.desc if hasattr(exception, "desc") else str(exception)
+            if (
+                "Path does not exist:" in message
+                or "is not a Streaming data" in message
+            ):
+                return False
+            raise
+        return True
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/partitions/incremental_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/partitions/incremental_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """``IncrementalDataset`` inherits from ``PartitionedDataset``, which loads
 and saves partitioned file-like data using the underlying dataset
 definition. ``IncrementalDataset`` also stores the information about the last
 processed partition in so-called `checkpoint` that is persisted to the location
 of the data partitions by default, so that subsequent pipeline run loads only
 new partitions past the checkpoint.It also uses `fsspec` for filesystem level operations.
 """
+
 from __future__ import annotations
 
 import operator
 from copy import deepcopy
 from typing import Any, Callable
 
 from cachetools import cachedmethod
@@ -40,15 +41,17 @@
 
     Example:
 
     .. code-block:: pycon
 
         >>> from kedro_datasets.partitions import IncrementalDataset
         >>>
-        >>> dataset = IncrementalDataset(path=str(tmp_path/ "test_data"), dataset="pandas.CSVDataset")
+        >>> dataset = IncrementalDataset(
+        ...     path=str(tmp_path / "test_data"), dataset="pandas.CSVDataset"
+        ... )
         >>> loaded = dataset.load()  # loads all available partitions
         >>> # assert isinstance(loaded, dict)
         >>>
         >>> dataset.confirm()  # update checkpoint value to the last processed partition ID
         >>> reloaded = dataset.load()  # still loads all available partitions
         >>>
         >>> dataset.release()  # clears load cache
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/partitions/partitioned_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/partitions/partitioned_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``PartitionedDataset`` loads and saves partitioned file-like data using the
 underlying dataset definition. It also uses `fsspec` for filesystem level operations.
 """
+
 from __future__ import annotations
 
 import operator
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Callable
 from urllib.parse import urlparse
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pickle/pickle_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``PickleDataset`` loads/saves data from/to a Pickle file using an underlying
 filesystem (e.g.: local, S3, GCS). The underlying functionality is supported by
 the specified backend library passed in (defaults to the ``pickle`` library), so it
 supports all allowed options for loading and saving pickle files.
 """
+
 import importlib
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/pillow/image_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``ImageDataset`` loads/saves image data as `numpy` from an underlying
 filesystem (e.g.: local, S3, GCS). It uses Pillow to handle image file.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
     AbstractVersionedDataset,
@@ -30,15 +31,17 @@
         >>>
         >>> import pytest
         >>> from kedro_datasets.pillow import ImageDataset
         >>>
         >>> if sys.platform.startswith("win"):
         ...     pytest.skip("this doctest hangs on Windows CI runner")
         ...
-        >>> dataset = ImageDataset(filepath="https://storage.googleapis.com/gtv-videos-bucket/sample/images/ForBiggerBlazes.jpg")
+        >>> dataset = ImageDataset(
+        ...     filepath="https://storage.googleapis.com/gtv-videos-bucket/sample/images/ForBiggerBlazes.jpg"
+        ... )
         >>> image = dataset.load()
         >>> image.show()
 
     """
 
     DEFAULT_SAVE_ARGS: dict[str, Any] = {}
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/plotly/json_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``JSONDataset`` loads/saves a plotly figure from/to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS).
 """
+
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Union
 
 import fsspec
 import plotly.io as pio
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/plotly/plotly_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``PlotlyDataset`` generates a plot from a pandas DataFrame and saves it to a JSON
 file using an underlying filesystem (e.g.: local, S3, GCS). It loads the JSON into a
 plotly figure.
 """
+
 import json
 from copy import deepcopy
 from typing import Any
 
 import pandas as pd
 import plotly.express as px
 from kedro.io.core import Version, get_filepath_str
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/polars/__init__.py` & `kedro-datasets-3.0.0/kedro_datasets/polars/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """``AbstractDataset`` implementations that produce pandas DataFrames."""
+
 from typing import Any
 
 import lazy_loader as lazy
 
 # https://github.com/pylint-dev/pylint/issues/4300#issuecomment-1043601901
 CSVDataset: Any
 EagerPolarsDataset: Any
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/polars/csv_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``CSVDataset`` loads/saves data from/to a CSV file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the CSV file.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/polars/eager_polars_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/polars/eager_polars_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``EagerPolarsDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the
 type of read/write target.
 """
+
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import polars as pl
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/polars/lazy_polars_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/polars/lazy_polars_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``LazyPolarsDataset`` loads/saves data from/to a data file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses polars to handle the
 type of read/write target.
 """
+
 import logging
 from copy import deepcopy
 from io import BytesIO
 from pathlib import PurePosixPath
 from typing import Any, ClassVar, Optional, Union
 
 import fsspec
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/redis/redis_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``PickleDataset`` loads/saves data from/to a Redis database. The underlying
 functionality is supported by the redis library, so it supports all allowed
 options for instantiating the redis app ``from_url`` and setting a value."""
+
 import importlib
 import os
 from copy import deepcopy
 from typing import Any
 
 import redis
 from kedro.io.core import AbstractDataset, DatasetError
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """``AbstractDataset`` implementation to access Snowflake using Snowpark dataframes
 """
+
 import logging
 from copy import deepcopy
 from typing import Any
 
 import snowflake.snowpark as sp
 from kedro.io.core import AbstractDataset, DatasetError
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/spark/__init__.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides I/O modules for Apache Spark."""
+
 from typing import Any
 
 import lazy_loader as lazy
 
 # https://github.com/pylint-dev/pylint/issues/4300#issuecomment-1043601901
 DeltaTableDataset: Any
 SparkDataset: Any
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/deltatable_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``AbstractDataset`` implementation to access DeltaTables using
 ``delta-spark``.
 """
+
 from pathlib import PurePosixPath
 from typing import Any, NoReturn
 
 from delta.tables import DeltaTable
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql.utils import AnalysisException
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/spark_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``AbstractVersionedDataset`` implementation to access Spark dataframes using
 ``pyspark``.
 """
+
 from __future__ import annotations
 
 import json
 import logging
 import os
 from copy import deepcopy
 from fnmatch import fnmatch
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``AbstractDataset`` implementation to access Spark dataframes using
 ``pyspark`` on Apache Hive.
 """
+
 import pickle
 from copy import deepcopy
 from typing import Any
 
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql import DataFrame, Window
 from pyspark.sql.functions import col, lit, row_number
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """SparkJDBCDataset to load and save a PySpark DataFrame via JDBC."""
+
 from copy import deepcopy
 from typing import Any
 
 from kedro.io.core import AbstractDataset, DatasetError
 from pyspark.sql import DataFrame
 
 from kedro_datasets.spark.spark_dataset import _get_spark
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``SVMLightDataset`` loads/saves data from/to a svmlight/libsvm file using an
 underlying filesystem (e.g.: local, S3, GCS). It uses sklearn functions
 ``dump_svmlight_file`` to save and ``load_svmlight_file`` to load a file.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Optional, Union
 
 import fsspec
 from kedro.io.core import (
     AbstractVersionedDataset,
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``TensorFlowModelDataset`` is a dataset implementation which can save and load
 TensorFlow models.
 """
+
 import copy
 import tempfile
 from pathlib import PurePath, PurePosixPath
 from typing import Any
 
 import fsspec
 import tensorflow as tf
@@ -13,14 +14,15 @@
     DatasetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
 TEMPORARY_H5_FILE = "tmp_tensorflow_model.h5"
+TEMPORARY_KERAS_FILE = "tmp_tensorflow_model.keras"
 
 
 class TensorFlowModelDataset(AbstractVersionedDataset[tf.keras.Model, tf.keras.Model]):
     """``TensorFlowModelDataset`` loads and saves TensorFlow models.
     The underlying functionality is supported by, and passes input arguments through to,
     TensorFlow 2.X load_model and save_model methods.
 
@@ -46,27 +48,31 @@
 
     .. code-block:: pycon
 
         >>> from kedro_datasets.tensorflow import TensorFlowModelDataset
         >>> import tensorflow as tf
         >>> import numpy as np
         >>>
-        >>> dataset = TensorFlowModelDataset(filepath=tmp_path / "data/06_models/tensorflow_model.h5")
-        >>> model = tf.keras.Sequential([tf.keras.layers.Dense(5, input_shape=(3,)),tf.keras.layers.Softmax()])
+        >>> dataset = TensorFlowModelDataset(
+        ...     filepath=tmp_path / "data/06_models/tensorflow_model.h5"
+        ... )
+        >>> model = tf.keras.Sequential(
+        ...     [tf.keras.layers.Dense(5, input_shape=(3,)), tf.keras.layers.Softmax()]
+        ... )
         >>>
-        >>> # x = tf.random.uniform((10, 3))
+        >>> # x = tf.random.uniform((10, 3))
         >>> # predictions = model.predict(x)
         >>>
         >>> dataset.save(model)
         >>> loaded_model = dataset.load()
 
     """
 
     DEFAULT_LOAD_ARGS: dict[str, Any] = {}
-    DEFAULT_SAVE_ARGS: dict[str, Any] = {"save_format": "tf"}
+    DEFAULT_SAVE_ARGS: dict[str, Any] = {}
 
     def __init__(  # noqa: PLR0913
         self,
         *,
         filepath: str,
         load_args: dict[str, Any] = None,
         save_args: dict[str, Any] = None,
@@ -130,47 +136,47 @@
             self._save_args.update(save_args)
 
         self._is_h5 = self._save_args.get("save_format") == "h5"
 
     def _load(self) -> tf.keras.Model:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
 
-        with tempfile.TemporaryDirectory(prefix=self._tmp_prefix) as path:
+        with tempfile.TemporaryDirectory(prefix=self._tmp_prefix) as tempdir:
             if self._is_h5:
-                path = str(PurePath(path) / TEMPORARY_H5_FILE)  # noqa: PLW2901
-                self._fs.copy(load_path, path)
+                path = str(PurePath(tempdir) / TEMPORARY_H5_FILE)  # noqa: PLW2901
             else:
-                self._fs.get(load_path + "/", path, recursive=True)
+                # We assume .keras
+                path = str(PurePath(tempdir) / TEMPORARY_KERAS_FILE)  # noqa: PLW2901
+
+            self._fs.copy(load_path, path)
 
             # Pass the local temporary directory/file path to keras.load_model
             device_name = self._load_args.pop("tf_device", None)
             if device_name:
                 with tf.device(device_name):
                     model = tf.keras.models.load_model(path, **self._load_args)
             else:
                 model = tf.keras.models.load_model(path, **self._load_args)
             return model
 
     def _save(self, data: tf.keras.Model) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
 
-        with tempfile.TemporaryDirectory(prefix=self._tmp_prefix) as path:
+        with tempfile.TemporaryDirectory(prefix=self._tmp_prefix) as tempdir:
             if self._is_h5:
-                path = str(PurePath(path) / TEMPORARY_H5_FILE)  # noqa: PLW2901
+                path = str(PurePath(tempdir) / TEMPORARY_H5_FILE)  # noqa: PLW2901
+            else:
+                # We assume .keras
+                path = str(PurePath(tempdir) / TEMPORARY_KERAS_FILE)  # noqa: PLW2901
 
             tf.keras.models.save_model(data, path, **self._save_args)
 
             # Use fsspec to take from local tempfile directory/file and
             # put in ArbitraryFileSystem
-            if self._is_h5:
-                self._fs.copy(path, save_path)
-            else:
-                if self._fs.exists(save_path):
-                    self._fs.rm(save_path, recursive=True)
-                self._fs.put(path, save_path, recursive=True)
+            self._fs.copy(path, save_path)
 
     def _exists(self) -> bool:
         try:
             load_path = get_filepath_str(self._get_load_path(), self._protocol)
         except DatasetError:
             return False
         return self._fs.exists(load_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/text/text_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/text/text_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``TextDataset`` loads/saves data from/to a text file using an underlying
 filesystem (e.g.: local, S3, GCS).
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 from kedro.io.core import (
     AbstractVersionedDataset,
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/tracking/json_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``JSONDataset`` saves data to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 The ``JSONDataset`` is part of Kedro Experiment Tracking. The dataset is versioned by default.
 """
+
 import json
 from typing import NoReturn
 
 from kedro.io.core import DatasetError, get_filepath_str
 
 from kedro_datasets._typing import JSONTrackingPreview
 from kedro_datasets.json import json_dataset
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/tracking/metrics_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``MetricsDataset`` saves data to a JSON file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 The ``MetricsDataset`` is part of Kedro Experiment Tracking. The dataset is versioned by default
 and only takes metrics of numeric values.
 """
+
 import json
 from typing import NoReturn
 
 from kedro.io.core import DatasetError, get_filepath_str
 
 from kedro_datasets._typing import MetricsTrackingPreview
 from kedro_datasets.json import json_dataset
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/video/video_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/video/video_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """``VideoDataset`` loads/saves video data from an underlying
 filesystem (e.g.: local, S3, GCS). It uses OpenCV VideoCapture to read
 and decode videos and OpenCV VideoWriter to encode and write video.
 """
+
 import itertools
 import tempfile
 from collections import abc
 from collections.abc import Generator, Sequence
 from copy import deepcopy
 from pathlib import Path, PurePosixPath
 from typing import Any, Optional, Union
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-3.0.0/kedro_datasets/yaml/yaml_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """``YAMLDataset`` loads/saves data from/to a YAML file using an underlying
 filesystem (e.g.: local, S3, GCS). It uses PyYAML to handle the YAML file.
 """
+
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any
 
 import fsspec
 import yaml
 from kedro.io.core import (
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets.egg-info/PKG-INFO` & `kedro-datasets-3.0.0/kedro_datasets.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,246 +1,254 @@
 Metadata-Version: 2.1
 Name: kedro-datasets
-Version: 2.1.0
+Version: 3.0.0
 Summary: Kedro-Datasets is where you can find all of Kedro's data connectors.
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-datasets
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: kedro>=0.19
 Requires-Dist: lazy_loader
-Provides-Extra: api
-Requires-Dist: requests~=2.20; extra == "api"
-Provides-Extra: biosequence
-Requires-Dist: biopython~=1.73; extra == "biosequence"
-Provides-Extra: dask
-Requires-Dist: dask[complete]>=2021.10; extra == "dask"
-Requires-Dist: triad<1.0,>=0.6.7; extra == "dask"
-Provides-Extra: databricks
-Requires-Dist: delta-spark~=1.2.1; extra == "databricks"
-Requires-Dist: pandas<3.0,>=1.3; extra == "databricks"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "databricks"
-Provides-Extra: geopandas
-Requires-Dist: geopandas<1.0,>=0.6.0; extra == "geopandas"
-Requires-Dist: pyproj~=3.0; extra == "geopandas"
-Provides-Extra: holoviews
-Requires-Dist: holoviews~=1.13.0; extra == "holoviews"
-Provides-Extra: huggingface
-Requires-Dist: datasets; extra == "huggingface"
-Requires-Dist: huggingface_hub; extra == "huggingface"
-Requires-Dist: transformers; extra == "huggingface"
-Provides-Extra: matlab
-Requires-Dist: scipy; extra == "matlab"
-Provides-Extra: matplotlib
-Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "matplotlib"
-Provides-Extra: networkx
-Requires-Dist: networkx~=2.4; extra == "networkx"
-Provides-Extra: pandas
-Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas"
-Requires-Dist: deltalake>=0.10.0; extra == "pandas"
-Requires-Dist: lxml~=4.6; extra == "pandas"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas"
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas"
-Requires-Dist: pyarrow>=6.0; extra == "pandas"
-Requires-Dist: pyodbc~=4.0; extra == "pandas"
-Requires-Dist: tables~=3.6; extra == "pandas"
-Provides-Extra: pickle
-Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "pickle"
-Provides-Extra: pillow
-Requires-Dist: Pillow~=9.0; extra == "pillow"
-Provides-Extra: plotly
-Requires-Dist: pandas<3.0,>=1.3; extra == "plotly"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly"
-Provides-Extra: polars
-Requires-Dist: deltalake>=0.6.2; extra == "polars"
-Requires-Dist: polars>=0.18.0; extra == "polars"
-Requires-Dist: pyarrow>=4.0; extra == "polars"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "polars"
-Provides-Extra: redis
-Requires-Dist: redis~=4.1; extra == "redis"
-Provides-Extra: snowflake
-Requires-Dist: snowflake-snowpark-python~=1.0; extra == "snowflake"
-Provides-Extra: spark
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark"
-Provides-Extra: svmlight
-Requires-Dist: scikit-learn>=1.0.2; extra == "svmlight"
-Requires-Dist: scipy~=1.7.3; extra == "svmlight"
-Provides-Extra: tensorflow
-Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "tensorflow"
-Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "tensorflow"
-Provides-Extra: video
-Requires-Dist: opencv-python~=4.5.5.64; extra == "video"
-Provides-Extra: yaml
-Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml"
-Requires-Dist: pandas<3.0,>=1.3; extra == "yaml"
+Provides-Extra: pandas-base
+Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-base"
+Provides-Extra: spark-base
+Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-base"
+Provides-Extra: hdfs-base
+Requires-Dist: hdfs<3.0,>=2.5.8; extra == "hdfs-base"
+Provides-Extra: s3fs-base
+Requires-Dist: s3fs<2024.1,>=2021.4; extra == "s3fs-base"
+Provides-Extra: polars-base
+Requires-Dist: polars>=0.18.0; extra == "polars-base"
+Provides-Extra: plotly-base
+Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-base"
+Provides-Extra: delta-base
+Requires-Dist: delta-spark~=1.2.1; extra == "delta-base"
+Provides-Extra: networkx-base
+Requires-Dist: networkx~=2.4; extra == "networkx-base"
 Provides-Extra: api-apidataset
 Requires-Dist: requests~=2.20; extra == "api-apidataset"
+Provides-Extra: api
+Requires-Dist: kedro-datasets[api-apidataset]; extra == "api"
 Provides-Extra: biosequence-biosequencedataset
 Requires-Dist: biopython~=1.73; extra == "biosequence-biosequencedataset"
+Provides-Extra: biosequence
+Requires-Dist: kedro-datasets[biosequence-biosequencedataset]; extra == "biosequence"
 Provides-Extra: dask-parquetdataset
 Requires-Dist: dask[complete]>=2021.10; extra == "dask-parquetdataset"
 Requires-Dist: triad<1.0,>=0.6.7; extra == "dask-parquetdataset"
+Provides-Extra: dask
+Requires-Dist: kedro-datasets[dask-parquetdataset]; extra == "dask"
 Provides-Extra: databricks-managedtabledataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "databricks-managedtabledataset"
-Requires-Dist: pandas<3.0,>=1.3; extra == "databricks-managedtabledataset"
-Requires-Dist: delta-spark~=1.2.1; extra == "databricks-managedtabledataset"
+Requires-Dist: kedro-datasets[delta-base,pandas-base,spark-base]; extra == "databricks-managedtabledataset"
+Provides-Extra: databricks
+Requires-Dist: kedro-datasets[databricks-managedtabledataset]; extra == "databricks"
 Provides-Extra: geopandas-geojsondataset
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "geopandas-geojsondataset"
 Requires-Dist: pyproj~=3.0; extra == "geopandas-geojsondataset"
+Provides-Extra: geopandas
+Requires-Dist: kedro-datasets[geopandas-geojsondataset]; extra == "geopandas"
 Provides-Extra: holoviews-holoviewswriter
 Requires-Dist: holoviews~=1.13.0; extra == "holoviews-holoviewswriter"
+Provides-Extra: holoviews
+Requires-Dist: kedro-datasets[holoviews-holoviewswriter]; extra == "holoviews"
+Provides-Extra: huggingface-hfdataset
+Requires-Dist: datasets; extra == "huggingface-hfdataset"
+Requires-Dist: huggingface_hub; extra == "huggingface-hfdataset"
+Provides-Extra: huggingface-hftransformerpipelinedataset
+Requires-Dist: transformers; extra == "huggingface-hftransformerpipelinedataset"
+Provides-Extra: huggingface
+Requires-Dist: kedro-datasets[huggingface-hfdataset,huggingface-hftransformerpipelinedataset]; extra == "huggingface"
+Provides-Extra: ibis-bigquery
+Requires-Dist: ibis-framework[bigquery]; extra == "ibis-bigquery"
+Provides-Extra: ibis-clickhouse
+Requires-Dist: ibis-framework[clickhouse]; extra == "ibis-clickhouse"
+Provides-Extra: ibis-dask
+Requires-Dist: ibis-framework[dask]; extra == "ibis-dask"
+Provides-Extra: ibis-datafusion
+Requires-Dist: ibis-framework[datafusion]; extra == "ibis-datafusion"
+Provides-Extra: ibis-druid
+Requires-Dist: ibis-framework[druid]; extra == "ibis-druid"
+Provides-Extra: ibis-duckdb
+Requires-Dist: ibis-framework[duckdb]; extra == "ibis-duckdb"
+Provides-Extra: ibis-exasol
+Requires-Dist: ibis-framework[exasol]; extra == "ibis-exasol"
+Provides-Extra: ibis-flink
+Requires-Dist: ibis-framework; extra == "ibis-flink"
+Requires-Dist: apache-flink; extra == "ibis-flink"
+Provides-Extra: ibis-impala
+Requires-Dist: ibis-framework[impala]; extra == "ibis-impala"
+Provides-Extra: ibis-mssql
+Requires-Dist: ibis-framework[mssql]; extra == "ibis-mssql"
+Provides-Extra: ibis-mysql
+Requires-Dist: ibis-framework[mysql]; extra == "ibis-mysql"
+Provides-Extra: ibis-oracle
+Requires-Dist: ibis-framework[oracle]; extra == "ibis-oracle"
+Provides-Extra: ibis-pandas
+Requires-Dist: ibis-framework[pandas]; extra == "ibis-pandas"
+Provides-Extra: ibis-polars
+Requires-Dist: ibis-framework[polars]; extra == "ibis-polars"
+Provides-Extra: ibis-postgres
+Requires-Dist: ibis-framework[postgres]; extra == "ibis-postgres"
+Provides-Extra: ibis-pyspark
+Requires-Dist: ibis-framework[pyspark]; extra == "ibis-pyspark"
+Provides-Extra: ibis-risingwave
+Requires-Dist: ibis-framework[risingwave]; extra == "ibis-risingwave"
+Provides-Extra: ibis-snowflake
+Requires-Dist: ibis-framework[snowflake]; extra == "ibis-snowflake"
+Provides-Extra: ibis-sqlite
+Requires-Dist: ibis-framework[sqlite]; extra == "ibis-sqlite"
+Provides-Extra: ibis-trino
+Requires-Dist: ibis-framework[trino]; extra == "ibis-trino"
+Provides-Extra: ibis
+Requires-Dist: ibis-framework; extra == "ibis"
+Provides-Extra: json-jsondataset
+Provides-Extra: json
+Requires-Dist: kedro-datasets[json-jsondataset]; extra == "json"
+Provides-Extra: matlab-matlabdataset
+Requires-Dist: scipy; extra == "matlab-matlabdataset"
+Provides-Extra: matlab
+Requires-Dist: kedro-datasets[matlab-matlabdataset]; extra == "matlab"
 Provides-Extra: matplotlib-matplotlibwriter
 Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "matplotlib-matplotlibwriter"
-Provides-Extra: networkx-networkxdataset
-Requires-Dist: networkx~=2.4; extra == "networkx-networkxdataset"
+Provides-Extra: matplotlib
+Requires-Dist: kedro-datasets[matplotlib-matplotlibwriter]; extra == "matplotlib"
+Provides-Extra: netcdf-netcdfdataset
+Requires-Dist: h5netcdf>=1.2.0; extra == "netcdf-netcdfdataset"
+Requires-Dist: netcdf4>=1.6.4; extra == "netcdf-netcdfdataset"
+Requires-Dist: xarray>=2023.1.0; extra == "netcdf-netcdfdataset"
+Provides-Extra: netcdf
+Requires-Dist: kedro-datasets[netcdf-netcdfdataset]; extra == "netcdf"
+Provides-Extra: networkx-gmldataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-gmldataset"
+Provides-Extra: networkx-graphmldataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-graphmldataset"
+Provides-Extra: networkx-jsondataset
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx-jsondataset"
+Provides-Extra: networkx
+Requires-Dist: kedro-datasets[networkx-base]; extra == "networkx"
 Provides-Extra: pandas-csvdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-csvdataset"
-Provides-Extra: pandas-exceldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-exceldataset"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas-exceldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-csvdataset"
 Provides-Extra: pandas-deltatabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-deltatabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-deltatabledataset"
 Requires-Dist: deltalake>=0.10.0; extra == "pandas-deltatabledataset"
+Provides-Extra: pandas-exceldataset
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-exceldataset"
+Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "pandas-exceldataset"
 Provides-Extra: pandas-featherdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-featherdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-featherdataset"
 Provides-Extra: pandas-gbqtabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-gbqtabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-gbqtabledataset"
 Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas-gbqtabledataset"
 Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas-gbqtabledataset"
 Provides-Extra: pandas-gbqquerydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-gbqquerydataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-gbqquerydataset"
 Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "pandas-gbqquerydataset"
 Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "pandas-gbqquerydataset"
+Provides-Extra: pandas-genericdataset
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-genericdataset"
 Provides-Extra: pandas-hdfdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-hdfdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-hdfdataset"
 Requires-Dist: tables~=3.6; extra == "pandas-hdfdataset"
 Provides-Extra: pandas-jsondataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-jsondataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-jsondataset"
 Provides-Extra: pandas-parquetdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-parquetdataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-parquetdataset"
 Requires-Dist: pyarrow>=6.0; extra == "pandas-parquetdataset"
 Provides-Extra: pandas-sqltabledataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-sqltabledataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-sqltabledataset"
 Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas-sqltabledataset"
 Provides-Extra: pandas-sqlquerydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-sqlquerydataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-sqlquerydataset"
 Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "pandas-sqlquerydataset"
-Requires-Dist: pyodbc~=4.0; extra == "pandas-sqlquerydataset"
+Requires-Dist: pyodbc>=4.0; extra == "pandas-sqlquerydataset"
 Provides-Extra: pandas-xmldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-xmldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "pandas-xmldataset"
 Requires-Dist: lxml~=4.6; extra == "pandas-xmldataset"
-Provides-Extra: pandas-genericdataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "pandas-genericdataset"
+Provides-Extra: pandas
+Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-deltatabledataset,pandas-exceldataset,pandas-featherdataset,pandas-gbqquerydataset,pandas-gbqtabledataset.pandas-genericdataset,pandas-hdfdataset,pandas-jsondataset,pandas-parquetdataset,pandas-sqlquerydataset,pandas-sqltabledataset,pandas-xmldataset]; extra == "pandas"
 Provides-Extra: pickle-pickledataset
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "pickle-pickledataset"
+Provides-Extra: pickle
+Requires-Dist: kedro-datasets[pickle-pickledataset]; extra == "pickle"
 Provides-Extra: pillow-imagedataset
 Requires-Dist: Pillow~=9.0; extra == "pillow-imagedataset"
-Provides-Extra: plotly-plotlydataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "plotly-plotlydataset"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-plotlydataset"
+Provides-Extra: pillow
+Requires-Dist: kedro-datasets[pillow-imagedataset]; extra == "pillow"
 Provides-Extra: plotly-jsondataset
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "plotly-jsondataset"
+Requires-Dist: kedro-datasets[plotly-base]; extra == "plotly-jsondataset"
+Provides-Extra: plotly-plotlydataset
+Requires-Dist: kedro-datasets[pandas-base,plotly-base]; extra == "plotly-plotlydataset"
+Provides-Extra: plotly
+Requires-Dist: kedro-datasets[plotly-jsondataset,plotly-plotlydataset]; extra == "plotly"
 Provides-Extra: polars-csvdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-csvdataset"
-Provides-Extra: polars-genericdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-genericdataset"
-Requires-Dist: pyarrow>=4.0; extra == "polars-genericdataset"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-genericdataset"
-Requires-Dist: deltalake>=0.6.2; extra == "polars-genericdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-csvdataset"
 Provides-Extra: polars-eagerpolarsdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-eagerpolarsdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-eagerpolarsdataset"
 Requires-Dist: pyarrow>=4.0; extra == "polars-eagerpolarsdataset"
 Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-eagerpolarsdataset"
 Requires-Dist: deltalake>=0.6.2; extra == "polars-eagerpolarsdataset"
+Provides-Extra: polars-genericdataset
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-genericdataset"
+Requires-Dist: pyarrow>=4.0; extra == "polars-genericdataset"
+Requires-Dist: xlsx2csv>=0.8.0; extra == "polars-genericdataset"
+Requires-Dist: deltalake>=0.6.2; extra == "polars-genericdataset"
 Provides-Extra: polars-lazypolarsdataset
-Requires-Dist: polars>=0.18.0; extra == "polars-lazypolarsdataset"
+Requires-Dist: kedro-datasets[polars-base]; extra == "polars-lazypolarsdataset"
 Requires-Dist: pyarrow>=4.0; extra == "polars-lazypolarsdataset"
 Requires-Dist: deltalake>=0.6.2; extra == "polars-lazypolarsdataset"
+Provides-Extra: polars
+Requires-Dist: kedro-datasets[polars-genericdataset]; extra == "polars"
+Provides-Extra: redis-pickledataset
+Requires-Dist: redis~=4.1; extra == "redis-pickledataset"
+Provides-Extra: redis
+Requires-Dist: kedro-datasets[redis-pickledataset]; extra == "redis"
 Provides-Extra: snowflake-snowparktabledataset
 Requires-Dist: snowflake-snowpark-python~=1.0; extra == "snowflake-snowparktabledataset"
+Provides-Extra: snowflake
+Requires-Dist: kedro-datasets[snowflake-snowparktabledataset]; extra == "snowflake"
+Provides-Extra: spark-deltatabledataset
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-deltatabledataset"
+Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark-deltatabledataset"
 Provides-Extra: spark-sparkdataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkdataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkdataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkdataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkdataset"
 Provides-Extra: spark-sparkhivedataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkhivedataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkhivedataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkhivedataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkhivedataset"
 Provides-Extra: spark-sparkjdbcdataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-sparkjdbcdataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-sparkjdbcdataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-sparkjdbcdataset"
-Provides-Extra: spark-deltatabledataset
-Requires-Dist: pyspark<4.0,>=2.2; extra == "spark-deltatabledataset"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "spark-deltatabledataset"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "spark-deltatabledataset"
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "spark-deltatabledataset"
+Requires-Dist: kedro-datasets[hdfs-base,s3fs-base,spark-base]; extra == "spark-sparkjdbcdataset"
+Provides-Extra: spark
+Requires-Dist: kedro-datasets[spark-deltatabledataset]; extra == "spark"
 Provides-Extra: svmlight-svmlightdataset
 Requires-Dist: scikit-learn>=1.0.2; extra == "svmlight-svmlightdataset"
 Requires-Dist: scipy~=1.7.3; extra == "svmlight-svmlightdataset"
+Provides-Extra: svmlight
+Requires-Dist: kedro-datasets[svmlight-svmlightdataset]; extra == "svmlight"
 Provides-Extra: tensorflow-tensorflowmodeldataset
 Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "tensorflow-tensorflowmodeldataset"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "tensorflow-tensorflowmodeldataset"
+Provides-Extra: tensorflow
+Requires-Dist: kedro-datasets[tensorflow-tensorflowmodeldataset]; extra == "tensorflow"
+Provides-Extra: text-textdataset
+Provides-Extra: text
+Requires-Dist: kedro-datasets[text-textdataset]; extra == "text"
+Provides-Extra: tracking-jsondataset
+Provides-Extra: tracking-metricsdataset
+Provides-Extra: tracking
+Requires-Dist: kedro-datasets[tracking-jsondataset,tracking-metricsdataset]; extra == "tracking"
 Provides-Extra: video-videodataset
 Requires-Dist: opencv-python~=4.5.5.64; extra == "video-videodataset"
+Provides-Extra: video
+Requires-Dist: kedro-datasets[video-videodataset]; extra == "video"
 Provides-Extra: yaml-yamldataset
-Requires-Dist: pandas<3.0,>=1.3; extra == "yaml-yamldataset"
+Requires-Dist: kedro-datasets[pandas-base]; extra == "yaml-yamldataset"
 Requires-Dist: PyYAML<7.0,>=4.2; extra == "yaml-yamldataset"
-Provides-Extra: all
-Requires-Dist: Pillow~=9.0; extra == "all"
-Requires-Dist: PyYAML<7.0,>=4.2; extra == "all"
-Requires-Dist: SQLAlchemy<3.0,>=1.4; extra == "all"
-Requires-Dist: biopython~=1.73; extra == "all"
-Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "all"
-Requires-Dist: dask[complete]>=2021.10; extra == "all"
-Requires-Dist: datasets; extra == "all"
-Requires-Dist: delta-spark<3.0,>=1.0; extra == "all"
-Requires-Dist: delta-spark~=1.2.1; extra == "all"
-Requires-Dist: deltalake>=0.6.2; extra == "all"
-Requires-Dist: deltalake>=0.10.0; extra == "all"
-Requires-Dist: geopandas<1.0,>=0.6.0; extra == "all"
-Requires-Dist: hdfs<3.0,>=2.5.8; extra == "all"
-Requires-Dist: holoviews~=1.13.0; extra == "all"
-Requires-Dist: huggingface_hub; extra == "all"
-Requires-Dist: lxml~=4.6; extra == "all"
-Requires-Dist: matplotlib<4.0,>=3.0.3; extra == "all"
-Requires-Dist: networkx~=2.4; extra == "all"
-Requires-Dist: opencv-python~=4.5.5.64; extra == "all"
-Requires-Dist: openpyxl<4.0,>=3.0.6; extra == "all"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "all"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "all"
-Requires-Dist: pandas<3.0,>=1.3; extra == "all"
-Requires-Dist: plotly<6.0,>=4.8.0; extra == "all"
-Requires-Dist: polars>=0.18.0; extra == "all"
-Requires-Dist: pyarrow>=4.0; extra == "all"
-Requires-Dist: pyarrow>=6.0; extra == "all"
-Requires-Dist: pyodbc~=4.0; extra == "all"
-Requires-Dist: pyproj~=3.0; extra == "all"
-Requires-Dist: pyspark<4.0,>=2.2; extra == "all"
-Requires-Dist: redis~=4.1; extra == "all"
-Requires-Dist: requests~=2.20; extra == "all"
-Requires-Dist: s3fs<2024.1,>=2021.4; extra == "all"
-Requires-Dist: scikit-learn>=1.0.2; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: scipy~=1.7.3; extra == "all"
-Requires-Dist: snowflake-snowpark-python~=1.0; extra == "all"
-Requires-Dist: tables~=3.6; extra == "all"
-Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "all"
-Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "all"
-Requires-Dist: transformers; extra == "all"
-Requires-Dist: triad<1.0,>=0.6.7; extra == "all"
-Requires-Dist: xlsx2csv>=0.8.0; extra == "all"
+Provides-Extra: yaml
+Requires-Dist: kedro-datasets[yaml-yamldataset]; extra == "yaml"
 Provides-Extra: docs
 Requires-Dist: docutils==0.16; extra == "docs"
 Requires-Dist: sphinx~=5.3.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme==1.2.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.20.2; extra == "docs"
 Requires-Dist: sphinx_copybutton==0.3.1; extra == "docs"
 Requires-Dist: sphinx-notfound-page; extra == "docs"
@@ -256,72 +264,75 @@
 Requires-Dist: blacken-docs==1.9.2; extra == "test"
 Requires-Dist: black~=22.0; extra == "test"
 Requires-Dist: cloudpickle<=2.0.0; extra == "test"
 Requires-Dist: compress-pickle[lz4]~=2.1.0; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: dask[complete]>=2021.10; extra == "test"
 Requires-Dist: delta-spark<3.0,>=1.0; extra == "test"
-Requires-Dist: deltalake<0.15.2,>=0.10.0; extra == "test"
+Requires-Dist: deltalake>=0.10.0; extra == "test"
 Requires-Dist: dill~=0.3.1; extra == "test"
 Requires-Dist: filelock<4.0,>=3.4.0; extra == "test"
 Requires-Dist: gcsfs<2023.3,>=2023.1; extra == "test"
 Requires-Dist: geopandas<1.0,>=0.6.0; extra == "test"
 Requires-Dist: hdfs<3.0,>=2.5.8; extra == "test"
 Requires-Dist: holoviews>=1.13.0; extra == "test"
+Requires-Dist: ibis-framework[duckdb,examples]; extra == "test"
 Requires-Dist: import-linter[toml]==1.2.6; extra == "test"
 Requires-Dist: ipython<8.0,>=7.31.1; extra == "test"
 Requires-Dist: Jinja2<3.1.0; extra == "test"
 Requires-Dist: joblib>=0.14; extra == "test"
-Requires-Dist: jupyterlab~=3.0; extra == "test"
+Requires-Dist: jupyterlab>=3.0; extra == "test"
 Requires-Dist: jupyter~=1.0; extra == "test"
 Requires-Dist: lxml~=4.6; extra == "test"
 Requires-Dist: matplotlib<3.4,>=3.0.3; python_version < "3.10" and extra == "test"
 Requires-Dist: matplotlib<3.6,>=3.5; python_version >= "3.10" and extra == "test"
 Requires-Dist: memory_profiler<1.0,>=0.50.0; extra == "test"
 Requires-Dist: moto==5.0.0; extra == "test"
 Requires-Dist: networkx~=2.4; extra == "test"
 Requires-Dist: opencv-python~=4.5.5.64; extra == "test"
 Requires-Dist: openpyxl<4.0,>=3.0.3; extra == "test"
-Requires-Dist: pandas-gbq<0.18.0,>=0.12.0; python_version < "3.11" and extra == "test"
-Requires-Dist: pandas-gbq>=0.18.0; python_version >= "3.11" and extra == "test"
-Requires-Dist: pandas~=1.3; extra == "test"
+Requires-Dist: pandas-gbq>=0.12.0; extra == "test"
+Requires-Dist: pandas>=2.0; extra == "test"
 Requires-Dist: Pillow~=9.0; extra == "test"
 Requires-Dist: plotly<6.0,>=4.8.0; extra == "test"
 Requires-Dist: polars[deltalake,xlsx2csv]~=0.18.0; extra == "test"
 Requires-Dist: pre-commit>=2.9.2; extra == "test"
 Requires-Dist: pyarrow>=1.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyarrow>=7.0; python_version >= "3.11" and extra == "test"
-Requires-Dist: pyodbc~=4.0.35; extra == "test"
+Requires-Dist: pyodbc~=5.0; extra == "test"
 Requires-Dist: pyproj~=3.0; extra == "test"
-Requires-Dist: pyspark<3.4,>=2.2; python_version < "3.11" and extra == "test"
+Requires-Dist: pyspark<3.4,>=3.0; python_version < "3.11" and extra == "test"
 Requires-Dist: pyspark>=3.4; python_version >= "3.11" and extra == "test"
 Requires-Dist: pytest-cov~=3.0; extra == "test"
 Requires-Dist: pytest-mock<2.0,>=1.7.1; extra == "test"
 Requires-Dist: pytest-xdist[psutil]~=2.2.1; extra == "test"
 Requires-Dist: pytest~=7.2; extra == "test"
 Requires-Dist: redis~=4.1; extra == "test"
 Requires-Dist: requests-mock~=1.6; extra == "test"
 Requires-Dist: requests~=2.20; extra == "test"
 Requires-Dist: ruff~=0.0.290; extra == "test"
 Requires-Dist: s3fs<2024.1,>=2021.04; extra == "test"
 Requires-Dist: snowflake-snowpark-python~=1.0; python_version == "3.9" and extra == "test"
 Requires-Dist: scikit-learn<2,>=1.0.2; extra == "test"
 Requires-Dist: scipy>=1.7.3; extra == "test"
 Requires-Dist: packaging; extra == "test"
-Requires-Dist: SQLAlchemy~=1.2; extra == "test"
-Requires-Dist: tables~=3.8.0; platform_system == "Windows" and extra == "test"
+Requires-Dist: SQLAlchemy>=1.2; extra == "test"
+Requires-Dist: tables>=3.8.0; platform_system == "Windows" and extra == "test"
 Requires-Dist: tables~=3.6; platform_system != "Windows" and extra == "test"
 Requires-Dist: tensorflow-macos~=2.0; (platform_system == "Darwin" and platform_machine == "arm64") and extra == "test"
 Requires-Dist: tensorflow~=2.0; (platform_system != "Darwin" or platform_machine != "arm64") and extra == "test"
 Requires-Dist: triad<1.0,>=0.6.7; extra == "test"
 Requires-Dist: trufflehog~=2.1; extra == "test"
+Requires-Dist: xarray>=2023.1.0; extra == "test"
 Requires-Dist: xlsxwriter~=1.0; extra == "test"
 Requires-Dist: datasets; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
-Requires-Dist: transformers; extra == "test"
+Requires-Dist: transformers[torch]; extra == "test"
+Provides-Extra: all
+Requires-Dist: kedro-datasets[docs,test]; extra == "all"
 
 # Kedro-Datasets
 
 <!-- Note that the contents of this file are also used in the documentation, see docs/source/index.md -->
 
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://pypi.org/project/kedro-datasets/)
```

### Comparing `kedro-datasets-2.1.0/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-3.0.0/kedro_datasets.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 kedro_datasets/__init__.py
 kedro_datasets/_typing.py
 kedro_datasets.egg-info/PKG-INFO
 kedro_datasets.egg-info/SOURCES.txt
 kedro_datasets.egg-info/dependency_links.txt
 kedro_datasets.egg-info/requires.txt
 kedro_datasets.egg-info/top_level.txt
@@ -22,20 +21,24 @@
 kedro_datasets/geopandas/__init__.py
 kedro_datasets/geopandas/geojson_dataset.py
 kedro_datasets/holoviews/__init__.py
 kedro_datasets/holoviews/holoviews_writer.py
 kedro_datasets/huggingface/__init__.py
 kedro_datasets/huggingface/hugging_face_dataset.py
 kedro_datasets/huggingface/transformer_pipeline_dataset.py
+kedro_datasets/ibis/__init__.py
+kedro_datasets/ibis/table_dataset.py
 kedro_datasets/json/__init__.py
 kedro_datasets/json/json_dataset.py
 kedro_datasets/matlab/__init__.py
 kedro_datasets/matlab/matlab_dataset.py
 kedro_datasets/matplotlib/__init__.py
 kedro_datasets/matplotlib/matplotlib_writer.py
+kedro_datasets/netcdf/__init__.py
+kedro_datasets/netcdf/netcdf_dataset.py
 kedro_datasets/networkx/__init__.py
 kedro_datasets/networkx/gml_dataset.py
 kedro_datasets/networkx/graphml_dataset.py
 kedro_datasets/networkx/json_dataset.py
 kedro_datasets/pandas/__init__.py
 kedro_datasets/pandas/csv_dataset.py
 kedro_datasets/pandas/deltatable_dataset.py
```

