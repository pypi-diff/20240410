# Comparing `tmp/CosmoTech-SupplyChain-5.2.2.tar.gz` & `tmp/CosmoTech-SupplyChain-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-5.2.2.tar", last modified: Mon Oct  2 14:35:31 2023, max compression
+gzip compressed data, was "CosmoTech-SupplyChain-5.3.0.tar", last modified: Wed Apr 10 10:18:34 2024, max compression
```

## Comparing `CosmoTech-SupplyChain-5.2.2.tar` & `CosmoTech-SupplyChain-5.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.637900 CosmoTech-SupplyChain-5.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.625899 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-02 14:35:31.000000 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-10-02 14:35:31.000000 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 14:35:31.000000 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-02 14:35:31.000000 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-02 14:35:31.000000 CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-02 14:35:31.637900 CosmoTech-SupplyChain-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.625899 CosmoTech-SupplyChain-5.2.2/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.629899 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.629899 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.633900 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/stochastic_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24264 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22540 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis_helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.633900 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    23267 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.633900 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    40023 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    52415 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.633900 CosmoTech-SupplyChain-5.2.2/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21965 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:31.633900 CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    18536 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-02 14:35:31.637900 CosmoTech-SupplyChain-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-10-02 14:35:19.000000 CosmoTech-SupplyChain-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 10:18:34.000000 CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.911934 CosmoTech-SupplyChain-5.3.0/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.915934 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.915934 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20725 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/stochastic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41114 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52415 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.919934 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23908 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19839 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:18:34.923935 CosmoTech-SupplyChain-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-10 10:18:31.000000 CosmoTech-SupplyChain-5.3.0/setup.py
```

### Comparing `CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/PKG-INFO` & `CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-SupplyChain
-Version: 5.2.2
+Version: 5.3.0
 Summary: A support package for SupplyChain
 Home-page: https://github.com/Cosmo-Tech/supplychain-python-library<
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: azure-core
```

### Comparing `CosmoTech-SupplyChain-5.2.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `CosmoTech-SupplyChain-5.3.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/LICENSE` & `CosmoTech-SupplyChain-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/PKG-INFO` & `CosmoTech-SupplyChain-5.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CosmoTech-SupplyChain
-Version: 5.2.2
+Version: 5.3.0
 Summary: A support package for SupplyChain
 Home-page: https://github.com/Cosmo-Tech/supplychain-python-library<
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: azure-core
```

### Comparing `CosmoTech-SupplyChain-5.2.2/README.md` & `CosmoTech-SupplyChain-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adt_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adx_and_file_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/adx_wrapper.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/cosmo_api_parameters.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/csv_folder_reader.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/csv_folder_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/duration.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/excel_folder_reader.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/excel_folder_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/folder_io.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/json_folder_reader.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/json_folder_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/memory_folder_io.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/simulator_io.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/storage_queue_writer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Generic/timer.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/default_transformation.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/default_transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,22 @@
         - a list of entities
         - an index in the final array
         """
         index = None
         size = None
         entities = None
         end_index = None
+        schedule = None
 
-        def __init__(self, index, size, entities, end_index=0):
+        def __init__(self, index, size, entities, end_index=0, schedule=False):
             self.index = index
             self.size = size
             self.entities = entities
             self.end_index = end_index
+            self.schedule = schedule
 
         def transform(self, d):
             """
 
             :param d: the entrance datas
             :return: the transformed datas
             """
@@ -80,40 +82,43 @@
 
         def transform(self, data):
             return [(self.entities[0], data[self.index: self.index + self.size]), ]
 
     transformation_template = None
     start_cycle = None
     array_size = None
+    steps_per_cycle = None
 
     @staticmethod
     def rowToKey(row):
         """
         :param row: an entry of the decision_variable.csv
         :return: a tuple (datapath , <optional> subentity)
         """
         entity_name = row['Entity']
         attribute_name = row['Attribute']
         if attribute_name is None:
             return None
-        key = 'Model::{Entity}IndustrialNetwork::{Entity}' + entity_name + '::@' + attribute_name
+        entity_key = f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{entity_name}"
+        attribute_key = f"::@{attribute_name}"
         if row['Type'] == 'Machine':
             sub_entity_name = row['Operation']
-            return key, sub_entity_name
-        return key,
+            return f"{entity_key}::{{Entity}}{sub_entity_name}{attribute_key}",
+        return f"{entity_key}{attribute_key}",
 
-    def __init__(self, dv_df, machines, total_cycles):
+    def __init__(self, dv_df, machines, total_cycles, steps_per_cycle):
         """
         We initialize the transformation using the decision variables
         :param dv_df: A pandas DF using decision_variable.csv
         """
         self.transformation_template = list()
         index = 0
         self.start_cycle = 0
         self.array_size = total_cycles
+        self.steps_per_cycle = steps_per_cycle
 
         if not dv_df.empty:
             nb_group = max(list(dv_df['Group'])) + 1
             # Loop on the different groups
             for group in range(nb_group):
                 temp = dv_df[dv_df['Group'] == group]
                 temp.index = pd.RangeIndex(len(temp.index))
@@ -134,21 +139,28 @@
                 else:
                     self.transformation_template.append(self.NormalisationTransform(index=index,
                                                                                     size=cycles,
                                                                                     entities=entries,
                                                                                     end_index=final_index))
                     index += cycles * nb_entries
         for machine in machines:
-            machine_data_path = ("Model::{Entity}IndustrialNetwork::{Entity}" + machine + "::@OpeningRates",)
+            machine_data_path = ("Model::{Entity}IndustrialNetwork::{Entity}" + machine + "::@OpeningRateSchedule",)
             self.transformation_template.append(self.NoTransform(index=index,
                                                                  size=total_cycles,
                                                                  entities=[machine_data_path, ],
-                                                                 end_index=0))
+                                                                 end_index=0,
+                                                                 schedule=True))
             index += total_cycles
 
+    def list_to_schedule(self, values):
+        return {
+            str(i * self.steps_per_cycle): v
+            for i, v in enumerate(values)
+        }
+
     def applies(self, _data, _seed=0):
         """
         We apply the tranformation on the data
         :param _data: an array of data
         :param _seed: an int used as the seed for the simulation
         :return: a dict ready to be given to the simulation
         """
@@ -160,27 +172,29 @@
         for t in self.transformation_template:
             index = t.end_index
             padding = t.size
             for a, b in t.transform(data):
                 if a is None:
                     # Non used DVs have entity names set to None
                     continue
+                entity = a[0]
                 if len(a) == 1:
-                    if not len(ret_dict[a[0]]):
-                        ret_dict[a[0]] = [0] * self.array_size
-                    ret_dict[a[0]][index:index + padding] = b
+                    if not len(ret_dict[entity]):
+                        ret_dict[entity] = [0] * self.array_size
+                    ret_dict[entity][index:index + padding] = b
+                    if t.schedule:
+                        ret_dict[entity] = self.list_to_schedule(ret_dict[entity])
                 else:
-                    entity = a[0]
-                    _type = a[1]
+                    subentity = a[1]
                     # Array is empty
                     if not len(ret_dict[entity]):
                         for i in range(self.array_size):
-                            ret_dict[entity].append({_type: 0})
-                    # _type is not in the array
-                    if _type not in ret_dict[entity][0]:
+                            ret_dict[entity].append({subentity: 0})
+                    # subentity is not in the array
+                    if subentity not in ret_dict[entity][0]:
                         for i in range(self.array_size):
-                            ret_dict[entity][i][_type] = 0
+                            ret_dict[entity][i][subentity] = 0
                     # Set values from transformation to array
                     for i in range(len(b)):
-                        ret_dict[entity][index + i][_type] = b[i]
+                        ret_dict[entity][index + i][subentity] = b[i]
         # We apply a transformation to str on all the values
         return {k: str(ret_dict[k]).replace("'", "\"") for k in ret_dict}
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/multiprocessing_optimization.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/objective_functions.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Protocol/protocol.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/cmaes_optimization.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/cmaes_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         # Reduce log level to Error during optimization
         logger = CosmoEngine.LoggerManager.GetInstance().GetLogger()
         logger.SetLogLevel(logger.eAssertion)
 
         # Get data from the simulator
         df_decision_vars = simulator.decision_variables_df
         _end_cycle = simulator.GetModel().GetParameter('NumberOfCycle').GetAsInt()
+        _steps_per_cycle = simulator.GetModel().GetParameter('TimeStepPerCycle').GetAsInt()
 
         nb_pars = 0
 
         if simulator.FindAttribute("{Model}Model::{Attribute}ActivateVariableMachineOpeningRate").GetAsBool():
             machines = list(sorted(simulator.machine_list))
             nb_pars += len(machines) * simulator.FindAttribute("{Model}Model::{Attribute}NumberOfCycle").GetAsInt()
         else:
@@ -72,15 +73,16 @@
         algorithm = CMAESOptimization(parameter_count=nb_pars,
                                       **specs)
         t.split(time_prefix + "Prepare CMAES")
 
         # Initialization of the transformation which takes CMAES results and transform them on map: datapath -> value
         transformation = DefaultTransformation(df_decision_vars,
                                                machines,
-                                               _end_cycle)
+                                               _end_cycle,
+                                               _steps_per_cycle)
         t.split(time_prefix + "Prepare transformation")
 
         objective_function = DefaultObjectiveFunction()
 
         if optimization_objective == "ProfitMaximization":
             objective_function = ProfitMaximizationObjectiveFunction()
         t.split(time_prefix + "Prepare Objective Function")
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/consumers.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/consumers.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
     def Consume(self, p_data):
         probe_output = self.engine.StocksProbeOutput.Cast(p_data)
         f = probe_output.GetFacts()
         timestep = int(probe_output.GetProbeRunDimension().GetProbeOutputCounter())
         for data in f:
             fact = [
-                str(data.GetAttributeAsString("ID")),
+                str(data.GetAttributeAsString("id")),
                 timestep,
-                float(data.GetAttributeAsFloat64("Demand")),
-                float(data.GetAttributeAsFloat64("RemainingQuantity")),
-                float(data.GetAttributeAsFloat64("ServedQuantity")),
-                float(data.GetAttributeAsFloat64("UnservedQuantity")),
-                float(data.GetAttributeAsFloat64("ServiceLevel")),
-                float(data.GetAttributeAsFloat64("Value")),
+                float(data.GetAttributeAsDouble("Demand")),
+                float(data.GetAttributeAsDouble("RemainingQuantity")),
+                float(data.GetAttributeAsDouble("ServedQuantity")),
+                float(data.GetAttributeAsDouble("UnservedQuantity")),
+                float(data.GetAttributeAsDouble("ServiceLevel")),
+                float(data.GetAttributeAsDouble("Value")),
             ]
             self.memory.append(fact)
 
 
 class PerformanceConsumer:
     """
     Python Consumer for performance indicators at the end of the simulation.
