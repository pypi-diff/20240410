# Comparing `tmp/ecosystem-notebooks-0.1.5.tar.gz` & `tmp/ecosystem-notebooks-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecosystem-notebooks-0.1.5.tar", last modified: Thu Dec  7 10:33:36 2023, max compression
+gzip compressed data, was "ecosystem-notebooks-0.1.6.tar", last modified: Tue Apr  9 12:11:34 2024, max compression
```

## Comparing `ecosystem-notebooks-0.1.5.tar` & `ecosystem-notebooks-0.1.6.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.669695 ecosystem-notebooks-0.1.5/
--rw-rw-rw-   0        0        0     1090 2023-10-23 10:44:53.000000 ecosystem-notebooks-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      418 2023-10-23 10:44:53.000000 ecosystem-notebooks-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3746 2023-12-07 10:33:36.668702 ecosystem-notebooks-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2023-11-03 07:25:35.000000 ecosystem-notebooks-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.404054 ecosystem-notebooks-0.1.5/docs/
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.412072 ecosystem-notebooks-0.1.5/docs/images/
--rw-rw-rw-   0        0        0    62723 2023-10-23 10:44:53.000000 ecosystem-notebooks-0.1.5/docs/images/jupyter_landing_page.png
--rw-rw-rw-   0        0        0    25467 2023-10-23 10:44:53.000000 ecosystem-notebooks-0.1.5/docs/images/login.png
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.424627 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/
--rw-rw-rw-   0        0        0     3746 2023-12-07 10:33:36.000000 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2933 2023-12-07 10:33:36.000000 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 10:33:36.000000 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-12-07 10:33:36.000000 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-12-07 10:33:36.000000 ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.442189 ecosystem-notebooks-0.1.5/prediction/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.522044 ecosystem-notebooks-0.1.5/prediction/apis/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/__init__.py
--rw-rw-rw-   0        0        0     6850 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/algorithm_client_pulse.py
--rw-rw-rw-   0        0        0     1326 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/auth_controller.py
--rw-rw-rw-   0        0        0     2933 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/data_ingestion_engine.py
--rw-rw-rw-   0        0        0    10704 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/data_management_engine.py
--rw-rw-rw-   0        0        0    13476 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/data_munging_engine.py
--rw-rw-rw-   0        0        0     1105 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/ecosystem_generation_engine.py
--rw-rw-rw-   0        0        0      917 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/ecosystem_home.py
--rw-rw-rw-   0        0        0      421 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/ecosystem_main.py
--rw-rw-rw-   0        0        0     1190 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/ecosystem_user_profiles.py
--rw-rw-rw-   0        0        0     2145 2023-12-07 10:30:36.000000 ecosystem-notebooks-0.1.5/prediction/apis/functions.py
--rw-rw-rw-   0        0        0      270 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/interactions.py
--rw-rw-rw-   0        0        0     7684 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/prediction_engine.py
--rw-rw-rw-   0        0        0     2136 2023-12-07 10:30:36.000000 ecosystem-notebooks-0.1.5/prediction/apis/quickflat.py
--rw-rw-rw-   0        0        0      254 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/settings_controller.py
--rw-rw-rw-   0        0        0      833 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/transaction_categorization.py
--rw-rw-rw-   0        0        0     1179 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/user_controller.py
--rw-rw-rw-   0        0        0     2695 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/utilities.py
--rw-rw-rw-   0        0        0     2532 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_aws.py
--rw-rw-rw-   0        0        0     4008 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_file_service.py
--rw-rw-rw-   0        0        0      539 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_google.py
--rw-rw-rw-   0        0        0     5110 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_h2o.py
--rw-rw-rw-   0        0        0      321 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_microsoft.py
--rw-rw-rw-   0        0        0      298 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_open_ai.py
--rw-rw-rw-   0        0        0     2941 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/apis/worker_uber.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.616466 ecosystem-notebooks-0.1.5/prediction/endpoints/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/__init__.py
--rw-rw-rw-   0        0        0     3124 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/algorithm_client_pulse.py
--rw-rw-rw-   0        0        0     1201 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/auth_controller.py
--rw-rw-rw-   0        0        0     1826 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/data_ingestion_engine.py
--rw-rw-rw-   0        0        0     6067 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/data_management_engine.py
--rw-rw-rw-   0        0        0     5551 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/data_munging_engine.py
--rw-rw-rw-   0        0        0      871 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_generation_engine.py
--rw-rw-rw-   0        0        0      624 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_home.py
--rw-rw-rw-   0        0        0      349 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_main.py
--rw-rw-rw-   0        0        0      787 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_user_profiles.py
--rw-rw-rw-   0        0        0      160 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/interaction.py
--rw-rw-rw-   0        0        0     5150 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/prediction_engine.py
--rw-rw-rw-   0        0        0      184 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/settings_controller.py
--rw-rw-rw-   0        0        0      559 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/transaction_categorization.py
--rw-rw-rw-   0        0        0      489 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/user_controller.py
--rw-rw-rw-   0        0        0     1872 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/utilities.py
--rw-rw-rw-   0        0        0     1842 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_aws.py
--rw-rw-rw-   0        0        0     2334 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_file_service.py
--rw-rw-rw-   0        0        0      344 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_google.py
--rw-rw-rw-   0        0        0     3722 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_h2o.py
--rw-rw-rw-   0        0        0      179 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_microsoft.py
--rw-rw-rw-   0        0        0      172 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_open_ai.py
--rw-rw-rw-   0        0        0      865 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/endpoints/worker_uber.py
--rw-rw-rw-   0        0        0      337 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/export_to_notebook.py
--rw-rw-rw-   0        0        0     3051 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/jwt_access.py
--rw-rw-rw-   0        0        0     2016 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/nlp_utils.py
--rw-rw-rw-   0        0        0     4548 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/notebook_functions.py
--rw-rw-rw-   0        0        0     1744 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/prediction_utils.py
--rw-rw-rw-   0        0        0     3669 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/request_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.620466 ecosystem-notebooks-0.1.5/prediction/utils/
--rw-rw-rw-   0        0        0     6105 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/prediction/utils/endpoint_diff.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.625510 ecosystem-notebooks-0.1.5/runtime/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/__init__.py
--rw-rw-rw-   0        0        0      520 2023-12-07 10:30:36.000000 ecosystem-notebooks-0.1.5/runtime/access.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.645612 ecosystem-notebooks-0.1.5/runtime/apis/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/__init__.py
--rw-rw-rw-   0        0        0     4654 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/data_management_engine.py
--rw-rw-rw-   0        0        0     9025 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/predictor_engine.py
--rw-rw-rw-   0        0        0      468 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/restart_controller.py
--rw-rw-rw-   0        0        0      869 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/runtime_engine.py
--rw-rw-rw-   0        0        0    14478 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/apis/worker_utilities.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.664688 ecosystem-notebooks-0.1.5/runtime/endpoints/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2515 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/data_management_engine.py
--rw-rw-rw-   0        0        0     2627 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/predictor_engine.py
--rw-rw-rw-   0        0        0      313 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/restart_controller.py
--rw-rw-rw-   0        0        0      294 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/runtime_engine.py
--rw-rw-rw-   0        0        0     6372 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/endpoints/worker_utilities.py
--rw-rw-rw-   0        0        0      337 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/export_to_notebook.py
--rw-rw-rw-   0        0        0     3723 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/request_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-07 10:33:36.668702 ecosystem-notebooks-0.1.5/runtime/utils/
--rw-rw-rw-   0        0        0     5271 2023-10-23 10:44:54.000000 ecosystem-notebooks-0.1.5/runtime/utils/endpoint_diff.py
--rw-rw-rw-   0        0        0       42 2023-12-07 10:33:36.669695 ecosystem-notebooks-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2234 2023-12-07 10:33:14.000000 ecosystem-notebooks-0.1.5/setup.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.229302 ecosystem-notebooks-0.1.6/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/LICENSE
+-rw-r--r--   0 ericnewby   (501) staff       (20)      400 2023-10-13 03:48:11.000000 ecosystem-notebooks-0.1.6/MANIFEST.in
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-09 12:11:34.228935 ecosystem-notebooks-0.1.6/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2966 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.6/README.rst
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.198794 ecosystem-notebooks-0.1.6/docs/
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.201292 ecosystem-notebooks-0.1.6/docs/images/
+-rw-r--r--   0 ericnewby   (501) staff       (20)    62723 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/docs/images/jupyter_landing_page.png
+-rw-r--r--   0 ericnewby   (501) staff       (20)    25467 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/docs/images/login.png
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.202206 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-09 12:11:34.000000 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2024-04-09 12:11:34.000000 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/SOURCES.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)        1 2024-04-09 12:11:34.000000 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/dependency_links.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       17 2024-04-09 12:11:34.000000 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/requires.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       19 2024-04-09 12:11:34.000000 ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/top_level.txt
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.204673 ecosystem-notebooks-0.1.6/prediction/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/__init__.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.212786 ecosystem-notebooks-0.1.6/prediction/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6645 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2852 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    10341 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    13059 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    97109 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.6/prediction/apis/deployment_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      889 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      408 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1146 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2085 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.6/prediction/apis/functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      263 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/interactions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    14570 2024-04-09 12:05:58.000000 ecosystem-notebooks-0.1.6/prediction/apis/online_learning_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     7959 2024-04-07 09:49:09.000000 ecosystem-notebooks-0.1.6/prediction/apis/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2067 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.6/prediction/apis/quickflat.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      246 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      811 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1145 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2601 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2439 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4005 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      520 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4954 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      311 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      291 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2860 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/apis/worker_uber.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.223507 ecosystem-notebooks-0.1.6/prediction/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1159 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1765 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5864 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5350 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      598 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      335 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      754 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      155 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/interaction.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5299 2024-04-07 09:47:48.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      178 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      540 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      471 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1806 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1766 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2238 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      331 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3591 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      173 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      167 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      831 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/endpoints/worker_uber.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/prediction/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2955 2023-06-02 11:33:45.000000 ecosystem-notebooks-0.1.6/prediction/jwt_access.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1952 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/nlp_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4412 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/notebook_functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1689 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/prediction_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3815 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.6/prediction/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.223733 ecosystem-notebooks-0.1.6/prediction/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5888 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/prediction/utils/endpoint_diff.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.224895 ecosystem-notebooks-0.1.6/runtime/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      517 2024-04-08 10:10:12.000000 ecosystem-notebooks-0.1.6/runtime/access.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.226838 ecosystem-notebooks-0.1.6/runtime/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4488 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/runtime/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     8791 2024-04-09 06:48:15.000000 ecosystem-notebooks-0.1.6/runtime/apis/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      452 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/apis/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/apis/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    14076 2023-04-24 06:53:33.000000 ecosystem-notebooks-0.1.6/runtime/apis/worker_utilities.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.228086 ecosystem-notebooks-0.1.6/runtime/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2431 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2538 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      302 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      283 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6123 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/runtime/endpoints/worker_utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.6/runtime/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3632 2024-04-08 10:10:58.000000 ecosystem-notebooks-0.1.6/runtime/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-09 12:11:34.228335 ecosystem-notebooks-0.1.6/runtime/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5079 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.6/runtime/utils/endpoint_diff.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)       38 2024-04-09 12:11:34.229510 ecosystem-notebooks-0.1.6/setup.cfg
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2151 2024-04-09 12:11:21.000000 ecosystem-notebooks-0.1.6/setup.py
```

### Comparing `ecosystem-notebooks-0.1.5/PKG-INFO` & `ecosystem-notebooks-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,102 @@
-Metadata-Version: 2.1
-Name: ecosystem-notebooks
-Version: 0.1.5
-Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
-Home-page: https://github.com/ecosystemai/ecosystem-notebooks
-Author: EcosystemAi
-Author-email: jay@ecosystem.ai
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter :: JupyterLab
-License-File: LICENSE
-
-Ecosystem Notebooks
-===================
-
-What is Ecosystem Notebooks?
-----------------------------
-
-Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
-be used for both the Prediction and Runtime servers.
-
-The notebooks are a great interface to work from in order to test, and
-explore the server’s capabilities. They allow you to navigate them
-easily by removing the complexities of directly interacting with the
-APIs.
-
-Ecosystem Notebooks are built using the Jupyter Notebook coding
-environment, and Python 3 kernel for code execution.
-
-Requirements
-------------
-
--  To use any of the notebooks, access to an Ecosystem API server is
-   required
--  `Jupyter Notebook <https://jupyter.org/>`__
--  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
-   built using python 3.6, but most Python 3 versions will work
-
-Getting started
----------------
-
-To begin using Ecosystem Notebooks, you need to first install Jupyter
-Notebook.
-
-This can be done by running the configure_jupyter.sh shell script. In
-addition, recommended styling options can be added by running the
-configure_jupyter_styling.sh shell script. While this is not required,
-you are welcome to play around with it to personalise the Ecosystem
-workbench style.
-
-To install the relevant python code, add the parent directory
-(ecosystem-notebooks) to the PYTHONPATH environment variable.
-
-Once Jupyter is installed, enter the directory containing the notebooks.
-At the designated .ipynb extension, run the command:
-
-.. code:: bash
-
-   jupyter notebook
-
-This will open up a default web browser to the Jupyter Notebook landing
-page from which you can open up one of the desired notebooks.
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
-   :alt: Jupyter Landing Page
-
-   Jupyter Landing Page
-
-How does Ecosystem Notebooks work
----------------------------------
-
-From within a chosen notebook, Ecosystem Notebooks can be used. This
-coding environment, from which you can edit and run live code, provides
-the interface with which to utilise the API endpoints for Ecosystem
-Prediction and Runtime servers.For easy navigation within any of the
-notebooks, you can use the table of contents which will be situated on
-the left.
-
-In order for the API endpoints to properly function, you will need to
-login. Depending on which notebooks you have chosen to use, logging in
-could require a URL endpoint. Or a username, password and URL
-combination, which will generate an authentication token. This token
-will activate the API, then you can begin using Ecosystem Notebooks!
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
-   :alt: Login
-
-   Login
-
-Ecosystem Notebooks contains all the available API endpoints on the
-Ecosystem Servers. You can either play around in the ecosystem
-environment, or you can use it in your own chosen infrastructure.
+Metadata-Version: 2.1
+Name: ecosystem-notebooks
+Version: 0.1.6
+Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
+Home-page: https://github.com/ecosystemai/ecosystem-notebooks
+Author: EcosystemAi
+Author-email: jay@ecosystem.ai
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Jupyter :: JupyterLab
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pymongo
+
+Ecosystem Notebooks
+===================
+
+What is Ecosystem Notebooks?
+----------------------------
+
+Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
+be used for both the Prediction and Runtime servers.
+
+The notebooks are a great interface to work from in order to test, and
+explore the server’s capabilities. They allow you to navigate them
+easily by removing the complexities of directly interacting with the
+APIs.
+
+Ecosystem Notebooks are built using the Jupyter Notebook coding
+environment, and Python 3 kernel for code execution.
+
+Requirements
+------------
+
+-  To use any of the notebooks, access to an Ecosystem API server is
+   required
+-  `Jupyter Notebook <https://jupyter.org/>`__
+-  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
+   built using python 3.6, but most Python 3 versions will work
+
+Getting started
+---------------
+
+To begin using Ecosystem Notebooks, you need to first install Jupyter
+Notebook.
+
+This can be done by running the configure_jupyter.sh shell script. In
+addition, recommended styling options can be added by running the
+configure_jupyter_styling.sh shell script. While this is not required,
+you are welcome to play around with it to personalise the Ecosystem
+workbench style.
+
+To install the relevant python code, add the parent directory
+(ecosystem-notebooks) to the PYTHONPATH environment variable.
+
+Once Jupyter is installed, enter the directory containing the notebooks.
+At the designated .ipynb extension, run the command:
+
+.. code:: bash
+
+   jupyter notebook
+
+This will open up a default web browser to the Jupyter Notebook landing
+page from which you can open up one of the desired notebooks.
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
+   :alt: Jupyter Landing Page
+
+   Jupyter Landing Page
+
+How does Ecosystem Notebooks work
+---------------------------------
+
+From within a chosen notebook, Ecosystem Notebooks can be used. This
+coding environment, from which you can edit and run live code, provides
+the interface with which to utilise the API endpoints for Ecosystem
+Prediction and Runtime servers.For easy navigation within any of the
+notebooks, you can use the table of contents which will be situated on
+the left.
+
+In order for the API endpoints to properly function, you will need to
+login. Depending on which notebooks you have chosen to use, logging in
+could require a URL endpoint. Or a username, password and URL
+combination, which will generate an authentication token. This token
+will activate the API, then you can begin using Ecosystem Notebooks!
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
+   :alt: Login
+
+   Login
+
+Ecosystem Notebooks contains all the available API endpoints on the
+Ecosystem Servers. You can either play around in the ecosystem
+environment, or you can use it in your own chosen infrastructure.
```

### Comparing `ecosystem-notebooks-0.1.5/README.rst` & `ecosystem-notebooks-0.1.6/README.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-Ecosystem Notebooks
-===================
-
-What is Ecosystem Notebooks?
-----------------------------
-
-Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
-be used for both the Prediction and Runtime servers.
-
-The notebooks are a great interface to work from in order to test, and
-explore the server’s capabilities. They allow you to navigate them
-easily by removing the complexities of directly interacting with the
-APIs.
-
-Ecosystem Notebooks are built using the Jupyter Notebook coding
-environment, and Python 3 kernel for code execution.
-
-Requirements
-------------
-
--  To use any of the notebooks, access to an Ecosystem API server is
-   required
--  `Jupyter Notebook <https://jupyter.org/>`__
--  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
-   built using python 3.6, but most Python 3 versions will work
-
-Getting started
----------------
-
-To begin using Ecosystem Notebooks, you need to first install Jupyter
-Notebook.
-
-This can be done by running the configure_jupyter.sh shell script. In
-addition, recommended styling options can be added by running the
-configure_jupyter_styling.sh shell script. While this is not required,
-you are welcome to play around with it to personalise the Ecosystem
-workbench style.
-
-To install the relevant python code, add the parent directory
-(ecosystem-notebooks) to the PYTHONPATH environment variable.
-
-Once Jupyter is installed, enter the directory containing the notebooks.
-At the designated .ipynb extension, run the command:
-
-.. code:: bash
-
-   jupyter notebook
-
-This will open up a default web browser to the Jupyter Notebook landing
-page from which you can open up one of the desired notebooks.
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
-   :alt: Jupyter Landing Page
-
-   Jupyter Landing Page
-
-How does Ecosystem Notebooks work
----------------------------------
-
-From within a chosen notebook, Ecosystem Notebooks can be used. This
-coding environment, from which you can edit and run live code, provides
-the interface with which to utilise the API endpoints for Ecosystem
-Prediction and Runtime servers.For easy navigation within any of the
-notebooks, you can use the table of contents which will be situated on
-the left.
-
-In order for the API endpoints to properly function, you will need to
-login. Depending on which notebooks you have chosen to use, logging in
-could require a URL endpoint. Or a username, password and URL
-combination, which will generate an authentication token. This token
-will activate the API, then you can begin using Ecosystem Notebooks!
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
-   :alt: Login
-
-   Login
-
-Ecosystem Notebooks contains all the available API endpoints on the
-Ecosystem Servers. You can either play around in the ecosystem
+Ecosystem Notebooks
+===================
+
+What is Ecosystem Notebooks?
+----------------------------
+
+Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
+be used for both the Prediction and Runtime servers.
+
+The notebooks are a great interface to work from in order to test, and
+explore the server’s capabilities. They allow you to navigate them
+easily by removing the complexities of directly interacting with the
+APIs.
+
+Ecosystem Notebooks are built using the Jupyter Notebook coding
+environment, and Python 3 kernel for code execution.
+
+Requirements
+------------
+
+-  To use any of the notebooks, access to an Ecosystem API server is
+   required
+-  `Jupyter Notebook <https://jupyter.org/>`__
+-  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
+   built using python 3.6, but most Python 3 versions will work
+
+Getting started
+---------------
+
+To begin using Ecosystem Notebooks, you need to first install Jupyter
+Notebook.
+
+This can be done by running the configure_jupyter.sh shell script. In
+addition, recommended styling options can be added by running the
+configure_jupyter_styling.sh shell script. While this is not required,
+you are welcome to play around with it to personalise the Ecosystem
+workbench style.
+
+To install the relevant python code, add the parent directory
+(ecosystem-notebooks) to the PYTHONPATH environment variable.
+
+Once Jupyter is installed, enter the directory containing the notebooks.
+At the designated .ipynb extension, run the command:
+
+.. code:: bash
+
+   jupyter notebook
+
+This will open up a default web browser to the Jupyter Notebook landing
+page from which you can open up one of the desired notebooks.
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
+   :alt: Jupyter Landing Page
+
+   Jupyter Landing Page
+
+How does Ecosystem Notebooks work
+---------------------------------
+
+From within a chosen notebook, Ecosystem Notebooks can be used. This
+coding environment, from which you can edit and run live code, provides
+the interface with which to utilise the API endpoints for Ecosystem
+Prediction and Runtime servers.For easy navigation within any of the
+notebooks, you can use the table of contents which will be situated on
+the left.
+
+In order for the API endpoints to properly function, you will need to
+login. Depending on which notebooks you have chosen to use, logging in
+could require a URL endpoint. Or a username, password and URL
+combination, which will generate an authentication token. This token
+will activate the API, then you can begin using Ecosystem Notebooks!
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
+   :alt: Login
+
+   Login
+
+Ecosystem Notebooks contains all the available API endpoints on the
+Ecosystem Servers. You can either play around in the ecosystem
 environment, or you can use it in your own chosen infrastructure.
```

### Comparing `ecosystem-notebooks-0.1.5/docs/images/jupyter_landing_page.png` & `ecosystem-notebooks-0.1.6/docs/images/jupyter_landing_page.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.5/docs/images/login.png` & `ecosystem-notebooks-0.1.6/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/PKG-INFO` & `ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,102 @@
-Metadata-Version: 2.1
-Name: ecosystem-notebooks
-Version: 0.1.5
-Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
-Home-page: https://github.com/ecosystemai/ecosystem-notebooks
-Author: EcosystemAi
-Author-email: jay@ecosystem.ai
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter :: JupyterLab
-License-File: LICENSE
-
-Ecosystem Notebooks
-===================
-
-What is Ecosystem Notebooks?
-----------------------------
-
-Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
-be used for both the Prediction and Runtime servers.
-
-The notebooks are a great interface to work from in order to test, and
-explore the server’s capabilities. They allow you to navigate them
-easily by removing the complexities of directly interacting with the
-APIs.
-
-Ecosystem Notebooks are built using the Jupyter Notebook coding
-environment, and Python 3 kernel for code execution.
-
-Requirements
-------------
-
--  To use any of the notebooks, access to an Ecosystem API server is
-   required
--  `Jupyter Notebook <https://jupyter.org/>`__
--  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
-   built using python 3.6, but most Python 3 versions will work
-
-Getting started
----------------
-
-To begin using Ecosystem Notebooks, you need to first install Jupyter
-Notebook.
-
-This can be done by running the configure_jupyter.sh shell script. In
-addition, recommended styling options can be added by running the
-configure_jupyter_styling.sh shell script. While this is not required,
-you are welcome to play around with it to personalise the Ecosystem
-workbench style.
-
-To install the relevant python code, add the parent directory
-(ecosystem-notebooks) to the PYTHONPATH environment variable.
-
-Once Jupyter is installed, enter the directory containing the notebooks.
-At the designated .ipynb extension, run the command:
-
-.. code:: bash
-
-   jupyter notebook
-
-This will open up a default web browser to the Jupyter Notebook landing
-page from which you can open up one of the desired notebooks.
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
-   :alt: Jupyter Landing Page
-
-   Jupyter Landing Page
-
-How does Ecosystem Notebooks work
----------------------------------
-
-From within a chosen notebook, Ecosystem Notebooks can be used. This
-coding environment, from which you can edit and run live code, provides
-the interface with which to utilise the API endpoints for Ecosystem
-Prediction and Runtime servers.For easy navigation within any of the
-notebooks, you can use the table of contents which will be situated on
-the left.
-
-In order for the API endpoints to properly function, you will need to
-login. Depending on which notebooks you have chosen to use, logging in
-could require a URL endpoint. Or a username, password and URL
-combination, which will generate an authentication token. This token
-will activate the API, then you can begin using Ecosystem Notebooks!
-
-.. figure::
-   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
-   :alt: Login
-
-   Login
-
-Ecosystem Notebooks contains all the available API endpoints on the
-Ecosystem Servers. You can either play around in the ecosystem
-environment, or you can use it in your own chosen infrastructure.
+Metadata-Version: 2.1
+Name: ecosystem-notebooks
+Version: 0.1.6
+Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
+Home-page: https://github.com/ecosystemai/ecosystem-notebooks
+Author: EcosystemAi
+Author-email: jay@ecosystem.ai
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Jupyter :: JupyterLab
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pymongo
+
+Ecosystem Notebooks
+===================
+
+What is Ecosystem Notebooks?
+----------------------------
+
+Ecosystem Notebooks is a wrapper for the Ecosystem API servers. They can
+be used for both the Prediction and Runtime servers.
+
+The notebooks are a great interface to work from in order to test, and
+explore the server’s capabilities. They allow you to navigate them
+easily by removing the complexities of directly interacting with the
+APIs.
+
+Ecosystem Notebooks are built using the Jupyter Notebook coding
+environment, and Python 3 kernel for code execution.
+
+Requirements
+------------
+
+-  To use any of the notebooks, access to an Ecosystem API server is
+   required
+-  `Jupyter Notebook <https://jupyter.org/>`__
+-  `Python 3 <https://www.python.org/downloads/>`__: The notebooks were
+   built using python 3.6, but most Python 3 versions will work
+
+Getting started
+---------------
+
+To begin using Ecosystem Notebooks, you need to first install Jupyter
+Notebook.
+
+This can be done by running the configure_jupyter.sh shell script. In
+addition, recommended styling options can be added by running the
+configure_jupyter_styling.sh shell script. While this is not required,
+you are welcome to play around with it to personalise the Ecosystem
+workbench style.
+
+To install the relevant python code, add the parent directory
+(ecosystem-notebooks) to the PYTHONPATH environment variable.
+
+Once Jupyter is installed, enter the directory containing the notebooks.
+At the designated .ipynb extension, run the command:
+
+.. code:: bash
+
+   jupyter notebook
+
+This will open up a default web browser to the Jupyter Notebook landing
+page from which you can open up one of the desired notebooks.
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/jupyter_landing_page.png?raw=true
+   :alt: Jupyter Landing Page
+
+   Jupyter Landing Page
+
+How does Ecosystem Notebooks work
+---------------------------------
+
+From within a chosen notebook, Ecosystem Notebooks can be used. This
+coding environment, from which you can edit and run live code, provides
+the interface with which to utilise the API endpoints for Ecosystem
+Prediction and Runtime servers.For easy navigation within any of the
+notebooks, you can use the table of contents which will be situated on
+the left.
+
+In order for the API endpoints to properly function, you will need to
+login. Depending on which notebooks you have chosen to use, logging in
+could require a URL endpoint. Or a username, password and URL
+combination, which will generate an authentication token. This token
+will activate the API, then you can begin using Ecosystem Notebooks!
+
+.. figure::
+   https://github.com/ecosystemai/ecosystem-notebooks/blob/master/docs/images/login.png?raw=true
+   :alt: Login
+
+   Login
+
+Ecosystem Notebooks contains all the available API endpoints on the
+Ecosystem Servers. You can either play around in the ecosystem
+environment, or you can use it in your own chosen infrastructure.
```

### Comparing `ecosystem-notebooks-0.1.5/ecosystem_notebooks.egg-info/SOURCES.txt` & `ecosystem-notebooks-0.1.6/ecosystem_notebooks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 prediction/request_utils.py
 prediction/apis/__init__.py
 prediction/apis/algorithm_client_pulse.py
 prediction/apis/auth_controller.py
 prediction/apis/data_ingestion_engine.py
 prediction/apis/data_management_engine.py
 prediction/apis/data_munging_engine.py
+prediction/apis/deployment_management.py
 prediction/apis/ecosystem_generation_engine.py
 prediction/apis/ecosystem_home.py
 prediction/apis/ecosystem_main.py
 prediction/apis/ecosystem_user_profiles.py
 prediction/apis/functions.py
 prediction/apis/interactions.py