@@ -33,49 +33,49 @@
         self.memory = list()
 
     def Consume(self, p_data):
         probe_output = self.engine.PerformanceIndicatorsProbeOutput.Cast(p_data)
         f = probe_output.GetFacts()
         for data in f:
             fact = {
-                "OPEX": float(data.GetAttributeAsFloat64("OPEX")),
-                "Profit": float(data.GetAttributeAsFloat64("Profit")),
+                "OPEX": float(data.GetAttributeAsDouble("OPEX")),
+                "Profit": float(data.GetAttributeAsDouble("Profit")),
                 "AverageStockValue": float(
-                    data.GetAttributeAsFloat64("AverageStockValue")
+                    data.GetAttributeAsDouble("AverageStockValue")
                 ),
                 "ServiceLevelIndicator": float(
-                    data.GetAttributeAsFloat64("ServiceLevelIndicator")
+                    data.GetAttributeAsDouble("ServiceLevelIndicator")
                 ),
-                "CO2Emissions": float(data.GetAttributeAsFloat64("CO2Emissions")),
-                "TotalDemand": float(data.GetAttributeAsFloat64("TotalDemand")),
+                "CO2Emissions": float(data.GetAttributeAsDouble("CO2Emissions")),
+                "TotalDemand": float(data.GetAttributeAsDouble("TotalDemand")),
                 "TotalServedQuantity": float(
-                    data.GetAttributeAsFloat64("TotalServedQuantity")
+                    data.GetAttributeAsDouble("TotalServedQuantity")
                 ),
                 "ServiceLevelSatisfaction": data.GetTotalServedQuantity().GetAsFloat()
                 / data.GetTotalDemand().GetAsFloat()
                 * 100
                 if data.GetTotalDemand().GetAsFloat() != 0
                 else 0,
             }
             self.memory.append(fact)
 
 
-class StocksFinalConsumer:
+class StocksAtEndOfSimulationConsumer:
     """
     Python Consumer for stocks global indicators at the end of the simulation.
     """
 
     def __init__(self):
         self.memory = list()
 
     def Consume(self, p_data):
-        probe_output = self.engine.StocksFinalProbeOutput.Cast(p_data)
+        probe_output = self.engine.StocksAtEndOfSimulationProbeOutput.Cast(p_data)
         f = probe_output.GetFacts()
         for data in f:
             fact = {
-                "ID": str(data.GetAttributeAsString("ID")),
-                "TotalDemand": float(data.GetAttributeAsFloat64("TotalDemand")),
-                "TotalServedQuantity": float(data.GetAttributeAsFloat64("TotalServedQuantity")),
-                "ServiceLevelSatisfaction": 100 * float(data.GetAttributeAsFloat64("ServiceLevelSatisfaction")),
-                "CycleServiceLevel": float(data.GetAttributeAsFloat64("CycleServiceLevel")),
+                "id": str(data.GetAttributeAsString("id")),
+                "TotalDemand": float(data.GetAttributeAsDouble("TotalDemand")),
+                "TotalServedQuantity": float(data.GetAttributeAsDouble("TotalServedQuantity")),
+                "ServiceLevelSatisfaction": 100 * float(data.GetAttributeAsDouble("ServiceLevelSatisfaction")),
+                "CycleServiceLevel": float(data.GetAttributeAsDouble("CycleServiceLevel")),
             }
             self.memory.append(fact)
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/local_sensitivity_analysis_comets.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,15 +806,15 @@
     df["TimeInterval"] = bool(timeinterval)
     df["InitialTimeStep"] = int(initialtimestep)
     df["FinalTimeStep"] = int(finaltimestep)
 
     df = df.rename(
         columns={
             "Output": "KPI",
-            "Name": "ID",
+            "Name": "id",
             "ReferenceOutputValue": "ReferenceKPI",
             "NewOutputValue": "NewKPI",
             "Difference": "Gap",
         }
     )
     # if type(df["ReferenceInputValue"][0]) == dict:
     #     for i in range(len(df.index)):
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/simulation.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/simulation_comets.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/stochastic_optimization.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/stochastic_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             self.decision_variable_min,
             self.decision_variable_max,
         )
 
         # Create uncertainty analyzer
         consumers = ["Performances"]
         if self.KPI == "IndividualServiceLevelSatisfaction":
-            consumers.append("StocksFinal")
+            consumers.append("StocksAtEndOfSimulation")
 
         self.ua = UncertaintyAnalyzer(
             simulation_name=self.simulation_name,
             simulation_path=self.simulation_path,
             amqp_consumer_adress=None,
             sample_size=self.sample_size_uncertainty_analysis,
             batch_size=self.batch_size_uncertainty_analysis,
@@ -423,19 +423,19 @@
         results["Performances"] = results["Performances"].set_index("KPI")
         kpi = results["Performances"].loc[KPI, stat]
         if optimization_mode == "target":
             objective = {"Objective": (kpi - target_value) ** 2, "KPI": kpi}
         else:
             objective = {"Objective": kpi, "KPI": kpi}
     else:
-        df_service = results["StocksFinal"][
-            results["StocksFinal"]["Indicator"] == "ServiceLevelSatisfaction"
+        df_service = results["StocksAtEndOfSimulation"][
+            results["StocksAtEndOfSimulation"]["Indicator"] == "ServiceLevelSatisfaction"
         ]
         if service_level_of_stocks != []:
-            df_service = df_service[df_service["StockId"].isin(service_level_of_stocks)]
+            df_service = df_service[df_service["id"].isin(service_level_of_stocks)]
         vector_of_service_levels = df_service[stat].to_numpy()
         if optimization_mode == "target":
             distance_to_target = (vector_of_service_levels - target_value) ** 2
             objective = {
                 "Objective": np.max(distance_to_target),  # np.sum(distance_to_target)
                 "KPI": list(vector_of_service_levels),
             }
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,20 @@
         memory = list()
 
         def Consume(self, p_data):
             probe_output = CosmoEngine.StocksProbeOutput.Cast(p_data)
             f = probe_output.GetFacts()
             timestep = int(probe_output.GetProbeRunDimension().GetProbeOutputCounter())
             for data in f:
-                fact = [str(data.GetAttributeAsString('ID')),
+                fact = [str(data.GetAttributeAsString('id')),
                         timestep,
-                        float(data.GetAttributeAsFloat64('Demand')),
-                        float(data.GetAttributeAsFloat64('RemainingQuantity')),
-                        float(data.GetAttributeAsFloat64('ServedQuantity')),
-                        float(data.GetAttributeAsFloat64('UnservedQuantity'))]
+                        float(data.GetAttributeAsDouble('Demand')),
+                        float(data.GetAttributeAsDouble('RemainingQuantity')),
+                        float(data.GetAttributeAsDouble('ServedQuantity')),
+                        float(data.GetAttributeAsDouble('UnservedQuantity'))]
                 self.memory.append(fact)
 
     consumer = StockConsumer("LocalConsumer")
     consumer.Connect(simulator.GetProbe("Stocks"))
 
     # Run simulation
     simulator.Run()
@@ -94,76 +94,84 @@
             for i in range(0, len(seedlist), batch_size):
                 subseedlist = seedlist[i:i + batch_size]
                 params = list(map(lambda seed: (simulation_name, seed, amqp_consumer_adress, probe_data), subseedlist))
                 p.starmap(run_simulation_with_seed, params)
         t.split("Ended simulations : {time_since_start}")
 
         df = pd.DataFrame((record for record in probe_data))
-        df.columns = ['StockId', 'TimeStep', 'Demand', 'RemainingQuantity', 'ServedQuantity', 'UnservedQuantity']
+        df.columns = ['id', 'TimeStep', 'Demand', 'RemainingQuantity', 'ServedQuantity', 'UnservedQuantity']
         t.split("Create dataframes for stats computation: {time_since_last_split}")
 
-        quantile_list = [0.05, 0.25, 0.5, 0.75, 0.95]
-        groups = df.groupby(['StockId', 'TimeStep'])
+        quantiles = (
+            (0.05, 'FirstVigintile'),
+            (0.25, 'FirstQuartile'),
+            (0.50, 'Median'),
+            (0.75, 'LastQuartile'),
+            (0.95, 'LastVigintile'),
+        )
+        quantile_list, quantile_name_list = [list(t) for t in zip(*quantiles)]
+        groups = df.groupby(['id', 'TimeStep'])
         df_quantiles = groups.quantile(quantile_list)
         df_average = groups.mean()
         df_error = groups.agg(lambda x: x.std() / sqrt(x.count()))
         t.split("Compute stats : {time_since_last_split}")
 
         # since use of pivot to have 1 column per tuple (quantile, valuetype)
         # then use of stack to have 1 line per (stock, timestep, valuetype)
-        df3 = df_quantiles.reset_index().pivot(index=['StockId',
+        df3 = df_quantiles.reset_index().pivot(index=['id',
                                                       'TimeStep'],
                                                columns='level_2',
                                                values=['Demand',
                                                        'RemainingQuantity',
                                                        'ServedQuantity',
                                                        'UnservedQuantity']).stack(level=0)
         df3.reset_index(inplace=True)
-        df3.columns = ['StockId',
+        df3.columns = ['id',
                        'TimeStep',
-                       'Category'] + [f'Percentile{int(v * 100)}'
-                                      for v in quantile_list]
+                       'Category'] + quantile_name_list
 
         # use of stack to have 1 line per (stock, timestep, valuetype)
         df4 = df_average.stack(level=0)
         df4 = df4.reset_index()
-        df4.columns = ['StockId',
+        df4.columns = ['id',
                        'TimeStep',
                        'Category',
                        'Mean']
 
         # use of stack to have 1 line per (stock, timestep, valuetype)
         df5 = df_error.stack(level=0)
         df5 = df5.reset_index()
-        df5.columns = ['StockId',
+        df5.columns = ['id',
                        'TimeStep',
                        'Category',
                        'SE']
 
         # Merge of dfs to final df
-        final_df = pd.merge(df3, df4, on=['StockId',
+        final_df = pd.merge(df3, df4, on=['id',
                                           'TimeStep',
                                           'Category'])
-        final_df = pd.merge(final_df, df5, on=['StockId',
+        final_df = pd.merge(final_df, df5, on=['id',
                                                'TimeStep',
                                                'Category'])
 
         final_df['SimulationRun'] = EnvironmentVariables.simulation_id
-        final_df = final_df[['TimeStep',
-                             'SimulationRun',
-                             'StockId',
-                             'Percentile5',
-                             'Percentile25',
-                             'Percentile50',
-                             'Percentile75',
-                             'Percentile95',
-                             'Mean',
-                             'SE',
-                             'Category']]
-        adx_writer.write_target_file(final_df.to_dict('records'), 'StockUncertaintiesStatistics', EnvironmentVariables.simulation_id)
+        final_df = final_df[
+            [
+                'TimeStep',
+                'SimulationRun',
+                'id',
+            ]
+            + quantile_name_list
+            + [
+                'Mean',
+                'SE',
+                'Category',
+            ]
+        ]
+        adx_writer.write_target_file(final_df.to_dict('records'), 'StockUncertaintyStatistics', EnvironmentVariables.simulation_id)
 
         t.split("Sent stats to ADX : {time_since_last_split}")
         t.display_message("Running simple simulation to fill ADX")
         # Put back log level to Info for final simulation
         # Reduce log level to Error during optimization
         logger = CosmoEngine.LoggerManager.GetInstance().GetLogger()
         logger.SetLogLevel(logger.eInfo)
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis_comets.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 from Supplychain.Wrappers.simulator import CosmoEngine
 from Supplychain.Generic.adx_and_file_writer import ADXAndFileWriter
 from Supplychain.Generic.timer import Timer
 from Supplychain.Run.simulation import run_simple_simulation
 from Supplychain.Run.consumers import (
     StockConsumer,
     PerformanceConsumer,
-    StocksFinalConsumer,
+    StocksAtEndOfSimulationConsumer,
 )
 from Supplychain.Run.uncertainty_analysis_helper_functions import (
     get_max_time_step,
     get_attribute,
     get_stocks,
     get_transports,
     collect_transport_information,
     extend_dic,
     add_tag_to_parameterset,
     collect_simulated_stock_final_output,
     collect_simulated_stock_output,
     collect_simulated_transport_output,
-    transform_transport_data,
-    transform_stock_data,
-    transform_stocksfinal_data,
+    transform_data,
     create_transport_distribution_sampling,
     create_demand_generator,
 )
 
 
 class UncertaintyAnalyzer:
     """
@@ -40,28 +38,28 @@
 
     Args:
         simulation_name (str): Name of simulation, used by the probes
         simulation_path (str): Name of the simulation file (typically Simulation)
         sample_size (int): Number of simulations runs by the uncertainty analysis
         batch_size (int): Number of simulations runs that are run in a same batch by the uncertainty analysis
         amqp_consumer_adress (Union[str, None], optional): Adress of consumer to send probe results to. Defaults to None.
-        consumers (list, optional): Which consumers are activated. Defaults to ["Stocks", "Transport", "Performances", "StocksFinal", "PerformanceAMQP"].
+        consumers (list, optional): Which consumers are activated. Defaults to ["Stocks", "Transport", "Performances", "StocksAtEndOfSimulation", "PerformanceAMQP"].
         validation_folder (str, optional): Local folder to which results are written to, used by the tests. Defaults to None.
         cold_inputs (dict, optional): Parameters that are passed to the simulator at each simulation and don't change during the analysis. Defaults to {}.
         timer (Timer object, optional): Timer object that can be used for logs and counting time. Defaults to None.
     """
 
     def __init__(
         self,
         simulation_name,
         simulation_path,
         sample_size,
         batch_size,
         amqp_consumer_adress=None,
-        consumers=["Stocks", "Transport", "Performances", "StocksFinal"],
+        consumers=["Stocks", "Transport", "Performances", "StocksAtEndOfSimulation"],
         validation_folder=None,
         cold_inputs={},
         timer=None,
         n_jobs=-1,
     ):
         if timer is None:
             self.t = Timer("[Run Uncertainty]")
@@ -84,15 +82,15 @@
         else:
             self.processes_size = n_jobs
 
     def execute(self):
         """Setup and run the uncertainty analysis
 
         Returns:
-            dict: dictionary with keys among ["Stock", "Transport", "Performances", "StocksFinal"]
+            dict: dictionary with keys among ["Stock", "Transport", "Performances", "StocksAtEndOfSimulation"]
                 containing the output tables. Which table is available depends on the specified
                 consumers of the UncertaintyAnalyzer.
         """
         self.t.split("Initialize uncertainty analysis")
         self.initialize_simulator_interface()
         self.collect_simulation_parameters()
         self.create_encoder()
@@ -121,18 +119,18 @@
         used_probes = []
         used_consumers = []
         custom_consumers = []
 
         if "Stocks" in self.consumers:
             used_probes.append("Stocks")
             custom_consumers.append((StockConsumer, "LocalConsumer", "Stocks"))
-        if "StocksFinal" in self.consumers:
-            used_probes.append("StocksFinal")
+        if "StocksAtEndOfSimulation" in self.consumers:
+            used_probes.append("StocksAtEndOfSimulation")
             custom_consumers.append(
-                (StocksFinalConsumer, "StocksFinalConsumer", "StocksFinal")
+                (StocksAtEndOfSimulationConsumer, "StocksAtEndOfSimulationConsumer", "StocksAtEndOfSimulation")
             )
         if "Performances" in self.consumers:
             used_probes.append("PerformanceIndicators")
             custom_consumers.append(
                 (
                     PerformanceConsumer,
                     "LocalPerformanceConsumer",
@@ -334,20 +332,20 @@
                 )
             if "Performances" in consumers:
                 output_parameterset.update(
                     add_tag_to_parameterset(
                         "3_", modelinterface.LocalPerformanceConsumer.memory[0]
                     )
                 )
-            if "StocksFinal" in consumers:
+            if "StocksAtEndOfSimulation" in consumers:
                 output_parameterset.update(
                     add_tag_to_parameterset(
                         "4_",
                         collect_simulated_stock_final_output(
-                            modelinterface.StocksFinalConsumer.memory
+                            modelinterface.StocksAtEndOfSimulationConsumer.memory
                         ),
                     )
                 )
             return output_parameterset
 
         self.get_outcomes = get_outcomes
 
@@ -421,15 +419,15 @@
         )
 
         self.experiment.run()
 
     def reformat_results(self):
         """Reformat results of the experiment so that they are compatible with the output tables"""
         self.results = {}
-        # Separating the results data on the different types of outputs (stock, transport, performances, stocksfinal)
+        # Separating the results data on the different types of outputs (stock, transport, performances, stocksatendofsimulation)
         self.experiment.results["statistics"].reset_index(inplace=True)
         self.experiment.results["statistics"]["OutputType"] = (
             self.experiment.results["statistics"]["index"]
             .str.split(pat="_", expand=False, n=1)
             .str[0]
         )
         self.experiment.results["statistics"]["index"] = (
@@ -438,37 +436,37 @@
             .str[1]
         )
         if "Transports" in self.consumers:
             df_transport_duration = self.experiment.results["statistics"][
                 self.experiment.results["statistics"]["OutputType"] == "1"
             ]
             df_transport_duration = df_transport_duration.drop("OutputType", axis=1)
-            df_transport_final = transform_transport_data(df_transport_duration)
+            df_transport_final = transform_data(df_transport_duration)
             self.results["Transport"] = df_transport_final
         if "Stocks" in self.consumers:
             df_probe_data = self.experiment.results["statistics"][
                 self.experiment.results["statistics"]["OutputType"] == "2"
             ]
             df_probe_data = df_probe_data.drop("OutputType", axis=1)
-            df_stock_final = transform_stock_data(df_probe_data)
+            df_stock_final = transform_data(df_probe_data)
             self.results["Stock"] = df_stock_final
         if "Performances" in self.consumers:
             performances = self.experiment.results["statistics"][
                 self.experiment.results["statistics"]["OutputType"] == "3"
             ]
             performances = performances.drop("OutputType", axis=1)
             performances = performances.rename(columns={"index": "KPI"})
             self.results["Performances"] = performances
-        if "StocksFinal" in self.consumers:
-            df_stocksfinalconsumer = self.experiment.results["statistics"][
+        if "StocksAtEndOfSimulation" in self.consumers:
+            df_stocksatendofsimulationconsumer = self.experiment.results["statistics"][
                 self.experiment.results["statistics"]["OutputType"] == "4"
             ]
-            df_stocksfinalconsumer = df_stocksfinalconsumer.drop("OutputType", axis=1)
-            df_stocksfinalconsumer = transform_stocksfinal_data(df_stocksfinalconsumer)
-            self.results["StocksFinal"] = df_stocksfinalconsumer
+            df_stocksatendofsimulationconsumer = df_stocksatendofsimulationconsumer.drop("OutputType", axis=1)
+            df_stocksatendofsimulationconsumer = transform_data(df_stocksatendofsimulationconsumer, timestep=False)
+            self.results["StocksAtEndOfSimulation"] = df_stocksatendofsimulationconsumer
 
     def write_results_locally(self):
         """Write the results tables locally to csv files"""
 
         # Get all demands directly from the experiment, before aggregation of statistics
         demands = []
         j = 0
@@ -489,16 +487,16 @@
         demand_df = pandas.DataFrame(demands)
         demand_df.to_csv(
             str(self.validation_folder) + "/df_all_demands.csv", index=False
         )
         self.results["Stock"].to_csv(
             str(self.validation_folder) + "/final_df_comets.csv", index=False
         )
-        self.results["StocksFinal"].to_csv(
-            str(self.validation_folder) + "/df_stocksfinal.csv", index=False
+        self.results["StocksAtEndOfSimulation"].to_csv(
+            str(self.validation_folder) + "/df_stocksatendofsimulation.csv", index=False
         )
         self.results["Transport"].to_csv(
             str(self.validation_folder) + "/df_transport.csv", index=False
         )
         self.results["Performances"].to_csv(
             str(self.validation_folder) + "/df_performances.csv", index=False
         )
@@ -522,28 +520,28 @@
             simulation_name=simulation_name,
             simulation_path=simulation_path,
             amqp_consumer_adress=amqp_consumer_adress,
             sample_size=sample_size,
             batch_size=batch_size,
             n_jobs=n_jobs,
             validation_folder=validation_folder,
-            consumers=["Transports", "Stocks", "StocksFinal", "Performances", "PerformanceAMQP"],
+            consumers=["Transports", "Stocks", "StocksAtEndOfSimulation", "Performances", "PerformanceAMQP"],
             cold_inputs=cold_inputs,
             timer=t,
         )
 
         results = ua.execute()
 
         if adx_writer is not None:
             t.split("Sending stats to ADX")
             adx_writer.write_target_file(
-                results["Stock"].to_dict("records"), "StockUncertaintiesStatistics"
+                results["Stock"].to_dict("records"), "StockUncertaintyStatistics"
             )
             adx_writer.write_target_file(
-                results["StocksFinal"].to_dict("records"), "StocksFinalUncertaintyStatistics"
+                results["StocksAtEndOfSimulation"].to_dict("records"), "StocksAtEndOfSimulationUncertaintyStatistics"
             )
             adx_writer.write_target_file(
                 results["Transport"].to_dict("records"),
                 "TransportUncertaintyStatistics",
             )
 
             t.split("Sent stats to ADX : {time_since_last_split}")
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Run/uncertainty_analysis_helper_functions.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Run/uncertainty_analysis_helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             actual_duration_schedule,
             max_time_step,
         )
         time_step = 0
         for value in transport_duration[
             f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
         ].values():
-            transport_duration_transformed[f"{transport}__&@&__{time_step}"] = value
+            transport_duration_transformed[f"{transport}__&@&__ActualDuration__&@&__{time_step}"] = value
             time_step += 1
     return transport_duration_transformed
 
 
 def collect_simulated_stock_output(consumer_memory):
     """
     This function transforms the consumer memory from a list of list to a list of
@@ -362,15 +362,15 @@
 def collect_simulated_stock_final_output(consumer):
     """
     This function transforms the consumer memory to a dictionary of
     ParameterSets, where one ParameterSet is used for each stock-category.
     """
     categories = ("TotalDemand", "TotalServedQuantity", "ServiceLevelSatisfaction", "CycleServiceLevel")
     return {
-        f"{elements['ID']}__&@&__{category}": elements[category]
+        f"{elements['id']}__&@&__{category}": elements[category]
         for elements in consumer
         for category in categories
     }
 
 
 """
 -------------------------------------------------
@@ -468,141 +468,59 @@
             }
         )
     return sampling
 
 
 """
 -------------------------------------------------
-Functions that reformat the outputs of the uncertainty analysis
+Function that reformat the outputs of the uncertainty analysis
 -------------------------------------------------
 """
 
 
-def transform_stocksfinal_data(data):
+def transform_data(data, timestep=True):
     """
-    Transform output data by splitting the index column into a column of stock name, and a column with indicator name
+    Transform output data so that it matches the ADX table format
     """
-    restructured_df = data.copy()
-    restructured_df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
-    restructured_df[["StockId", "Category"]] = restructured_df["index"].str.split(
-        pat="__&@&__", expand=True
-    )
-    restructured_df = restructured_df[[
+    df = data.copy()
+    index_cols = [
+        "id",
+        "Category",
+        "TimeStep"
+    ]
+    if not timestep:
+        index_cols.remove("TimeStep")
+    if not df.empty:
+        df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
+        df[index_cols] = df["index"].str.split(pat="__&@&__", expand=True)
+    else:
+        index_cols.insert(0, "SimulationRun")
+        df[index_cols] = None
+    cols = [
         "SimulationRun",
-        "StockId",
+        "TimeStep",
+        "id",
         "Category",
-        "mean",
-        "sem",
         "quantile 5%",
         "quantile 25%",
         "quantile 50%",
         "quantile 75%",
         "quantile 95%",
-    ]]
-    restructured_df.rename(
-        columns={
-            "mean": "Mean",
-            "sem": "SE",
-            "quantile 5%": "Percentile5",
-            "quantile 25%": "Percentile25",
-            "quantile 50%": "Median",
-            "quantile 75%": "Percentile75",
-            "quantile 95%": "Percentile95",
-        },
-        inplace=True,
-    )
-    return restructured_df
-
-
-def transform_stock_data(data):
-    """
-    Transform output data so that it matches the ADX table format
-    """
-    # Splitting the first columns into 3 columns: TimeStep, StockId, Category
-    # And adding the simulationRun
-    temporary_df = data.copy()
-    temporary_df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
-    temporary_df[["StockId", "Category", "TimeStep"]] = temporary_df["index"].str.split(
-        pat="__&@&__", expand=True
-    )
-
-    # Removing unused columns such as index, quantile 10 ...
-    temporary_df = temporary_df.iloc[:, [1, 3, 5, 9, 14, 19, 23, 24, 25, 26, 27]]
-
-    # Changing the columns' order and renaming them to match the adx table
-    df_final = temporary_df[
-        [
-            "TimeStep",
-            "SimulationRun",
-            "StockId",
-            "quantile 5%",
-            "quantile 25%",
-            "quantile 50%",
-            "quantile 75%",
-            "quantile 95%",
-            "mean",
-            "sem",
-            "Category",
-        ]
+        "mean",
+        "sem",
     ]
-
-    df_final.rename(
+    if not timestep:
+        cols.remove("TimeStep")
+    df = df[cols]
+    df.rename(
         columns={
-            "quantile 5%": "Percentile5",
-            "quantile 25%": "Percentile25",
-            "quantile 50%": "Percentile50",
-            "quantile 75%": "Percentile75",
-            "quantile 95%": "Percentile95",
+            "quantile 5%": "FirstVigintile",
+            "quantile 25%": "FirstQuartile",
+            "quantile 50%": "Median",
+            "quantile 75%": "LastQuartile",
+            "quantile 95%": "LastVigintile",
             "mean": "Mean",
             "sem": "SE",
         },
         inplace=True,
     )
-    return df_final
-
-
-def transform_transport_data(data):
-    """
-    Transform output data so that it matches the ADX table format
-    """
-    # Adding the simulation run to the df
-    temporary_df = data.copy()
-    if not temporary_df.empty:
-        temporary_df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
-        # Splitting the first column into 2 columns: TransportOperation, TimeStep
-        temporary_df["TransportOperation"] = (
-            temporary_df["index"].str.split(pat="__&@&__", expand=False, n=1).str[0]
-        )
-        temporary_df["TimeStep"] = (
-            temporary_df["index"].str.split(pat="__&@&__", expand=False, n=1).str[1]
-        )
-    else:
-        temporary_df[["TransportOperation", "TimeStep"]] = None
-    df_final = temporary_df.iloc[:, 1:]
-
-    df_final.rename(
-        columns={
-            "confidence interval of the mean at 95%": "ConfidenceIntervalOfTheMeanAt95",
-            "quantile 5%": "Percentile5",
-            "quantile 10%": "Percentile10",
-            "quantile 15%": "Percentile15",
-            "quantile 20%": "Percentile20",
-            "quantile 25%": "Percentile25",
-            "quantile 30%": "Percentile30",
-            "quantile 35%": "Percentile35",
-            "quantile 40%": "Percentile40",
-            "quantile 45%": "Percentile45",
-            "quantile 50%": "Percentile50",
-            "quantile 55%": "Percentile55",
-            "quantile 60%": "Percentile60",
-            "quantile 65%": "Percentile65",
-            "quantile 70%": "Percentile70",
-            "quantile 75%": "Percentile75",
-            "quantile 80%": "Percentile80",
-            "quantile 85%": "Percentile85",
-            "quantile 90%": "Percentile90",
-            "quantile 95%": "Percentile95",
-        },
-        inplace=True,
-    )
-
-    return df_final
+    return df
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/adt_column_description.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/adt_column_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                 "DispatchPolicy",
                 "ReviewPeriod",
                 "FirstReview",
                 "Advance",
                 "Latitude",
                 "Longitude",
                 "IgnoreDownstreamRequiredQuantities",
+                "SourcingLimit",
             ],
             "change": [
                 "StorageUnitCosts",
                 "OrderPoints",
                 "OrderQuantities",
                 "OrderUpToLevels",
                 "SafetyQuantities",
@@ -51,14 +52,19 @@
                     "DemandUncertainties",
                     "DemandWeights",
                 ],
                 "SalesForecasts": [
                     "SalesForecasts",
                 ],
             },
+            "quantity": {
+                "PurchasingCosts": [
+                    "VariablePurchasingUnitCosts"
+                ],
+            },
         },
         "Transport": {
             "fixed": [
                 "Label",  # TODO to be replaced by RelationshipId when available from azure-digital-twins-simulator-connector
                 "source",
                 "target",
                 "Duration",
@@ -80,14 +86,15 @@
             ],
             "event": {
                 "InitialTransports": [
                     "InitialTransportedQuantities",
                     "InitialTransportedValues",
                 ]
             },
+            "quantity": {},
         },
         "Configuration": {
             "fixed": [
                 "ActivateUncertainties",
                 "ActivateVariableMachineOpeningRate",
                 "BatchSize",
                 "EmptyObsoleteStocks",
@@ -120,55 +127,61 @@
                 "FinalSampleSizeUncertaintyAnalysis",
                 "MaxIterationsForOptim",
                 "AutomaticParallelizationConfig",
                 "MaxNumberOfSimInParallel",
             ],
             "change": [],
             "event": {},
+            "quantity": {},
         },
         "contains": {
             "fixed": [
                 "source",
                 "target",
             ],
             "change": [],
             "event": {},
+            "quantity": {},
         },
         "output": {
             "fixed": [
                 "source",
                 "target",
             ],
             "change": [],
             "event": {},
+            "quantity": {},
         },
         "input": {
             "fixed": [
                 "source",
                 "target",
                 "InputQuantity",
             ],
             "change": [],
             "event": {},
+            "quantity": {},
         },
         "ProductionResource": {
             "fixed": [
                 "id",
                 "Label",
                 "PlantName",
                 "ProductionStep",
                 "ProductionPolicy",
                 "Latitude",
                 "Longitude",
             ],
             "change": [
                 "FixedProductionCosts",
                 "OpeningTimes",
+                "OpeningRates",
             ],
             "event": {},
+            "quantity": {},
         },
         "ProductionOperation": {
             "fixed": [
                 "id",
                 "Label",
                 "PlantName",
                 "IsContractor",
@@ -183,11 +196,13 @@
                 "RejectRates",
                 "OperatingPerformanceUncertainties",
                 "ProductionUnitCosts",
                 "CO2UnitEmissions",
                 "MinimumOrderQuantities",
                 "MultipleOrderQuantities",
                 "SourcingProportions",
+                "ProductionProportions",
             ],
             "event": {},
+            "quantity": {},
         },
     }
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/default_values.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/default_values.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,29 @@
         "PartId": "",
         "MinimalStock": -1,
         "MaximalStock": None,
         # "InitialStock",
         # "InitialValue",
         # "IsInfinite",
         "PurchasingUnitCosts": {},
+        "VariablePurchasingUnitCosts": {},
         "CO2UnitEmissions": {},
         "UnitIncomes": {},
         "BacklogWeight": 1,
         "MaximizationWeight": 0,
         "StockPolicy": "None",
         "SourcingPolicy": "Equidistribution",
         "DispatchPolicy": "Equidistribution",
         "ReviewPeriod": 1,
         "FirstReview": 0,
         "Advance": 0,
         "Latitude": 0.0,
         "Longitude": 0.0,
         "IgnoreDownstreamRequiredQuantities": False,
+        "SourcingLimit": "Capacity",
         "StorageUnitCosts": {},
         "OrderPoints": {},
         "OrderQuantities": {},
         "OrderUpToLevels": {},
         "SafetyQuantities": {},
         "Demands": {},
         "DemandUncertainties": {},
@@ -110,14 +112,15 @@
         "PlantName": "",
         "ProductionStep": "",
         "ProductionPolicy": "Equidistribution",
         "Latitude": 0.0,
         "Longitude": 0.0,
         "FixedProductionCosts": {},
         # "OpeningTimes",
+        "OpeningRates": {},
     },
     "ProductionOperation": {
         # "id",
         # "Label",
         "PlantName": "",
         "IsContractor": False,
         "InvestmentCost": 0,
@@ -129,28 +132,30 @@
         "RejectRates": {},
         "OperatingPerformanceUncertainties": {},
         "ProductionUnitCosts": {},
         "CO2UnitEmissions": {},
         "MinimumOrderQuantities": {},
         "MultipleOrderQuantities": {},
         # "SourcingProportions",
+        # "ProductionProportions",
     },
 }
 variables_default_values = {
     "Stock": {
         "StorageUnitCosts": 0,
         "OrderPoints": 0,
         "OrderQuantities": 0,
         "OrderUpToLevels": 0,
         "SafetyQuantities": 0,
         "Demands": 0,
         "DemandUncertainties": 0,
         "DemandWeights": 1,
         "SalesForecasts": 0,
         "PurchasingUnitCosts": 0,
+        "VariablePurchasingUnitCosts": 0,
         "CO2UnitEmissions": 0,
         "UnitIncomes": 0,
     },
     "Transport": {
         "CustomFees": 0,
         "TransportUnitCosts": 0,
         "CO2UnitEmissions": 0,
@@ -168,21 +173,23 @@
     "Configuration": {},
     "contains": {},
     "output": {},
     "input": {},
     "ProductionResource": {
         "FixedProductionCosts": 0,
         "OpeningTimes": 1440,
+        "OpeningRates": 1,
     },
     "ProductionOperation": {
         "QuantitiesToProduce": 0,
         "OperatingPerformances": 1,
         "CycleTimes": 1,
         "RejectRates": 0,
         "OperatingPerformanceUncertainties": 0,
         "ProductionUnitCosts": 0,
         "CO2UnitEmissions": 0,
         "MinimumOrderQuantities": 0,
         "MultipleOrderQuantities": 0,
         "SourcingProportions": 0,
+        "ProductionProportions": 0,
     },
 }
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/simulator_files_description.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/simulator_files_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "BE_Stock": [
         "Name",
         "CurrentStock",
         "MinimalStock",
         "MaximalStock",
         "Value",
         "PurchasingUnitCostSchedule",
+        "VariablePurchasingUnitCostSchedule",
         "CO2UnitEmissionsSchedule",
         "UnitIncomeSchedule",
         "Demand",
         "StorageUnitCostSchedule",
         "IsInfinite",
         "StockPolicy",
         "SourcingPolicy",
@@ -41,23 +42,24 @@
         "LeadTime",
         "SalesForecasts",
         "OrderPointSchedule",
         "OrderQuantitySchedule",
         "SafetyQuantitySchedule",
         "SchedulingStep",
         "IgnoreDownstreamRequiredQuantities",
+        "SourcingLimit",
     ],
     "CE_Machine": [
         "Name",
-        "StockTypeProportion",
         "Groups",
-        "OpeningRates",
+        "OpeningRateSchedule",
         "OpeningTimeSchedule",
         "ProductionCostSchedule",
         "ProductionPolicy",
+        "FutureRange",
     ],
     "BE_Operation": [
         "Name",
         "ParentName",
         "OperatingPerformanceSchedule",
         "CycleTimeSchedule",
         "RejectRateSchedule",
@@ -71,14 +73,15 @@
         "SchedulingStep",
         "FollowsStockPolicy",
         "Duration",
         "LeadTime",
         "MinimumOrderQuantitySchedule",
         "MultipleOrderQuantitySchedule",
         "SourcingProportionSchedule",
+        "ProductionProportionSchedule",
     ],
     "BE_TransportOperation": [
         "Name",
         "Duration",
         "Shipments",
         "TransportUnitCostSchedule",
         "CustomsUnitCostSchedule",
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Schema/validation_schemas.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Schema/validation_schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,20 @@
                     "type": "object",
                     "patternProperties": {
                         "^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}
                     },
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
+                "ProductionProportions": {
+                    "type": "object",
+                    "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}},
+                    "if": {"minProperties": 1},
+                    "then": {"required": ["0"]},
+                },
                 "IsContractor": {"type": "boolean"},
                 "InvestmentCost": {
                     "type": "number",
                     "minimum": 0,
                 },
                 "Priority": {"type": "integer", "minimum": 0},
                 "Duration": {"type": "integer", "minimum": 0},
@@ -252,27 +258,33 @@
         "ProductionResource": {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "type": "object",
             "properties": {
                 "ProductionPolicy": {
                     "type": "string",
                     "enum": [
-                        "None",
                         "Equidistribution",
                         "GreatestWorkload",
                         "SmallestWorkload",
                         "HighestPriority",
+                        "ProductionProportions",
                     ],
                 },
                 "OpeningTimes": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
+                "OpeningRates": {
+                    "type": "object",
+                    "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}},
+                    "if": {"minProperties": 1},
+                    "then": {"required": ["0"]},
+                },
                 "FixedProductionCosts": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "Latitude": {"type": "number", "minimum": -90, "maximum": 90},
@@ -307,14 +319,22 @@
                 "InitialValue": {"type": "number", "minimum": 0},
                 "PurchasingUnitCosts": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
+                "VariablePurchasingUnitCosts": {
+                    "type": "object",
+                    "patternProperties": {
+                        "^[0-9]+$": {"type": "object", "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}}}
+                    },
+                    "if": {"minProperties": 1},
+                    "then": {"required": ["0"]},
+                },
                 "CO2UnitEmissions": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "UnitIncomes": {
@@ -398,14 +418,21 @@
                 "SalesForecasts": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                 },
                 "Latitude": {"type": "number", "minimum": -90, "maximum": 90},
                 "Longitude": {"type": "number", "minimum": -180, "maximum": 180},
                 "IgnoreDownstreamRequiredQuantities": {"type": "boolean"},
+                "SourcingLimit": {
+                    "type": "string",
+                    "enum": [
+                        "Capacity",
+                        "CapacityQuantity",
+                    ],
+                },
             },
             "dependencies": {"InitialValue": ["InitialStock"]},
         },
         "Transport": {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "type": "object",
             "properties": {
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/complete_dict.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/complete_dict.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,14 +82,36 @@
                         sourcing_proportions[source] = {}
 
         for operation in self.reader.files.get('ProductionOperation', []):
             operation['SourcingProportions'] = sourcing_proportions[operation['id']]
         for transport in self.reader.files.get("Transport", []):
             transport['SourcingProportions'] = sourcing_proportions[transport['Label']]
 
+    def __complete_production_proportions(self):
+        operations_by_resource = {}
+        production_proportions = {}
+
+        for contains in self.reader.files.get('contains', []):
+            operations_by_resource.setdefault(contains['source'], []).append(contains['target'])
+        for operation in self.reader.files.get('ProductionOperation', []):
+            production_proportions[operation['id']] = operation.get('ProductionProportions')
+
+        for operations in operations_by_resource.values():
+            if all(production_proportions[operation] is None for operation in operations):
+                p = 1.0 / len(operations)
+                for operation in operations:
+                    production_proportions[operation] = {'0': p}
+            else:
+                for operation in operations:
+                    if production_proportions[operation] is None:
+                        production_proportions[operation] = {}
+
+        for operation in self.reader.files.get('ProductionOperation', []):
+            operation['ProductionProportions'] = production_proportions[operation['id']]
+
     def __complete_data_specific(self):
         for configuration in self.reader.files.get('Configuration', []):
             if configuration.get('StartingDate') is None:
                 configuration['StartingDate'] = date.today().isoformat()
 
         may_be_infinite = (
             set(s['id'] for s in self.reader.files.get('Stock', []))
@@ -119,14 +141,15 @@
                     demands_uncertainties[time_step] = variables_default_values['Stock']['DemandUncertainties']
 
         for resource in self.reader.files.get('ProductionResource', []):
             if resource.get('OpeningTimes') is None:
                 resource['OpeningTimes'] = {'0': self.reader.files['Configuration'][0]['TimeStepDuration']}
 
         self.__complete_sourcing_proportions()
+        self.__complete_production_proportions()
 
     def __write_updated_files(self):
         for file_name, dict_list in self.reader.files.items():
             self.writer.write_from_list(dict_list, file_name)
 
     def complete(self):
         self.display_message("Starting completion")
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_dict_to_simulator.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from Supplychain.Generic.folder_io import FolderReader, FolderWriter
 from Supplychain.Generic.timer import Timer
 from Supplychain.Schema.simulator_files_description import simulator_format
-from Supplychain.Schema.default_values import variables_default_values
+from Supplychain.Schema.default_values import parameters_default_values, variables_default_values
 from Supplychain.Generic.duration import seconds_to_iso_8061_duration
 from datetime import datetime, tzinfo, timedelta
 from Supplychain.Wrappers.environment_variables import SECONDS_IN_MINUTE
 
 from collections import defaultdict, deque
 
 
@@ -22,14 +22,28 @@
         return dict()
     return {
         key_type(k): value_type(v)
         for k, v in sorted(dict_item.items(), key=lambda i: key_type(i[0]))
     }
 
 
+def convert_nested_dict(key_type, subkey_type, value_type, dict_item) -> dict:
+    if dict_item is None:
+        return dict()
+    return {
+        key_type(key): {
+            subkey_type(subkey): value_type(value)
+            for subkey, value
+            in sorted(subdict_item.items(), key=lambda i: subkey_type(i[0]))
+        }
+        for key, subdict_item
+        in sorted(dict_item.items(), key=lambda i: key_type(i[0]))
+    }
+
+
 def find_effective_value_for_time_step(time_step: int, schedule: dict) -> float:
     if time_step in schedule:
         return schedule[time_step]
 
     effective_time_step = max(int(k) for k in schedule.keys() if int(k) <= time_step)
     return schedule.get(str(effective_time_step), 0.0)
 
@@ -434,14 +448,17 @@
                 ),
                 "MultipleOrderQuantitySchedule": convert_dict(
                     int, float, operation["MultipleOrderQuantities"]
                 ),
                 "SourcingProportionSchedule": convert_dict(
                     int, float, operation["SourcingProportions"]
                 ),
+                "ProductionProportionSchedule": convert_dict(
+                    int, float, operation["ProductionProportions"]
+                ),
                 "InvestmentCost": operation["InvestmentCost"],
                 "IsContractor": operation["IsContractor"],
                 "Priority": operation["Priority"],
                 "SchedulingStep": self.entity_order.get(operation["id"], -1),
                 "FollowsStockPolicy": follows_stock_policy,
                 "Duration": operation["Duration"],
                 "LeadTime": self.lead_times[operation["id"]],
@@ -507,14 +524,17 @@
                 "CurrentStock": stock["InitialStock"],
                 "MinimalStock": stock["MinimalStock"],
                 "MaximalStock": maximal_stock if maximal_stock is not None else -1,
                 "Value": stock["InitialValue"],
                 "PurchasingUnitCostSchedule": convert_dict(
                     int, float, stock["PurchasingUnitCosts"]
                 ),
+                "VariablePurchasingUnitCostSchedule": convert_nested_dict(
+                    int, int, float, stock["VariablePurchasingUnitCosts"]
+                ),
                 "CO2UnitEmissionsSchedule": convert_dict(
                     int, float, stock["CO2UnitEmissions"]
                 ),
                 "UnitIncomeSchedule": convert_dict(int, float, stock["UnitIncomes"]),
                 "Demand": dict(),
                 "StorageUnitCostSchedule": convert_dict(
                     int, float, stock["StorageUnitCosts"]
@@ -531,14 +551,15 @@
                 "OrderPointSchedule": convert_dict(int, float, stock["OrderPoints"]),
                 "OrderQuantitySchedule": dict(),
                 "SafetyQuantitySchedule": convert_dict(
                     int, float, stock["SafetyQuantities"]
                 ),
                 "SchedulingStep": self.entity_order.get(stock["id"], -1),
                 "IgnoreDownstreamRequiredQuantities": stock["IgnoreDownstreamRequiredQuantities"],
+                "SourcingLimit": stock["SourcingLimit"],
             }
 
             if stock_item["StockPolicy"] == "OrderPointFixedQuantity":
                 stock_item["OrderQuantitySchedule"] = convert_dict(
                     int, float, stock["OrderQuantities"]
                 )
             elif stock_item["StockPolicy"] == "OrderPointVariableQuantity":
@@ -683,45 +704,53 @@
                 )
                 theoretical_maximum += (max_opening_time / ct) * op * (1.0 - rr)
         return theoretical_maximum
 
     def __machine(self):
         pr_csv = self.reader.files.get("ProductionResource", [])
         contains_csv = self.reader.files.get("contains", [])
+        output_csv = self.reader.files.get("output", [])
+        stock_csv = self.reader.files.get("Stock", [])
 
         for pr in pr_csv:
             target_operations = [
                 c["target"] for c in contains_csv if c["source"] == pr["id"]
             ]
             operations_count = len(target_operations)
-            target_propotions = {
-                op: 1.0 / operations_count for op in sorted(target_operations)
-            }
 
             group = {}
             if operations_count > 1:
                 group = {
                     self.current_group: {
                         "StartCycle": 0,
                         "EndCycle": self.configuration["SimulatedCycles"] - 1,
                     }
                 }
                 self.current_group += 1
 
+            output_stocks = [
+                o["target"] for o in output_csv if o["source"] in target_operations
+            ]
+
+            future_range = 1 + max(
+                self.lead_times[stock["id"]] + stock["Advance"]
+                for stock in stock_csv
+                if stock["id"] in output_stocks
+            )
+
             pr_item = {
                 "Name": pr["id"],
-                "StockTypeProportion": [target_propotions]
-                * self.configuration["SimulatedCycles"],
                 "Groups": group,
-                "OpeningRates": [1] * self.configuration["SimulatedCycles"],
+                "OpeningRateSchedule": convert_dict(int, float, pr["OpeningRates"]),
                 "OpeningTimeSchedule": convert_dict(int, float, pr["OpeningTimes"]),
                 "ProductionCostSchedule": convert_dict(
                     int, float, pr["FixedProductionCosts"]
                 ),
                 "ProductionPolicy": pr["ProductionPolicy"],
+                "FutureRange": future_range,
             }
             self.files_content["CE_Machine"].append(pr_item)
         self.writer.write_from_list(
             self.files_content["CE_Machine"], "CE_Machine", ordering_key="Name"
         )
 
     def __op_to_stock(self):
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_dict_to_table.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_dict_to_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         time_elements = list(file_description['change'])
 
         max_time_step = 0
 
         for events in file_description['event'].values():
             time_elements.extend(events)
 
+        for quantity_descriptor in file_description['quantity'].values():
+            time_elements.extend(quantity_descriptor)
+
         for element in file_to_convert:
             _local_max = 0
             for time_element in time_elements:
                 time_dict = element.get(time_element, {})
                 if time_dict:
                     _end_time_step = max(map(int, time_dict.keys()))
                     _local_max = max(_local_max, _end_time_step)
@@ -55,25 +58,31 @@
         temporal_data_filename = file_name + "Schedules"
 
         file_description = dataset_description[file_name]
 
         fixed_data = list()
         temporal_data = list()
 
-        events_filenames = list(file_description['event'].keys())
-        event_data = dict()
-        for _name in events_filenames:
-            event_data[_name] = list()
+        event_data = {
+            name: []
+            for name in file_description['event']
+        }
+
+        quantity_data = {
+            name: []
+            for name in file_description['quantity']
+        }
 
         for element in file_to_convert:
             # Each element will be converted separatly
             current_fixed_data = dict()
             if self.simulation_id is not None:
                 current_fixed_data['SimulationRun'] = self.simulation_id
             current_events = dict()
+            current_quantity_data = {}
 
             # First fixed data are read
             for _key in file_description['fixed']:
                 if _key in element:
                     current_fixed_data[_key] = element[_key]
                 else:
                     current_fixed_data[_key] = None
@@ -91,40 +100,56 @@
                             if _timestep not in value:
                                 continue
                             measure = value[str(_timestep)]
                             # This time we have a single key so we directly add it's value
                             schedule[str(_timestep)][change] = measure
                 return schedule
 
+            def read_quantity_data(columns: list) -> dict:
+                schedule = {}
+                for column in columns:
+                    values = element.get(column, {})
+                    if values:
+                        for t in sorted(values, key=int):
+                            for q in sorted(values[t], key=int):
+                                schedule.setdefault(str(t), {}).setdefault(str(q), {})[column] = values[t][q]
+                return schedule
+
             # We read the temporal data for "changes" and "events"
             current_changes = read_data(file_description['change'])
-            for event_name, event_columns in file_description['event'].items():
-                current_events[event_name] = read_data(event_columns)
+            for name, columns in file_description['event'].items():
+                current_events[name] = read_data(columns)
+            for name, columns in file_description['quantity'].items():
+                current_quantity_data[name] = read_quantity_data(columns)
 
             fixed_data.append(current_fixed_data)
 
             # We prepare a data structure to keep the latest change value for our data
             current_change_value = dict()
             for k in file_description['change']:
                 current_change_value[k] = variables_default_values[file_name][k]
+            current_quantity_value = dict()
+            for k in file_description['change']:
+                current_change_value[k] = variables_default_values[file_name][k]
 
             # We create a base row which will be duplicated and filed for each timestep
             present_base = [_k for _k in base_row_keys if _k in current_fixed_data]
             base_row = {_k: current_fixed_data[_k] for _k in present_base}
             previous_row = None
-            for timestep in range(self.total_time_step):
+            for t in range(self.total_time_step):
+                timestep = str(t)
                 if file_description['change']:
                     current_row = base_row.copy()
-                    current_row['Timestep'] = str(timestep)
+                    current_row['Timestep'] = timestep
 
                     def change_from_key(local_key):
                         # In case of a change if the value exists in the data at a given time step
                         # we update our current value then set it in the row
-                        if str(timestep) in current_changes and local_key in current_changes[str(timestep)]:
-                            current_change_value[local_key] = current_changes[str(timestep)][local_key]
+                        if timestep in current_changes and local_key in current_changes[timestep]:
+                            current_change_value[local_key] = current_changes[timestep][local_key]
                         current_row[local_key] = current_change_value[local_key]
 
                     # We loop over all our keys in "changes" and in "events"
                     for change_key in file_description['change']:
                         change_from_key(change_key)
 
                     # If we have any data in "changes" or "events" we keep the created row
@@ -138,27 +163,43 @@
                                     break
                     if to_be_kept:
                         previous_row = current_row
                         temporal_data.append(current_row)
 
                 for event_name, event_columns in file_description['event'].items():
                     event_row = base_row.copy()
-                    event_row['Timestep'] = str(timestep)
+                    event_row['Timestep'] = timestep
                     event_exists = False
                     current_event = current_events[event_name]
                     for event_key in event_columns:
-                        if str(timestep) in current_event and event_key in current_event[str(timestep)]:
-                            event_row[event_key] = current_event[str(timestep)][event_key]
+                        if timestep in current_event and event_key in current_event[timestep]:
+                            event_row[event_key] = current_event[timestep][event_key]
                             event_exists = True
                         else:
-                            # Needs a default value depending on the key
-                            event_row[event_key] = 0.0
+                            event_row[event_key] = variables_default_values[file_name][event_key]
                     if event_exists or self.keep_duplicate:
                         event_data[event_name].append(event_row)
 
+                for name, columns in file_description['quantity'].items():
+                    datum = current_quantity_data[name]
+                    if timestep in datum:
+                        for quantity, values in datum[timestep].items():
+                            row = base_row.copy()
+                            row['Timestep'] = timestep
+                            row['Quantity'] = quantity
+                            value_is_defined = False
+                            for column in columns:
+                                if column in values:
+                                    row[column] = values[column]
+                                    value_is_defined = True
+                                else:
+                                    row[column] = variables_default_values[file_name][column]
+                            if value_is_defined or self.keep_duplicate:
+                                quantity_data[name].append(row)
+
         if fixed_data:
             self.write_target_file(fixed_data, fixed_data_filename, self.simulation_id)
         else:
             fake_fixed_element = dict()
             for key in file_description['fixed']:
                 fake_fixed_element[key] = None
             if self.simulation_id:
@@ -186,14 +227,26 @@
                 fake_event_element = dict()
                 for column_list in fake_row_keys, ['Timestep', ], file_description['event'][event_name]:
                     for key in column_list:
                         fake_event_element[key] = None
                 if self.simulation_id:
                     fake_event_element['SimulationRun'] = self.simulation_id
                 self.write_target_file([fake_event_element, ], event_name, self.simulation_id)
+        for name, file_content in quantity_data.items():
+            if file_content:
+                self.write_target_file(file_content, name, self.simulation_id)
+            elif file_description['quantity'][name]:
+                fake_content = {
+                    column: None
+                    for columns in (fake_row_keys, ['Timestep', 'Quantity'], file_description['quantity'][name])
+                    for column in columns
+                }
+                if self.simulation_id:
+                    fake_content['SimulationRun'] = self.simulation_id
+                self.write_target_file([fake_content, ], name, self.simulation_id)
         self.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - " + file_name)
 
     def __init__(self,
                  simulation_id: Union[str, None],
                  reader: FolderReader,
                  writer: Union[FolderWriter, None] = None,
                  adx_connector: Union[ADXQueriesWrapper, ADXWrapper, None] = None,
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_table_to_dict.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,32 +63,36 @@
             if master_key and entity.get(master_key) is None:
                 continue
             entities.append(entity)
 
         if master_key:
             errors += self.check_indices(file_name, [entity[master_key] for entity in entities])
 
-        if file_description['event'] or file_description['change']:
+        if any(file_description[timed] for timed in ('event', 'change', 'quantity')):
 
             entity_by_id = dict()
             for entity in entities:
                 entity_by_id[entity[master_key]] = entity
 
             time_files = dict()
             time_files[file_name + "Schedules"] = file_description['change']
             for _event_name, _event_descriptor in file_description['event'].items():
                 time_files[_event_name] = _event_descriptor
+            for _quantity_name, _quantity_descriptor in file_description['quantity'].items():
+                time_files[_quantity_name] = _quantity_descriptor
+            quantity_files = set(file_description['quantity'].keys())
 
             for _sheet_name, _columns in time_files.items():
                 if _sheet_name not in self.reader.files or not _columns:
                     continue
                 _sheet_to_convert = self.reader.files[_sheet_name]
                 indices = []
                 unknown_ids = set()
                 invalid_timesteps = set()
+                invalid_quantities = set()
                 for line in _sheet_to_convert:
                     _id = line.get(master_key)
                     if _id is None:
                         continue
                     if _id not in entity_by_id:
                         unknown_ids.add(_id)
                         continue
@@ -97,38 +101,59 @@
                     except ValueError:
                         invalid_timesteps.add((_id, line.get('Timestep')))
                         continue
                     if timestep != int(timestep):
                         invalid_timesteps.add((_id, line.get('Timestep')))
                         continue
                     timestep = str(int(timestep))
-                    indices.append((_id, timestep))
+                    index = (_id, timestep)
+                    if _sheet_name in quantity_files:
+                        try:
+                            quantity = float(line.get('Quantity') or 0)
+                        except ValueError:
+                            invalid_quantities.add((_id, line.get('Quantity')))
+                            continue
+                        if quantity != int(quantity):
+                            invalid_quantities.add((_id, line.get('Quantity')))
+                            continue
+                        quantity = str(int(quantity))
+                        index = (*index, quantity)
+                    indices.append(index)
                     target_entity = entity_by_id[_id]
                     for column in (c for c in _columns if line.get(c) is not None):
                         if column not in target_entity:
                             target_entity[column] = dict()
                         if column in line:
-                            target_entity[column][timestep] = line[column]
+                            if _sheet_name in quantity_files:
+                                target_entity[column].setdefault(timestep, {})[quantity] = line[column]
+                            else:
+                                target_entity[column][timestep] = line[column]
                 if unknown_ids:
                     n = len(unknown_ids)
                     errors += n
                     self.display_message(f"ERROR: {master_key} value{'s' if n > 1 else ''} from {_sheet_name} not found in {file_name}:")
                     for _id in unknown_ids:
                         self.display_message(f"  {_id}")
-                    non_referenced_ids = set(entity_by_id.keys()) - set(_id for _id, _ in indices)
+                    non_referenced_ids = set(entity_by_id.keys()) - set(index[0] for index in indices)
                     if non_referenced_ids:
                         self.display_message(f"Suggestion: {master_key} value{'s' if len(non_referenced_ids) > 1 else ''} from {file_name} not found in {_sheet_name}:")
                         for _id in non_referenced_ids:
                             self.display_message(f"  {_id}")
                 if invalid_timesteps:
                     n = len(invalid_timesteps)
                     errors += n
                     self.display_message(f"ERROR: invalid Timestep value{'s' if n > 1 else ''} from {_sheet_name}:")
                     for _id, timestep in invalid_timesteps:
                         self.display_message(f"  {master_key} {_id}: {timestep}")
+                if invalid_quantities:
+                    n = len(invalid_quantities)
+                    errors += n
+                    self.display_message(f"ERROR: invalid Quantity value{'s' if n > 1 else ''} from {_sheet_name}:")
+                    for _id, quantity in invalid_timesteps:
+                        self.display_message(f"  {master_key} {_id}: {quantity}")
                 errors += self.check_indices(_sheet_name, indices)
 
         for entity in entities:
             for change in file_description['change']:
                 raw_values = entity.get(change)
                 if not raw_values:
                     continue
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/from_table_to_dict_old.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/patch_dict_with_parameters.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/patch_dict_with_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Transform/production_route.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Validate/validate_dict.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Validate/validate_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,14 +209,17 @@
 
         self.__obsolescence_check()
         self.split("\tobsolescence_check: {time_since_last_split:6.4f}s")
 
         self.__sourcing_proportions_check()
         self.split("\tsourcing_proportions_check: {time_since_last_split:6.4f}s")
 
+        self.__production_proportions_check()
+        self.split("\tproduction_proportions_check: {time_since_last_split:6.4f}s")
+
         self.__check_resource_dependencies()
         self.split("\tcheck_resource_dependencies: {time_since_last_split:6.4f}s")
 
         self.__mandatory_attributes_check()
         self.split("\tmandatory_attributes_check: {time_since_last_split:6.4f}s")
 
         if self.errors:
@@ -378,14 +381,46 @@
                     if proportions_sum < 1 - e or proportions_sum > 1 + e:
                         errors.append(time_step)
                 if errors:
                     self.errors.append(('ProductionOperationSchedules/TransportSchedules',
                                         'SourcingProportions',
                                         f"The sum of the {stock} sources proportions ({', '.join(sources)}) is not equal to one for the time step{'s' if len(errors) > 1 else ''}: {', '.join(errors)}"))
 
+    def __production_proportions_check(self):
+        operations_by_resource = {}
+        production_proportions = {}
+
+        for contains in self.reader.files.get('contains', []):
+            operations_by_resource.setdefault(contains['source'], []).append(contains['target'])
+        for operation in self.reader.files.get('ProductionOperation', []):
+            production_proportions[operation['id']] = operation.get('ProductionProportions')
+
+        e = 1e-2
+        for resource, operations in operations_by_resource.items():
+            considered_operations = {operation for operation in operations if production_proportions[operation] is not None}
+            if considered_operations:
+                time_steps = sorted(set(
+                    t
+                    for operation in considered_operations
+                    for t in production_proportions[operation]
+                ), key=int)
+                proportions = {}
+                errors = []
+                for time_step in time_steps:
+                    for operation in considered_operations:
+                        if time_step in production_proportions[operation]:
+                            proportions[operation] = production_proportions[operation][time_step]
+                    proportions_sum = sum(proportions.values())
+                    if proportions_sum < 1 - e or proportions_sum > 1 + e:
+                        errors.append(time_step)
+                if errors:
+                    self.errors.append(('ProductionOperationSchedules',
+                                        'ProductionProportions',
+                                        f"The sum of the {resource} operations proportions ({', '.join(operations)}) is not equal to one for the time step{'s' if len(errors) > 1 else ''}: {', '.join(errors)}"))
+
     def find_relations_by_id(self, relation_name: str, looked_id: str, relation_column: str):
         if (relation_name, looked_id, relation_column) not in self.lookup_memory:
             self.lookup_memory[(relation_name, looked_id, relation_column)] = [
                 row
                 for row in self.reader.files[relation_name]
                 if row.get(relation_column) == looked_id
             ]
```

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/environment_variables.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.2.2/Supplychain/Wrappers/simulator.py` & `CosmoTech-SupplyChain-5.3.0/Supplychain/Wrappers/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             name = machine.GetName()
             op_name = operation.GetName()
             for k in map(str, groups.GetKeys()):
                 yield (
                     "Machine",
                     name,
                     op_name,
-                    "StockTypeProportions",
+                    "ProductionProportionSchedule",
                     groups.GetAttribute(k).GetAttributeAsString("StartCycle"),
                     groups.GetAttribute(k).GetAttributeAsString("EndCycle"),
                     k
                 )
 
 
 @register_into_simulatorinterface
@@ -448,7 +448,32 @@
                 demand.GetAttribute("InternalDemand").Get(),
                 demand.GetAttribute("MaxVal").Get(),
                 demand.GetAttribute("ExternalWeight").Get(),
                 demand.GetAttribute("InternalWeight").Get(),
                 demand.GetAttribute("BacklogWeight").Get(),
                 demand.GetAttribute("WeightMax").Get(),
             )
+
+
+@register_into_simulatorinterface
+def uses_variable_purchasing_costs(self, force=False):
+    return any(
+        stock.GetAttribute("VariablePurchasingUnitCostSchedule").Get()
+        for stock in self.get_entities_by_type('Stock', force=force)
+    )
+
+
+@register_into_simulatorinterface
+def get_variable_purchasing_costs_by_stock(self, force=False):
+    purchasing_costs_by_stock = {}
+    for stock in self.get_entities_by_type('Stock', force=force):
+        purchasing_unit_cost = stock.GetAttribute("PurchasingUnitCost").Get()
+        purchasing_unit_costs = stock.GetAttribute("PurchasingUnitCostSchedule").Get()
+        variable_purchasing_unit_costs = stock.GetAttribute("VariablePurchasingUnitCostSchedule").Get()
+        if variable_purchasing_unit_costs:
+            for t, variable_purchasing_unit_cost in variable_purchasing_unit_costs.items():
+                if 0 not in variable_purchasing_unit_cost.keys():
+                    if purchasing_unit_costs:
+                        purchasing_unit_cost = purchasing_unit_costs[max(u for u in purchasing_unit_costs.keys() if u <= t)]
+                    variable_purchasing_unit_cost[0] = purchasing_unit_cost
+            purchasing_costs_by_stock[stock.GetName()] = variable_purchasing_unit_costs
+    return purchasing_costs_by_stock
```

### Comparing `CosmoTech-SupplyChain-5.2.2/setup.py` & `CosmoTech-SupplyChain-5.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "5.2.2"
+VERSION = "5.3.0"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