+prediction/apis/online_learning_management.py
 prediction/apis/prediction_engine.py
 prediction/apis/quickflat.py
 prediction/apis/settings_controller.py
 prediction/apis/transaction_categorization.py
 prediction/apis/user_controller.py
 prediction/apis/utilities.py
 prediction/apis/worker_aws.py
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/algorithm_client_pulse.py` & `ecosystem-notebooks-0.1.6/prediction/apis/algorithm_client_pulse.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from prediction.endpoints import algorithm_client_pulse as endpoints
-from prediction import request_utils
-
-def get_timeline(auth, user, limit, info=False):
-# Get Timeline:
-#   auth: Authentication token generated by jwt_access.Authenticate()
-#   user: User name (string)
-#   limit: Output limit (int)
-	ep = endpoints.GET_TIMELINE
-	param_dict = {
-		"user": user, 
-		"limit": limit
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_basket(auth, dbcust, colcust, searchcust, custfield, dbitem, colitem, itemfield, supportcount, info=False):
-# Process Basket:
-#   auth: Authentication token generated by jwt_access.Authenticate()
-#   dbcust: (str)
-#   colcust: (str)
-#   searchcust: (str)
-#   custfield: (str)
-#   dbitem: (str)
-#   colitem: (str)
-#   itemfield: (str)
-#   supportcount: (int)
-	ep = endpoints.PROCESS_BASKET
-	param_dict = {
-		"dbCust": dbcust, 
-		"colCust": colcust,
-		"searchCust": searchcust,
-		"custField": custfield,
-		"dbItem": dbitem,
-		"colItem": colitem,
-		"itemField": itemfield,
-		"supportCount": supportcount
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_directed_graph(auth, graphMeta, graphParam, info=False):
-# Analyze graph from data using graph meta data and analysis parameters. 
-# Meta data format example: {"vertex":[0,1],"edges":[{"from":0,"to":1}],"from":0,"source":"/data/data.csv","dotfile":"/data/data.dot","to":1} Analysis parameter example: {"destination":"Bakeries","source":"12345678"} 
-# Columns in file start at 0 and is sequenced.
-#   auth: Authentication token generated by jwt_access.Authenticate()
-#   graphMeta: (str)
-#   graphParam: (str)
-	ep = endpoints.PROCESS_BASKET
-	param_dict = {
-		"graphMeta": graphMeta, 
-		"graphParam": graphParam
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-
-def generate_forecast(auth, attribute, collection, collectionOut, database, dateattribute, find, historicsteps, steps, info=False):
-	ep = endpoints.GENERATE_FORECAST
-	param_dict = {
-		"attribute": attribute,
-		"collection": collection,
-		"collectionOut": collectionOut,
-		"database": database,
-		"dateattribute": dateattribute,
-		"find": find,
-		"historicsteps": historicsteps,
-		"steps": steps
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_apriori(auth, colItem, collection, collectionOut, custField, database, dbItem, find, itemField, supportCount, info=False):
-	ep = endpoints.PROCESS_APRIORI
-	param_dict = {
-		"colItem": colItem,
-		"collection": collection,
-		"collectionOut": collectionOut,
-		"custField": custField,
-		"database": database,
-		"dbItem": dbItem,
-		"find": find,
-		"itemField": itemField,
-		"supportCount": supportCount
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_ecogenetic_network(auth, collection, collectionOut, database, find, graphMeta, graphParam, info=False):
-	ep = endpoints.PROCESS_ECOGENETIC_NETWORK
-	param_dict = {
-		"collection": collection,
-		"collectionOut": collectionOut,
-		"database": database,
-		"find": find,
-		"graphMeta": graphMeta,
-		"graphParam": graphParam
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_directed_graph2(auth, db, collection, collection_out, graphMeta, graphParam, info=False):
-# Analyze graph from data using graph meta data and analysis parameters. 
-# Meta data format example: {"vertex":[0,1],"edges":[{"from":0,"to":1}],"from":0,"source":"/data/data.csv","dotfile":"/data/data.dot","to":1} Analysis parameter example: {"destination":"Bakeries","source":"12345678"} 
-# Columns in file start at 0 and is sequenced.
-#   auth: Authentication token generated by jwt_access.Authenticate()
-#   graphMeta: (str)
-#   graphParam: (str)
-	ep = endpoints.PROCESS_DIRECTED_GRAPH2
-	param_dict = {
-		"database": db,
-		"collection": collection,
-		"collectionOut": collection_out,
-		"graphMeta": graphMeta,
-		"graphParam": graphParam
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def generate_cox_ph_data(auth, collection, collection_out, customer_field, database, database_out, date_field, find, info=False):
-	ep = endpoints.GENERATE_COX_PH_DATA
-	param_dict = {
-		"collection": collection, 
-		"collectionOut": collection_out,
-		"customer_field": customer_field,
-		"database": database,
-		"databaseOut": database_out,
-		"date_field": date_field,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_arima_forecast(auth, json, info=False):
-	ep = endpoints.PROCESS_ARIMA_FORECAST
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	response = resp.json()
-	return response
-
-
-
-def list_pulse_responder_dynamic(auth, info=False):
-	ep = endpoints.LIST_PULSE_RESPONDER_DYNAMIC
-	resp = request_utils.create(auth, ep, info=info)
-	result = resp.json()
-	return result
-
-def delete_pulse_responder_dynamic(auth, db, collection, find, info=False):
-	ep = endpoints.DELETE_PULSE_RESPONDER_DYNAMIC
-	param_dict = {
-		"database": db,
-		"collection": collection,
-		"find": find,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_pulse_responder_messages(auth, db, collection, info=False):
-	ep = endpoints.GET_PULSE_RESPONDER_MESSAGES
-	param_dict = {
-		"database": db,
-		"collection": collection,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_pulse_responder_options(auth, params, info=False):
-	ep = endpoints.GET_PULSE_RESPONDER_OPTIONS
-	param_dict = {
-		"params": params,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_pulse_responder_profile(auth, db, collection, info=False):
-	ep = endpoints.GET_PULSE_RESPONDER_PROFILE
-	param_dict = {
-		"database": db,
-		"collection": collection,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def update_client_pulse_responder(auth, json, info=False):
-	ep = endpoints.UPDATE_CLIENT_PULSE_RESPONDER
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	response = resp.json()
-	return response
-
-def save_pulse_responder_dynamic(auth, json, info=False):
-	ep = endpoints.SAVE_PULSE_RESPONDER_DYNAMIC
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	response = resp.json()
+from prediction.endpoints import algorithm_client_pulse as endpoints
+from prediction import request_utils
+
+def get_timeline(auth, user, limit, info=False):
+# Get Timeline:
+#   auth: Authentication token generated by jwt_access.Authenticate()
+#   user: User name (string)
+#   limit: Output limit (int)
+	ep = endpoints.GET_TIMELINE
+	param_dict = {
+		"user": user, 
+		"limit": limit
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_basket(auth, dbcust, colcust, searchcust, custfield, dbitem, colitem, itemfield, supportcount, info=False):
+# Process Basket:
+#   auth: Authentication token generated by jwt_access.Authenticate()
+#   dbcust: (str)
+#   colcust: (str)
+#   searchcust: (str)
+#   custfield: (str)
+#   dbitem: (str)
+#   colitem: (str)
+#   itemfield: (str)
+#   supportcount: (int)
+	ep = endpoints.PROCESS_BASKET
+	param_dict = {
+		"dbCust": dbcust, 
+		"colCust": colcust,
+		"searchCust": searchcust,
+		"custField": custfield,
+		"dbItem": dbitem,
+		"colItem": colitem,
+		"itemField": itemfield,
+		"supportCount": supportcount
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_directed_graph(auth, graphMeta, graphParam, info=False):
+# Analyze graph from data using graph meta data and analysis parameters. 
+# Meta data format example: {"vertex":[0,1],"edges":[{"from":0,"to":1}],"from":0,"source":"/data/data.csv","dotfile":"/data/data.dot","to":1} Analysis parameter example: {"destination":"Bakeries","source":"12345678"} 
+# Columns in file start at 0 and is sequenced.
+#   auth: Authentication token generated by jwt_access.Authenticate()
+#   graphMeta: (str)
+#   graphParam: (str)
+	ep = endpoints.PROCESS_BASKET
+	param_dict = {
+		"graphMeta": graphMeta, 
+		"graphParam": graphParam
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+
+def generate_forecast(auth, attribute, collection, collectionOut, database, dateattribute, find, historicsteps, steps, info=False):
+	ep = endpoints.GENERATE_FORECAST
+	param_dict = {
+		"attribute": attribute,
+		"collection": collection,
+		"collectionOut": collectionOut,
+		"database": database,
+		"dateattribute": dateattribute,
+		"find": find,
+		"historicsteps": historicsteps,
+		"steps": steps
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_apriori(auth, colItem, collection, collectionOut, custField, database, dbItem, find, itemField, supportCount, info=False):
+	ep = endpoints.PROCESS_APRIORI
+	param_dict = {
+		"colItem": colItem,
+		"collection": collection,
+		"collectionOut": collectionOut,
+		"custField": custField,
+		"database": database,
+		"dbItem": dbItem,
+		"find": find,
+		"itemField": itemField,
+		"supportCount": supportCount
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_ecogenetic_network(auth, collection, collectionOut, database, find, graphMeta, graphParam, info=False):
+	ep = endpoints.PROCESS_ECOGENETIC_NETWORK
+	param_dict = {
+		"collection": collection,
+		"collectionOut": collectionOut,
+		"database": database,
+		"find": find,
+		"graphMeta": graphMeta,
+		"graphParam": graphParam
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_directed_graph2(auth, db, collection, collection_out, graphMeta, graphParam, info=False):
+# Analyze graph from data using graph meta data and analysis parameters. 
+# Meta data format example: {"vertex":[0,1],"edges":[{"from":0,"to":1}],"from":0,"source":"/data/data.csv","dotfile":"/data/data.dot","to":1} Analysis parameter example: {"destination":"Bakeries","source":"12345678"} 
+# Columns in file start at 0 and is sequenced.
+#   auth: Authentication token generated by jwt_access.Authenticate()
+#   graphMeta: (str)
+#   graphParam: (str)
+	ep = endpoints.PROCESS_DIRECTED_GRAPH2
+	param_dict = {
+		"database": db,
+		"collection": collection,
+		"collectionOut": collection_out,
+		"graphMeta": graphMeta,
+		"graphParam": graphParam
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def generate_cox_ph_data(auth, collection, collection_out, customer_field, database, database_out, date_field, find, info=False):
+	ep = endpoints.GENERATE_COX_PH_DATA
+	param_dict = {
+		"collection": collection, 
+		"collectionOut": collection_out,
+		"customer_field": customer_field,
+		"database": database,
+		"databaseOut": database_out,
+		"date_field": date_field,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_arima_forecast(auth, json, info=False):
+	ep = endpoints.PROCESS_ARIMA_FORECAST
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	response = resp.json()
+	return response
+
+
+
+def list_pulse_responder_dynamic(auth, info=False):
+	ep = endpoints.LIST_PULSE_RESPONDER_DYNAMIC
+	resp = request_utils.create(auth, ep, info=info)
+	result = resp.json()
+	return result
+
+def delete_pulse_responder_dynamic(auth, db, collection, find, info=False):
+	ep = endpoints.DELETE_PULSE_RESPONDER_DYNAMIC
+	param_dict = {
+		"database": db,
+		"collection": collection,
+		"find": find,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_pulse_responder_messages(auth, db, collection, info=False):
+	ep = endpoints.GET_PULSE_RESPONDER_MESSAGES
+	param_dict = {
+		"database": db,
+		"collection": collection,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_pulse_responder_options(auth, params, info=False):
+	ep = endpoints.GET_PULSE_RESPONDER_OPTIONS
+	param_dict = {
+		"params": params,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_pulse_responder_profile(auth, db, collection, info=False):
+	ep = endpoints.GET_PULSE_RESPONDER_PROFILE
+	param_dict = {
+		"database": db,
+		"collection": collection,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def update_client_pulse_responder(auth, json, info=False):
+	ep = endpoints.UPDATE_CLIENT_PULSE_RESPONDER
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	response = resp.json()
+	return response
+
+def save_pulse_responder_dynamic(auth, json, info=False):
+	ep = endpoints.SAVE_PULSE_RESPONDER_DYNAMIC
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	response = resp.json()
 	return response
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.6/prediction/apis/data_ingestion_engine.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from prediction.endpoints import data_ingestion_engine as endpoints
-from prediction import request_utils
-
-def add_metadocumemnts(auth, meta_documents, info=False):
-    ep = endpoints.ADD_META_DOCUMENTS
-    resp = request_utils.create(auth, ep, json=meta_documents, info=info)
-    response = resp.json()
-    return response
-
-def delete_ingestmeta(auth, ingest_meta, info=False):
-    ep = endpoints.DELETE_INGEST_META
-    resp = request_utils.create(auth, ep, json=ingest_meta, info=info)
-    response = resp.json()
-    return response	
-
-def get_databasesmeta(auth, info=False):
-    ep = endpoints.GET_DATABASES_META
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def get_databasetablecolumnmeta(auth, databasename, tablename, columnname, info=False):
-    ep = endpoints.GET_DATABASE_TABLE_COLUMN_META
-    param_dict = {
-        "databasename": databasename,
-        "tablename": tablename,
-        "columnname": columnname
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def get_databasetablecolumnsmeta(auth, databasename, tablename, info=False):
-    ep = endpoints.GET_DATABASE_TABLE_COLUMNS_META
-    param_dict = {"databasename": databasename, "tablename": tablename}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def get_databasetablesmeta(auth, databasename, info=False):
-    ep = endpoints.GET_DATABASES_TABLES_META
-    param_dict = {"databasename": databasename}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def get_ingestmeta(auth, ingest_name, info=False):
-    ep = endpoints.GET_INGEST_META
-    param_dict = {"ingest_name": ingest_name}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def get_ingestmetas(auth, info=False):
-    ep = endpoints.GET_INGEST_METAS
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
-    if "data" in meta:
-        meta = meta["data"]
-    return meta
-
-def save_databasetablecolumn(auth, database_table_column_json, info=False):
-    ep = endpoints.SAVE_DATABASE_TABLE_COLUMN_META
-    resp = request_utils.create(auth, ep, json=database_table_column_json, info=info)
-    response = resp.json()
-    return response
-
-def save_ingestion(auth, ingestion_json, info=False):
-    ep = endpoints.SAVE_INGEST_META
-    resp = request_utils.create(auth, ep, json=ingestion_json, info=info)
-    response = resp.json()
+from prediction.endpoints import data_ingestion_engine as endpoints
+from prediction import request_utils
+
+def add_metadocumemnts(auth, meta_documents, info=False):
+    ep = endpoints.ADD_META_DOCUMENTS
+    resp = request_utils.create(auth, ep, json=meta_documents, info=info)
+    response = resp.json()
+    return response
+
+def delete_ingestmeta(auth, ingest_meta, info=False):
+    ep = endpoints.DELETE_INGEST_META
+    resp = request_utils.create(auth, ep, json=ingest_meta, info=info)
+    response = resp.json()
+    return response	
+
+def get_databasesmeta(auth, info=False):
+    ep = endpoints.GET_DATABASES_META
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def get_databasetablecolumnmeta(auth, databasename, tablename, columnname, info=False):
+    ep = endpoints.GET_DATABASE_TABLE_COLUMN_META
+    param_dict = {
+        "databasename": databasename,
+        "tablename": tablename,
+        "columnname": columnname
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def get_databasetablecolumnsmeta(auth, databasename, tablename, info=False):
+    ep = endpoints.GET_DATABASE_TABLE_COLUMNS_META
+    param_dict = {"databasename": databasename, "tablename": tablename}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def get_databasetablesmeta(auth, databasename, info=False):
+    ep = endpoints.GET_DATABASES_TABLES_META
+    param_dict = {"databasename": databasename}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def get_ingestmeta(auth, ingest_name, info=False):
+    ep = endpoints.GET_INGEST_META
+    param_dict = {"ingest_name": ingest_name}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def get_ingestmetas(auth, info=False):
+    ep = endpoints.GET_INGEST_METAS
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
+    if "data" in meta:
+        meta = meta["data"]
+    return meta
+
+def save_databasetablecolumn(auth, database_table_column_json, info=False):
+    ep = endpoints.SAVE_DATABASE_TABLE_COLUMN_META
+    resp = request_utils.create(auth, ep, json=database_table_column_json, info=info)
+    response = resp.json()
+    return response
+
+def save_ingestion(auth, ingestion_json, info=False):
+    ep = endpoints.SAVE_INGEST_META
+    resp = request_utils.create(auth, ep, json=ingestion_json, info=info)
+    response = resp.json()
     return response
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/data_management_engine.py` & `ecosystem-notebooks-0.1.6/prediction/apis/data_management_engine.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-from prediction.endpoints import data_management_engine as endpoints
-from prediction import request_utils
-
-# Data Management Engine
-def get_document_db_aggregate2(auth, database, collection, aggregate, field, limit, projections, skip, sort, info=False):
-	ep = endpoints.GET_MONGO_DB_AGGREGATE2
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"aggregate": aggregate,
-		"field": field,
-		"limit": limit,
-		"projections": projections,
-		"skip": skip,
-		"sort": sort
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def add_document_collection(auth, database, collection, info=False):
-	ep = endpoints.ADD_MONGO_COLLECTION
-	param_dict = {
-		"database": database, 
-		"collection": collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def add_document_database(auth, database, info=False):
-	ep = endpoints.ADD_MONGO_DATABASE
-	param_dict = {
-		"database": database
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def add_documents(auth, json, info=False):
-	ep = endpoints.ADD_MONGO_DOCUMENTS
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def csv_file_to_json(auth, csv_file, json_file, info=False):
-	ep = endpoints.CSV_FILE_TO_JSON
-	param_dict = {
-		"csv_file": csv_file,
-		"json_file": json_file
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def csv_import(auth, database, collection, csv_file, info=False):
-	ep = endpoints.CSV_FILE_TO_MONGO_DB_IMPORT
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"csv_file": csv_file
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def csv_import2(auth, database, collection, csv_file, headerline, import_type, info=False):
-	ep = endpoints.CSV_FILE_TO_MONGO_DB_IMPORT2
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"csv_file": csv_file,
-		"headerline": headerline,
-		"type": import_type
-
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def delete_all_documents(auth, doc_json, info=False):
-	ep = endpoints.DELETE_ALL_MONGO_DOCUMENTS
-	resp = request_utils.create(auth, ep, json=doc_json, info=info)
-	response = resp.json()
-	return response
-
-def delete_documents(auth, doc_json, info=False):
-	ep = endpoints.DELETE_MONGO_DOCUMENTS
-	resp = request_utils.create(auth, ep, json=doc_json, info=info)
-	response = resp.json()
-	return response
-
-def drop_document_collection(auth, database, collection, info=False):
-	ep = endpoints.DROP_MONGO_COLLECTION
-	param_dict = {
-		"database": database, 
-		"collection": collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def drop_document_collection_index(auth, database, collection, index, info=False):
-	ep = endpoints.DROP_MONGO_COLLECTION_INDEX
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"index": index
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def drop_document_database(auth, database, info=False):
-	ep = endpoints.DROP_MONGO_DATABASE
-	param_dict = {
-		"database": database
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def dump_document_database(auth, database, collection, folder, option, info=False):
-	ep = endpoints.DUMP_MONGO_DATABASE
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"folder": folder,
-		"option": option
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def export_documents(auth, filename, filetype, database, collection, field, sort, projection, limit, info=False):
-	ep = endpoints.EXPORT_MONGO_DOCUMENTS 
-	param_dict = {
-		"file_name": filename,
-		"file_type": filetype,
-		"database": database, 
-		"collection": collection,
-		"field": field,
-		"sort": sort,
-		"projection": projection,
-		"limit": limit
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def get_document_collection_indexes(auth, database, collection, info=False):
-	ep = endpoints.GET_MONGO_COLLECTION_INDEXES
-	param_dict = {
-		"database": database, 
-		"collection": collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_data_aggregate(auth, database, collection, field, projections, aggregate, sort, info=False):
-	ep = endpoints.GET_MONGO_DB_AGGREGATE 
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"field": field,
-		"projections": projections,
-		"aggregate": aggregate,
-		"sort": sort
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-	
-def get_document_db_collections(auth, database, info=False):
-	ep = endpoints.GET_MONGO_DB_COLLECTIONS
-	param_dict = {
-		"database": database
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_document_db_collection_stats(auth, database, collection, info=False):
-	ep = endpoints.GET_MONGO_DB_COLLECTION_STATS
-	param_dict = {
-		"database": database, 
-		"collection": collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_data(auth, database, collection, field, limit, projections, skip, info=False):
-	ep = endpoints.GET_MONGO_DB_FIND
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"field": field,
-		"limit": limit,
-		"projections": projections, 
-		"skip": skip
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	if "data" in meta:
-		meta = meta["data"]
-	return meta
-	
-def get_document_db_find_labels(auth, database, collection, field, projections, skip, info=False):
-	ep = endpoints.GET_MONGO_DB_FIND_LABELS
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"field": field,
-		"projections": projections, 
-		"skip": skip
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	if "data" in meta:
-		meta = meta["data"]
-	return meta
-
-def get_data_sort(auth, database, collection, field, limit, projections, skip, sort, info=False):
-	ep = endpoints.GET_MONGO_DB_FIND_SORT
-	param_dict = {
-		"database": database, 
-		"collection": collection,
-		"field": field,
-		"limit": limit,
-		"projections": projections, 
-		"skip": skip,
-		"sort": sort
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	if "data" in meta:
-		meta = meta["data"]
-	return meta
-
-def get_document_db_list(auth, server=None, info=False):
-	ep = endpoints.GET_MONGO_DB_LIST
-	if server == None:
-		server = auth.get_server()
-	param_dict = {
-		"server": server
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	if "data" in meta:
-		meta = meta["data"]
-	return meta
-
-def import_documents(auth, database, collection, file_name, file_type, info=False):
-	ep = endpoints.IMPORT_MONGO_DOCUMENTS
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"file_name": file_name,
-		"file_type": file_type
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def restore_document_database(auth, database, collection, folder, info=False):
-	ep = endpoints.RESTORE_MONGO_DATABASE
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"folder": folder
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def create_document_collection_index(auth, database, collection, index, info=False):
-	ep = endpoints.CREATE_MONGO_COLLECTION_INDEX
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"index": index
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def post_mongo_db_aggregate_pipeline(auth, json, info=False):
-	ep = endpoints.POST_MONGO_DB_AGGREGATE_PIPELINE
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def rename_collection(auth, database, collection, new_collection, info=False):
-	ep = endpoints.RENAME_COLLECTION
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"new_collection": new_collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def update_key_name(auth, database, collection, find, from_key, to_key, info=False):
-	ep = endpoints.UPDATE_KEY_NAME
-	param_dict = {
-		"database": database,
-		"collection": collection,
-		"find": find,
-		"from": from_key,
-		"to": to_key
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_document_labels(auth, database, collection, info=False):
-	ep = endpoints.GET_MONGO_DOCUMENT_LABELS
-	param_dict = {
-		"database": database,
-		"collection": collection
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def execute_mongo_db_script(auth, json, info=False):
-	ep = endpoints.EXECUTE_MONGO_DB_SCRIPT
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-# # Data Management Engine: Cassandra
-# def get_cassandra_sql(auth, sql, info=False):
-# 	ep = endpoints.GET_CASSANDRA_SQL
-# 	param_dict = {
-# 		"sql": sql
-# 	}
-# 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-# 	result = resp.json()
-# 	return result
-
-# Data Management Engine: Presto
-def create_presto_sql(auth, connection, sql, info=False):
-	ep = endpoints.CREATE_PRESTO_SQL
-	param_dict = {
-		"connection": connection,
-		"sql": sql
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_presto_sql(auth, connection, sql, info=False):
-	ep = endpoints.GET_PRESTO_SQL
-	param_dict = {
-		"connection": connection,
-		"sql": sql
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
+from prediction.endpoints import data_management_engine as endpoints
+from prediction import request_utils
+
+# Data Management Engine
+def get_document_db_aggregate2(auth, database, collection, aggregate, field, limit, projections, skip, sort, info=False):
+	ep = endpoints.GET_MONGO_DB_AGGREGATE2
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"aggregate": aggregate,
+		"field": field,
+		"limit": limit,
+		"projections": projections,
+		"skip": skip,
+		"sort": sort
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def add_document_collection(auth, database, collection, info=False):
+	ep = endpoints.ADD_MONGO_COLLECTION
+	param_dict = {
+		"database": database, 
+		"collection": collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def add_document_database(auth, database, info=False):
+	ep = endpoints.ADD_MONGO_DATABASE
+	param_dict = {
+		"database": database
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def add_documents(auth, json, info=False):
+	ep = endpoints.ADD_MONGO_DOCUMENTS
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def csv_file_to_json(auth, csv_file, json_file, info=False):
+	ep = endpoints.CSV_FILE_TO_JSON
+	param_dict = {
+		"csv_file": csv_file,
+		"json_file": json_file
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def csv_import(auth, database, collection, csv_file, info=False):
+	ep = endpoints.CSV_FILE_TO_MONGO_DB_IMPORT
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"csv_file": csv_file
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def csv_import2(auth, database, collection, csv_file, headerline, import_type, info=False):
+	ep = endpoints.CSV_FILE_TO_MONGO_DB_IMPORT2
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"csv_file": csv_file,
+		"headerline": headerline,
+		"type": import_type
+
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def delete_all_documents(auth, doc_json, info=False):
+	ep = endpoints.DELETE_ALL_MONGO_DOCUMENTS
+	resp = request_utils.create(auth, ep, json=doc_json, info=info)
+	response = resp.json()
+	return response
+
+def delete_documents(auth, doc_json, info=False):
+	ep = endpoints.DELETE_MONGO_DOCUMENTS
+	resp = request_utils.create(auth, ep, json=doc_json, info=info)
+	response = resp.json()
+	return response
+
+def drop_document_collection(auth, database, collection, info=False):
+	ep = endpoints.DROP_MONGO_COLLECTION
+	param_dict = {
+		"database": database, 
+		"collection": collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def drop_document_collection_index(auth, database, collection, index, info=False):
+	ep = endpoints.DROP_MONGO_COLLECTION_INDEX
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"index": index
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def drop_document_database(auth, database, info=False):
+	ep = endpoints.DROP_MONGO_DATABASE
+	param_dict = {
+		"database": database
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def dump_document_database(auth, database, collection, folder, option, info=False):
+	ep = endpoints.DUMP_MONGO_DATABASE
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"folder": folder,
+		"option": option
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def export_documents(auth, filename, filetype, database, collection, field, sort, projection, limit, info=False):
+	ep = endpoints.EXPORT_MONGO_DOCUMENTS 
+	param_dict = {
+		"file_name": filename,
+		"file_type": filetype,
+		"database": database, 
+		"collection": collection,
+		"field": field,
+		"sort": sort,
+		"projection": projection,
+		"limit": limit
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def get_document_collection_indexes(auth, database, collection, info=False):
+	ep = endpoints.GET_MONGO_COLLECTION_INDEXES
+	param_dict = {
+		"database": database, 
+		"collection": collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_data_aggregate(auth, database, collection, field, projections, aggregate, sort, info=False):
+	ep = endpoints.GET_MONGO_DB_AGGREGATE 
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"field": field,
+		"projections": projections,
+		"aggregate": aggregate,
+		"sort": sort
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+	
+def get_document_db_collections(auth, database, info=False):
+	ep = endpoints.GET_MONGO_DB_COLLECTIONS
+	param_dict = {
+		"database": database
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_document_db_collection_stats(auth, database, collection, info=False):
+	ep = endpoints.GET_MONGO_DB_COLLECTION_STATS
+	param_dict = {
+		"database": database, 
+		"collection": collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_data(auth, database, collection, field, limit, projections, skip, info=False):
+	ep = endpoints.GET_MONGO_DB_FIND
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"field": field,
+		"limit": limit,
+		"projections": projections, 
+		"skip": skip
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	if "data" in meta:
+		meta = meta["data"]
+	return meta
+	
+def get_document_db_find_labels(auth, database, collection, field, projections, skip, info=False):
+	ep = endpoints.GET_MONGO_DB_FIND_LABELS
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"field": field,
+		"projections": projections, 
+		"skip": skip
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	if "data" in meta:
+		meta = meta["data"]
+	return meta
+
+def get_data_sort(auth, database, collection, field, limit, projections, skip, sort, info=False):
+	ep = endpoints.GET_MONGO_DB_FIND_SORT
+	param_dict = {
+		"database": database, 
+		"collection": collection,
+		"field": field,
+		"limit": limit,
+		"projections": projections, 
+		"skip": skip,
+		"sort": sort
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	if "data" in meta:
+		meta = meta["data"]
+	return meta
+
+def get_document_db_list(auth, server=None, info=False):
+	ep = endpoints.GET_MONGO_DB_LIST
+	if server == None:
+		server = auth.get_server()
+	param_dict = {
+		"server": server
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	if "data" in meta:
+		meta = meta["data"]
+	return meta
+
+def import_documents(auth, database, collection, file_name, file_type, info=False):
+	ep = endpoints.IMPORT_MONGO_DOCUMENTS
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"file_name": file_name,
+		"file_type": file_type
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def restore_document_database(auth, database, collection, folder, info=False):
+	ep = endpoints.RESTORE_MONGO_DATABASE
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"folder": folder
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def create_document_collection_index(auth, database, collection, index, info=False):
+	ep = endpoints.CREATE_MONGO_COLLECTION_INDEX
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"index": index
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def post_mongo_db_aggregate_pipeline(auth, json, info=False):
+	ep = endpoints.POST_MONGO_DB_AGGREGATE_PIPELINE
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def rename_collection(auth, database, collection, new_collection, info=False):
+	ep = endpoints.RENAME_COLLECTION
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"new_collection": new_collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def update_key_name(auth, database, collection, find, from_key, to_key, info=False):
+	ep = endpoints.UPDATE_KEY_NAME
+	param_dict = {
+		"database": database,
+		"collection": collection,
+		"find": find,
+		"from": from_key,
+		"to": to_key
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_document_labels(auth, database, collection, info=False):
+	ep = endpoints.GET_MONGO_DOCUMENT_LABELS
+	param_dict = {
+		"database": database,
+		"collection": collection
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def execute_mongo_db_script(auth, json, info=False):
+	ep = endpoints.EXECUTE_MONGO_DB_SCRIPT
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+# # Data Management Engine: Cassandra
+# def get_cassandra_sql(auth, sql, info=False):
+# 	ep = endpoints.GET_CASSANDRA_SQL
+# 	param_dict = {
+# 		"sql": sql
+# 	}
+# 	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+# 	result = resp.json()
+# 	return result
+
+# Data Management Engine: Presto
+def create_presto_sql(auth, connection, sql, info=False):
+	ep = endpoints.CREATE_PRESTO_SQL
+	param_dict = {
+		"connection": connection,
+		"sql": sql
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_presto_sql(auth, connection, sql, info=False):
+	ep = endpoints.GET_PRESTO_SQL
+	param_dict = {
+		"connection": connection,
+		"sql": sql
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/data_munging_engine.py` & `ecosystem-notebooks-0.1.6/prediction/apis/data_munging_engine.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,418 +1,418 @@
-from prediction.endpoints import data_munging_engine as endpoints
-from prediction import request_utils
-# from prediction.apis import quickflat as qf
-
-def concat_columns2(auth, database, collection, attribute, separator, info=False):
-	ep = endpoints.CONCAT_COLUMNS2
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"separator": separator
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_date2(auth, database, collection, attribute, find, info=False):
-	ep = endpoints.DATE_ENRICH2
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def auto_normalize_all(auth, database, collection, fields, find, normalized_high, normalized_low, info=False):
-	ep = endpoints.AUTO_NORMALIZE_ALL
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"fields": fields,
-		"find": find,
-		"normalizedHigh": normalized_high,
-		"normalizedLow": normalized_low
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def concat_columns(auth, databasename, collection, attribute, info=False):
-	ep = endpoints.CONCAT_COLUMNS
-	param_dict = {"mongodb": databasename, "collection": collection, "attribute": attribute}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_date(auth, database, collection, attribute, info=False):
-	ep = endpoints.DATE_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enum_convert(auth, database, collection, attribute, info=False):
-	ep = endpoints.ENUM_CONVERT
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def fill_zeros(auth, database, collection, attribute, info=False):
-	ep = endpoints.FILL_ZEROS
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def fill_values(auth, database, collection, find, attribute, value, info=False):
-	ep = endpoints.FILL_VALUES
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"find": find,
-		"attribute": attribute,
-		"value": value
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-
-def foreign_key_aggregator(auth, database, collection, attribute, search, mongodbf, collectionf, attributef, fields, info=False):
-	ep = endpoints.FOREIGN_KEY_AGGREGATOR
-	param_dict = {
-		"mongodb": database,
-		"collection": collection,
-		"attribute": attribute,
-		"search": search,
-		"mongodbf": mongodbf,
-		"collectionf": collectionf,
-		"attributef": attributef,
-		"fields": fields
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def foreign_key_lookup(auth, database, collection, attribute, search, mongodbf, collectionf, attributef, fields, info=False):
-	ep = endpoints.FOREIGN_KEY_LOOKUP
-	param_dict = {
-		"mongodb": database,
-		"collection": collection,
-		"attribute": attribute,
-		"search": search,
-		"mongodbf": mongodbf,
-		"collectionf": collectionf,
-		"attributef": attributef,
-		"fields": fields
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_fragments(auth, database, collection, attribute, strings, info=False):
-	ep = endpoints.FRAGMENT_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"stringOnly": strings
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_fragments2(auth, database, collection, attribute, strings, find, info=False):
-	ep = endpoints.FRAGMENT_ENRICH2
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"stringOnly": strings,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def generate_features(auth, database, collection, featureset, categoryfield, datefield, numfield, groupby, find, info=False):
-	ep = endpoints.GENERATE_FEATURES
-	param_dict = {"database": database, "collection": collection, "featureset":featureset, "categoryfield":categoryfield, "datefield":datefield, "numfield":numfield, "groupby":groupby, "find":find}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def generate_features_normalize(auth, database, collection, find, inplace, normalized_high, normalized_low, numfields, info=False):
-	ep = endpoints.GENERATE_FEATURES_NORMALIZE
-	param_dict = {"database": database, "collection": collection, "find":find, "inPlace": inplace, "normalizedHigh": normalized_high, "normalizedLow": normalized_low, "numfields": numfields}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def get_categories(auth, database, collection, categoryfield, find, total, info=False):
-	ep = endpoints.GET_CATEGORIES
-	param_dict = {"database": database, "collection":collection, "categoryfield":categoryfield, "total": total, "find": find}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def get_categories_ratio(auth, database, collection, categoryfield, find, total, info=False):
-	ep = endpoints.GET_CATEGORIES_RATIOS
-	param_dict = {"database": database, "collection":collection, "categoryfield":categoryfield, "total": total, "find": find}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_location(auth, database, collection, attribute, info=False):
-	ep = endpoints.LOCATION_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_mcc(auth, database, collection, attribute, find, info=False):
-	ep = endpoints.MCC_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def prediction_enrich_fast(auth, database, collection, search, sort, predictor, predictor_label, attributes, skip, limit, info=False):
-	ep = endpoints.PREDICTION_ENRICH_FAST_GET
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"search": search,
-		"sort": sort,
-		"predictor": predictor,
-		"predictor_label": predictor_label,
-		"attributes": attributes,
-		"skip": skip,
-		"limit": limit
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-	
-# predicition_enrich(auth, database, collection2, search, sort, predictor, predictor_label, attributes) 
-def predicition_enrich(auth, database, collection, search, sort, predictor, predictor_label, attributes, info=False):
-	ep = endpoints.PREDICTION_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"search": search,
-		"predictor": predictor,
-		"predictor_label": predictor_label,
-		"attributes": attributes,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def enrich_sic(auth, database, collection, attribute, find, info=False):
-	ep = endpoints.SIC_ENRICH
-	param_dict = {
-		"mongodb": database, 
-		"collection": collection,
-		"attribute": attribute,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-# def quickflat(config, info=False):
-# 	quick_flat = qf.QuickFlat(config)
-# 	quick_flat.flatten()
-
-def process_client_pulse_reliability(auth, collection, collectionOut, database, find, groupby, mongoAttribute, typeName, info=False):
-	ep = endpoints.PROCESS_CLIENT_PULSE_RELIABILITY
-	param_dict = {
-		"collection": collection,
-		"collectionOut": collectionOut,
-		"database": database,
-		"find": find,
-		"groupby": groupby,
-		"mongoAttribute": mongoAttribute,
-		"type": typeName
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def generate_time_series_features(auth, categoryfield, collection, database, datefield, featureset, find, groupby, numfield, startdate=None, windowsize=1, info=False):
-	ep = endpoints.GENERATE_TIME_SERIES_FEATURES
-	param_dict = {
-		"categoryfield": categoryfield,
-		"collection": collection,
-		"database": database,
-		"datefield": datefield,
-		"featureset": featureset,
-		"find": find,
-		"groupby": groupby,
-		"numfield": numfield,
-		"startdate": startdate,
-		"windowsize": windowsize
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def personality_enrich(auth, category, collection, collectionOut, database, find, groupby, info=False):
-	ep = endpoints.PERSONALITY_ENRICH
-	param_dict = {
-		"category": category,
-		"collection": collection,
-		"collectionOut": collectionOut,
-		"database": database,
-		"find": find,
-		"groupby": groupby		
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def munge_transactions_aggregate(auth, munging_step, project_id, info=False):
-	ep = endpoints.MUNGE_TRANSACTIONS_AGGREGATE
-	param_dict = {
-		"munging_step": munging_step,
-		"project_id": project_id
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def munge_transactions(auth, munging_step, project_id, info=False):
-	ep = endpoints.MUNGE_TRANSACTIONS
-	param_dict = {
-		"munging_step": munging_step,
-		"project_id": project_id
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def flatten_document(auth, db, collection, attribute, find, info=False):
-	ep = endpoints.FLATTEN_DOCUMENT
-	param_dict = {
-		"mongodb": db,
-		"collection": collection,
-		"attribute": attribute,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def delete_key(auth, db, collection, attribute, find, info=False):
-	ep = endpoints.DELETE_KEY
-	param_dict = {
-		"mongodb": db,
-		"collection": collection,
-		"attribute": attribute,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def delete_many_documents(auth, db, collection, find, info=False):
-	ep = endpoints.DELETE_MANY_DOCUMENTS
-	param_dict = {
-		"mongodb": db,
-		"collection": collection,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_range(auth, db, collection, attribute, new_attribute, find, rules, info=False):
-	ep = endpoints.PROCESS_RANGE
-	param_dict = {
-		"database": db,
-		"collection": collection,
-		"mongoAttribute": attribute,
-		"newAttribute": new_attribute,
-		"find": find,
-		"rules": rules
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def nlp_worker(auth, database, collection, database_out, collection_out, attribute, find, model="original", summarization_max=10, summarization_min=5, transformer="t5-small", model_type="nlp_b5_base", info=False):
-	ep = endpoints.NLP_WORKER
-	param_dict = {
-		"database": db,
-		"collection": collection,
-		"database_out": database_out,
-		"collection_out": collection_out,
-		"attribute": attribute,
-		"find": find,
-		"model": model,
-		"summarization_max": summarization_max,
-		"summarization_min": summarization_min,
-		"transformer": transformer,
-		"type": model_type,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def delete_many_documents(auth, db, collection, find, info=False):
-	ep = endpoints.DELETE_MANY_DOCUMENTS
-	param_dict = {
-		"mongodb": db,
-		"collection": collection,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def process_range(auth, db, collection, find, attribute, new_attribute, rules, info=False):
-	ep = endpoints.PROCESS_RANGE
-	param_dict = {
-		"database": db,
-		"collection": collection,
-		"find": find,
-		"mongoAttribute": attribute,
-		"newAttribute": new_attribute,
-		"rules": rules
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-
-def prediction_enrich_fast_post(auth, json, info=False):
-	ep = endpoints.PREDICTION_ENRICH_FAST_POST
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
+from prediction.endpoints import data_munging_engine as endpoints
+from prediction import request_utils
+# from prediction.apis import quickflat as qf
+
+def concat_columns2(auth, database, collection, attribute, separator, info=False):
+	ep = endpoints.CONCAT_COLUMNS2
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"separator": separator
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_date2(auth, database, collection, attribute, find, info=False):
+	ep = endpoints.DATE_ENRICH2
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def auto_normalize_all(auth, database, collection, fields, find, normalized_high, normalized_low, info=False):
+	ep = endpoints.AUTO_NORMALIZE_ALL
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"fields": fields,
+		"find": find,
+		"normalizedHigh": normalized_high,
+		"normalizedLow": normalized_low
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def concat_columns(auth, databasename, collection, attribute, info=False):
+	ep = endpoints.CONCAT_COLUMNS
+	param_dict = {"mongodb": databasename, "collection": collection, "attribute": attribute}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_date(auth, database, collection, attribute, info=False):
+	ep = endpoints.DATE_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enum_convert(auth, database, collection, attribute, info=False):
+	ep = endpoints.ENUM_CONVERT
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def fill_zeros(auth, database, collection, attribute, info=False):
+	ep = endpoints.FILL_ZEROS
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def fill_values(auth, database, collection, find, attribute, value, info=False):
+	ep = endpoints.FILL_VALUES
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"find": find,
+		"attribute": attribute,
+		"value": value
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+
+def foreign_key_aggregator(auth, database, collection, attribute, search, mongodbf, collectionf, attributef, fields, info=False):
+	ep = endpoints.FOREIGN_KEY_AGGREGATOR
+	param_dict = {
+		"mongodb": database,
+		"collection": collection,
+		"attribute": attribute,
+		"search": search,
+		"mongodbf": mongodbf,
+		"collectionf": collectionf,
+		"attributef": attributef,
+		"fields": fields
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def foreign_key_lookup(auth, database, collection, attribute, search, mongodbf, collectionf, attributef, fields, info=False):
+	ep = endpoints.FOREIGN_KEY_LOOKUP
+	param_dict = {
+		"mongodb": database,
+		"collection": collection,
+		"attribute": attribute,
+		"search": search,
+		"mongodbf": mongodbf,
+		"collectionf": collectionf,
+		"attributef": attributef,
+		"fields": fields
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_fragments(auth, database, collection, attribute, strings, info=False):
+	ep = endpoints.FRAGMENT_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"stringOnly": strings
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_fragments2(auth, database, collection, attribute, strings, find, info=False):
+	ep = endpoints.FRAGMENT_ENRICH2
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"stringOnly": strings,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def generate_features(auth, database, collection, featureset, categoryfield, datefield, numfield, groupby, find, info=False):
+	ep = endpoints.GENERATE_FEATURES
+	param_dict = {"database": database, "collection": collection, "featureset":featureset, "categoryfield":categoryfield, "datefield":datefield, "numfield":numfield, "groupby":groupby, "find":find}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def generate_features_normalize(auth, database, collection, find, inplace, normalized_high, normalized_low, numfields, info=False):
+	ep = endpoints.GENERATE_FEATURES_NORMALIZE
+	param_dict = {"database": database, "collection": collection, "find":find, "inPlace": inplace, "normalizedHigh": normalized_high, "normalizedLow": normalized_low, "numfields": numfields}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def get_categories(auth, database, collection, categoryfield, find, total, info=False):
+	ep = endpoints.GET_CATEGORIES
+	param_dict = {"database": database, "collection":collection, "categoryfield":categoryfield, "total": total, "find": find}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def get_categories_ratio(auth, database, collection, categoryfield, find, total, info=False):
+	ep = endpoints.GET_CATEGORIES_RATIOS
+	param_dict = {"database": database, "collection":collection, "categoryfield":categoryfield, "total": total, "find": find}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_location(auth, database, collection, attribute, info=False):
+	ep = endpoints.LOCATION_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_mcc(auth, database, collection, attribute, find, info=False):
+	ep = endpoints.MCC_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def prediction_enrich_fast(auth, database, collection, search, sort, predictor, predictor_label, attributes, skip, limit, info=False):
+	ep = endpoints.PREDICTION_ENRICH_FAST_GET
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"search": search,
+		"sort": sort,
+		"predictor": predictor,
+		"predictor_label": predictor_label,
+		"attributes": attributes,
+		"skip": skip,
+		"limit": limit
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+	
+# predicition_enrich(auth, database, collection2, search, sort, predictor, predictor_label, attributes) 
+def predicition_enrich(auth, database, collection, search, sort, predictor, predictor_label, attributes, info=False):
+	ep = endpoints.PREDICTION_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"search": search,
+		"predictor": predictor,
+		"predictor_label": predictor_label,
+		"attributes": attributes,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def enrich_sic(auth, database, collection, attribute, find, info=False):
+	ep = endpoints.SIC_ENRICH
+	param_dict = {
+		"mongodb": database, 
+		"collection": collection,
+		"attribute": attribute,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+# def quickflat(config, info=False):
+# 	quick_flat = qf.QuickFlat(config)
+# 	quick_flat.flatten()
+
+def process_client_pulse_reliability(auth, collection, collectionOut, database, find, groupby, mongoAttribute, typeName, info=False):
+	ep = endpoints.PROCESS_CLIENT_PULSE_RELIABILITY
+	param_dict = {
+		"collection": collection,
+		"collectionOut": collectionOut,
+		"database": database,
+		"find": find,
+		"groupby": groupby,
+		"mongoAttribute": mongoAttribute,
+		"type": typeName
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def generate_time_series_features(auth, categoryfield, collection, database, datefield, featureset, find, groupby, numfield, startdate=None, windowsize=1, info=False):
+	ep = endpoints.GENERATE_TIME_SERIES_FEATURES
+	param_dict = {
+		"categoryfield": categoryfield,
+		"collection": collection,
+		"database": database,
+		"datefield": datefield,
+		"featureset": featureset,
+		"find": find,
+		"groupby": groupby,
+		"numfield": numfield,
+		"startdate": startdate,
+		"windowsize": windowsize
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def personality_enrich(auth, category, collection, collectionOut, database, find, groupby, info=False):
+	ep = endpoints.PERSONALITY_ENRICH
+	param_dict = {
+		"category": category,
+		"collection": collection,
+		"collectionOut": collectionOut,
+		"database": database,
+		"find": find,
+		"groupby": groupby		
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def munge_transactions_aggregate(auth, munging_step, project_id, info=False):
+	ep = endpoints.MUNGE_TRANSACTIONS_AGGREGATE
+	param_dict = {
+		"munging_step": munging_step,
+		"project_id": project_id
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def munge_transactions(auth, munging_step, project_id, info=False):
+	ep = endpoints.MUNGE_TRANSACTIONS
+	param_dict = {
+		"munging_step": munging_step,
+		"project_id": project_id
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def flatten_document(auth, db, collection, attribute, find, info=False):
+	ep = endpoints.FLATTEN_DOCUMENT
+	param_dict = {
+		"mongodb": db,
+		"collection": collection,
+		"attribute": attribute,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def delete_key(auth, db, collection, attribute, find, info=False):
+	ep = endpoints.DELETE_KEY
+	param_dict = {
+		"mongodb": db,
+		"collection": collection,
+		"attribute": attribute,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def delete_many_documents(auth, db, collection, find, info=False):
+	ep = endpoints.DELETE_MANY_DOCUMENTS
+	param_dict = {
+		"mongodb": db,
+		"collection": collection,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_range(auth, db, collection, attribute, new_attribute, find, rules, info=False):
+	ep = endpoints.PROCESS_RANGE
+	param_dict = {
+		"database": db,
+		"collection": collection,
+		"mongoAttribute": attribute,
+		"newAttribute": new_attribute,
+		"find": find,
+		"rules": rules
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def nlp_worker(auth, database, collection, database_out, collection_out, attribute, find, model="original", summarization_max=10, summarization_min=5, transformer="t5-small", model_type="nlp_b5_base", info=False):
+	ep = endpoints.NLP_WORKER
+	param_dict = {
+		"database": db,
+		"collection": collection,
+		"database_out": database_out,
+		"collection_out": collection_out,
+		"attribute": attribute,
+		"find": find,
+		"model": model,
+		"summarization_max": summarization_max,
+		"summarization_min": summarization_min,
+		"transformer": transformer,
+		"type": model_type,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def delete_many_documents(auth, db, collection, find, info=False):
+	ep = endpoints.DELETE_MANY_DOCUMENTS
+	param_dict = {
+		"mongodb": db,
+		"collection": collection,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def process_range(auth, db, collection, find, attribute, new_attribute, rules, info=False):
+	ep = endpoints.PROCESS_RANGE
+	param_dict = {
+		"database": db,
+		"collection": collection,
+		"find": find,
+		"mongoAttribute": attribute,
+		"newAttribute": new_attribute,
+		"rules": rules
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+
+def prediction_enrich_fast_post(auth, json, info=False):
+	ep = endpoints.PREDICTION_ENRICH_FAST_POST
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/ecosystem_home.py` & `ecosystem-notebooks-0.1.6/prediction/apis/ecosystem_generation_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-from prediction.endpoints import ecosystem_home as endpoints
-from prediction import request_utils
-
-def get_v1_health(auth, info=False):
-	ep = endpoints.GET_V1_HEALTH
-	resp = request_utils.create(auth, ep, info=info)
-	result = resp.json()
-	return result
-
-def post_v1_health(auth, notification, info=False):
-	ep = endpoints.POST_V1_HEALTH
-	param_dict = {"notification": notification}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def ping(auth, message, info=False):
-	ep = endpoints.PING
-	param_dict = {"message": message}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def fling(auth, message, info=False):
-	ep = endpoints.FLING
-	param_dict = {"message": message}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
+from prediction.endpoints import ecosystem_generation_engine as endpoints
+from prediction import request_utils
+
+def generate_build(auth, json, info=False):
+	ep = endpoints.GENERATE_BUILD
+	resp = request_utils.create(auth, ep, json=json, info=False)
+	result = resp.json()
+	return result
+
+# def generate_properties(auth, json, info=False):
+# 	ep = endpoints.GENERATE_PROPERTIES
+# 	resp = request_utils.create(auth, ep, json=json, info=False)
+# 	result = resp.json()
+# 	return result
+
+def get_build(auth, uuid, info=False):
+	ep = endpoints.GET_BUILD
+	param_dict = {
+		"uuid": uuid
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=False)
+	meta = resp.json()
+	if "data" in meta:
+		meta = meta["data"]
+	return meta
+
+def process_build(auth, json, info=False):
+	ep = endpoints.PROCESS_BUILD
+	resp = request_utils.create(auth, ep, json=json, info=False)
+	result = resp.json()
+	return result
+
+def process_push(auth, json, info=False):
+	ep = endpoints.PROCESS_PUSH
+	resp = request_utils.create(auth, ep, json=json, info=False)
+	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/quickflat.py` & `ecosystem-notebooks-0.1.6/prediction/apis/quickflat.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import pymongo
-import json
-import datetime
-
-class QuickFlat:
-	def __init__(self, config):
-		login = config["login"]
-		login_string = "mongodb://{}:{}@{}:{}/".format(login["username"], login["password"], login["ip"], login["port"])
-		self.client = pymongo.MongoClient(login_string)
-		self.db = self.client[config["database"]]
-		self.output_db = config["output_database"]
-		self.output_col = config["output_collection"]
-		self.root_col = config["root_collection"]
-		self.connections = config["connections"]
-
-
-	def _index_field(self, collection_name, field):
-		col = self.db[collection_name]
-		index_results = col.create_index(field)
-		# print(index_results)
-
-	def _get_fields(self, collection_name):
-		col = self.db[collection_name]
-		cursor = col.find().limit(1)
-		keys = None
-		for doc in cursor:
-			keys = list(doc.keys())
-		keys.remove("_id")
-		return keys
-
-	def _generate_mongo_command(self, root_col):
-		commands = []
-		# commands.append({"$limit": 10000})
-		project_command = {
-			"$project": {
-				"_id": 0
-			}
-		}
-		for con in self.connections:
-			self._index_field(con["collection"], con["foreign_field"])
-			self._index_field(root_col, con["local_field"])
-			commands.append({
-				"$lookup": {
-					"from": con["collection"],
-					"localField": con["local_field"],
-					"foreignField": con["foreign_field"],
-					"as": con["collection"]
-				}
-			})
-			commands.append({"$unwind": "${}".format(con["collection"])})
-			fields = self._get_fields(con["collection"])
-			fields.remove(con["foreign_field"])
-			for field in fields:
-				project_command["$project"]["{}_{}".format(con["collection"], field)] = "${}.{}".format(con["collection"], field)
-
-		fields = self._get_fields(root_col)
-		for field in fields:
-			project_command["$project"][field] = 1
-
-		commands.append(project_command)
-
-
-		merge_command = {"$merge": {"into": {"db": self.output_db, "coll": self.output_col}}}
-		commands.append(merge_command)
-
-		return commands
-
-	def flatten(self):
-		root_col = self.db[self.root_col]
+import pymongo
+import json
+import datetime
+
+class QuickFlat:
+	def __init__(self, config):
+		login = config["login"]
+		login_string = "mongodb://{}:{}@{}:{}/".format(login["username"], login["password"], login["ip"], login["port"])
+		self.client = pymongo.MongoClient(login_string)
+		self.db = self.client[config["database"]]
+		self.output_db = config["output_database"]
+		self.output_col = config["output_collection"]
+		self.root_col = config["root_collection"]
+		self.connections = config["connections"]
+
+
+	def _index_field(self, collection_name, field):
+		col = self.db[collection_name]
+		index_results = col.create_index(field)
+		# print(index_results)
+
+	def _get_fields(self, collection_name):
+		col = self.db[collection_name]
+		cursor = col.find().limit(1)
+		keys = None
+		for doc in cursor:
+			keys = list(doc.keys())
+		keys.remove("_id")
+		return keys
+
+	def _generate_mongo_command(self, root_col):
+		commands = []
+		# commands.append({"$limit": 10000})
+		project_command = {
+			"$project": {
+				"_id": 0
+			}
+		}
+		for con in self.connections:
+			self._index_field(con["collection"], con["foreign_field"])
+			self._index_field(root_col, con["local_field"])
+			commands.append({
+				"$lookup": {
+					"from": con["collection"],
+					"localField": con["local_field"],
+					"foreignField": con["foreign_field"],
+					"as": con["collection"]
+				}
+			})
+			commands.append({"$unwind": "${}".format(con["collection"])})
+			fields = self._get_fields(con["collection"])
+			fields.remove(con["foreign_field"])
+			for field in fields:
+				project_command["$project"]["{}_{}".format(con["collection"], field)] = "${}.{}".format(con["collection"], field)
+
+		fields = self._get_fields(root_col)
+		for field in fields:
+			project_command["$project"][field] = 1
+
+		commands.append(project_command)
+
+
+		merge_command = {"$merge": {"into": {"db": self.output_db, "coll": self.output_col}}}
+		commands.append(merge_command)
+
+		return commands
+
+	def flatten(self):
+		root_col = self.db[self.root_col]
 		results = root_col.aggregate(self._generate_mongo_command(self.root_col))
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/transaction_categorization.py` & `ecosystem-notebooks-0.1.6/prediction/apis/transaction_categorization.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from prediction.endpoints import transaction_categorization as endpoints
-from prediction import request_utils
-
-def get_transactions(auth, json, info=False):
-	ep = endpoints.GET_TRANSACTIONS
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def get_transactions_cat_predicted(auth, json, info=False):
-	ep = endpoints.GET_TRANSACTIONS_CAT_PREDICTED
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def get_transactions_processed(auth, count, info=False):
-	ep = endpoints.GET_TRANSACTIONS_PROCESSED
-	param_dict = {"count": count}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	transactions = resp.json()
-	if "items" in transactions:
-		transactions = transactions["items"]
+from prediction.endpoints import transaction_categorization as endpoints
+from prediction import request_utils
+
+def get_transactions(auth, json, info=False):
+	ep = endpoints.GET_TRANSACTIONS
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def get_transactions_cat_predicted(auth, json, info=False):
+	ep = endpoints.GET_TRANSACTIONS_CAT_PREDICTED
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def get_transactions_processed(auth, count, info=False):
+	ep = endpoints.GET_TRANSACTIONS_PROCESSED
+	param_dict = {"count": count}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	transactions = resp.json()
+	if "items" in transactions:
+		transactions = transactions["items"]
 	return transactions
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/user_controller.py` & `ecosystem-notebooks-0.1.6/prediction/apis/user_controller.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from prediction.endpoints import user_controller as endpoints
-from prediction import request_utils
-
-def users(auth, filterByage, filterBycity, filterByemail, filterByfirstName, filterBylastName, filterBylogin, filterBystreet, filterByzipcode, orderBy, pageNumber, pageSize, sortBy, info=False):
-	ep = endpoints.USERS
-	param_dict = {
-		"filterByage": filterByage,
-		"filterBycity": filterBycity,
-		"filterByemail": filterByemail,
-		"filterByfirstName": filterByfirstName,
-		"filterBylastName": filterBylastName,
-		"filterBylogin": filterBylogin,
-		"filterBystreet": filterBystreet,
-		"filterByzipcode": filterByzipcode,
-		"orderBy": orderBy,
-		"pageNumber": pageNumber,
-		"pageSize": pageSize,
-		"sortBy": sortBy
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def post_users(auth, json, info=False):
-	ep = endpoints.POST_USERS
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def get_current_user(auth, info=False):
-	ep = endpoints.USERS_CURRENT
-	resp = request_utils.create(auth, ep, info=info)
-	result = resp.json()
-	return result
+from prediction.endpoints import user_controller as endpoints
+from prediction import request_utils
+
+def users(auth, filterByage, filterBycity, filterByemail, filterByfirstName, filterBylastName, filterBylogin, filterBystreet, filterByzipcode, orderBy, pageNumber, pageSize, sortBy, info=False):
+	ep = endpoints.USERS
+	param_dict = {
+		"filterByage": filterByage,
+		"filterBycity": filterBycity,
+		"filterByemail": filterByemail,
+		"filterByfirstName": filterByfirstName,
+		"filterBylastName": filterBylastName,
+		"filterBylogin": filterBylogin,
+		"filterBystreet": filterBystreet,
+		"filterByzipcode": filterByzipcode,
+		"orderBy": orderBy,
+		"pageNumber": pageNumber,
+		"pageSize": pageSize,
+		"sortBy": sortBy
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def post_users(auth, json, info=False):
+	ep = endpoints.POST_USERS
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def get_current_user(auth, info=False):
+	ep = endpoints.USERS_CURRENT
+	resp = request_utils.create(auth, ep, info=info)
+	result = resp.json()
+	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/utilities.py` & `ecosystem-notebooks-0.1.6/prediction/apis/utilities.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from prediction.endpoints import utilities as endpoints
-from prediction import request_utils
-
-def convert_json_to_yaml(auth, json, info=False):
-	ep = endpoints.CONVERT_JSON_TO_YAML
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	yaml = resp.json()
-	return yaml
-
-def convert_range_from_to(auth, rules, value, info=False):
-	ep = endpoints.CONVERT_RANGE_FROM_TO
-	param_dict = {
-		"rules": rules,
-		"value": value
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def convert_text_file_from_to(auth, in_delimiter, in_file, out_delimiter, out_file, rules, info=False):
-	ep = endpoints.CONVERT_TEXT_FILE_FROM_TO
-	param_dict = {
-		"inDelimiter": in_delimiter,
-		"inFile": in_file,
-		"outDelimiter": out_delimiter,
-		"outFile": out_file,
-		"rules": rules
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def convert_json_to_yaml(auth, yaml, info=False):
-	ep = endpoints.CONVERT_YAML_TO_JSON
-	resp = request_utils.create(auth, ep, json=yaml, info=info)
-	json = resp.json()
-	return json
-
-def copy_file(auth, f_from, f_to, info=False):
-	ep = endpoints.COPY_FILE
-	param_dict = {
-		"from": f_from,
-		"to": f_to
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp
-	return result
-
-def get_file(auth, file_name, lines, info=False):
-	ep = endpoints.GET_FILE
-	param_dict = {
-		"file": file_name,
-		"lines": lines
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def execute_generic(auth, script, info=False):
-	ep = endpoints.EXECUTE_GENERIC
-	resp = request_utils.create(auth, ep, data=script, info=info)
-	result = resp.json()
-	return result
-
-def get_config(auth, info=False):
-	ep = endpoints.GET_CONFIG
-	resp = request_utils.create(auth, ep, info=info)
-	result = resp.json()
-	return result
-
-def create_json_from_text(auth, in_file, out_file, info=False):
-	ep = endpoints.CREATE_JSON_FROM_TEXT
-	param_dict = {
-		"inFile": in_file,
-		"outFile": out_file,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_container_log(auth, lines, type, info=False):
-	ep = endpoints.GET_CONTAINER_LOGS
-	param_dict = {
-		"lines": lines,
-		"type": type,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def get_rest_generic(auth, data, info=False):
-	ep = endpoints.GET_REST_GENERIC
-	resp = request_utils.create(auth, ep, data=data, info=info)
-	result = resp.json()
+from prediction.endpoints import utilities as endpoints
+from prediction import request_utils
+
+def convert_json_to_yaml(auth, json, info=False):
+	ep = endpoints.CONVERT_JSON_TO_YAML
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	yaml = resp.json()
+	return yaml
+
+def convert_range_from_to(auth, rules, value, info=False):
+	ep = endpoints.CONVERT_RANGE_FROM_TO
+	param_dict = {
+		"rules": rules,
+		"value": value
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def convert_text_file_from_to(auth, in_delimiter, in_file, out_delimiter, out_file, rules, info=False):
+	ep = endpoints.CONVERT_TEXT_FILE_FROM_TO
+	param_dict = {
+		"inDelimiter": in_delimiter,
+		"inFile": in_file,
+		"outDelimiter": out_delimiter,
+		"outFile": out_file,
+		"rules": rules
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def convert_json_to_yaml(auth, yaml, info=False):
+	ep = endpoints.CONVERT_YAML_TO_JSON
+	resp = request_utils.create(auth, ep, json=yaml, info=info)
+	json = resp.json()
+	return json
+
+def copy_file(auth, f_from, f_to, info=False):
+	ep = endpoints.COPY_FILE
+	param_dict = {
+		"from": f_from,
+		"to": f_to
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp
+	return result
+
+def get_file(auth, file_name, lines, info=False):
+	ep = endpoints.GET_FILE
+	param_dict = {
+		"file": file_name,
+		"lines": lines
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def execute_generic(auth, script, info=False):
+	ep = endpoints.EXECUTE_GENERIC
+	resp = request_utils.create(auth, ep, data=script, info=info)
+	result = resp.json()
+	return result
+
+def get_config(auth, info=False):
+	ep = endpoints.GET_CONFIG
+	resp = request_utils.create(auth, ep, info=info)
+	result = resp.json()
+	return result
+
+def create_json_from_text(auth, in_file, out_file, info=False):
+	ep = endpoints.CREATE_JSON_FROM_TEXT
+	param_dict = {
+		"inFile": in_file,
+		"outFile": out_file,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_container_log(auth, lines, type, info=False):
+	ep = endpoints.GET_CONTAINER_LOGS
+	param_dict = {
+		"lines": lines,
+		"type": type,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def get_rest_generic(auth, data, info=False):
+	ep = endpoints.GET_REST_GENERIC
+	resp = request_utils.create(auth, ep, data=data, info=info)
+	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/worker_aws.py` & `ecosystem-notebooks-0.1.6/prediction/apis/worker_aws.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from prediction.endpoints import worker_aws as endpoints
-from prediction import request_utils
-
-def set_credentials(auth, cred_string, info=False):
-	ep = endpoints.SET_CREDENTIALS
-	param_dict = {
-		"string": cred_string
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def post_set_credentials(auth, data, info=False):
-	ep = endpoints.POST_SET_CREDENTIALS
-	resp = request_utils.create(auth, ep, data=data, info=info)
-	result = resp.json()
-	return result
-
-def set_tenant(auth, tenant_string, info=False):
-	ep = endpoints.SET_TENANT
-	param_dict = {
-		"string": tenant_string
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def manage_tenant(auth, tenant, action, info=False):
-	ep = endpoints.MANAGE_TENANT
-	param_dict = {
-		"tenant": tenant,
-		"action": action
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def create_tenant(auth, tenant, info=False):
-	ep = endpoints.CREATE_TENANT
-	param_dict = {
-		"tenant": tenant,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def post_create_tenant(auth, data, info=False):
-	ep = endpoints.POST_CREATE_TENANT
-	resp = request_utils.create(auth, ep, data=data, info=info)
-	result = resp.json()
-	return result
-
-def delete_tenant(auth, tenant, action, info=False):
-	ep = endpoints.DELETE_TENANT
-	param_dict = {
-		"tenant": tenant,
-		"action": action
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def set_configuration(auth, conf_string, info=False):
-	ep = endpoints.SET_CONFIGURATION
-	param_dict = {
-		"string": conf_string
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def validate_tenant(auth, tenant, info=False):
-	ep = endpoints.VALIDATE_TENANT
-	param_dict = {
-		"tenant": tenant,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def get_status(auth, tenant, info=False):
-	ep = endpoints.GET_STATUS
-	param_dict = {
-		"tenant": tenant,
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def list_tenants(auth, info=False):
-	ep = endpoints.LIST_TENANTS
-	resp = request_utils.create(auth, ep, info=info)
-	result = resp.json()
+from prediction.endpoints import worker_aws as endpoints
+from prediction import request_utils
+
+def set_credentials(auth, cred_string, info=False):
+	ep = endpoints.SET_CREDENTIALS
+	param_dict = {
+		"string": cred_string
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def post_set_credentials(auth, data, info=False):
+	ep = endpoints.POST_SET_CREDENTIALS
+	resp = request_utils.create(auth, ep, data=data, info=info)
+	result = resp.json()
+	return result
+
+def set_tenant(auth, tenant_string, info=False):
+	ep = endpoints.SET_TENANT
+	param_dict = {
+		"string": tenant_string
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def manage_tenant(auth, tenant, action, info=False):
+	ep = endpoints.MANAGE_TENANT
+	param_dict = {
+		"tenant": tenant,
+		"action": action
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def create_tenant(auth, tenant, info=False):
+	ep = endpoints.CREATE_TENANT
+	param_dict = {
+		"tenant": tenant,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def post_create_tenant(auth, data, info=False):
+	ep = endpoints.POST_CREATE_TENANT
+	resp = request_utils.create(auth, ep, data=data, info=info)
+	result = resp.json()
+	return result
+
+def delete_tenant(auth, tenant, action, info=False):
+	ep = endpoints.DELETE_TENANT
+	param_dict = {
+		"tenant": tenant,
+		"action": action
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def set_configuration(auth, conf_string, info=False):
+	ep = endpoints.SET_CONFIGURATION
+	param_dict = {
+		"string": conf_string
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def validate_tenant(auth, tenant, info=False):
+	ep = endpoints.VALIDATE_TENANT
+	param_dict = {
+		"tenant": tenant,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def get_status(auth, tenant, info=False):
+	ep = endpoints.GET_STATUS
+	param_dict = {
+		"tenant": tenant,
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def list_tenants(auth, info=False):
+	ep = endpoints.LIST_TENANTS
+	resp = request_utils.create(auth, ep, info=info)
+	result = resp.json()
 	return result
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/worker_file_service.py` & `ecosystem-notebooks-0.1.6/prediction/apis/worker_file_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,146 @@
-from prediction.endpoints import worker_file_service as endpoints
-from prediction import request_utils
-
-def upload_file(auth, path, target_path, info=False):
-	ep = endpoints.UPLOAD_FILE
-	fileFp = open(path, "rb")
-	files = {"file": fileFp}
-	data = {"path": target_path}
-	resp = request_utils.create_only_auth_no_error(auth, ep, data=data, files=files)
-	return resp
-
-def update_properties(auth, properties, info=False):
-	ep = endpoints.UPDATE_PROPERTIES
-	resp = request_utils.create_only_auth(auth, ep, data=properties)
-	return resp
-
-def get_file_tail(auth, path, file_path, lines, info=False):
-	ep = endpoints.GET_FILE_TAIL
-	param_dict = {
-		"file": file_path,
-		"lines": lines,
-		"path": path
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	data = resp.content.decode("utf-8")[1:-1]
-	rows = data.split("\n")
-	new_rows = []
-	new_rows.append(rows[0])
-	for i in range(1, len(rows), info=False):
-		row = rows[i]
-		new_rows.append(row[2:])
-	new_data = "\n".join(new_rows)
-	return new_data
-
-def get_file(auth, path, file_path, lines, info=False):
-	ep = endpoints.GET_FILE
-	param_dict = {
-		"file": file_path,
-		"lines": lines,
-		"path": path
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	data = resp.content.decode("utf-8")[1:-1]
-	rows = data.split("\n")
-	new_rows = []
-	new_rows.append(rows[0])
-	for i in range(1, len(rows), info=False):
-		row = rows[i]
-		new_rows.append(row[2:])
-	new_data = "\n".join(new_rows)
-	return new_data
-
-def get_property(auth, property_key, info=False):
-	ep = endpoints.GET_PROPERTY
-	param_dict = {
-		"key": property_key
-	}
-	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
-	data = resp.content.decode("utf-8")
-	return data
-
-def get_files(auth, path="./", user="", info=False):
-	ep = endpoints.GET_FILES
-	param_dict = {
-		"path": path,
-		"user": user
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	result = resp.json()
-	return result
-
-def copy_file(auth, from_path, to_path, user="", info=False):
-	ep = endpoints.COPY_FILE
-	param_dict = {
-		"from": from_path,
-		"to": to_path,
-		"user": user
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def download(auth, path, user="", info=False):
-	ep = endpoints.DOWNLOAD
-	param_dict = {
-		"path": path,
-		"user": user
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def delete_file(auth, path, user="", info=False):
-	ep = endpoints.DELETE_FILE
-	param_dict = {
-		"path": path,
-		"user": user
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def file_delete(auth, path, info=False):
-	ep = endpoints.FILE_DELETE
-	param_dict = {
-		"path": path
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def convert_remove_non_printables(auth, infile, outfile, info=False):
-	ep = endpoints.CONVERT_REMOVE_NON_PRINTABLES
-	param_dict = {
-		"inFile": infile,
-		"outFile": outfile
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def process_push(auth, json, info=False):
-	ep = endpoints.PROCESS_PUSH
-	resp = request_utils.create(auth, ep, json=json, info=info)
-	result = resp.json()
-	return result
-
-def convert_csv_from_to(auth, char, infile, outfile, info=False):
-	ep = endpoints.CONVERT_CSV_FROM_TO
-	param_dict = {
-		"char": char,
-		"inFile": infile,
-		"outFile": outfile
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	return resp
-
-def convert_text_file_from_to(auth, in_delimiter, infile, out_delimiter, outfile, rules, info=False):
-	ep = endpoints.CONVERT_TEXT_FILE_FROM_TO
-	param_dict = {
-		"inDelimiter": in_delimiter,
-		"inFile": infile,
-		"outDelimiter": out_delimiter,
-		"outFile": outfile,
-		"rules": rules
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+from prediction.endpoints import worker_file_service as endpoints
+from prediction import request_utils
+
+def upload_file(auth, path, target_path, info=False):
+	ep = endpoints.UPLOAD_FILE
+	fileFp = open(path, "rb")
+	files = {"file": fileFp}
+	data = {"path": target_path}
+	resp = request_utils.create_only_auth_no_error(auth, ep, data=data, files=files)
+	return resp
+
+def update_properties(auth, properties, info=False):
+	ep = endpoints.UPDATE_PROPERTIES
+	resp = request_utils.create_only_auth(auth, ep, data=properties)
+	return resp
+
+def get_file_tail(auth, path, file_path, lines, info=False):
+	ep = endpoints.GET_FILE_TAIL
+	param_dict = {
+		"file": file_path,
+		"lines": lines,
+		"path": path
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	data = resp.content.decode("utf-8")[1:-1]
+	rows = data.split("\n")
+	new_rows = []
+	new_rows.append(rows[0])
+	for i in range(1, len(rows), info=False):
+		row = rows[i]
+		new_rows.append(row[2:])
+	new_data = "\n".join(new_rows)
+	return new_data
+
+def get_file(auth, path, file_path, lines, info=False):
+	ep = endpoints.GET_FILE
+	param_dict = {
+		"file": file_path,
+		"lines": lines,
+		"path": path
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	data = resp.content.decode("utf-8")[1:-1]
+	rows = data.split("\n")
+	new_rows = []
+	new_rows.append(rows[0])
+	for i in range(1, len(rows), info=False):
+		row = rows[i]
+		new_rows.append(row[2:])
+	new_data = "\n".join(new_rows)
+	return new_data
+
+def get_property(auth, property_key, info=False):
+	ep = endpoints.GET_PROPERTY
+	param_dict = {
+		"key": property_key
+	}
+	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
+	data = resp.content.decode("utf-8")
+	return data
+
+def get_files(auth, path="./", user="", info=False):
+	ep = endpoints.GET_FILES
+	param_dict = {
+		"path": path,
+		"user": user
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	result = resp.json()
+	return result
+
+def copy_file(auth, from_path, to_path, user="", info=False):
+	ep = endpoints.COPY_FILE
+	param_dict = {
+		"from": from_path,
+		"to": to_path,
+		"user": user
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	return resp
+
+def download(auth, target_path, download_path, info=False):
+	ep = endpoints.DOWNLOAD
+	param_dict = {
+		"name": target_path,
+		"path": ""
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, stream=True, info=info)
+	with open(download_path, "wb") as fd:
+		for chunk in resp.iter_content(chunk_size=128):
+			fd.write(chunk)
+	return resp
+
+def delete_file(auth, path, user="", info=False):
+	ep = endpoints.DELETE_FILE
+	param_dict = {
+		"path": path,
+		"user": user
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	return resp
+
+def file_delete(auth, path, info=False):
+	ep = endpoints.FILE_DELETE
+	param_dict = {
+		"path": path
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	return resp
+
+def convert_remove_non_printables(auth, infile, outfile, info=False):
+	ep = endpoints.CONVERT_REMOVE_NON_PRINTABLES
+	param_dict = {
+		"inFile": infile,
+		"outFile": outfile
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	return resp
+
+def process_push(auth, json, info=False):
+	ep = endpoints.PROCESS_PUSH
+	resp = request_utils.create(auth, ep, json=json, info=info)
+	result = resp.json()
+	return result
+
+def convert_csv_from_to(auth, char, infile, outfile, info=False):
+	ep = endpoints.CONVERT_CSV_FROM_TO
+	param_dict = {
+		"char": char,
+		"inFile": infile,
+		"outFile": outfile
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	return resp
+
+def convert_text_file_from_to(auth, in_delimiter, infile, out_delimiter, outfile, rules, info=False):
+	ep = endpoints.CONVERT_TEXT_FILE_FROM_TO
+	param_dict = {
+		"inDelimiter": in_delimiter,
+		"inFile": infile,
+		"outDelimiter": out_delimiter,
+		"outFile": outfile,
+		"rules": rules
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
 	return resp
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/apis/worker_uber.py` & `ecosystem-notebooks-0.1.6/prediction/apis/worker_uber.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from prediction.endpoints import worker_uber as endpoints
-from prediction import request_utils
-
-def build_model_ludwig(auth, model_name, model_definition, info=False):
-	ep = endpoints.BUILD_MODEL_LUDWIG
-	param_dict = {
-		"model_name": model_name,
-		"model_definition": model_definition
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def build_orbit_btvc(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, params, info=False):
-	ep = endpoints.BUILD_ORBIT_BTVC
-	param_dict = {
-		"input_database": input_database,
-		"input_collection": input_collection,
-		"output_database": output_database,
-		"output_collection": output_collection,
-		"response_column": response_column,
-		"date_column": date_column,
-		"seasonality": seasonality,
-		"seed": seed,
-		"find": find,
-		"params": params
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def build_orbit_dlt(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, params, info=False):
-	ep = endpoints.BUILD_ORBIT_DLT
-	param_dict = {
-		"input_database": input_database,
-		"input_collection": input_collection,
-		"output_database": output_database,
-		"output_collection": output_collection,
-		"response_column": response_column,
-		"date_column": date_column,
-		"seasonality": seasonality,
-		"seed": seed,
-		"find": find,
-		"params": params
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def build_orbit_ets(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, info=False):
-	ep = endpoints.BUILD_ORBIT_ETS
-	param_dict = {
-		"input_database": input_database,
-		"input_collection": input_collection,
-		"output_database": output_database,
-		"output_collection": output_collection,
-		"response_column": response_column,
-		"date_column": date_column,
-		"seasonality": seasonality,
-		"seed": seed,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
-	return meta
-
-def build_orbit_lgt(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, info=False):
-	ep = endpoints.BUILD_ORBIT_LGT
-	param_dict = {
-		"input_database": input_database,
-		"input_collection": input_collection,
-		"output_database": output_database,
-		"output_collection": output_collection,
-		"response_column": response_column,
-		"date_column": date_column,
-		"seasonality": seasonality,
-		"seed": seed,
-		"find": find
-	}
-	resp = request_utils.create(auth, ep, params=param_dict, info=info)
-	meta = resp.json()
+from prediction.endpoints import worker_uber as endpoints
+from prediction import request_utils
+
+def build_model_ludwig(auth, model_name, model_definition, info=False):
+	ep = endpoints.BUILD_MODEL_LUDWIG
+	param_dict = {
+		"model_name": model_name,
+		"model_definition": model_definition
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def build_orbit_btvc(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, params, info=False):
+	ep = endpoints.BUILD_ORBIT_BTVC
+	param_dict = {
+		"input_database": input_database,
+		"input_collection": input_collection,
+		"output_database": output_database,
+		"output_collection": output_collection,
+		"response_column": response_column,
+		"date_column": date_column,
+		"seasonality": seasonality,
+		"seed": seed,
+		"find": find,
+		"params": params
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def build_orbit_dlt(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, params, info=False):
+	ep = endpoints.BUILD_ORBIT_DLT
+	param_dict = {
+		"input_database": input_database,
+		"input_collection": input_collection,
+		"output_database": output_database,
+		"output_collection": output_collection,
+		"response_column": response_column,
+		"date_column": date_column,
+		"seasonality": seasonality,
+		"seed": seed,
+		"find": find,
+		"params": params
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def build_orbit_ets(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, info=False):
+	ep = endpoints.BUILD_ORBIT_ETS
+	param_dict = {
+		"input_database": input_database,
+		"input_collection": input_collection,
+		"output_database": output_database,
+		"output_collection": output_collection,
+		"response_column": response_column,
+		"date_column": date_column,
+		"seasonality": seasonality,
+		"seed": seed,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
+	return meta
+
+def build_orbit_lgt(auth, input_database, input_collection, output_database, output_collection, response_column, date_column, seasonality, seed, find, info=False):
+	ep = endpoints.BUILD_ORBIT_LGT
+	param_dict = {
+		"input_database": input_database,
+		"input_collection": input_collection,
+		"output_database": output_database,
+		"output_collection": output_collection,
+		"response_column": response_column,
+		"date_column": date_column,
+		"seasonality": seasonality,
+		"seed": seed,
+		"find": find
+	}
+	resp = request_utils.create(auth, ep, params=param_dict, info=info)
+	meta = resp.json()
 	return meta
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/algorithm_client_pulse.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/algorithm_client_pulse.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-GET_TIMELINE = {
-	"type": "get",
-	"endpoint": "/getTimeline",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_BASKET = {
-	"type": "get",
-	"endpoint": "/processBasket",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_DIRECTED_GRAPH = {
-	"type": "get",
-	"endpoint": "/processDirectedGraph",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_ECOGENETIC_NETWORK = {
-	"type": "get",
-	"endpoint": "/processEcogeneticNetwork",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_APRIORI = {
-	"type": "get",
-	"endpoint": "/processApriori",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_FORECAST = {
-	"type": "get",
-	"endpoint": "/generateForecast",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_DIRECTED_GRAPH2 = {
-	"type": "get",
-	"endpoint": "/processDirectedGraph2",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_COX_PH_DATA = {
-	"type": "get",
-	"endpoint": "/generateCoxPhData",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_ARIMA_FORECAST = {
-	"type": "post",
-	"endpoint": "/processArimaForecast",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-
-
-LIST_PULSE_RESPONDER_DYNAMIC = {
-	"type": "get",
-	"endpoint": "/listPulseResponderDynamic",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DELETE_PULSE_RESPONDER_DYNAMIC = {
-	"type": "get",
-	"endpoint": "/deletePulseResponderDynamic",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_PULSE_RESPONDER_MESSAGES = {
-	"type": "get",
-	"endpoint": "/getPulseResponderMessages",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_PULSE_RESPONDER_OPTIONS = {
-	"type": "get",
-	"endpoint": "/getPulseResponderOptions",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_PULSE_RESPONDER_PROFILE = {
-	"type": "get",
-	"endpoint": "/getPulseResponderProfile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-UPDATE_CLIENT_PULSE_RESPONDER = {
-	"type": "post",
-	"endpoint": "/updateClientPulseResponder",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-SAVE_PULSE_RESPONDER_DYNAMIC = {
-	"type": "post",
-	"endpoint": "/savePulseResponderDynamic",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-SAVE_PULSE_RESPONDER_PROFILE = {
-	"type": "post",
-	"endpoint": "/savePulseResponderProfile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+GET_TIMELINE = {
+	"type": "get",
+	"endpoint": "/getTimeline",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_BASKET = {
+	"type": "get",
+	"endpoint": "/processBasket",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_DIRECTED_GRAPH = {
+	"type": "get",
+	"endpoint": "/processDirectedGraph",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_ECOGENETIC_NETWORK = {
+	"type": "get",
+	"endpoint": "/processEcogeneticNetwork",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_APRIORI = {
+	"type": "get",
+	"endpoint": "/processApriori",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GENERATE_FORECAST = {
+	"type": "get",
+	"endpoint": "/generateForecast",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_DIRECTED_GRAPH2 = {
+	"type": "get",
+	"endpoint": "/processDirectedGraph2",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GENERATE_COX_PH_DATA = {
+	"type": "get",
+	"endpoint": "/generateCoxPhData",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_ARIMA_FORECAST = {
+	"type": "post",
+	"endpoint": "/processArimaForecast",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+
+
+LIST_PULSE_RESPONDER_DYNAMIC = {
+	"type": "get",
+	"endpoint": "/listPulseResponderDynamic",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_PULSE_RESPONDER_DYNAMIC = {
+	"type": "get",
+	"endpoint": "/deletePulseResponderDynamic",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_PULSE_RESPONDER_MESSAGES = {
+	"type": "get",
+	"endpoint": "/getPulseResponderMessages",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_PULSE_RESPONDER_OPTIONS = {
+	"type": "get",
+	"endpoint": "/getPulseResponderOptions",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_PULSE_RESPONDER_PROFILE = {
+	"type": "get",
+	"endpoint": "/getPulseResponderProfile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+UPDATE_CLIENT_PULSE_RESPONDER = {
+	"type": "post",
+	"endpoint": "/updateClientPulseResponder",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+SAVE_PULSE_RESPONDER_DYNAMIC = {
+	"type": "post",
+	"endpoint": "/savePulseResponderDynamic",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+SAVE_PULSE_RESPONDER_PROFILE = {
+	"type": "post",
+	"endpoint": "/savePulseResponderProfile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/data_ingestion_engine.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# Data Ingestion Engine
-ADD_META_DOCUMENTS = {
-	"type": "post",
-	"endpoint": "/addMetaDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DELETE_INGEST_META = {
-	"type": "post",
-	"endpoint": "/deleteIngestMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_DATABASES_META = {
-	"type": "get",
-	"endpoint": "/getDatabasesMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_DATABASE_TABLE_COLUMN_META = {
-	"type": "get",
-	"endpoint": "/getDatabaseTableColumnMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_DATABASE_TABLE_COLUMNS_META = {
-	"type": "get",
-	"endpoint": "/getDatabaseTableColumnsMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_DATABASE_TABLES_META = {
-	"type": "get",
-	"endpoint": "/getDatabaseTablesMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_INGEST_META = {
-	"type": "get",
-	"endpoint": "/getIngestMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_INGEST_METAS = {
-	"type": "get",
-	"endpoint": "/getIngestMetas",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-SAVE_DATABASE_TABLE_COLUMN_META = {
-	"type": "post",
-	"endpoint": "/saveDatabaseTableColumnMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-SAVE_INGEST_META = {
-	"type": "post",
-	"endpoint": "/saveIngestMeta",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+# Data Ingestion Engine
+ADD_META_DOCUMENTS = {
+	"type": "post",
+	"endpoint": "/addMetaDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_INGEST_META = {
+	"type": "post",
+	"endpoint": "/deleteIngestMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_DATABASES_META = {
+	"type": "get",
+	"endpoint": "/getDatabasesMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_DATABASE_TABLE_COLUMN_META = {
+	"type": "get",
+	"endpoint": "/getDatabaseTableColumnMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_DATABASE_TABLE_COLUMNS_META = {
+	"type": "get",
+	"endpoint": "/getDatabaseTableColumnsMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_DATABASE_TABLES_META = {
+	"type": "get",
+	"endpoint": "/getDatabaseTablesMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_INGEST_META = {
+	"type": "get",
+	"endpoint": "/getIngestMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_INGEST_METAS = {
+	"type": "get",
+	"endpoint": "/getIngestMetas",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+SAVE_DATABASE_TABLE_COLUMN_META = {
+	"type": "post",
+	"endpoint": "/saveDatabaseTableColumnMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+SAVE_INGEST_META = {
+	"type": "post",
+	"endpoint": "/saveIngestMeta",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/data_management_engine.py` & `ecosystem-notebooks-0.1.6/runtime/endpoints/worker_utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,204 +1,250 @@
-# Data Management Engine
-GET_MONGO_DB_AGGREGATE2 = {
-	"type": "get",
-	"endpoint": "/2/getMongoDBAggregate",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-ADD_MONGO_COLLECTION = {
-	"type": "get",
-	"endpoint": "/addMongoCollection",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-ADD_MONGO_DATABASE = {
-	"type": "get",
-	"endpoint": "/addMongoDatabase",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-ADD_MONGO_DOCUMENTS = {
-	"type": "post",
-	"endpoint": "/addMongoDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CSV_FILE_TO_JSON = {
-	"type": "get",
-	"endpoint": "/csvFileToJSON",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CSV_FILE_TO_MONGO_DB_IMPORT = {
-	"type": "get",
-	"endpoint": "/csvFileToMongoDBImport",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CSV_FILE_TO_MONGO_DB_IMPORT2 = {
-	"type": "get",
-	"endpoint": "/csvFileToMongoDBImport2",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DELETE_ALL_MONGO_DOCUMENTS = {
-	"type": "post",
-	"endpoint": "/deleteAllMongoDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DELETE_MONGO_DOCUMENTS = {
-	"type": "post",
-	"endpoint": "/deleteMongoDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DROP_MONGO_COLLECTION = {
-	"type": "get",
-	"endpoint": "/dropMongoCollection",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DROP_MONGO_COLLECTION_INDEX = {
-	"type": "get",
-	"endpoint": "/dropMongoCollectionIndex",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DROP_MONGO_DATABASE = {
-	"type": "get",
-	"endpoint": "/dropMongoDatabase",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DUMP_MONGO_DATABASE = {
-	"type": "get",
-	"endpoint": "/dumpMongoDatabase",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-EXPORT_MONGO_DOCUMENTS = {
-	"type": "get",
-	"endpoint": "/exportMongoDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_COLLECTION_INDEXES = {
-	"type": "get",
-	"endpoint": "/getMongoCollectionIndexes",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_AGGREGATE = {
-	"type": "get",
-	"endpoint": "/getMongoDBAggregate",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_COLLECTIONS = {
-	"type": "get",
-	"endpoint": "/getMongoDBCollections",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_COLLECTION_STATS = {
-	"type": "get",
-	"endpoint": "/getMongoDBCollectionStats",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_FIND = {
-	"type": "get",
-	"endpoint": "/getMongoDBFind",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_FIND_LABELS = {
-	"type": "get",
-	"endpoint": "/getMongoDBFindLabels",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_FIND_SORT = {
-	"type": "get",
-	"endpoint": "/getMongoDBFindSort",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DB_LIST = {
-	"type": "get",
-	"endpoint": "/getMongoDBList",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-IMPORT_MONGO_DOCUMENTS = {
-	"type": "get",
-	"endpoint": "/importMongoDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-RESTORE_MONGO_DATABASE = {
-	"type": "get",
-	"endpoint": "/restoreMongoDatabase",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CREATE_MONGO_COLLECTION_INDEX = {
-	"type": "get",
-	"endpoint": "/createMongoCollectionIndex",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-POST_MONGO_DB_AGGREGATE_PIPELINE = {
-	"type": "post",
-	"endpoint": "/postMongoDBAggregatePipeline",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-RENAME_COLLECTION = {
-	"type": "get",
-	"endpoint": "/renameCollection",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}	
-UPDATE_KEY_NAME = {
-	"type": "get",
-	"endpoint": "/updateKeyName",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MONGO_DOCUMENT_LABELS = {
-	"type": "get",
-	"endpoint": "/getMongoDocumentLabels",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-EXECUTE_MONGO_DB_SCRIPT = {
-	"type": "post",
-	"endpoint": "/executeMongoDBscript",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-
-# # Data Management Engine: Cassandra
-# GET_CASSANDRA_SQL = {
-# 	"type": "get",
-# 	"endpoint": "/getCassandraSQL",
-# 	"call_message": "{type} {endpoint}",
-# 	"error_message": "{type} {endpoint} {response_code}"	
-# }
-
-# Data Management Engine: Presto
-CREATE_PRESTO_SQL = {
-	"type": "get",
-	"endpoint": "/createPrestoSQL",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-GET_PRESTO_SQL = {
-	"type": "get",
-	"endpoint": "/getPrestoSQL",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
+SEND_GET = {
+	"type": "get",
+	"endpoint": "/sendGet",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_REST = {
+	"type": "get",
+	"endpoint": "/getRest",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CASSANDRA = {
+	"type": "get",
+	"endpoint": "/getCassandra",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CASSANDRA_VERSION = {
+	"type": "get",
+	"endpoint": "/getCassandraVersion",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_FILE = {
+	"type": "get",
+	"endpoint": "/getFile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_FILE_LIST = {
+	"type": "get",
+	"endpoint": "/getFileList",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_IP = {
+	"type": "get",
+	"endpoint": "/getIP",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_REST = {
+	"type": "get",
+	"endpoint": "/getREST",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+LIST_TO_MATRIX = {
+	"type": "get",
+	"endpoint": "/listToMatrix",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+MATRIX_TO_LIST = {
+	"type": "get",
+	"endpoint": "/matrixToList",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PULL_KAFKA_TOPIC = {
+	"type": "get",
+	"endpoint": "/pullKafkaTopic",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PUSH_KAFKA_TOPICS = {
+	"type": "get",
+	"endpoint": "/pushKafkaTopics",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+UPLOAD_FILE = {
+	"type": "post",
+	"endpoint": "/upload",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+FILE_DATABASE_IMPORT = {
+	"type": "get",
+	"endpoint": "/fileDatabaseImport",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_PROPERTY = {
+	"type": "get",
+	"endpoint": "/getProperty",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+UPDATE_PROPERTIES = {
+	"type": "post",
+	"endpoint": "/updateProperties",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+UPDATE_PROPERTIES_KEY = {
+	"type": "get",
+	"endpoint": "/updatePropertiesKey",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+REFRESH = {
+	"type": "get",
+	"endpoint": "/refresh",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_SPEND_PERSONALITY = {
+	"type": "get",
+	"endpoint": "/getSpendingPersonality",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+
+GET_FINANCIAL_WELLNESS = {
+	"type": "get",
+	"endpoint": "/getFinancialWellnessScore",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_FINANCIAL_WELLNESS = {
+	"type": "put",
+	"endpoint": "/getFinancialWellnessScore",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+SQL_CASSANDRA = {
+	"type": "get",
+	"endpoint": "/sqlCassandra",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+CLOSE_CASSANDRA = {
+	"type": "get",
+	"endpoint": "/closeCassandra",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+TEST_KAFKA_KERBEROS = {
+	"type": "get",
+	"endpoint": "/testKafkaKerberos",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+ESTORE_RECOMMENDATIONS = {
+	"type": "get",
+	"endpoint": "/estoreRecommendations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_ESTORE_RECOMMENDATIONS = {
+	"type": "put",
+	"endpoint": "/estoreRecommendations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+CONNECT_U = {
+	"type": "get",
+	"endpoint": "/connectU",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_CONNECT_U = {
+	"type": "put",
+	"endpoint": "/connectU",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+JUST_FOR_YOU = {
+	"type": "get",
+	"endpoint": "/justforyou",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_JUST_FOR_YOU = {
+	"type": "put",
+	"endpoint": "/justforyou",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+ESTORE_RECOMMENDER_NON_GSM = {
+	"type": "get",
+	"endpoint": "/estoreRecommenderNonGSM",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_ESTORE_RECOMMENDER_NON_GSM = {
+	"type": "put",
+	"endpoint": "/estoreRecommenderNonGSM",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GIFT_RECOMMENDATIONS_FREE = {
+	"type": "get",
+	"endpoint": "/giftRecommendationsFree",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GIFT_RECOMMENDATIONS_PURCHASED = {
+	"type": "get",
+	"endpoint": "/giftRecommendationsPurchased",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GIFT_RECOMMENDATIONS = {
+	"type": "put",
+	"endpoint": "/giftRecommendations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+BEHAVIOR_RECOMMENDER = {
+	"type": "get",
+	"endpoint": "/behaviorRecommender",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PUT_BEHAVIOR_RECOMMENDER = {
+	"type": "put",
+	"endpoint": "/behaviorRecommender",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+
+
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/data_munging_engine.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/data_management_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,202 +1,204 @@
-# Data Munging Engine
-CONCAT_COLUMNS2 = {
-	"type": "get",
-	"endpoint": "/2/concatColumns",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DATE_ENRICH2 = {
-	"type": "get",
-	"endpoint": "/2/dateEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-AUTO_NORMALIZE_ALL = {
-	"type": "get",
-	"endpoint": "/autoNormalizeAll",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CONCAT_COLUMNS = {
-	"type": "get",
-	"endpoint": "/concatColumns",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DATE_ENRICH = {
-	"type": "get",
-	"endpoint": "/dateEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-ENUM_CONVERT = {
-	"type": "get",
-	"endpoint": "/enumConvert",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FILL_ZEROS = {
-	"type": "get",
-	"endpoint": "/fillZeros",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FILL_VALUES = {
-	"type": "get",
-	"endpoint": "/fillValues",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FOREIGN_KEY_AGGREGATOR = {
-	"type": "get",
-	"endpoint": "/foreignKeyAggregator",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FOREIGN_KEY_LOOKUP = {
-	"type": "get",
-	"endpoint": "/foreignKeyLookup",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FRAGMENT_ENRICH = {
-	"type": "get",
-	"endpoint": "/fragmentEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-FRAGMENT_ENRICH2 = {
-	"type": "get",
-	"endpoint": "/fragmentEnrich2",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_FEATURES = {
-	"type": "get",
-	"endpoint": "/generateFeatures",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_FEATURES_NORMALIZE = {
-	"type": "get",
-	"endpoint": "/generateFeaturesNormalize",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_CATEGORIES = {
-	"type": "get",
-	"endpoint": "/getCategories",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_CATEGORIES_RATIOS = {
-	"type": "get",
-	"endpoint": "/getCategoriesRatios",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-LOCATION_ENRICH = {
-	"type": "get",
-	"endpoint": "/locationEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-MCC_ENRICH = {
-	"type": "get",
-	"endpoint": "/mccEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PREDICTION_ENRICH = {
-	"type": "get",
-	"endpoint": "/predictionEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PREDICTION_ENRICH_FAST_GET = {
-	"type": "get",
-	"endpoint": "/predictionEnrichFast",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-SIC_ENRICH = {
-	"type": "get",
-	"endpoint": "/sicEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_CLIENT_PULSE_RELIABILITY = {
-	"type": "get",
-	"endpoint": "/processClientPulseReliability",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_TIME_SERIES_FEATURES = {
-	"type": "get",
-	"endpoint": "/generateTimeSeriesFeatures",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-PERSONALITY_ENRICH = {
-	"type": "get",
-	"endpoint": "/personalityEnrich",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-MUNGE_TRANSACTIONS_AGGREGATE = {
-	"type": "get",
-	"endpoint": "/mungeTransactionsAggregate",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-MUNGE_TRANSACTIONS = {
-	"type": "get",
-	"endpoint": "/mungeTransactions",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-FLATTEN_DOCUMENT = {
-	"type": "get",
-	"endpoint": "/flattenDocument",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-DELETE_KEY = {
-	"type": "get",
-	"endpoint": "/deleteKey",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-NLP_WORKER = {
-	"type": "get",
-	"endpoint": "/nlpWorker",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-DELETE_MANY_DOCUMENTS = {
-	"type": "get",
-	"endpoint": "/deleteManyDocuments",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-PROCESS_RANGE = {
-	"type": "get",
-	"endpoint": "/processRange",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-PREDICTION_ENRICH_FAST_POST = {
-	"type": "post",
-	"endpoint": "/predictionEnrichFast",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
+# Data Management Engine
+GET_MONGO_DB_AGGREGATE2 = {
+	"type": "get",
+	"endpoint": "/2/getMongoDBAggregate",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+ADD_MONGO_COLLECTION = {
+	"type": "get",
+	"endpoint": "/addMongoCollection",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+ADD_MONGO_DATABASE = {
+	"type": "get",
+	"endpoint": "/addMongoDatabase",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+ADD_MONGO_DOCUMENTS = {
+	"type": "post",
+	"endpoint": "/addMongoDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CSV_FILE_TO_JSON = {
+	"type": "get",
+	"endpoint": "/csvFileToJSON",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CSV_FILE_TO_MONGO_DB_IMPORT = {
+	"type": "get",
+	"endpoint": "/csvFileToMongoDBImport",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CSV_FILE_TO_MONGO_DB_IMPORT2 = {
+	"type": "get",
+	"endpoint": "/csvFileToMongoDBImport2",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_ALL_MONGO_DOCUMENTS = {
+	"type": "post",
+	"endpoint": "/deleteAllMongoDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_MONGO_DOCUMENTS = {
+	"type": "post",
+	"endpoint": "/deleteMongoDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DROP_MONGO_COLLECTION = {
+	"type": "get",
+	"endpoint": "/dropMongoCollection",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DROP_MONGO_COLLECTION_INDEX = {
+	"type": "get",
+	"endpoint": "/dropMongoCollectionIndex",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DROP_MONGO_DATABASE = {
+	"type": "get",
+	"endpoint": "/dropMongoDatabase",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DUMP_MONGO_DATABASE = {
+	"type": "get",
+	"endpoint": "/dumpMongoDatabase",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+EXPORT_MONGO_DOCUMENTS = {
+	"type": "get",
+	"endpoint": "/exportMongoDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_COLLECTION_INDEXES = {
+	"type": "get",
+	"endpoint": "/getMongoCollectionIndexes",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_AGGREGATE = {
+	"type": "get",
+	"endpoint": "/getMongoDBAggregate",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_COLLECTIONS = {
+	"type": "get",
+	"endpoint": "/getMongoDBCollections",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_COLLECTION_STATS = {
+	"type": "get",
+	"endpoint": "/getMongoDBCollectionStats",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_FIND = {
+	"type": "get",
+	"endpoint": "/getMongoDBFind",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_FIND_LABELS = {
+	"type": "get",
+	"endpoint": "/getMongoDBFindLabels",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_FIND_SORT = {
+	"type": "get",
+	"endpoint": "/getMongoDBFindSort",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_LIST = {
+	"type": "get",
+	"endpoint": "/getMongoDBList",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+IMPORT_MONGO_DOCUMENTS = {
+	"type": "get",
+	"endpoint": "/importMongoDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+RESTORE_MONGO_DATABASE = {
+	"type": "get",
+	"endpoint": "/restoreMongoDatabase",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CREATE_MONGO_COLLECTION_INDEX = {
+	"type": "get",
+	"endpoint": "/createMongoCollectionIndex",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+POST_MONGO_DB_AGGREGATE_PIPELINE = {
+	"type": "post",
+	"endpoint": "/postMongoDBAggregatePipeline",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+RENAME_COLLECTION = {
+	"type": "get",
+	"endpoint": "/renameCollection",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}	
+UPDATE_KEY_NAME = {
+	"type": "get",
+	"endpoint": "/updateKeyName",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DOCUMENT_LABELS = {
+	"type": "get",
+	"endpoint": "/getMongoDocumentLabels",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+EXECUTE_MONGO_DB_SCRIPT = {
+	"type": "post",
+	"endpoint": "/executeMongoDBscript",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+
+# # Data Management Engine: Cassandra
+# GET_CASSANDRA_SQL = {
+# 	"type": "get",
+# 	"endpoint": "/getCassandraSQL",
+# 	"call_message": "{type} {endpoint}",
+# 	"error_message": "{type} {endpoint} {response_code}"	
+# }
+
+# Data Management Engine: Presto
+CREATE_PRESTO_SQL = {
+	"type": "get",
+	"endpoint": "/createPrestoSQL",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+GET_PRESTO_SQL = {
+	"type": "get",
+	"endpoint": "/getPrestoSQL",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_home.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/transaction_categorization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-GET_V1_HEALTH = {
-	"type": "get",
-	"endpoint": "/v1/health",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-POST_V1_HEALTH = {
-	"type": "post",
-	"endpoint": "/v1/health",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-PING = {
-	"type": "get",
-	"endpoint": "/ping",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-FLING = {
-	"type": "get",
-	"endpoint": "/fling",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+GET_TRANSACTIONS = {
+	"type": "post",
+	"endpoint": "/getTransactions",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_TRANSACTIONS_CAT_PREDICTED = {
+	"type": "post",
+	"endpoint": "/getTransactionsCatPredicted",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_TRANSACTIONS_PROCESSED = {
+	"type": "get",
+	"endpoint": "/getTransactionsProcessed",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/ecosystem_user_profiles.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/ecosystem_user_profiles.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-VALIDATE = {
-	"type": "get",
-	"endpoint": "/validate",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-PROFILE = {
-	"type": "get",
-	"endpoint": "/profile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-ARCHIVE = {
-	"type": "get",
-	"endpoint": "/archive",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-ACTIVITIES = {
-	"type": "get",
-	"endpoint": "/activities",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-POST_ACTIVITY = {
-	"type": "post",
-	"endpoint": "/activity",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+VALIDATE = {
+	"type": "get",
+	"endpoint": "/validate",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+PROFILE = {
+	"type": "get",
+	"endpoint": "/profile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+ARCHIVE = {
+	"type": "get",
+	"endpoint": "/archive",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+ACTIVITIES = {
+	"type": "get",
+	"endpoint": "/activities",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+POST_ACTIVITY = {
+	"type": "post",
+	"endpoint": "/activity",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/utilities.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/worker_aws.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-CONVERT_JSON_TO_YAML = {
-	"type": "post",
-	"endpoint": "/convertJSONtoYAML",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CONVERT_RANGE_FROM_TO = {
-	"type": "get",
-	"endpoint": "/convertRangeFromTo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CONVERT_TEXT_FILE_FROM_TO = {
-	"type": "get",
-	"endpoint": "/convertTextFileFromTo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CONVERT_YAML_TO_JSON = {
-	"type": "post",
-	"endpoint": "/convertYAMLtoJSON",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-COPY_FILE = {
-	"type": "get",
-	"endpoint": "/copyFile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_FILE = {
-	"type": "get",
-	"endpoint": "/getFile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-EXECUTE_GENERIC = {
-	"type": "post",
-	"endpoint": "/executeGeneric",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_CONFIG = {
-	"type": "get",
-	"endpoint": "/config",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CREATE_JSON_FROM_TEXT = {
-	"type": "get",
-	"endpoint": "/createJSONfromTEXT",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_CONTAINER_LOGS = {
-	"type": "get",
-	"endpoint": "/getContainerLogs",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_REST_GENERIC = {
-	"type": "post",
-	"endpoint": "/getRestGeneric",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+SET_CREDENTIALS = {
+	"type": "get",
+	"endpoint": "/setCredentials",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+POST_SET_CREDENTIALS = {
+	"type": "post",
+	"endpoint": "/setCredentials",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+
+SET_TENANT = {
+	"type": "get",
+	"endpoint": "/setTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+MANAGE_TENANT = {
+	"type": "get",
+	"endpoint": "/manageTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+CREATE_TENANT = {
+	"type": "get",
+	"endpoint": "/createTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+POST_CREATE_TENANT = {
+	"type": "post",
+	"endpoint": "/createTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+DELETE_TENANT = {
+	"type": "get",
+	"endpoint": "/deleteTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+SET_CONFIGURATION = {
+	"type": "get",
+	"endpoint": "/setConfiguration",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+VALIDATE_TENANT = {
+	"type": "get",
+	"endpoint": "/validateTenant",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+GET_STATUS = {
+	"type": "get",
+	"endpoint": "/getStatus",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+LIST_TENANTS = {
+	"type": "get",
+	"endpoint": "/listTenants",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/worker_aws.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,67 @@
-SET_CREDENTIALS = {
-	"type": "get",
-	"endpoint": "/setCredentials",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-POST_SET_CREDENTIALS = {
-	"type": "post",
-	"endpoint": "/setCredentials",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-
-SET_TENANT = {
-	"type": "get",
-	"endpoint": "/setTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-MANAGE_TENANT = {
-	"type": "get",
-	"endpoint": "/manageTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-CREATE_TENANT = {
-	"type": "get",
-	"endpoint": "/createTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-POST_CREATE_TENANT = {
-	"type": "post",
-	"endpoint": "/createTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-DELETE_TENANT = {
-	"type": "get",
-	"endpoint": "/deleteTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-SET_CONFIGURATION = {
-	"type": "get",
-	"endpoint": "/setConfiguration",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-VALIDATE_TENANT = {
-	"type": "get",
-	"endpoint": "/validateTenant",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_STATUS = {
-	"type": "get",
-	"endpoint": "/getStatus",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-LIST_TENANTS = {
-	"type": "get",
-	"endpoint": "/listTenants",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+CONVERT_JSON_TO_YAML = {
+	"type": "post",
+	"endpoint": "/convertJSONtoYAML",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CONVERT_RANGE_FROM_TO = {
+	"type": "get",
+	"endpoint": "/convertRangeFromTo",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CONVERT_TEXT_FILE_FROM_TO = {
+	"type": "get",
+	"endpoint": "/convertTextFileFromTo",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CONVERT_YAML_TO_JSON = {
+	"type": "post",
+	"endpoint": "/convertYAMLtoJSON",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+COPY_FILE = {
+	"type": "get",
+	"endpoint": "/copyFile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_FILE = {
+	"type": "get",
+	"endpoint": "/getFile",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+EXECUTE_GENERIC = {
+	"type": "post",
+	"endpoint": "/executeGeneric",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CONFIG = {
+	"type": "get",
+	"endpoint": "/config",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CREATE_JSON_FROM_TEXT = {
+	"type": "get",
+	"endpoint": "/createJSONfromTEXT",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CONTAINER_LOGS = {
+	"type": "get",
+	"endpoint": "/getContainerLogs",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_REST_GENERIC = {
+	"type": "post",
+	"endpoint": "/getRestGeneric",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/worker_file_service.py` & `ecosystem-notebooks-0.1.6/runtime/endpoints/data_management_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,85 @@
-UPDATE_PROPERTIES = {
-	"type": "post",
-	"endpoint": "/updateProperties",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-UPLOAD_FILE = {
-	"type": "post",
-	"endpoint": "/upload",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_FILE = {
-	"type": "get",
-	"endpoint": "/getFile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_FILE_TAIL = {
-	"type": "get",
-	"endpoint": "/getFileTail",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_PROPERTY = {
-	"type": "get",
-	"endpoint": "/getProperty",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-GET_FILES = {
-	"type": "get",
-	"endpoint": "/getFiles",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-
-COPY_FILE = {
-	"type": "get",
-	"endpoint": "/copyFile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-DOWNLOAD = {
-	"type": "get",
-	"endpoint": "/download",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-DELETE_FILE = {
-	"type": "get",
-	"endpoint": "/deleteFile",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-FILE_DELETE = {
-	"type": "delete",
-	"endpoint": "/file",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-CONVERT_REMOVE_NON_PRINTABLES = {
-	"type": "get",
-	"endpoint": "/convertRemoveNonPrintables",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-PROCESS_PUSH = {
-	"type": "post",
-	"endpoint": "/processPush",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-CONVERT_CSV_FROM_TO = {
-	"type": "get",
-	"endpoint": "/convertCsvFromTo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-CONVERT_TEXT_FILE_FROM_TO = {
-	"type": "get",
-	"endpoint": "/convertTextFileFromTo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+# Data Management Engine
+UPDATE_DYNAMIC_PARAMETERS = {
+	"type": "post",
+	"endpoint": "/updateDynamicParameters",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+UPDATE_DYNAMIC_PARAMETERS_MULTI = {
+	"type": "post",
+	"endpoint": "/updateDynamicParametersMulti",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+RENAME_COLLECTION = {
+	"type": "get",
+	"endpoint": "/renameCollection",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_LIST = {
+	"type": "get",
+	"endpoint": "/getMongoDBList",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_FIND = {
+	"type": "get",
+	"endpoint": "/getMongoDBFind",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_FIND_SORT = {
+	"type": "get",
+	"endpoint": "/getMongoDBFindSort",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MONGO_DB_COLLECTIONS = {
+	"type": "get",
+	"endpoint": "/getMongoDBCollections",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CASSANDRA = {
+	"type": "get",
+	"endpoint": "/getCassandra",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CASSANDRA_VERSION = {
+	"type": "get",
+	"endpoint": "/getCassandraVersion",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_CASSANDRA_SQL = {
+	"type": "get",
+	"endpoint": "/getCassandraSql",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+FILE_DATABASE_IMPORT = {
+	"type": "get",
+	"endpoint": "/fileDataImport",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_MONGO_DB_DOCUMENTS = {
+	"type": "get",
+	"endpoint": "/deleteMongoDBDocuments",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CREATE_MONGO_COLLECTION_INDEX = {
+	"type": "get",
+	"endpoint": "/createMongoCollectionIndex",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CREATE_INDEX = {
+	"type": "get",
+	"endpoint": "/createIndex",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/worker_h2o.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/worker_h2o.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-BUILD_MODEL = {
-	"type": "get",
-	"endpoint": "/buildModel",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-CANCEL_JOB = {
-	"type": "get",
-	"endpoint": "/cancelJob",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DELETE_FRAME = {
-	"type": "delete",
-	"endpoint": "/deleteFrame",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-DOWNLOAD_MODEL_MOJO = {
-	"type": "get",
-	"endpoint": "/downloadModelMojo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_AUTO_ML_MODEL = {
-	"type": "get",
-	"endpoint": "/getAutoMLmodel",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-GET_FRAME = {
-	"type": "get",
-	"endpoint": "/getFrame",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_FRAME_COLUMNS = {
-	"type": "get",
-	"endpoint": "/getFrameColumns",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_MODEL = {
-	"type": "get",
-	"endpoint": "/getModel",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-GET_MODEL_STATS = {
-	"type": "get",
-	"endpoint": "/getModelStats",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-MODEL_GRIDS = {
-	"type": "get",
-	"endpoint": "/modelGrids",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-PREDICTION_FRAMES = {
-	"type": "get",
-	"endpoint": "/predictionFrames",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-PREDICTION_JOBS = {
-	"type": "get",
-	"endpoint": "/predictionJobs",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-PREDICTION_MODELS = {
-	"type": "get",
-	"endpoint": "/predictionModels",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-PROCESS_FILE_TO_FRAME_IMPORT = {
-	"type": "get",
-	"endpoint": "/processFileToFrameImport",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-PROCESS_TO_FRAME_PARSE = {
-	"type": "post",
-	"endpoint": "/processToFrameParse",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-SPLIT_FRAME = {
-	"type": "get",
-	"endpoint": "/splitFrame",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-GENERATE_MODEL_DETAIL = {
-	"type": "get",
-	"endpoint": "/generateModelDetail",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-DOWNLOAD_MODEL = {
-	"type": "get",
-	"endpoint": "/downloadModel",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-IMPORT_SQL_TABLE = {
-	"type": "post",
-	"endpoint": "/importSQLTable",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-CHANGE_TO_ENUM = {
-	"type": "get",
-	"endpoint": "/changeToEnum",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-GET_FRAME_COLUMN_SUMMARY = {
-	"type": "get",
-	"endpoint": "/getFrameColumnSummary",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
-}
-EXPORT_FRAME = {
-	"type": "get",
-	"endpoint": "/exportFrame",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
+BUILD_MODEL = {
+	"type": "get",
+	"endpoint": "/buildModel",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+CANCEL_JOB = {
+	"type": "get",
+	"endpoint": "/cancelJob",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DELETE_FRAME = {
+	"type": "delete",
+	"endpoint": "/deleteFrame",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+DOWNLOAD_MODEL_MOJO = {
+	"type": "get",
+	"endpoint": "/downloadModelMojo",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_AUTO_ML_MODEL = {
+	"type": "get",
+	"endpoint": "/getAutoMLmodel",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+GET_FRAME = {
+	"type": "get",
+	"endpoint": "/getFrame",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_FRAME_COLUMNS = {
+	"type": "get",
+	"endpoint": "/getFrameColumns",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_MODEL = {
+	"type": "get",
+	"endpoint": "/getModel",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+GET_MODEL_STATS = {
+	"type": "get",
+	"endpoint": "/getModelStats",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+MODEL_GRIDS = {
+	"type": "get",
+	"endpoint": "/modelGrids",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+PREDICTION_FRAMES = {
+	"type": "get",
+	"endpoint": "/predictionFrames",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+PREDICTION_JOBS = {
+	"type": "get",
+	"endpoint": "/predictionJobs",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+PREDICTION_MODELS = {
+	"type": "get",
+	"endpoint": "/predictionModels",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+PROCESS_FILE_TO_FRAME_IMPORT = {
+	"type": "get",
+	"endpoint": "/processFileToFrameImport",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+PROCESS_TO_FRAME_PARSE = {
+	"type": "post",
+	"endpoint": "/processToFrameParse",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+SPLIT_FRAME = {
+	"type": "get",
+	"endpoint": "/splitFrame",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+GENERATE_MODEL_DETAIL = {
+	"type": "get",
+	"endpoint": "/generateModelDetail",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+DOWNLOAD_MODEL = {
+	"type": "get",
+	"endpoint": "/downloadModel",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+IMPORT_SQL_TABLE = {
+	"type": "post",
+	"endpoint": "/importSQLTable",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+CHANGE_TO_ENUM = {
+	"type": "get",
+	"endpoint": "/changeToEnum",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+GET_FRAME_COLUMN_SUMMARY = {
+	"type": "get",
+	"endpoint": "/getFrameColumnSummary",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
+}
+EXPORT_FRAME = {
+	"type": "get",
+	"endpoint": "/exportFrame",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/endpoints/worker_uber.py` & `ecosystem-notebooks-0.1.6/prediction/endpoints/worker_uber.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Worker: Uber
-BUILD_MODEL_LUDWIG = {
-	"type": "get",
-	"endpoint": "/buildModelLudwig",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-BUILD_ORBIT_BTVC = {
-	"type": "get",
-	"endpoint": "/buildOrbitBTVC",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-BUILD_ORBIT_DLT = {
-	"type": "get",
-	"endpoint": "/buildOrbitDLT",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-BUILD_ORBIT_ETS = {
-	"type": "get",
-	"endpoint": "/buildOrbitETS",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-
-BUILD_ORBIT_LGT = {
-	"type": "get",
-	"endpoint": "/buildOrbitLGT",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
+# Worker: Uber
+BUILD_MODEL_LUDWIG = {
+	"type": "get",
+	"endpoint": "/buildModelLudwig",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+BUILD_ORBIT_BTVC = {
+	"type": "get",
+	"endpoint": "/buildOrbitBTVC",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+BUILD_ORBIT_DLT = {
+	"type": "get",
+	"endpoint": "/buildOrbitDLT",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+BUILD_ORBIT_ETS = {
+	"type": "get",
+	"endpoint": "/buildOrbitETS",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+
+BUILD_ORBIT_LGT = {
+	"type": "get",
+	"endpoint": "/buildOrbitLGT",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
 }
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/jwt_access.py` & `ecosystem-notebooks-0.1.6/prediction/jwt_access.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import requests
-from prediction.endpoints import auth_controller as endpoints
-from datetime import datetime
-import time
-
-def stringify_data(data):
-	str_data = str(data).replace("'", '"') 	# API requires input data to be in string format and must use " for denoting key and value pairs. Python's
-											# to string method uses ' as to indicate strings in the key value pairs.
-	return str_data
-
-class AuthenticationError(Exception):
-	"""Exception raised for incorrect authentication details."""
-	def __init__(self):
-		message = "Username and Password combination not valid."
-		super().__init__(message)
-
-class AuthenticationExpiry(Exception):
-	"""Exception raised for expired authentication token."""
-	def __init__(self, expiry):
-		expiry_datetime = datetime.utcfromtimestamp(expiry).strftime("%Y-%m-%d %H:%M:%S")
-		message = "Authentication token expired on {}. Please login again.".format(expiry_datetime)
-		super().__init__(message)
-
-class Authenticate:
-	def __init__(self, api_address, username, password):
-		self.api_address = api_address
-		self.username = username
-		self.password = password
-		token = self.__login(api_address, username, password)
-		self.access_token = token["access_token"]
-		self.refresh_token = token["refresh_token"]
-		self.expires_in = self.__format_time(token["expires_in"])
-
-		self.auth_headers = {
-			"Accept": "*/*",
-			"Authorization": "Bearer {}".format(self.access_token)
-		}
-
-	def __login(self, api_address, username, password):
-		header = {
-			"Accept": "*/*",
-			"Content-Type": "application/json"
-		}
-
-		data = {
-			"email": username,
-			"password": password
-		}
-		
-		str_data = stringify_data(data) # Stringify dict: data need to be in string format
-		r = requests.post("{}{}".format(api_address, endpoints.AUTH_LOGIN["endpoint"]), headers=header, data=str_data)
-		if r.status_code == 403:
-			raise AuthenticationError()
-		token = r.json()["token"]
-		print("Login Successful.")
-		return token
-
-	def __format_time(self, t):
-		# unix time in jwt authentication process seems to be oddly formated.
-		# this function aligns the jwt expiry time with the python unix time.
-		front = str(t)[:-3]
-		end = str(t)[-3:]
-		return float(front + "." + end)
-
-	def __token_expired(self):
-		current_time = time.time()
-		if current_time >= self.expires_in:
-			raise AuthenticationExpiry(self.expires_in)
-		return False
-
-	def get_username(self):
-		if not self.__token_expired():
-			return self.username
-
-	def get_password(self):
-		if not self.__token_expired():
-			return self.password
-
-	def get_server(self):
-		if not self.__token_expired():
-			return self.api_address
-
-	def get_access_token(self):
-		if not self.__token_expired():
-			return self.access_token
-
-	def get_refresh_token(self):
-		if not self.__token_expired():
-			return self.refresh_token
-
-	def get_expiry_date(self):
-		if not self.__token_expired():
-			return self.expires_in
-
-	def get_auth_headers(self):
-		if not self.__token_expired():
+import requests
+from prediction.endpoints import auth_controller as endpoints
+from datetime import datetime
+import time
+
+def stringify_data(data):
+	str_data = str(data).replace("'", '"') 	# API requires input data to be in string format and must use " for denoting key and value pairs. Python's
+											# to string method uses ' as to indicate strings in the key value pairs.
+	return str_data
+
+class AuthenticationError(Exception):
+	"""Exception raised for incorrect authentication details."""
+	def __init__(self):
+		message = "Username and Password combination not valid."
+		super().__init__(message)
+
+class AuthenticationExpiry(Exception):
+	"""Exception raised for expired authentication token."""
+	def __init__(self, expiry):
+		expiry_datetime = datetime.utcfromtimestamp(expiry).strftime("%Y-%m-%d %H:%M:%S")
+		message = "Authentication token expired on {}. Please login again.".format(expiry_datetime)
+		super().__init__(message)
+
+class Authenticate:
+	def __init__(self, api_address, username, password):
+		self.api_address = api_address
+		self.username = username
+		self.password = password
+		token = self.__login(api_address, username, password)
+		self.access_token = token["access_token"]
+		self.refresh_token = token["refresh_token"]
+		self.expires_in = self.__format_time(token["expires_in"])
+
+		self.auth_headers = {
+			"Accept": "*/*",
+			"Authorization": "Bearer {}".format(self.access_token)
+		}
+
+	def __login(self, api_address, username, password):
+		header = {
+			"Accept": "*/*",
+			"Content-Type": "application/json"
+		}
+
+		data = {
+			"email": username,
+			"password": password
+		}
+		
+		str_data = stringify_data(data) # Stringify dict: data need to be in string format
+		r = requests.post("{}{}".format(api_address, endpoints.AUTH_LOGIN["endpoint"]), headers=header, data=str_data)
+		if r.status_code == 403:
+			raise AuthenticationError()
+		token = r.json()["token"]
+		print("Login Successful.")
+		return token
+
+	def __format_time(self, t):
+		# unix time in jwt authentication process seems to be oddly formated.
+		# this function aligns the jwt expiry time with the python unix time.
+		front = str(t)[:-3]
+		end = str(t)[-3:]
+		return float(front + "." + end)
+
+	def __token_expired(self):
+		current_time = time.time()
+		if current_time >= self.expires_in:
+			raise AuthenticationExpiry(self.expires_in)
+		return False
+
+	def get_username(self):
+		if not self.__token_expired():
+			return self.username
+
+	def get_password(self):
+		if not self.__token_expired():
+			return self.password
+
+	def get_server(self):
+		if not self.__token_expired():
+			return self.api_address
+
+	def get_access_token(self):
+		if not self.__token_expired():
+			return self.access_token
+
+	def get_refresh_token(self):
+		if not self.__token_expired():
+			return self.refresh_token
+
+	def get_expiry_date(self):
+		if not self.__token_expired():
+			return self.expires_in
+
+	def get_auth_headers(self):
+		if not self.__token_expired():
 			return self.auth_headers
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/nlp_utils.py` & `ecosystem-notebooks-0.1.6/prediction/nlp_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import nltk
-from nltk.corpus import stopwords
-from nltk.stem.snowball import SnowballStemmer
-from sklearn.feature_extraction.text import TfidfVectorizer
-
-nltk.download("stopwords")
-nltk.download('words')
-stop_english = set(stopwords.words('english'))
-english_words = set(x.lower() for x in nltk.corpus.words.words())
-
-def clean(df,field):
-	df[field] = df[field].str.replace("[^a-zA-Z ]", "")
-	df[field].str.lower()
-	df = df.dropna(how="all")
-	return df
-
-def stem_sentences(sentence):
-	tokens = sentence.split()
-	stemmed_tokens = [stemmer.stem(token) for token in tokens]
-	return " ".join(stemmed_tokens)
-
-def stem_df(df,field,language): 	
-	global stemmer
-	stemmer = SnowballStemmer(language)
-	df[field] = df[field].apply(stem_sentences)
-	return df
-    
-def drop_stop_df(df,field):
-	df[field] = df[field].apply(drop_stop_sentence)
-	return df
-
-def drop_stop_sentence(sentence):
-	tokens = sentence.split()
-	stopped_tokens = [x for x in tokens if x not in stop_english]
-	return " ".join(stopped_tokens)
-
-def remove_english(df,field):
-	df[field] = df[field].apply(drop_eng_sentence)
-	return df
-
-def drop_eng_sentence(sentence):
-	tokens = sentence.split()
-	stopped_tokens = [x for x in tokens if x not in english_words]
-	return " ".join(stopped_tokens)
-
-def remove_non_english(df,field):
-	df[field] = df[field].apply(drop_non_eng_sentence)
-	return df
-
-def drop_non_eng_sentence(sentence):
-	tokens = sentence.split()
-	stopped_tokens = [x for x in tokens if x in english_words]
-	return " ".join(stopped_tokens)
-
-def apply_tfidf(verbs):
-    tfidf = TfidfVectorizer(sublinear_tf= True,
-                            min_df= 3,
-                            norm= "l2",
-                            encoding= "latin-1",
-                            ngram_range= (1,2),
-                            stop_words= "english",
-#                             max_features = 40000,
-                           )
-    features = tfidf.fit_transform(verbs)
+import nltk
+from nltk.corpus import stopwords
+from nltk.stem.snowball import SnowballStemmer
+from sklearn.feature_extraction.text import TfidfVectorizer
+
+nltk.download("stopwords")
+nltk.download('words')
+stop_english = set(stopwords.words('english'))
+english_words = set(x.lower() for x in nltk.corpus.words.words())
+
+def clean(df,field):
+	df[field] = df[field].str.replace("[^a-zA-Z ]", "")
+	df[field].str.lower()
+	df = df.dropna(how="all")
+	return df
+
+def stem_sentences(sentence):
+	tokens = sentence.split()
+	stemmed_tokens = [stemmer.stem(token) for token in tokens]
+	return " ".join(stemmed_tokens)
+
+def stem_df(df,field,language): 	
+	global stemmer
+	stemmer = SnowballStemmer(language)
+	df[field] = df[field].apply(stem_sentences)
+	return df
+    
+def drop_stop_df(df,field):
+	df[field] = df[field].apply(drop_stop_sentence)
+	return df
+
+def drop_stop_sentence(sentence):
+	tokens = sentence.split()
+	stopped_tokens = [x for x in tokens if x not in stop_english]
+	return " ".join(stopped_tokens)
+
+def remove_english(df,field):
+	df[field] = df[field].apply(drop_eng_sentence)
+	return df
+
+def drop_eng_sentence(sentence):
+	tokens = sentence.split()
+	stopped_tokens = [x for x in tokens if x not in english_words]
+	return " ".join(stopped_tokens)
+
+def remove_non_english(df,field):
+	df[field] = df[field].apply(drop_non_eng_sentence)
+	return df
+
+def drop_non_eng_sentence(sentence):
+	tokens = sentence.split()
+	stopped_tokens = [x for x in tokens if x in english_words]
+	return " ".join(stopped_tokens)
+
+def apply_tfidf(verbs):
+    tfidf = TfidfVectorizer(sublinear_tf= True,
+                            min_df= 3,
+                            norm= "l2",
+                            encoding= "latin-1",
+                            ngram_range= (1,2),
+                            stop_words= "english",
+#                             max_features = 40000,
+                           )
+    features = tfidf.fit_transform(verbs)
     return features, tfidf
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/notebook_functions.py` & `ecosystem-notebooks-0.1.6/prediction/notebook_functions.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import uuid
-from IPython.display import display_javascript, display_html, display
-import json
-import pandas as pd
-import matplotlib.pyplot as plt
-from prediction.apis import worker_h2o
-from prediction.apis import prediction_engine
-import datetime
-
-class RenderJSON(object):
-	def __init__(self, json_data):
-		if isinstance(json_data, dict):
-			self.json_str = json.dumps(json_data)
-		else:
-			self.json_str = json_data
-		self.uuid = str(uuid.uuid4())
-
-	def _ipython_display_(self):
-		display_html('<div id="{}" style="height: 600px; width:100%;"></div>'.format(self.uuid), raw=True)
-		display_javascript("""
-		require(["https://rawgit.com/caldwell/renderjson/master/renderjson.js"], function() {
-		document.getElementById('%s').appendChild(renderjson(%s))
-		});
-		""" % (self.uuid, self.json_str), raw=True)
-
-def list_automl_models(model_data):
-	sort_metric = model_data["leaderboard"]["sort_metric"]
-	model_names = []
-	for model in model_data["leaderboard"]["models"]:
-		model_names.append(model["name"])
-
-	model_metrics = model_data["leaderboard"]["sort_metrics"]
-
-	df = pd.DataFrame(
-		{
-			"model_names": model_names,
-			"model_metrics": model_metrics
-		}
-	)
-	df.sort_values("model_metrics", inplace=True, ascending=False)
-	return df
-
-def show_automl_leaderboard(model_data, aml_name=None):
-	sort_metric = model_data["leaderboard"]["sort_metric"]
-	df = list_automl_models(model_data)
-	ax = df.plot(y="model_metrics", x="model_names", kind="bar", align="center", alpha=0.5, legend=None)
-	plt.xticks(rotation=90)
-	ax.set_title("Performance of Models. Sorted Using Metric: {}".format(sort_metric))
-	if aml_name != None:
-		ax.set_title("{}: Performance of Models. Sorted Using Metric: {}".format(aml_name, sort_metric))
-	ax.yaxis.grid(True)
-
-def save_best_model(auth, df, rename=None):
-	best_model_id = df.iloc[0]["model_names"]
-	h2o_name = best_model_id
-	_save_model(auth, h2o_name, df, rename)
-	return h2o_name
-
-def save_model(auth, h2o_model_name, df):
-	_save_model(auth, h2o_model_name, df)
-	return h2o_name
-
-def _save_model(auth, h2o_name, df, rename):
-	zip_name = h2o_name + ".zip"
-	worker_h2o.download_model_mojo(auth, h2o_name)
-	high_level_mojo = worker_h2o.get_train_model(auth, h2o_name, "single")
-	model_to_save = high_level_mojo["models"][0]
-	model_to_save["model_identity"] = h2o_name
-	if rename != None:
-		model_to_save["model_identity"] = rename
-		model_to_save["model_id"]["name"] = rename
-	model_to_save["userid"] = "user"
-	model_to_save["timestamp"] = "time_stamp"
-
-def show_variable_importance(stats):
-	var_names = []
-	for column in stats["columns"]:
-		var_names.append(column["name"])
-	# notebook_functions.RenderJSON(stats)
-	df = pd.DataFrame(
-		{
-			var_names[0]: stats["data"][0],
-			var_names[1]: stats["data"][1],
-			var_names[2]: stats["data"][2],
-			var_names[3]: stats["data"][3]
-		}
-	)
-	return df
-
-def save_file_as_userframe(auth, data_file, feature_store, user_name, columntypes=None):
-	timestampvar = datetime.datetime.now().isoformat()
-	data_file_prefix = ".".join(data_file.split(".")[:-1])
-	hexframename = data_file_prefix + ".hex"
-	imp = worker_h2o.file_to_frame(auth, data_file, 1, ",")
-	descrip = "Automated feature store generated for " + feature_store
-	frameID = feature_store
-	if columntypes != None:
-		for key in columntypes.keys():
-				idx = imp["columnNames"].index(key)
-				imp["columnTypes"][idx] = columntypes[key]
-				imp["columnProperties"][idx]["new_type"] = columntypes[key] 
-		
-	str_imp = {
-		"import": imp["import"],
-		"parseSetup": imp["parseSetup"],
-		"columnNames": imp["columnNames"],
-		"columnTypes": imp["columnTypes"],
-		"columnProperties": imp["columnProperties"]
-	}
-	str_imp = json.dumps(str_imp)
-	user_frame = {
-		"timestamp_parsed": timestampvar,
-		"parser": "csv",
-		"import": str_imp,
-		"destination_frame": hexframename,
-		"file_name": data_file,
-		"description": descrip,
-		"first_row_column_names": "1",
-		"feature_store_script": "",
-		"separator": "comma",
-		"frame_id": frameID,
-		"columnProperties": imp["columnProperties"],
-		"created_by": user_name,
-		"created_date": timestampvar,
-		"preview_detail": {
-			"summary": descrip,
-			"image": "/data/xyz.png",
-			"heading": frameID,
-			"active": True,
-			"detail": data_file
-		}
-	}
-
-	worker_h2o.delete_frame(auth, hexframename)
-	prediction_engine.save_user_frame(auth, user_frame)
-	frame = worker_h2o.featurestore_to_frame(auth, user_frame)
+import uuid
+from IPython.display import display_javascript, display_html, display
+import json
+import pandas as pd
+import matplotlib.pyplot as plt
+from prediction.apis import worker_h2o
+from prediction.apis import prediction_engine
+import datetime
+
+class RenderJSON(object):
+	def __init__(self, json_data):
+		if isinstance(json_data, dict):
+			self.json_str = json.dumps(json_data)
+		else:
+			self.json_str = json_data
+		self.uuid = str(uuid.uuid4())
+
+	def _ipython_display_(self):
+		display_html('<div id="{}" style="height: 600px; width:100%;"></div>'.format(self.uuid), raw=True)
+		display_javascript("""
+		require(["https://rawgit.com/caldwell/renderjson/master/renderjson.js"], function() {
+		document.getElementById('%s').appendChild(renderjson(%s))
+		});
+		""" % (self.uuid, self.json_str), raw=True)
+
+def list_automl_models(model_data):
+	sort_metric = model_data["leaderboard"]["sort_metric"]
+	model_names = []
+	for model in model_data["leaderboard"]["models"]:
+		model_names.append(model["name"])
+
+	model_metrics = model_data["leaderboard"]["sort_metrics"]
+
+	df = pd.DataFrame(
+		{
+			"model_names": model_names,
+			"model_metrics": model_metrics
+		}
+	)
+	df.sort_values("model_metrics", inplace=True, ascending=False)
+	return df
+
+def show_automl_leaderboard(model_data, aml_name=None):
+	sort_metric = model_data["leaderboard"]["sort_metric"]
+	df = list_automl_models(model_data)
+	ax = df.plot(y="model_metrics", x="model_names", kind="bar", align="center", alpha=0.5, legend=None)
+	plt.xticks(rotation=90)
+	ax.set_title("Performance of Models. Sorted Using Metric: {}".format(sort_metric))
+	if aml_name != None:
+		ax.set_title("{}: Performance of Models. Sorted Using Metric: {}".format(aml_name, sort_metric))
+	ax.yaxis.grid(True)
+
+def save_best_model(auth, df, rename=None):
+	best_model_id = df.iloc[0]["model_names"]
+	h2o_name = best_model_id
+	_save_model(auth, h2o_name, df, rename)
+	return h2o_name
+
+def save_model(auth, h2o_model_name, df):
+	_save_model(auth, h2o_model_name, df)
+	return h2o_name
+
+def _save_model(auth, h2o_name, df, rename):
+	zip_name = h2o_name + ".zip"
+	worker_h2o.download_model_mojo(auth, h2o_name)
+	high_level_mojo = worker_h2o.get_train_model(auth, h2o_name, "single")
+	model_to_save = high_level_mojo["models"][0]
+	model_to_save["model_identity"] = h2o_name
+	if rename != None:
+		model_to_save["model_identity"] = rename
+		model_to_save["model_id"]["name"] = rename
+	model_to_save["userid"] = "user"
+	model_to_save["timestamp"] = "time_stamp"
+
+def show_variable_importance(stats):
+	var_names = []
+	for column in stats["columns"]:
+		var_names.append(column["name"])
+	# notebook_functions.RenderJSON(stats)
+	df = pd.DataFrame(
+		{
+			var_names[0]: stats["data"][0],
+			var_names[1]: stats["data"][1],
+			var_names[2]: stats["data"][2],
+			var_names[3]: stats["data"][3]
+		}
+	)
+	return df
+
+def save_file_as_userframe(auth, data_file, feature_store, user_name, columntypes=None):
+	timestampvar = datetime.datetime.now().isoformat()
+	data_file_prefix = ".".join(data_file.split(".")[:-1])
+	hexframename = data_file_prefix + ".hex"
+	imp = worker_h2o.file_to_frame(auth, data_file, 1, ",")
+	descrip = "Automated feature store generated for " + feature_store
+	frameID = feature_store
+	if columntypes != None:
+		for key in columntypes.keys():
+				idx = imp["columnNames"].index(key)
+				imp["columnTypes"][idx] = columntypes[key]
+				imp["columnProperties"][idx]["new_type"] = columntypes[key] 
+		
+	str_imp = {
+		"import": imp["import"],
+		"parseSetup": imp["parseSetup"],
+		"columnNames": imp["columnNames"],
+		"columnTypes": imp["columnTypes"],
+		"columnProperties": imp["columnProperties"]
+	}
+	str_imp = json.dumps(str_imp)
+	user_frame = {
+		"timestamp_parsed": timestampvar,
+		"parser": "csv",
+		"import": str_imp,
+		"destination_frame": hexframename,
+		"file_name": data_file,
+		"description": descrip,
+		"first_row_column_names": "1",
+		"feature_store_script": "",
+		"separator": "comma",
+		"frame_id": frameID,
+		"columnProperties": imp["columnProperties"],
+		"created_by": user_name,
+		"created_date": timestampvar,
+		"preview_detail": {
+			"summary": descrip,
+			"image": "/data/xyz.png",
+			"heading": frameID,
+			"active": True,
+			"detail": data_file
+		}
+	}
+
+	worker_h2o.delete_frame(auth, hexframename)
+	prediction_engine.save_user_frame(auth, user_frame)
+	frame = worker_h2o.featurestore_to_frame(auth, user_frame)
 	return frame["parseSetup"]["destination_frame"], imp
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/prediction_utils.py` & `ecosystem-notebooks-0.1.6/prediction/prediction_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import datetime
-import time
-import copy
-import concurrent.futures
-from prediction.apis import worker_h2o
-from prediction.apis import data_management_engine
-from prediction.apis import prediction_engine
-
-def frame_csv_file(auth, filename, prefix, description):
-	filecsv = filename + ".csv"
-	filehex = filename + ".hex"
-	parsed = worker_h2o.file_to_frame(auth, filecsv, 1, "comma")
-	user_frame = {}
-	user_frame["timestamp_parsed"] = datetime.datetime.now().isoformat()
-	user_frame["parser"] = "CSV"
-	user_frame["import"] = parsed["import"]
-	user_frame["parseSetup"] = parsed["parseSetup"]
-	user_frame["destination_frame"] = filehex
-	user_frame["file_name"] = filecsv
-	user_frame["description"] = description
-	user_frame["first_row_column_names"] = "1"
-	user_frame["separator"] = "comma"
-	user_frame["frame_id"] = prefix + filename
-	user_frame["columnProperties"] = parsed["columnProperties"]
-
-	result = prediction_engine.save_user_frame(auth, user_frame)
-	frame = worker_h2o.featurestore_to_frame(auth, user_frame)
-
-
-def _async_thread(auth, j_dc_doc, count, total):
-		while True:
-			try:
-				data_management_engine.add_documents(auth, j_dc_doc, info=False)
-				print("{}/{}".format(count, total))
-				break
-			except:
-				pass
-	
-
-def async_upload(auth, dataframe, db_name, col_name):
-	data = list(dataframe.T.to_dict().values())
-	j_dc_doc = {
-		"database": db_name,
-		"collection": col_name,
-		"document": {}
-	}
-
-	with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
-		count = 0
-		for d in data:
-			count += 1
-			# if count >= 1000:
-			# 	break
-			j_dc_doc["document"] = dict(d)
-			d2 = copy.deepcopy(j_dc_doc)
+import datetime
+import time
+import copy
+import concurrent.futures
+from prediction.apis import worker_h2o
+from prediction.apis import data_management_engine
+from prediction.apis import prediction_engine
+
+def frame_csv_file(auth, filename, prefix, description):
+	filecsv = filename + ".csv"
+	filehex = filename + ".hex"
+	parsed = worker_h2o.file_to_frame(auth, filecsv, 1, "comma")
+	user_frame = {}
+	user_frame["timestamp_parsed"] = datetime.datetime.now().isoformat()
+	user_frame["parser"] = "CSV"
+	user_frame["import"] = parsed["import"]
+	user_frame["parseSetup"] = parsed["parseSetup"]
+	user_frame["destination_frame"] = filehex
+	user_frame["file_name"] = filecsv
+	user_frame["description"] = description
+	user_frame["first_row_column_names"] = "1"
+	user_frame["separator"] = "comma"
+	user_frame["frame_id"] = prefix + filename
+	user_frame["columnProperties"] = parsed["columnProperties"]
+
+	result = prediction_engine.save_user_frame(auth, user_frame)
+	frame = worker_h2o.featurestore_to_frame(auth, user_frame)
+
+
+def _async_thread(auth, j_dc_doc, count, total):
+		while True:
+			try:
+				data_management_engine.add_documents(auth, j_dc_doc, info=False)
+				print("{}/{}".format(count, total))
+				break
+			except:
+				pass
+	
+
+def async_upload(auth, dataframe, db_name, col_name):
+	data = list(dataframe.T.to_dict().values())
+	j_dc_doc = {
+		"database": db_name,
+		"collection": col_name,
+		"document": {}
+	}
+
+	with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
+		count = 0
+		for d in data:
+			count += 1
+			# if count >= 1000:
+			# 	break
+			j_dc_doc["document"] = dict(d)
+			d2 = copy.deepcopy(j_dc_doc)
 			executor.submit(_async_thread, auth, d2, count, len(data))
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/request_utils.py` & `ecosystem-notebooks-0.1.6/prediction/request_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-import requests
-from requests import RequestException
-
-class RequestTypeError(Exception):
-	"""Exception raised for non existant request type."""
-	def __init__(self, t):
-		message = "Non existant request type: {}.".format(t)
-		super().__init__(message)
-
-class ApiError(IOError):
-	"""There was an ambiguous exception that occurred while handling your
-		request.
-		"""
-	def __init__(self, *args, **kwargs):
-		"""Initialize RequestException with `request` and `response` objects."""
-		response = kwargs.pop('response', None)
-		self.response = response
-		self.request = kwargs.pop('request', None)
-		if (response is not None and not self.request and
-			hasattr(response, 'request')):
-			self.request = self.response.request
-			# super(RequestException, self).__init__(*args, **kwargs) TODO: this gives errors, might not be neccesay.
-			super().__init__(*args, **kwargs)
-
-def auto_format_params(d):
-	s = ""
-	for key in d:
-		d[key] = str(d[key])
-		s += "{key}={{{key}}}&".format(key=key)
-	return s.format(**d)
-
-def get_type(t):
-	if t == "get":
-		return requests.get
-	elif t == "post":
-		return requests.post
-	elif t == "put":
-		return request.put
-	elif t == "delete":
-		return requests.delete
-	elif t == "patch":
-		return request.patch
-	else:
-		raise RequestTypeError(t)
-
-def create_only_auth(auth, endpoint, **kwargs):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	print(call_message)
-	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
-	if resp.status_code != 200:
-		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
-		print(error_message)
-		raise ApiError(error_message, response=resp)
-	return resp
-
-def create_only_auth_no_error(auth, endpoint, **kwargs):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	print(call_message)
-	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
-	return resp
-
-def create(auth, endpoint, json=None, data=None, params=None, ep_arg=None, info=False):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	if ep_arg != None:
-		url_endpoint = url_endpoint + ep_arg
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	if json == None and data == None and params == None:
-		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False)
-	elif json == None and data == None:
-		call_message = call_message + "?" + auto_format_params(params)
-		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), params=params, verify=False)
-	elif params == None:
-		if json == None:
-			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), data=data, verify=False)
-		else:
-			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), json=json, verify=False)
-	else:
-		raise Exception("Error: Unsupported state: Both json and params parameters passed.")
-	if resp.status_code != 200:
-		print(call_message)
-		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
-		print(error_message)
-		raise ApiError(error_message, response=resp)
-	if info:
-		print(call_message)
+import requests
+from requests import RequestException
+
+class RequestTypeError(Exception):
+	"""Exception raised for non existant request type."""
+	def __init__(self, t):
+		message = "Non existant request type: {}.".format(t)
+		super().__init__(message)
+
+class ApiError(IOError):
+	"""There was an ambiguous exception that occurred while handling your
+		request.
+		"""
+	def __init__(self, *args, **kwargs):
+		"""Initialize RequestException with `request` and `response` objects."""
+		response = kwargs.pop('response', None)
+		self.response = response
+		self.request = kwargs.pop('request', None)
+		if (response is not None and not self.request and
+			hasattr(response, 'request')):
+			self.request = self.response.request
+			# super(RequestException, self).__init__(*args, **kwargs) TODO: this gives errors, might not be neccesay.
+			super().__init__(*args, **kwargs)
+
+def auto_format_params(d):
+	s = ""
+	for key in d:
+		d[key] = str(d[key])
+		s += "{key}={{{key}}}&".format(key=key)
+	return s.format(**d)
+
+def get_type(t):
+	if t == "get":
+		return requests.get
+	elif t == "post":
+		return requests.post
+	elif t == "put":
+		return request.put
+	elif t == "delete":
+		return requests.delete
+	elif t == "patch":
+		return request.patch
+	else:
+		raise RequestTypeError(t)
+
+def create_only_auth(auth, endpoint, **kwargs):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	print(call_message)
+	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
+	if resp.status_code != 200:
+		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
+		print(error_message)
+		raise ApiError(error_message, response=resp)
+	return resp
+
+def create_only_auth_no_error(auth, endpoint, **kwargs):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	print(call_message)
+	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
+	return resp
+
+def create(auth, endpoint, json=None, data=None, params=None, ep_arg=None, stream=None, info=False):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	if ep_arg != None:
+		url_endpoint = url_endpoint + ep_arg
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	if json == None and data == None and params == None and stream == None:
+		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False)
+	elif json == None and data == None and stream == None:
+		call_message = call_message + "?" + auto_format_params(params)
+		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), params=params, verify=False)
+	elif params == None and stream == None:
+		if json == None:
+			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), data=data, verify=False)
+		else:
+			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), json=json, verify=False)
+	elif stream != None and params != None:
+		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), params=params, stream=True, verify=False)
+	else:
+		raise Exception("Error: Unsupported state: Both json and params parameters passed.")
+	if resp.status_code != 200:
+		print(call_message)
+		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
+		print(error_message)
+		raise ApiError(error_message, response=resp)
+	if info:
+		print(call_message)
 	return resp
```

### Comparing `ecosystem-notebooks-0.1.5/prediction/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.6/prediction/utils/endpoint_diff.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-from os import listdir
-from os.path import isfile, join
-import sys
-import json
-import os
-from glob import glob
-
-prediction_server_path = "C:/Users/Ramsay/Documents/GitHub/ecosystem-server/"
-prediction_fp = prediction_server_path + "src/main/java/com/ecosystem/"
-# files = [f for f in listdir(prediction_fp) if isfile(join(prediction_fp, f))]
-files = [y for x in os.walk(prediction_fp) for y in glob(os.path.join(x[0], "*.java"))]
-
-server_endpoints = []
-api_request = "@RequestMapping"
-api_post_request = "@PostMapping"
-api_get_request = "@GetMapping"
-
-def stripping(parameter):
-	if parameter[0] == "=":
-		parameter = parameter[1:]
-	parameter = parameter.replace("'", "")
-	parameter = parameter.replace('"', "")
-	if parameter[0] == ":":
-		parameter = parameter[1:]
-	return parameter
-
-def create_endpoint(endpoint, method):
-	d = {
-		"endpoint": endpoint,
-		"method": method
-	}
-	return d
-
-def endpoints_equal(eps, epw):
-	if eps == epw:
-		return True
-	if epw[-1] == "/":
-		index1 = eps.find("{")
-		index2 = eps.find("}")
-		new_eps = eps[:index1] + eps[index2+1:]
-		if new_eps == epw:
-			return True
-	return False
-
-def compare_endpoints(server_endpoints, wrapper_endpoints):
-	both = []
-	server = []
-	wrapper = []
-	for d in server_endpoints:
-		se = d["endpoint"]
-		sm = d["method"]
-		found = False
-		for d2 in wrapper_endpoints:
-			we = d2["endpoint"]
-			wm = d2["method"]
-			if endpoints_equal(se, we) and wm.lower() in sm.lower():
-				both.append([d, d2])
-				found = True
-				break
-		if not found:
-			server.append(d)
-	for d2 in wrapper_endpoints:
-		we = d2["endpoint"]
-		wm = d2["method"]
-		found = False
-		for d in server_endpoints:
-			se = d["endpoint"]
-			sm = d["method"]
-			if endpoints_equal(se, we) and wm.lower() in sm.lower():
-				found = True
-				break
-		if not found:
-			wrapper.append(d2)
-
-	print("")
-	print("Found in both:")
-	data = [
-		["----SERVER----", "", "", "----WRAPPER----", ""],
-		["method", "endpoint", "", "method", "endpoint"],
-		["------", "------", "------", "------", "------"]
-	]
-	for b in both:
-		row = [b[0]["method"], b[0]["endpoint"], "|", b[1]["method"], b[1]["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(both)))
-
-	print("Only in one:")
-	data = [
-		["----SERVER----", ""],
-		["method", "endpoint"],
-		["------", "------"]
-	]
-	for s in server:
-		row = [s["method"], s["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(server)))
-	data = [
-		["----WRAPPER----", ""],
-		["method", "endpoint"],
-		["------", "------"]
-	]
-	for w in wrapper:
-		row = [w["method"], w["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(wrapper)))
-
-for file_path in files:
-	f = open(file_path, "r")
-	endpoint_prefix = ""
-	for line in f:
-		if line[:2] == "//":
-			continue
-		if api_request in line:
-			index = line.find(api_request)
-			comment_index = line.find("//")
-			if index != -1:
-				if comment_index != -1:
-					if comment_index < index:
-						continue
-				value = ""
-				method = ""
-				parameters = line[index+len(api_request):]
-				endpoint_prefix = parameters[2:-3]
-				parameters = parameters.split(",")
-				for parameter in parameters:
-					parameter = "".join(parameter.split())
-					if "value" in parameter:
-						if parameter[0] == "(":
-							parameter = parameter[1:]
-						if parameter[-1] == ")":
-							parameter = parameter[:-1]
-						index = parameter.find("value")
-						parameter = parameter[index+len("value"):]
-						value = stripping(parameter)
-
-					elif "method" in parameter:
-						if parameter[0] == "(":
-							parameter = parameter[1:]
-						if parameter[-1] == ")":
-							parameter = parameter[:-1]
-						index = parameter.find("method")
-						parameter = parameter[index+len("method"):]
-						method = stripping(parameter)
-				if value != "" and method != "":
-					server_endpoints.append(create_endpoint(value, method))
-		if api_post_request in line:
-			index = line.find(api_post_request)
-			line = line[index+len(api_post_request):]
-			line = line[2:-3]
-			if endpoint_prefix[0] == "/":
-				server_endpoints.append(create_endpoint(endpoint_prefix + line, "POST"))
-			else:
-				server_endpoints.append(create_endpoint(line, "POST"))
-		if api_get_request in line:
-			index = line.find(api_get_request)
-			line = line[index+len(api_get_request):]
-			line = line[2:-3]
-			if endpoint_prefix[0] == "/":
-				server_endpoints.append(create_endpoint(endpoint_prefix + line, "GET"))
-			else:
-				server_endpoints.append(create_endpoint(line, "GET"))
-			
-
-
-# for se in server_endpoints:
-# 	print(se)
-
-# print("count: {}".format(len(server_endpoints)))
-
-
-wrapper_endpoints = []
-
-wrapper_path = "../"
-wrapper_fp = wrapper_path + "endpoints/"
-files = [f for f in listdir(wrapper_fp) if isfile(join(wrapper_fp, f))]
-if "__init__.py" in files:
-	files.remove("__init__.py")
-
-for f_n in files:
-	file_path = wrapper_fp + f_n
-	f = open(file_path, "r")
-	data = f.read()
-	data = "".join(data.split())
-	while True:
-		index = data.find("{")
-		if index == -1:
-			break
-		open_count = 0
-		close_count = 0
-		for i in range(len(data[index:])):
-			c = data[i+index]
-			if c == "}":
-				close_count += 1
-			if c == "{":
-				open_count += 1
-			if open_count == close_count:
-				s = data[index: index+i+1]
-				j_str = eval(s)
-				# j_str = json.loads(s)
-				wrapper_endpoints.append(create_endpoint(j_str["endpoint"], j_str["type"]))
-				data = data[index+i:]
-				break
-
-# for we in wrapper_endpoints:
-# 	print(we)
-
-# print("count: {}".format(len(wrapper_endpoints)))
-
+from os import listdir
+from os.path import isfile, join
+import sys
+import json
+import os
+from glob import glob
+
+prediction_server_path = "C:/Users/Ramsay/Documents/GitHub/ecosystem-server/"
+prediction_fp = prediction_server_path + "src/main/java/com/ecosystem/"
+# files = [f for f in listdir(prediction_fp) if isfile(join(prediction_fp, f))]
+files = [y for x in os.walk(prediction_fp) for y in glob(os.path.join(x[0], "*.java"))]
+
+server_endpoints = []
+api_request = "@RequestMapping"
+api_post_request = "@PostMapping"
+api_get_request = "@GetMapping"
+
+def stripping(parameter):
+	if parameter[0] == "=":
+		parameter = parameter[1:]
+	parameter = parameter.replace("'", "")
+	parameter = parameter.replace('"', "")
+	if parameter[0] == ":":
+		parameter = parameter[1:]
+	return parameter
+
+def create_endpoint(endpoint, method):
+	d = {
+		"endpoint": endpoint,
+		"method": method
+	}
+	return d
+
+def endpoints_equal(eps, epw):
+	if eps == epw:
+		return True
+	if epw[-1] == "/":
+		index1 = eps.find("{")
+		index2 = eps.find("}")
+		new_eps = eps[:index1] + eps[index2+1:]
+		if new_eps == epw:
+			return True
+	return False
+
+def compare_endpoints(server_endpoints, wrapper_endpoints):
+	both = []
+	server = []
+	wrapper = []
+	for d in server_endpoints:
+		se = d["endpoint"]
+		sm = d["method"]
+		found = False
+		for d2 in wrapper_endpoints:
+			we = d2["endpoint"]
+			wm = d2["method"]
+			if endpoints_equal(se, we) and wm.lower() in sm.lower():
+				both.append([d, d2])
+				found = True
+				break
+		if not found:
+			server.append(d)
+	for d2 in wrapper_endpoints:
+		we = d2["endpoint"]
+		wm = d2["method"]
+		found = False
+		for d in server_endpoints:
+			se = d["endpoint"]
+			sm = d["method"]
+			if endpoints_equal(se, we) and wm.lower() in sm.lower():
+				found = True
+				break
+		if not found:
+			wrapper.append(d2)
+
+	print("")
+	print("Found in both:")
+	data = [
+		["----SERVER----", "", "", "----WRAPPER----", ""],
+		["method", "endpoint", "", "method", "endpoint"],
+		["------", "------", "------", "------", "------"]
+	]
+	for b in both:
+		row = [b[0]["method"], b[0]["endpoint"], "|", b[1]["method"], b[1]["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(both)))
+
+	print("Only in one:")
+	data = [
+		["----SERVER----", ""],
+		["method", "endpoint"],
+		["------", "------"]
+	]
+	for s in server:
+		row = [s["method"], s["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(server)))
+	data = [
+		["----WRAPPER----", ""],
+		["method", "endpoint"],
+		["------", "------"]
+	]
+	for w in wrapper:
+		row = [w["method"], w["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(wrapper)))
+
+for file_path in files:
+	f = open(file_path, "r")
+	endpoint_prefix = ""
+	for line in f:
+		if line[:2] == "//":
+			continue
+		if api_request in line:
+			index = line.find(api_request)
+			comment_index = line.find("//")
+			if index != -1:
+				if comment_index != -1:
+					if comment_index < index:
+						continue
+				value = ""
+				method = ""
+				parameters = line[index+len(api_request):]
+				endpoint_prefix = parameters[2:-3]
+				parameters = parameters.split(",")
+				for parameter in parameters:
+					parameter = "".join(parameter.split())
+					if "value" in parameter:
+						if parameter[0] == "(":
+							parameter = parameter[1:]
+						if parameter[-1] == ")":
+							parameter = parameter[:-1]
+						index = parameter.find("value")
+						parameter = parameter[index+len("value"):]
+						value = stripping(parameter)
+
+					elif "method" in parameter:
+						if parameter[0] == "(":
+							parameter = parameter[1:]
+						if parameter[-1] == ")":
+							parameter = parameter[:-1]
+						index = parameter.find("method")
+						parameter = parameter[index+len("method"):]
+						method = stripping(parameter)
+				if value != "" and method != "":
+					server_endpoints.append(create_endpoint(value, method))
+		if api_post_request in line:
+			index = line.find(api_post_request)
+			line = line[index+len(api_post_request):]
+			line = line[2:-3]
+			if endpoint_prefix[0] == "/":
+				server_endpoints.append(create_endpoint(endpoint_prefix + line, "POST"))
+			else:
+				server_endpoints.append(create_endpoint(line, "POST"))
+		if api_get_request in line:
+			index = line.find(api_get_request)
+			line = line[index+len(api_get_request):]
+			line = line[2:-3]
+			if endpoint_prefix[0] == "/":
+				server_endpoints.append(create_endpoint(endpoint_prefix + line, "GET"))
+			else:
+				server_endpoints.append(create_endpoint(line, "GET"))
+			
+
+
+# for se in server_endpoints:
+# 	print(se)
+
+# print("count: {}".format(len(server_endpoints)))
+
+
+wrapper_endpoints = []
+
+wrapper_path = "../"
+wrapper_fp = wrapper_path + "endpoints/"
+files = [f for f in listdir(wrapper_fp) if isfile(join(wrapper_fp, f))]
+if "__init__.py" in files:
+	files.remove("__init__.py")
+
+for f_n in files:
+	file_path = wrapper_fp + f_n
+	f = open(file_path, "r")
+	data = f.read()
+	data = "".join(data.split())
+	while True:
+		index = data.find("{")
+		if index == -1:
+			break
+		open_count = 0
+		close_count = 0
+		for i in range(len(data[index:])):
+			c = data[i+index]
+			if c == "}":
+				close_count += 1
+			if c == "{":
+				open_count += 1
+			if open_count == close_count:
+				s = data[index: index+i+1]
+				j_str = eval(s)
+				# j_str = json.loads(s)
+				wrapper_endpoints.append(create_endpoint(j_str["endpoint"], j_str["type"]))
+				data = data[index+i:]
+				break
+
+# for we in wrapper_endpoints:
+# 	print(we)
+
+# print("count: {}".format(len(wrapper_endpoints)))
+
 compare_endpoints(server_endpoints, wrapper_endpoints)
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/apis/predictor_engine.py` & `ecosystem-notebooks-0.1.6/runtime/apis/predictor_engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,252 @@
-from runtime.endpoints import predictor_engine as endpoints
-from runtime import request_utils
-
-
-def get_spending_personality(auth, campaign, channel, customer, headers, params, subcampaign, userid, info=False):
-# Provide spending personality scores for customers.
-#   auth: Authentication token generated by access.Authenticate()
-#   campaign: The name of the campaign. (string)
-#   channel: The type of channel. (options: "all", "") 
-#   customer: The id of the customer. (string)
-#   headers: Added headers. ()
-#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
-#   subcampaign: Name of the subcampaigns. (string)
-#   userid: The id of the user. (string)
-    ep = endpoints.GET_SPENDING_PERSONALITY
-    param_dict = {
-        "campaign": campaign, 
-        "channel": channel,
-        "customer": customer,
-        "headers": headers,
-        "params": params,
-        "subcampaign": subcampaign,
-        "userid": userid
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_spending_personality(auth, document, headers, info=False):
-# Update offers taken up by customers
-#  document: Documents to be updated. ()
-#  headers: Added headers. ()
-    ep = endpoints.PUT_SPENDING_PERSONALITY
-    param_dict = {
-        "document": document, 
-        "headers": headers
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def model_detail(auth, model, info=False):
-# Model details. 
-# model: Model's details to examine. Example parameter: {'mojo':'my_mojo.zip'}
-    ep = endpoints.GET_OFFER_RECOMMENDATIONS
-    param_dict = {
-        "model": model
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_offer_recommendations(auth, campaign, channel, customer, headers, numberoffers, params, subcampaign, userid, info=False):
-# Provide offers that form part of a campaign for particular customer.
-#   auth: Authentication token generated by access.Authenticate()
-#   campaign: The name of the campaign. (string)
-#   channel: The type of channel. (options: "all", "") 
-#   customer: The id of the customer. (string)
-#   headers: Added headers. ()
-#   numberoffers: Number of offers to get. (int)
-#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
-#   subcampaign: Name of the subcampaigns. (string)
-#   userid: The id of the user. (string)
-    ep = endpoints.GET_OFFER_RECOMMENDATIONS
-    param_dict = {
-        "campaign": campaign, 
-        "channel": channel,
-        "customer": customer,
-        "headers": headers,
-        "numberoffers": numberoffers,
-        "params": params,
-        "subcampaign": subcampaign,
-        "userid": userid
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_offer_recommendations(auth, document, headers, info=False):
-# Update offers taken up by customers
-#  document: Documents to be updated. ()
-#  headers: Added headers. ()
-    ep = endpoints.PUT_OFFER_RECOMMENDATIONS
-    param_dict = {
-        "document": document, 
-        "headers": headers
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_personality_recommender(auth, campaign, channel, customer, headers, numberoffers, params, subcampaign, userid, info=False):
-# Provide offers that form part of a campaign for particular customer.
-#   auth: Authentication token generated by access.Authenticate()
-#   campaign: The name of the campaign. (string)
-#   channel: The type of channel. (options: "all", "") 
-#   customer: The id of the customer. (string)
-#   headers: Added headers. ()
-#   numberoffers: Number of offers to get. (int)
-#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
-#   subcampaign: Name of the subcampaigns. (string)
-#   userid: The id of the user. (string)
-    ep = endpoints.GET_PERSONALITY_RECOMMENDER
-    param_dict = {
-        "campaign": campaign, 
-        "channel": channel,
-        "customer": customer,
-        "headers": headers,
-        "numberoffers": numberoffers,
-        "params": params,
-        "subcampaign": subcampaign,
-        "userid": userid
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_personality_recommender(auth, document, headers, info=False):
-# Update offers taken up by customers
-#  document: Documents to be updated. ()
-#  headers: Added headers. ()
-    ep = endpoints.PUT_PERSONALITY_RECOMMENDER
-    param_dict = {
-        "document": document, 
-        "headers": headers
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def predictor_response_preload(auth, detail, value, info=False):
-# Perform prediction on pre-loaded model with detail: none, basic or all. 
-# Perform a database lookup if properties file has been set. 
-# The predictor parameters are broken into two types namely, 
-# requiring all parameters via API or requiring a lookup key via API and extracting parameters from a data source.
-# Use this format for input prams only:
-# Update offers taken up by customers
-#  detail: Documents to be updated. (string: "none", "basic", "all")
-#  value: Input parameter. 
-#  {
-#   'name':'predict1', 
-#   'mojo':'model_mojo.zip',
-#   'dbparam':false,
-#   'input': ['x','y'],
-#   'value': ['val_x', 'val_y']
-#  }
-# Use this approach for inputs from data source: 
-#  {
-#   'name':'predict1', 
-#   'mojo':'model_mojo.zip',
-#   'dbparam':true, 
-#   'lookup':{key:'customer',value:1234567890}
-#  } 
-# For post-scoring logic, then use this configuration:
-#  {
-#   'name':'predict1', 
-#   'mojo':'1',
-#   'mab':{'class':'mabone', 'epsilon':0.4},
-#   'dbparam':true, 
-#   'lookup':{key:'customer',value:1234567890}, 
-#   'param':{key:'value_field', value:30}
-#}
-    ep = endpoints.PREDICTOR_RESPONSE_PRELOAD
-    param_dict = {
-        "detail": detail, 
-        "value": value
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def predictor_response_preload_kafka(auth, detail, value, info=False):
-# Perform prediction on pre-loaded model with detail and push onto Kafka topic: none, basic or all.
-# Perform a database lookup if properties file has been set. 
-#  detail: Documents to be updated. (string: "none", "basic", "all")
-#  value: Input parameter. 
-#  {
-#    'name':'predict1', 
-#    'kafka':{'TOPIC_NAME':'ecosystem1','log':'true'},
-#    'mojo':'1', 'input':['x','y'], 
-#    'value':['val_x','val_y']
-#  } 
-#  OR 
-#  {
-#    'name':'predict1',
-#    'kafka':{'TOPIC_NAME':'ecosystem1','log':'true'},
-#    'mojo':'1',
-#    'dbparam':true,
-#    'lookup':{key:'customer',value:'1234567890'} 
-#  }
-    ep = endpoints.PREDICTOR_RESPONSE_PRELOAD_KAFKA
-    param_dict = {
-        "detail": detail, 
-        "value": value
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def refresh(auth, headers, info=False):
-# Refresh product matrix and master
-#  headers: Added headers. ()
-    ep = endpoints.REFRESH
-    param_dict = {
-        "headers": headers
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def run_model_mojo(auth, detail, value, info=False):
-# Perform basic prediction on model with detail: none, basic or all. 
-#  detail: Documents to be updated. (string: "none", "basic", "all")
-#  value: Input parameter.
-#  {
-#    'mojo':'model_mojo.zip',
-#    'input': ['x','y'],
-#    'value': ['val_x', 'val_y']
-#  }
-    ep = endpoints.RUN_MODEL_MOJO
-    param_dict = {
-        "detail": detail, 
-        "value": value
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def invocations(auth, json, info=False):
-    ep = endpoints.INVOCATIONS
-    resp = request_utils.create(auth, ep, json=json, info=info)
-    meta = resp.json()
-    return meta
-
-def response(auth, json, info=False):
-    ep = endpoints.RESPONSE
-    resp = request_utils.create(auth, ep, json=json, info=info)
-    meta = resp.json()
-    return meta
-
-def process_batch(auth, json, info=False):
-    ep = endpoints.PROCESS_BATCH
-    resp = request_utils.create(auth, ep, json=json, info=info)
-    meta = resp.json()
-    return meta
-
-def generate_key(auth, info=False):
-    ep = endpoints.GENERATE_KEY
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
+from runtime.endpoints import predictor_engine as endpoints
+from runtime import request_utils
+
+
+def get_spending_personality(auth, campaign, channel, customer, headers, params, subcampaign, userid, info=False):
+# Provide spending personality scores for customers.
+#   auth: Authentication token generated by access.Authenticate()
+#   campaign: The name of the campaign. (string)
+#   channel: The type of channel. (options: "all", "") 
+#   customer: The id of the customer. (string)
+#   headers: Added headers. ()
+#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
+#   subcampaign: Name of the subcampaigns. (string)
+#   userid: The id of the user. (string)
+    ep = endpoints.GET_SPENDING_PERSONALITY
+    param_dict = {
+        "campaign": campaign, 
+        "channel": channel,
+        "customer": customer,
+        "headers": headers,
+        "params": params,
+        "subcampaign": subcampaign,
+        "userid": userid
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_spending_personality(auth, document, headers, info=False):
+# Update offers taken up by customers
+#  document: Documents to be updated. ()
+#  headers: Added headers. ()
+    ep = endpoints.PUT_SPENDING_PERSONALITY
+    param_dict = {
+        "document": document, 
+        "headers": headers
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def model_detail(auth, model, info=False):
+# Model details. 
+# model: Model's details to examine. Example parameter: {'mojo':'my_mojo.zip'}
+    ep = endpoints.GET_OFFER_RECOMMENDATIONS
+    param_dict = {
+        "model": model
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_offer_recommendations(auth, campaign, channel, customer, headers, numberoffers, params, subcampaign, userid, info=False):
+# Provide offers that form part of a campaign for particular customer.
+#   auth: Authentication token generated by access.Authenticate()
+#   campaign: The name of the campaign. (string)
+#   channel: The type of channel. (options: "all", "") 
+#   customer: The id of the customer. (string)
+#   headers: Added headers. ()
+#   numberoffers: Number of offers to get. (int)
+#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
+#   subcampaign: Name of the subcampaigns. (string)
+#   userid: The id of the user. (string)
+    ep = endpoints.GET_OFFER_RECOMMENDATIONS
+    param_dict = {
+        "campaign": campaign, 
+        "channel": channel,
+        "customer": customer,
+        "headers": headers,
+        "numberoffers": numberoffers,
+        "params": params,
+        "subcampaign": subcampaign,
+        "userid": userid
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_offer_recommendations(auth, document, headers, info=False):
+# Update offers taken up by customers
+#  document: Documents to be updated. ()
+#  headers: Added headers. ()
+    ep = endpoints.PUT_OFFER_RECOMMENDATIONS
+    param_dict = {
+        "document": document, 
+        "headers": headers
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_personality_recommender(auth, campaign, channel, customer, headers, numberoffers, params, subcampaign, userid, info=False):
+# Provide offers that form part of a campaign for particular customer.
+#   auth: Authentication token generated by access.Authenticate()
+#   campaign: The name of the campaign. (string)
+#   channel: The type of channel. (options: "all", "") 
+#   customer: The id of the customer. (string)
+#   headers: Added headers. ()
+#   numberoffers: Number of offers to get. (int)
+#   params: Addtional parameters added in a dictionary format as a string: ('{"value_1": 300, "value_2": "entry"}')
+#   subcampaign: Name of the subcampaigns. (string)
+#   userid: The id of the user. (string)
+    ep = endpoints.GET_PERSONALITY_RECOMMENDER
+    param_dict = {
+        "campaign": campaign, 
+        "channel": channel,
+        "customer": customer,
+        "headers": headers,
+        "numberoffers": numberoffers,
+        "params": params,
+        "subcampaign": subcampaign,
+        "userid": userid
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_personality_recommender(auth, document, headers, info=False):
+# Update offers taken up by customers
+#  document: Documents to be updated. ()
+#  headers: Added headers. ()
+    ep = endpoints.PUT_PERSONALITY_RECOMMENDER
+    param_dict = {
+        "document": document, 
+        "headers": headers
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def predictor_response_preload(auth, detail, value, info=False):
+# Perform prediction on pre-loaded model with detail: none, basic or all. 
+# Perform a database lookup if properties file has been set. 
+# The predictor parameters are broken into two types namely, 
+# requiring all parameters via API or requiring a lookup key via API and extracting parameters from a data source.
+# Use this format for input prams only:
+# Update offers taken up by customers
+#  detail: Documents to be updated. (string: "none", "basic", "all")
+#  value: Input parameter. 
+#  {
+#   'name':'predict1', 
+#   'mojo':'model_mojo.zip',
+#   'dbparam':false,
+#   'input': ['x','y'],
+#   'value': ['val_x', 'val_y']
+#  }
+# Use this approach for inputs from data source: 
+#  {
+#   'name':'predict1', 
+#   'mojo':'model_mojo.zip',
+#   'dbparam':true, 
+#   'lookup':{key:'customer',value:1234567890}
+#  } 
+# For post-scoring logic, then use this configuration:
+#  {
+#   'name':'predict1', 
+#   'mojo':'1',
+#   'mab':{'class':'mabone', 'epsilon':0.4},
+#   'dbparam':true, 
+#   'lookup':{key:'customer',value:1234567890}, 
+#   'param':{key:'value_field', value:30}
+#}
+    ep = endpoints.PREDICTOR_RESPONSE_PRELOAD
+    param_dict = {
+        "detail": detail, 
+        "value": value
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def predictor_response_preload_kafka(auth, detail, value, info=False):
+# Perform prediction on pre-loaded model with detail and push onto Kafka topic: none, basic or all.
+# Perform a database lookup if properties file has been set. 
+#  detail: Documents to be updated. (string: "none", "basic", "all")
+#  value: Input parameter. 
+#  {
+#    'name':'predict1', 
+#    'kafka':{'TOPIC_NAME':'ecosystem1','log':'true'},
+#    'mojo':'1', 'input':['x','y'], 
+#    'value':['val_x','val_y']
+#  } 
+#  OR 
+#  {
+#    'name':'predict1',
+#    'kafka':{'TOPIC_NAME':'ecosystem1','log':'true'},
+#    'mojo':'1',
+#    'dbparam':true,
+#    'lookup':{key:'customer',value:'1234567890'} 
+#  }
+    ep = endpoints.PREDICTOR_RESPONSE_PRELOAD_KAFKA
+    param_dict = {
+        "detail": detail, 
+        "value": value
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def refresh(auth, headers, info=False):
+# Refresh product matrix and master
+#  headers: Added headers. ()
+    ep = endpoints.REFRESH
+    param_dict = {
+        "headers": headers
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def run_model_mojo(auth, detail, value, info=False):
+# Perform basic prediction on model with detail: none, basic or all. 
+#  detail: Documents to be updated. (string: "none", "basic", "all")
+#  value: Input parameter.
+#  {
+#    'mojo':'model_mojo.zip',
+#    'input': ['x','y'],
+#    'value': ['val_x', 'val_y']
+#  }
+    ep = endpoints.RUN_MODEL_MOJO
+    param_dict = {
+        "detail": detail, 
+        "value": value
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def invocations(auth, json, info=False):
+    ep = endpoints.INVOCATIONS
+    resp = request_utils.create(auth, ep, json=json, info=info)
+    print(resp)
+    meta = resp.json()
+    return meta
+
+def response(auth, json, info=False):
+    ep = endpoints.RESPONSE
+    resp = request_utils.create(auth, ep, json=json, info=info)
+    meta = resp.json()
+    return meta
+
+def process_batch(auth, json, info=False):
+    ep = endpoints.PROCESS_BATCH
+    resp = request_utils.create(auth, ep, json=json, info=info)
+    meta = resp.json()
+    return meta
+
+def generate_key(auth, info=False):
+    ep = endpoints.GENERATE_KEY
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
     return meta
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/apis/runtime_engine.py` & `ecosystem-notebooks-0.1.6/runtime/apis/runtime_engine.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from runtime.endpoints import runtime_engine as endpoints
-from runtime import request_utils
-import requests
-
-# Get Login
-def login(auth, info=False):
-    ep = endpoints.LOGIN
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
-    return meta
-
-# Ping server and provide response
-#   message: The message to return. (string)
-def ping(auth, message, info=False):
-    ep = endpoints.PING
-    param_dict = {
-        "message": message
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def no_auth_ping(server, endpoint, headers, message, info=False):
-    url_endpoint = server + endpoint
-    param_dict = {
-        "message": message
-    }
-    resp = requests.get(url_endpoint, headers=headers, params=param_dict)
-    meta = resp.json()
+from runtime.endpoints import runtime_engine as endpoints
+from runtime import request_utils
+import requests
+
+# Get Login
+def login(auth, info=False):
+    ep = endpoints.LOGIN
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
+    return meta
+
+# Ping server and provide response
+#   message: The message to return. (string)
+def ping(auth, message, info=False):
+    ep = endpoints.PING
+    param_dict = {
+        "message": message
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def no_auth_ping(server, endpoint, headers, message, info=False):
+    url_endpoint = server + endpoint
+    param_dict = {
+        "message": message
+    }
+    resp = requests.get(url_endpoint, headers=headers, params=param_dict)
+    meta = resp.json()
     return meta
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/apis/worker_utilities.py` & `ecosystem-notebooks-0.1.6/runtime/apis/worker_utilities.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,403 +1,403 @@
-from runtime.endpoints import worker_utilities as endpoints
-from runtime import request_utils
-
-def send_get(auth, path, proxy, port, info=False):
-    ep = endpoints.SEND_GET
-    param_dict = {
-        "path": path, 
-        "proxy": proxy,
-        "port": port
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_rest(auth, path, info=False):
-    ep = endpoints.GET_REST
-    param_dict = {
-        "path": path
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_cassandra(auth, sql, c_type, info=False):
-# Cassandra database select
-#   auth: Authentication token generated by access.Authenticate()
-#   sql: select sql target. Default value: select release_version from system.local
-#   c_type: Default value: c OR r
-    ep = endpoints.GET_CASSANDRA
-    param_dict = {
-        "sql": sql, 
-        "type": c_type
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_cassandra_version(auth, params, info=False):
-# Cassandra database version
-#   auth: Authentication token generated by access.Authenticate()
-#   params: (string)
-    ep = endpoints.GET_CASSANDRA_VERSION
-    param_dict = {
-        "params": params
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_file(auth, file_name, lines, info=False):
-# Obtain log file: Retrive number of lines from file.
-#   auth: Authentication token generated by access.Authenticate()
-#   file_name: file to read (str)
-#   lines: number of lines to read (int)
-    ep = endpoints.GET_FILE
-    param_dict = {
-        "file": file_name, 
-        "lines": lines
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_file_list(auth, info=False):
-    ep = endpoints.GET_FILE_LIST
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
-    return meta
-
-def get_ip(auth, info=False):
-# Get IP of server.
-#   auth: Authentication token generated by access.Authenticate()
-    ep = endpoints.GET_IP
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.json()
-    return meta
-
-def get_rest(auth, path, info=False):
-# REST Interface: 
-#    auth: Authentication token generated by access.Authenticate()
-#    path: '-noData -u user -p pass http://lo...' 
-#    use the -noData option to indicate the use of ecosystem API. 
-#    Define user and password for authentication with -u and -p path='-key result -u user -p pass http://lo...' 
-#    use the -key [keyvalue] option to indicate the use of API where document is in JSON key.
-    ep = endpoints.GET_REST
-    param_dict = {
-        "path": path
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def list_to_matrix(auth, params, info=False):
-# Create matrix from transcation list from properties file as setup in budget tracker.
-#   auth: Authentication token generated by access.Authenticate()
-#   params: {type:'csv'} or {type:'json'}
-    ep = endpoints.LIST_TO_MATRIX
-    param_dict = {
-        "params": params
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def matrix_to_list(auth, params, info=False):
-# Create list from matrix, import csv file.
-#   auth: Authentication token generated by access.Authenticate()
-#   params: {test: true, file:'./file.csv'} (use test setting to check before update)
-    ep = endpoints.MATRIX_TO_LIST
-    param_dict = {
-        "params": params
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def pull_kafka_topic(auth, message, params, info=False):
-# Pull message from Kafka topic
-#   auth: Authentication token generated by access.Authenticate()
-#   message: Default value : [{}]
-#   params: Default value : [{"TOPIC_NAME":"ecosystem1","log":"true"}]
-    ep = endpoints.PULL_KAFKA_TOPIC
-    param_dict = {
-        "message": message, 
-        "params": params
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def push_kafka_topic(auth, message, params, info=False):
-    ep = endpoints.PULL_KAFKA_TOPIC
-    param_dict = {
-        "message": message, 
-        "params": params
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def upload_file(auth, path, target_path, info=False):
-    ep = endpoints.UPLOAD_FILE
-    fileFp = open(path, "rb")
-    files = {"file": fileFp}
-    data = {"path": target_path}
-    resp = request_utils.create_only_auth(auth, ep, data=data, files=files, info=info)
-    return resp
-
-def file_database_import(auth, database, collection, file_name, info=False):
-    ep = endpoints.FILE_DATABASE_IMPORT
-    param_dict = {
-        "database": database,
-        "collection": collection,
-        "file": file_name
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def get_property(auth, property_key, info=False):
-	ep = endpoints.GET_PROPERTY
-	param_dict = {
-		"key": property_key
-	}
-	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
-	data = resp.content.decode("utf-8")
-	return data
-
-def update_properties(auth, properties, info=False):
-    ep = endpoints.UPDATE_PROPERTIES
-    resp = request_utils.create_only_auth(auth, ep, data=properties, info=info)
-    return resp
-
-def update_properties_key(auth, key, value, info=False):
-	ep = endpoints.UPDATE_PROPERTIES_KEY
-	param_dict = {
-		"key": key,
-		"value": value
-	}
-	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
-	data = resp.content.decode("utf-8")
-	return data
-
-def refresh(auth, info=False):
-    ep = endpoints.REFRESH
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.content
-    return meta
-
-def get_spend_personality(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
-    ep = endpoints.GET_SPEND_PERSONALITY
-    param_dict = {
-      "campaign": campaign,
-      "channel": channel, 
-      "customer":customer, 
-      "params":params, 
-      "subcampaign":subcampaign, 
-      "userid":userid}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def get_financial_wellness(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
-    ep = endpoints.GET_FINANCIAL_WELLNESS
-    param_dict = {"campaign": campaign,
-                  "channel": channel, 
-                  "customer":customer, 
-                  "params":params, 
-                  "subcampaign":subcampaign, 
-                  "userid":userid}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_financial_wellness(auth, document, info=False):
-    ep = endpoints.PUT_FINANCIAL_WELLNESS
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def sql_cassandra(auth, sql, info=False):
-    ep = endpoints.SQL_CASSANDRA
-    param_dict = {
-        "sql": sql,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def close_cassandra(auth, info=False):
-    ep = endpoints.CLOSE_CASSANDRA
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.content
-    return meta	
-
-
-def test_kafka_kerberos(auth, info=False):
-    ep = endpoints.TEST_KAFKA_KERBEROS
-    resp = request_utils.create(auth, ep, info=info)
-    meta = resp.content
-    return meta	
-    
-
-def estore_recommendations(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
-    ep = endpoints.ESTORE_RECOMMENDATIONS
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def put_estore_recommendations(auth, document, info=False):
-    ep = endpoints.PUT_ESTORE_RECOMMENDATIONS
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def connect_u(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
-    ep = endpoints.CONNECT_U
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def put_connect_u(auth, document, info=False):
-    ep = endpoints.PUT_CONNECT_U
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def just_for_you(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
-    ep = endpoints.JUST_FOR_YOU
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def put_just_for_you(auth, document, info=False):
-    ep = endpoints.PUT_JUST_FOR_YOU
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def estore_recommender_non_gsm(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
-    ep = endpoints.ESTORE_RECOMMENDER_NON_GSM
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-
-def put_estore_recommender_non_gsm(auth, document, info=False):
-    ep = endpoints.PUT_ESTORE_RECOMMENDER_NON_GSM
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def gift_recommendations_free(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, transaction_id, info=False):
-    ep = endpoints.GIFT_RECOMMENDATIONS_FREE
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params,
-                  "transaction_id":transaction_id}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def gift_recommendations_purchased(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, transaction_id, info=False):
-    ep = endpoints.GIFT_RECOMMENDATIONS_PURCHASED
-    param_dict = {"msisdn": msisdn,
-                  "payment_method": payment_method, 
-                  "campaign_id":campaign_id, 
-                  "sub_campaign_id":sub_campaign_id, 
-                  "channel_name":channel_name, 
-                  "number_of_offers":number_of_offers, 
-                  "user_id":user_id, 
-                  "params":params,
-                  "transaction_id":transaction_id}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_gift_recommendations(auth, document, info=False):
-    ep = endpoints.GIFT_RECOMMENDATIONS
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def behavior_recommender(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
-    ep = endpoints.BEHAVIOR_RECOMMENDER
-    param_dict = {"campaign": campaign, 
-                  "subcampaign":subcampaign, 
-                  "customer":customer, 
-                  "channel":channel, 
-                  "userid":userid, 
-                  "params":params}
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
-    return meta
-
-def put_behavior_recommender(auth, document, info=False):
-    ep = endpoints.PUT_BEHAVIOR_RECOMMENDER
-    param_dict = {
-        "document": document,
-    }
-    resp = request_utils.create(auth, ep, params=param_dict, info=info)
-    meta = resp.json()
+from runtime.endpoints import worker_utilities as endpoints
+from runtime import request_utils
+
+def send_get(auth, path, proxy, port, info=False):
+    ep = endpoints.SEND_GET
+    param_dict = {
+        "path": path, 
+        "proxy": proxy,
+        "port": port
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_rest(auth, path, info=False):
+    ep = endpoints.GET_REST
+    param_dict = {
+        "path": path
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_cassandra(auth, sql, c_type, info=False):
+# Cassandra database select
+#   auth: Authentication token generated by access.Authenticate()
+#   sql: select sql target. Default value: select release_version from system.local
+#   c_type: Default value: c OR r
+    ep = endpoints.GET_CASSANDRA
+    param_dict = {
+        "sql": sql, 
+        "type": c_type
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_cassandra_version(auth, params, info=False):
+# Cassandra database version
+#   auth: Authentication token generated by access.Authenticate()
+#   params: (string)
+    ep = endpoints.GET_CASSANDRA_VERSION
+    param_dict = {
+        "params": params
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_file(auth, file_name, lines, info=False):
+# Obtain log file: Retrive number of lines from file.
+#   auth: Authentication token generated by access.Authenticate()
+#   file_name: file to read (str)
+#   lines: number of lines to read (int)
+    ep = endpoints.GET_FILE
+    param_dict = {
+        "file": file_name, 
+        "lines": lines
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_file_list(auth, info=False):
+    ep = endpoints.GET_FILE_LIST
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
+    return meta
+
+def get_ip(auth, info=False):
+# Get IP of server.
+#   auth: Authentication token generated by access.Authenticate()
+    ep = endpoints.GET_IP
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.json()
+    return meta
+
+def get_rest(auth, path, info=False):
+# REST Interface: 
+#    auth: Authentication token generated by access.Authenticate()
+#    path: '-noData -u user -p pass http://lo...' 
+#    use the -noData option to indicate the use of ecosystem API. 
+#    Define user and password for authentication with -u and -p path='-key result -u user -p pass http://lo...' 
+#    use the -key [keyvalue] option to indicate the use of API where document is in JSON key.
+    ep = endpoints.GET_REST
+    param_dict = {
+        "path": path
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def list_to_matrix(auth, params, info=False):
+# Create matrix from transcation list from properties file as setup in budget tracker.
+#   auth: Authentication token generated by access.Authenticate()
+#   params: {type:'csv'} or {type:'json'}
+    ep = endpoints.LIST_TO_MATRIX
+    param_dict = {
+        "params": params
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def matrix_to_list(auth, params, info=False):
+# Create list from matrix, import csv file.
+#   auth: Authentication token generated by access.Authenticate()
+#   params: {test: true, file:'./file.csv'} (use test setting to check before update)
+    ep = endpoints.MATRIX_TO_LIST
+    param_dict = {
+        "params": params
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def pull_kafka_topic(auth, message, params, info=False):
+# Pull message from Kafka topic
+#   auth: Authentication token generated by access.Authenticate()
+#   message: Default value : [{}]
+#   params: Default value : [{"TOPIC_NAME":"ecosystem1","log":"true"}]
+    ep = endpoints.PULL_KAFKA_TOPIC
+    param_dict = {
+        "message": message, 
+        "params": params
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def push_kafka_topic(auth, message, params, info=False):
+    ep = endpoints.PULL_KAFKA_TOPIC
+    param_dict = {
+        "message": message, 
+        "params": params
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def upload_file(auth, path, target_path, info=False):
+    ep = endpoints.UPLOAD_FILE
+    fileFp = open(path, "rb")
+    files = {"file": fileFp}
+    data = {"path": target_path}
+    resp = request_utils.create_only_auth(auth, ep, data=data, files=files, info=info)
+    return resp
+
+def file_database_import(auth, database, collection, file_name, info=False):
+    ep = endpoints.FILE_DATABASE_IMPORT
+    param_dict = {
+        "database": database,
+        "collection": collection,
+        "file": file_name
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def get_property(auth, property_key, info=False):
+	ep = endpoints.GET_PROPERTY
+	param_dict = {
+		"key": property_key
+	}
+	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
+	data = resp.content.decode("utf-8")
+	return data
+
+def update_properties(auth, properties, info=False):
+    ep = endpoints.UPDATE_PROPERTIES
+    resp = request_utils.create_only_auth(auth, ep, data=properties, info=info)
+    return resp
+
+def update_properties_key(auth, key, value, info=False):
+	ep = endpoints.UPDATE_PROPERTIES_KEY
+	param_dict = {
+		"key": key,
+		"value": value
+	}
+	resp = request_utils.create_only_auth(auth, ep, params=param_dict, info=info)
+	data = resp.content.decode("utf-8")
+	return data
+
+def refresh(auth, info=False):
+    ep = endpoints.REFRESH
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.content
+    return meta
+
+def get_spend_personality(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
+    ep = endpoints.GET_SPEND_PERSONALITY
+    param_dict = {
+      "campaign": campaign,
+      "channel": channel, 
+      "customer":customer, 
+      "params":params, 
+      "subcampaign":subcampaign, 
+      "userid":userid}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def get_financial_wellness(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
+    ep = endpoints.GET_FINANCIAL_WELLNESS
+    param_dict = {"campaign": campaign,
+                  "channel": channel, 
+                  "customer":customer, 
+                  "params":params, 
+                  "subcampaign":subcampaign, 
+                  "userid":userid}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_financial_wellness(auth, document, info=False):
+    ep = endpoints.PUT_FINANCIAL_WELLNESS
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def sql_cassandra(auth, sql, info=False):
+    ep = endpoints.SQL_CASSANDRA
+    param_dict = {
+        "sql": sql,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def close_cassandra(auth, info=False):
+    ep = endpoints.CLOSE_CASSANDRA
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.content
+    return meta	
+
+
+def test_kafka_kerberos(auth, info=False):
+    ep = endpoints.TEST_KAFKA_KERBEROS
+    resp = request_utils.create(auth, ep, info=info)
+    meta = resp.content
+    return meta	
+    
+
+def estore_recommendations(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
+    ep = endpoints.ESTORE_RECOMMENDATIONS
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def put_estore_recommendations(auth, document, info=False):
+    ep = endpoints.PUT_ESTORE_RECOMMENDATIONS
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def connect_u(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
+    ep = endpoints.CONNECT_U
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def put_connect_u(auth, document, info=False):
+    ep = endpoints.PUT_CONNECT_U
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def just_for_you(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
+    ep = endpoints.JUST_FOR_YOU
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def put_just_for_you(auth, document, info=False):
+    ep = endpoints.PUT_JUST_FOR_YOU
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def estore_recommender_non_gsm(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, info=False):
+    ep = endpoints.ESTORE_RECOMMENDER_NON_GSM
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+
+def put_estore_recommender_non_gsm(auth, document, info=False):
+    ep = endpoints.PUT_ESTORE_RECOMMENDER_NON_GSM
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def gift_recommendations_free(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, transaction_id, info=False):
+    ep = endpoints.GIFT_RECOMMENDATIONS_FREE
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params,
+                  "transaction_id":transaction_id}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def gift_recommendations_purchased(auth, msisdn, payment_method, campaign_id, sub_campaign_id, channel_name, number_of_offers, user_id, params, transaction_id, info=False):
+    ep = endpoints.GIFT_RECOMMENDATIONS_PURCHASED
+    param_dict = {"msisdn": msisdn,
+                  "payment_method": payment_method, 
+                  "campaign_id":campaign_id, 
+                  "sub_campaign_id":sub_campaign_id, 
+                  "channel_name":channel_name, 
+                  "number_of_offers":number_of_offers, 
+                  "user_id":user_id, 
+                  "params":params,
+                  "transaction_id":transaction_id}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_gift_recommendations(auth, document, info=False):
+    ep = endpoints.GIFT_RECOMMENDATIONS
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def behavior_recommender(auth, campaign, channel, customer, params, subcampaign, userid, info=False):
+    ep = endpoints.BEHAVIOR_RECOMMENDER
+    param_dict = {"campaign": campaign, 
+                  "subcampaign":subcampaign, 
+                  "customer":customer, 
+                  "channel":channel, 
+                  "userid":userid, 
+                  "params":params}
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
+    return meta
+
+def put_behavior_recommender(auth, document, info=False):
+    ep = endpoints.PUT_BEHAVIOR_RECOMMENDER
+    param_dict = {
+        "document": document,
+    }
+    resp = request_utils.create(auth, ep, params=param_dict, info=info)
+    meta = resp.json()
     return meta
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/endpoints/predictor_engine.py` & `ecosystem-notebooks-0.1.6/runtime/endpoints/predictor_engine.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-GET_SPENDING_PERSONALITY = {
-	"type": "get",
-	"endpoint": "/getSpendingPersonality",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PUT_SPENDING_PERSONALITY = {
-	"type": "put",
-	"endpoint": "/getSpendingPersonality",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-MODEL_DETAIL = {
-	"type": "get",
-	"endpoint": "/modelDetail",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_OFFER_RECOMMENDATIONS = {
-	"type": "get",
-	"endpoint": "/offerRecommendations",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PUT_OFFER_RECOMMENDATIONS = {
-	"type": "put",
-	"endpoint": "/offerRecommendations",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GET_PERSONALITY_RECOMMENDER = {
-	"type": "get",
-	"endpoint": "/personalityRecommender",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PUT_PERSONALITY_RECOMMENDER = {
-	"type": "put",
-	"endpoint": "/personalityRecommender",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PREDICTOR_RESPONSE_PRELOAD = {
-	"type": "get",
-	"endpoint": "/predictorResponsePreLoad",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PREDICTOR_RESPONSE_PRELOAD_KAFKA = {
-	"type": "get",
-	"endpoint": "/predictorResponsePreLoadKafKa",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-REFRESH = {
-	"type": "get",
-	"endpoint": "/refresh",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-RUN_MODEL_MOJO = {
-	"type": "get",
-	"endpoint": "/runModelMojo",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-INVOCATIONS = {
-	"type": "post",
-	"endpoint": "/invocations",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-RESPONSE = {
-	"type": "post",
-	"endpoint": "/response",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-PROCESS_BATCH = {
-	"type": "post",
-	"endpoint": "/processBatch",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"
-}
-GENERATE_KEY = {
-	"type": "get",
-	"endpoint": "/generateKey",
-	"call_message": "{type} {endpoint}",
-	"error_message": "{type} {endpoint} {response_code}"	
+GET_SPENDING_PERSONALITY = {
+	"type": "get",
+	"endpoint": "/getSpendingPersonality",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PUT_SPENDING_PERSONALITY = {
+	"type": "put",
+	"endpoint": "/getSpendingPersonality",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+MODEL_DETAIL = {
+	"type": "get",
+	"endpoint": "/modelDetail",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_OFFER_RECOMMENDATIONS = {
+	"type": "get",
+	"endpoint": "/offerRecommendations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PUT_OFFER_RECOMMENDATIONS = {
+	"type": "put",
+	"endpoint": "/offerRecommendations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GET_PERSONALITY_RECOMMENDER = {
+	"type": "get",
+	"endpoint": "/personalityRecommender",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PUT_PERSONALITY_RECOMMENDER = {
+	"type": "put",
+	"endpoint": "/personalityRecommender",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PREDICTOR_RESPONSE_PRELOAD = {
+	"type": "get",
+	"endpoint": "/predictorResponsePreLoad",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PREDICTOR_RESPONSE_PRELOAD_KAFKA = {
+	"type": "get",
+	"endpoint": "/predictorResponsePreLoadKafKa",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+REFRESH = {
+	"type": "get",
+	"endpoint": "/refresh",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+RUN_MODEL_MOJO = {
+	"type": "get",
+	"endpoint": "/runModelMojo",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+INVOCATIONS = {
+	"type": "post",
+	"endpoint": "/invocations",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+RESPONSE = {
+	"type": "post",
+	"endpoint": "/response",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+PROCESS_BATCH = {
+	"type": "post",
+	"endpoint": "/processBatch",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"
+}
+GENERATE_KEY = {
+	"type": "get",
+	"endpoint": "/generateKey",
+	"call_message": "{type} {endpoint}",
+	"error_message": "{type} {endpoint} {response_code}"	
 }
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/request_utils.py` & `ecosystem-notebooks-0.1.6/runtime/request_utils.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import requests
-from requests import RequestException
-
-class RequestTypeError(Exception):
-	"""Exception raised for non existant request type."""
-	def __init__(self, t):
-		message = "Non existant request type: {}.".format(t)
-		super().__init__(message)
-
-class ApiError(IOError):
-	"""There was an ambiguous exception that occurred while handling your
-		request.
-		"""
-	def __init__(self, *args, **kwargs):
-		"""Initialize RequestException with `request` and `response` objects."""
-		response = kwargs.pop('response', None)
-		self.response = response
-		self.request = kwargs.pop('request', None)
-		if (response is not None and not self.request and
-			hasattr(response, 'request')):
-			self.request = self.response.request
-			# super(RequestException, self).__init__(*args, **kwargs) TODO: this gives errors, might not be neccesay.
-			super().__init__(*args, **kwargs)
-
-def auto_format_params(d):
-	s = ""
-	for key in d:
-		d[key] = str(d[key])
-		s += "{key}={{{key}}}&".format(key=key)
-	return s.format(**d)
-
-def get_type(t):
-	if t == "get":
-		return requests.get
-	elif t == "post":
-		return requests.post
-	elif t == "put":
-		return requests.put
-	elif t == "delete":
-		return requests.delete
-	elif t == "patch":
-		return requests.patch
-	else:
-		raise RequestTypeError(t)
-
-def create_only_auth(auth, endpoint, info=False, **kwargs):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	print(call_message)
-	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
-	if resp.status_code != 200:
-		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
-		print(error_message)
-		raise ApiError(error_message, response=resp)
-	return resp
-
-def create_only_auth_no_error(auth, endpoint, info=False, **kwargs):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	print(call_message)
-	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
-	return resp
-
-def create(auth, endpoint, json=None, data=None, params=None, ep_arg=None, info=False):
-	url_endpoint = auth.get_server() + endpoint["endpoint"]
-	if ep_arg != None:
-		url_endpoint = url_endpoint + ep_arg
-	resp = None
-	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
-	if json == None and data == None and params == None:
-		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False)
-	elif json == None and data == None:
-		call_message = call_message + "?" + auto_format_params(params)
-		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), params=params, verify=False)
-	elif params == None:
-		if json == None:
-			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), data=data, verify=False)
-		else:
-			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), json=json, verify=False)
-	else:
-		raise Exception("Error: Unsupported state: Both json and params parameters passed.")
-	if resp.status_code != 200:
-		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
-		print(error_message)
-		raise ApiError(error_message, response=resp)
-	if info:
-		print(call_message)
-		if json != None:
-			print("\t{}".format(json))
+import requests
+from requests import RequestException
+
+class RequestTypeError(Exception):
+	"""Exception raised for non existant request type."""
+	def __init__(self, t):
+		message = "Non existant request type: {}.".format(t)
+		super().__init__(message)
+
+class ApiError(IOError):
+	"""There was an ambiguous exception that occurred while handling your
+		request.
+		"""
+	def __init__(self, *args, **kwargs):
+		"""Initialize RequestException with `request` and `response` objects."""
+		response = kwargs.pop('response', None)
+		self.response = response
+		self.request = kwargs.pop('request', None)
+		if (response is not None and not self.request and
+			hasattr(response, 'request')):
+			self.request = self.response.request
+			# super(RequestException, self).__init__(*args, **kwargs) TODO: this gives errors, might not be neccesay.
+			super().__init__(*args, **kwargs)
+
+def auto_format_params(d):
+	s = ""
+	for key in d:
+		d[key] = str(d[key])
+		s += "{key}={{{key}}}&".format(key=key)
+	return s.format(**d)
+
+def get_type(t):
+	if t == "get":
+		return requests.get
+	elif t == "post":
+		return requests.post
+	elif t == "put":
+		return requests.put
+	elif t == "delete":
+		return requests.delete
+	elif t == "patch":
+		return requests.patch
+	else:
+		raise RequestTypeError(t)
+
+def create_only_auth(auth, endpoint, info=False, **kwargs):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	print(call_message)
+	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
+	if resp.status_code != 200:
+		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
+		print(error_message)
+		raise ApiError(error_message, response=resp)
+	return resp
+
+def create_only_auth_no_error(auth, endpoint, info=False, **kwargs):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	print(call_message)
+	resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False, **kwargs)
+	return resp
+
+def create(auth, endpoint, json=None, data=None, params=None, ep_arg=None, info=False):
+	url_endpoint = auth.get_server() + endpoint["endpoint"]
+	if ep_arg != None:
+		url_endpoint = url_endpoint + ep_arg
+	resp = None
+	call_message = endpoint["call_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"])
+	if json == None and data == None and params == None:
+		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), verify=False)
+	elif json == None and data == None:
+		call_message = call_message + "?" + auto_format_params(params)
+		resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), params=params, verify=False)
+	elif params == None:
+		if json == None:
+			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), data=data, verify=False)
+		else:
+			resp = get_type(endpoint["type"])(url_endpoint, headers=auth.get_auth_headers(), json=json, verify=False)
+	else:
+		raise Exception("Error: Unsupported state: Both json and params parameters passed.")
+	if resp.status_code != 200:
+		error_message = endpoint["error_message"].format(type=endpoint["type"], endpoint=endpoint["endpoint"], response_code=resp.status_code)
+		print(error_message)
+		raise ApiError(error_message, response=resp)
+	if info:
+		print(call_message)
+		if json != None:
+			print("\t{}".format(json))
 	return resp
```

### Comparing `ecosystem-notebooks-0.1.5/runtime/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.6/runtime/utils/endpoint_diff.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-from os import listdir
-from os.path import isfile, join
-import sys
-import json
-
-runtime_server_path = "C:/Users/Ramsay/Documents/GitHub/ecosystem-runtime/"
-runtime_fp = runtime_server_path + "src/main/java/com/ecosystem/runtime/"
-files = [f for f in listdir(runtime_fp) if isfile(join(runtime_fp, f))]
-
-server_endpoints = []
-api_request = "@RequestMapping"
-api_post_request = "@PostMapping"
-
-def stripping(parameter):
-	if parameter[0] == "=":
-		parameter = parameter[1:]
-	parameter = parameter.replace("'", "")
-	parameter = parameter.replace('"', "")
-	if parameter[0] == ":":
-		parameter = parameter[1:]
-	# if parameter[0] == '"' or parameter[0] == "'":
-	# 	parameter = parameter[1:]
-	# if parameter[-1] == '"' or parameter[-1] == "'":	
-	# 	parameter = parameter[:-1]
-	return parameter
-
-def create_endpoint(endpoint, method):
-	d = {
-		"endpoint": endpoint,
-		"method": method
-	}
-	return d
-
-def compare_endpoints(server_endpoints, wrapper_endpoints):
-	both = []
-	server = []
-	wrapper = []
-	for d in server_endpoints:
-		se = d["endpoint"]
-		sm = d["method"]
-		found = False
-		for d2 in wrapper_endpoints:
-			we = d2["endpoint"]
-			wm = d2["method"]
-			if se == we and wm.lower() in sm.lower():
-				both.append([d, d2])
-				found = True
-				break
-		if not found:
-			server.append(d)
-	for d2 in wrapper_endpoints:
-		we = d2["endpoint"]
-		wm = d2["method"]
-		found = False
-		for d in server_endpoints:
-			se = d["endpoint"]
-			sm = d["method"]
-			if se == we and wm.lower() in sm.lower():
-				found = True
-				break
-		if not found:
-			wrapper.append(d2)
-
-	print("")
-	print("Found in both:")
-	data = [
-		["----SERVER----", "", "", "----WRAPPER----", ""],
-		["method", "endpoint", "", "method", "endpoint"],
-		["------", "------", "------", "------", "------"]
-	]
-	for b in both:
-		row = [b[0]["method"], b[0]["endpoint"], "|", b[1]["method"], b[1]["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(both)))
-
-	print("Only in one:")
-	data = [
-		["----SERVER----", ""],
-		["method", "endpoint"],
-		["------", "------"]
-	]
-	for s in server:
-		row = [s["method"], s["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(server)))
-	data = [
-		["----WRAPPER----", ""],
-		["method", "endpoint"],
-		["------", "------"]
-	]
-	for w in wrapper:
-		row = [w["method"], w["endpoint"]]
-		data.append(row)
-	col_width = max(len(word) for row in data for word in row) + 2
-	for row in data:
-		print("".join(word.ljust(col_width) for word in row))
-	print("Count:{}".format(len(wrapper)))
-
-for f_n in files:
-	file_path = runtime_fp + f_n
-	f = open(file_path, "r")
-	for line in f:
-		if api_request in line:
-			index = line.find(api_request)
-			comment_index = line.find("//")
-			if index != -1:
-				if comment_index != -1:
-					if comment_index < index:
-						continue
-				value = ""
-				method = ""
-				parameters = line[index+len(api_request):]
-				parameters = parameters.split(",")
-				for parameter in parameters:
-					parameter = "".join(parameter.split())
-					if parameter[0] == "(":
-						parameter = parameter[1:]
-					if parameter[-1] == ")":
-						parameter = parameter[:-1]
-					if "value" in parameter:
-						index = parameter.find("value")
-						parameter = parameter[index+len("value"):]
-						value = stripping(parameter)
-
-					elif "method" in parameter:
-						index = parameter.find("method")
-						parameter = parameter[index+len("method"):]
-						method = stripping(parameter)
-						
-				server_endpoints.append(create_endpoint(value, method))
-		if api_post_request in line:
-			index = line.find(api_post_request)
-			line = line[index+len(api_post_request):]
-			line = line[2:-3]
-			server_endpoints.append(create_endpoint(line, "POST"))
-
-
-# for se in server_endpoints:
-# 	print(se)
-
-# print("count: {}".format(len(server_endpoints)))
-
-
-wrapper_endpoints = []
-
-wrapper_path = "../"
-wrapper_fp = wrapper_path + "endpoints/"
-files = [f for f in listdir(wrapper_fp) if isfile(join(wrapper_fp, f))]
-if "__init__.py" in files:
-	files.remove("__init__.py")
-
-for f_n in files:
-	file_path = wrapper_fp + f_n
-	f = open(file_path, "r")
-	new_data = []
-	for line in f:
-		line = "".join(line.split())
-		if len(line) > 0:
-			if line[0] != "#":
-				new_data.append(line)
-	data = "".join(new_data)
-	while True:
-		index = data.find("{")
-		if index == -1:
-			break
-		open_count = 0
-		close_count = 0
-		for i in range(len(data[index:])):
-			c = data[i+index]
-			if c == "}":
-				close_count += 1
-			if c == "{":
-				open_count += 1
-			if open_count == close_count:
-				s = data[index: index+i+1]
-				j_str = eval(s)
-				# j_str = json.loads(s)
-				wrapper_endpoints.append(create_endpoint(j_str["endpoint"], j_str["type"]))
-				data = data[index+i:]
-				break
-
-# for we in wrapper_endpoints:
-# 	print(we)
-
-# print("count: {}".format(len(wrapper_endpoints)))
-
+from os import listdir
+from os.path import isfile, join
+import sys
+import json
+
+runtime_server_path = "C:/Users/Ramsay/Documents/GitHub/ecosystem-runtime/"
+runtime_fp = runtime_server_path + "src/main/java/com/ecosystem/runtime/"
+files = [f for f in listdir(runtime_fp) if isfile(join(runtime_fp, f))]
+
+server_endpoints = []
+api_request = "@RequestMapping"
+api_post_request = "@PostMapping"
+
+def stripping(parameter):
+	if parameter[0] == "=":
+		parameter = parameter[1:]
+	parameter = parameter.replace("'", "")
+	parameter = parameter.replace('"', "")
+	if parameter[0] == ":":
+		parameter = parameter[1:]
+	# if parameter[0] == '"' or parameter[0] == "'":
+	# 	parameter = parameter[1:]
+	# if parameter[-1] == '"' or parameter[-1] == "'":	
+	# 	parameter = parameter[:-1]
+	return parameter
+
+def create_endpoint(endpoint, method):
+	d = {
+		"endpoint": endpoint,
+		"method": method
+	}
+	return d
+
+def compare_endpoints(server_endpoints, wrapper_endpoints):
+	both = []
+	server = []
+	wrapper = []
+	for d in server_endpoints:
+		se = d["endpoint"]
+		sm = d["method"]
+		found = False
+		for d2 in wrapper_endpoints:
+			we = d2["endpoint"]
+			wm = d2["method"]
+			if se == we and wm.lower() in sm.lower():
+				both.append([d, d2])
+				found = True
+				break
+		if not found:
+			server.append(d)
+	for d2 in wrapper_endpoints:
+		we = d2["endpoint"]
+		wm = d2["method"]
+		found = False
+		for d in server_endpoints:
+			se = d["endpoint"]
+			sm = d["method"]
+			if se == we and wm.lower() in sm.lower():
+				found = True
+				break
+		if not found:
+			wrapper.append(d2)
+
+	print("")
+	print("Found in both:")
+	data = [
+		["----SERVER----", "", "", "----WRAPPER----", ""],
+		["method", "endpoint", "", "method", "endpoint"],
+		["------", "------", "------", "------", "------"]
+	]
+	for b in both:
+		row = [b[0]["method"], b[0]["endpoint"], "|", b[1]["method"], b[1]["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(both)))
+
+	print("Only in one:")
+	data = [
+		["----SERVER----", ""],
+		["method", "endpoint"],
+		["------", "------"]
+	]
+	for s in server:
+		row = [s["method"], s["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(server)))
+	data = [
+		["----WRAPPER----", ""],
+		["method", "endpoint"],
+		["------", "------"]
+	]
+	for w in wrapper:
+		row = [w["method"], w["endpoint"]]
+		data.append(row)
+	col_width = max(len(word) for row in data for word in row) + 2
+	for row in data:
+		print("".join(word.ljust(col_width) for word in row))
+	print("Count:{}".format(len(wrapper)))
+
+for f_n in files:
+	file_path = runtime_fp + f_n
+	f = open(file_path, "r")
+	for line in f:
+		if api_request in line:
+			index = line.find(api_request)
+			comment_index = line.find("//")
+			if index != -1:
+				if comment_index != -1:
+					if comment_index < index:
+						continue
+				value = ""
+				method = ""
+				parameters = line[index+len(api_request):]
+				parameters = parameters.split(",")
+				for parameter in parameters:
+					parameter = "".join(parameter.split())
+					if parameter[0] == "(":
+						parameter = parameter[1:]
+					if parameter[-1] == ")":
+						parameter = parameter[:-1]
+					if "value" in parameter:
+						index = parameter.find("value")
+						parameter = parameter[index+len("value"):]
+						value = stripping(parameter)
+
+					elif "method" in parameter:
+						index = parameter.find("method")
+						parameter = parameter[index+len("method"):]
+						method = stripping(parameter)
+						
+				server_endpoints.append(create_endpoint(value, method))
+		if api_post_request in line:
+			index = line.find(api_post_request)
+			line = line[index+len(api_post_request):]
+			line = line[2:-3]
+			server_endpoints.append(create_endpoint(line, "POST"))
+
+
+# for se in server_endpoints:
+# 	print(se)
+
+# print("count: {}".format(len(server_endpoints)))
+
+
+wrapper_endpoints = []
+
+wrapper_path = "../"
+wrapper_fp = wrapper_path + "endpoints/"
+files = [f for f in listdir(wrapper_fp) if isfile(join(wrapper_fp, f))]
+if "__init__.py" in files:
+	files.remove("__init__.py")
+
+for f_n in files:
+	file_path = wrapper_fp + f_n
+	f = open(file_path, "r")
+	new_data = []
+	for line in f:
+		line = "".join(line.split())
+		if len(line) > 0:
+			if line[0] != "#":
+				new_data.append(line)
+	data = "".join(new_data)
+	while True:
+		index = data.find("{")
+		if index == -1:
+			break
+		open_count = 0
+		close_count = 0
+		for i in range(len(data[index:])):
+			c = data[i+index]
+			if c == "}":
+				close_count += 1
+			if c == "{":
+				open_count += 1
+			if open_count == close_count:
+				s = data[index: index+i+1]
+				j_str = eval(s)
+				# j_str = json.loads(s)
+				wrapper_endpoints.append(create_endpoint(j_str["endpoint"], j_str["type"]))
+				data = data[index+i:]
+				break
+
+# for we in wrapper_endpoints:
+# 	print(we)
+
+# print("count: {}".format(len(wrapper_endpoints)))
+
 compare_endpoints(server_endpoints, wrapper_endpoints)
```

