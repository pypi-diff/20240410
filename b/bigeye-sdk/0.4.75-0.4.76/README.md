# Comparing `tmp/bigeye_sdk-0.4.75.tar.gz` & `tmp/bigeye_sdk-0.4.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.75.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.76.tar", max compression
```

## Comparing `bigeye_sdk-0.4.75.tar` & `bigeye_sdk-0.4.76.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     2092 2023-01-31 22:29:47.696692 bigeye_sdk-0.4.75/LICENSE
--rw-r--r--   0        0        0      873 2022-12-08 20:11:34.148834 bigeye_sdk-0.4.75/README.md
--rw-r--r--   0        0        0     3727 2022-12-08 20:11:34.148978 bigeye_sdk-0.4.75/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       76 2024-02-12 20:27:50.663055 bigeye_sdk-0.4.75/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.149159 bigeye_sdk-0.4.75/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    20437 2024-02-12 20:27:50.663399 bigeye_sdk-0.4.75/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0    12403 2024-02-12 20:27:50.663815 bigeye_sdk-0.4.75/bigeye_sdk/authentication/config.py
--rw-r--r--   0        0        0     1182 2023-06-08 22:52:59.202725 bigeye_sdk-0.4.75/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2023-06-26 21:49:38.515036 bigeye_sdk-0.4.75/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.149661 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10366 2024-02-12 20:27:50.664183 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2024-02-05 22:35:25.814148 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-04-04 21:08:42.109340 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      736 2024-02-12 20:27:50.664456 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9363 2024-02-12 20:27:50.664899 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3900 2024-01-11 20:39:12.552651 bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.150541 bigeye_sdk-0.4.75/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2022-12-08 20:11:34.150629 bigeye_sdk-0.4.75/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2022-12-08 20:11:34.150703 bigeye_sdk-0.4.75/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.150789 bigeye_sdk-0.4.75/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2022-12-08 20:11:34.150878 bigeye_sdk-0.4.75/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39844 2024-03-12 10:34:35.948115 bigeye_sdk-0.4.75/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2022-12-08 20:11:34.151133 bigeye_sdk-0.4.75/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    52140 2024-03-19 16:46:22.103791 bigeye_sdk-0.4.75/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.151454 bigeye_sdk-0.4.75/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0     2666 2024-01-11 20:39:12.553764 bigeye_sdk-0.4.75/bigeye_sdk/controller/delta_controller.py
--rw-r--r--   0        0        0    15116 2024-03-19 16:46:22.104241 bigeye_sdk-0.4.75/bigeye_sdk/controller/lineage_controller.py
--rw-r--r--   0        0        0     3209 2023-10-27 17:04:13.271114 bigeye_sdk-0.4.75/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    38904 2024-02-01 16:24:32.681378 bigeye_sdk-0.4.75/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.151805 bigeye_sdk-0.4.75/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2022-12-08 20:11:34.151911 bigeye_sdk-0.4.75/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2022-12-08 20:11:34.152032 bigeye_sdk-0.4.75/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     1582 2024-01-30 20:00:45.498927 bigeye_sdk-0.4.75/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-08 20:11:34.152204 bigeye_sdk-0.4.75/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2022-12-08 20:11:34.152314 bigeye_sdk-0.4.75/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2022-12-08 20:11:34.152433 bigeye_sdk-0.4.75/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     2450 2023-08-02 21:33:13.881173 bigeye_sdk-0.4.75/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2022-12-08 20:11:34.152647 bigeye_sdk-0.4.75/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2022-12-08 20:11:34.152744 bigeye_sdk-0.4.75/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0      370 2024-01-19 21:27:36.415522 bigeye_sdk-0.4.75/bigeye_sdk/functions/dbt.py
--rw-r--r--   0        0        0     4580 2024-01-11 20:39:12.554786 bigeye_sdk-0.4.75/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2814 2024-03-12 10:34:35.949697 bigeye_sdk-0.4.75/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      706 2024-01-11 20:39:12.554925 bigeye_sdk-0.4.75/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0      410 2024-01-11 20:39:12.555210 bigeye_sdk-0.4.75/bigeye_sdk/functions/issue_functions.py
--rw-r--r--   0        0        0    21897 2024-01-11 20:39:12.555450 bigeye_sdk-0.4.75/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     2701 2024-01-11 20:39:12.555603 bigeye_sdk-0.4.75/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2022-12-08 20:11:34.153551 bigeye_sdk-0.4.75/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2022-12-08 20:11:34.153668 bigeye_sdk-0.4.75/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5151 2024-02-05 22:35:09.173883 bigeye_sdk-0.4.75/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4031 2023-06-13 20:28:30.914513 bigeye_sdk-0.4.75/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-04-26 16:50:25.967759 bigeye_sdk-0.4.75/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2024-03-19 16:58:28.491943 bigeye_sdk-0.4.75/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 16:58:28.492073 bigeye_sdk-0.4.75/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 16:58:28.492179 bigeye_sdk-0.4.75/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 16:58:28.492262 bigeye_sdk-0.4.75/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   275481 2024-03-19 16:58:28.492391 bigeye_sdk-0.4.75/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2024-03-19 16:58:28.492617 bigeye_sdk-0.4.75/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2024-03-19 16:58:28.492830 bigeye_sdk-0.4.75/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      993 2023-07-15 12:11:35.877489 bigeye_sdk-0.4.75/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2022-12-08 20:11:34.155511 bigeye_sdk-0.4.75/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      492 2024-02-12 20:27:50.665725 bigeye_sdk-0.4.75/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    37552 2024-02-12 20:27:50.666084 bigeye_sdk-0.4.75/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-03-02 21:06:46.797639 bigeye_sdk-0.4.75/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0      872 2024-02-12 20:27:50.666393 bigeye_sdk-0.4.75/bigeye_sdk/model/dbt_manifest.py
--rw-r--r--   0        0        0     4518 2024-02-12 20:27:50.666587 bigeye_sdk-0.4.75/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     5521 2024-02-12 20:27:50.666930 bigeye_sdk-0.4.75/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0       89 2024-01-11 20:39:12.558140 bigeye_sdk-0.4.75/bigeye_sdk/model/enums.py
--rw-r--r--   0        0        0     9459 2024-02-12 20:27:50.667328 bigeye_sdk-0.4.75/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     9611 2024-02-02 11:22:08.573860 bigeye_sdk-0.4.75/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      221 2024-01-11 20:39:12.558571 bigeye_sdk-0.4.75/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    56945 2024-02-12 20:27:50.667770 bigeye_sdk-0.4.75/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-03-02 21:06:46.799911 bigeye_sdk-0.4.75/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7599 2024-02-12 20:27:50.668127 bigeye_sdk-0.4.75/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3373 2024-03-19 16:47:27.257111 bigeye_sdk-0.4.75/pyproject.toml
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.75/PKG-INFO
+-rw-r--r--   0        0        0     2092 2024-03-07 15:18:25.160096 bigeye_sdk-0.4.76/LICENSE
+-rw-r--r--   0        0        0      873 2024-03-07 15:18:25.160275 bigeye_sdk-0.4.76/README.md
+-rw-r--r--   0        0        0     3727 2024-03-07 15:18:25.160429 bigeye_sdk-0.4.76/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-07 15:18:25.160560 bigeye_sdk-0.4.76/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.160623 bigeye_sdk-0.4.76/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    20437 2024-03-07 15:18:25.160801 bigeye_sdk-0.4.76/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0    12403 2024-03-07 15:18:25.161026 bigeye_sdk-0.4.76/bigeye_sdk/authentication/config.py
+-rw-r--r--   0        0        0     1182 2024-03-07 15:18:25.161153 bigeye_sdk-0.4.76/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2024-03-07 15:18:25.161311 bigeye_sdk-0.4.76/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.161379 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10366 2024-03-07 15:18:25.161557 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2024-03-07 15:18:25.161727 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2024-03-07 15:18:25.161897 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      736 2024-03-07 15:18:25.162023 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9363 2024-03-07 15:18:25.162185 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3900 2024-03-07 15:18:25.162320 bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.162375 bigeye_sdk-0.4.76/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2024-03-07 15:18:25.162515 bigeye_sdk-0.4.76/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2024-03-07 15:18:25.162631 bigeye_sdk-0.4.76/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.162684 bigeye_sdk-0.4.76/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-07 15:18:25.162834 bigeye_sdk-0.4.76/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39844 2024-03-07 15:18:25.163026 bigeye_sdk-0.4.76/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2024-03-07 15:18:25.163201 bigeye_sdk-0.4.76/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    52140 2024-03-21 20:11:50.486024 bigeye_sdk-0.4.76/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.163484 bigeye_sdk-0.4.76/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0     2666 2024-03-07 15:18:25.163681 bigeye_sdk-0.4.76/bigeye_sdk/controller/delta_controller.py
+-rw-r--r--   0        0        0    15116 2024-03-21 20:11:50.486270 bigeye_sdk-0.4.76/bigeye_sdk/controller/lineage_controller.py
+-rw-r--r--   0        0        0     3209 2024-03-07 15:18:25.163991 bigeye_sdk-0.4.76/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    38904 2024-03-07 15:18:25.164187 bigeye_sdk-0.4.76/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.164260 bigeye_sdk-0.4.76/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2024-03-07 15:18:25.164607 bigeye_sdk-0.4.76/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2024-03-07 15:18:25.164747 bigeye_sdk-0.4.76/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1582 2024-03-07 15:18:25.164864 bigeye_sdk-0.4.76/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.164919 bigeye_sdk-0.4.76/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2024-03-07 15:18:25.165063 bigeye_sdk-0.4.76/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2024-03-07 15:18:25.165164 bigeye_sdk-0.4.76/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     2450 2024-03-07 15:18:25.165293 bigeye_sdk-0.4.76/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2024-03-07 15:18:25.165564 bigeye_sdk-0.4.76/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2024-03-07 15:18:25.165703 bigeye_sdk-0.4.76/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0      370 2024-03-07 15:18:25.165830 bigeye_sdk-0.4.76/bigeye_sdk/functions/dbt.py
+-rw-r--r--   0        0        0     4580 2024-03-07 15:18:25.165971 bigeye_sdk-0.4.76/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2814 2024-03-07 15:18:25.166104 bigeye_sdk-0.4.76/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      706 2024-03-07 15:18:25.166362 bigeye_sdk-0.4.76/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0      410 2024-03-07 15:18:25.166486 bigeye_sdk-0.4.76/bigeye_sdk/functions/issue_functions.py
+-rw-r--r--   0        0        0    21897 2024-03-07 15:18:25.166664 bigeye_sdk-0.4.76/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     2701 2024-03-07 15:18:25.166806 bigeye_sdk-0.4.76/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2024-03-07 15:18:25.167067 bigeye_sdk-0.4.76/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2024-03-07 15:18:25.167196 bigeye_sdk-0.4.76/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5151 2024-03-07 15:18:25.167321 bigeye_sdk-0.4.76/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4031 2024-03-07 15:18:25.167450 bigeye_sdk-0.4.76/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2024-03-07 15:18:25.167613 bigeye_sdk-0.4.76/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.167671 bigeye_sdk-0.4.76/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.167761 bigeye_sdk-0.4.76/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.167845 bigeye_sdk-0.4.76/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.167933 bigeye_sdk-0.4.76/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   274547 2024-04-09 15:10:47.488967 bigeye_sdk-0.4.76/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2024-03-07 15:18:25.168844 bigeye_sdk-0.4.76/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2024-03-07 15:18:25.169100 bigeye_sdk-0.4.76/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      993 2024-03-07 15:18:25.169247 bigeye_sdk-0.4.76/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2024-03-07 15:18:25.169389 bigeye_sdk-0.4.76/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      492 2024-03-07 15:18:25.169531 bigeye_sdk-0.4.76/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    37552 2024-03-07 15:18:25.169743 bigeye_sdk-0.4.76/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2024-03-07 15:18:25.170073 bigeye_sdk-0.4.76/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0      872 2024-03-07 15:18:25.170199 bigeye_sdk-0.4.76/bigeye_sdk/model/dbt_manifest.py
+-rw-r--r--   0        0        0     4518 2024-03-07 15:18:25.170331 bigeye_sdk-0.4.76/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     5521 2024-03-07 15:18:25.170469 bigeye_sdk-0.4.76/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0       89 2024-03-07 15:18:25.170737 bigeye_sdk-0.4.76/bigeye_sdk/model/enums.py
+-rw-r--r--   0        0        0     9459 2024-03-07 15:18:25.170897 bigeye_sdk-0.4.76/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     9611 2024-03-07 15:18:25.171182 bigeye_sdk-0.4.76/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      221 2024-03-07 15:18:25.171303 bigeye_sdk-0.4.76/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    56945 2024-03-07 15:18:25.171500 bigeye_sdk-0.4.76/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2024-03-07 15:18:25.171656 bigeye_sdk-0.4.76/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7599 2024-03-07 15:18:25.171954 bigeye_sdk-0.4.76/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3383 2024-04-10 19:11:32.563939 bigeye_sdk-0.4.76/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.76/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.75/LICENSE` & `bigeye_sdk-0.4.76/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/README.md` & `bigeye_sdk-0.4.76/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.76/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.76/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/authentication/config.py` & `bigeye_sdk-0.4.76/bigeye_sdk/authentication/config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.76/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.76/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.76/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.76/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.76/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/controller/delta_controller.py` & `bigeye_sdk-0.4.76/bigeye_sdk/controller/delta_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/controller/lineage_controller.py` & `bigeye_sdk-0.4.76/bigeye_sdk/controller/lineage_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/controller/metric_controller.py` & `bigeye_sdk-0.4.76/bigeye_sdk/controller/metric_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.76/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/helpers.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.76/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.76/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,17 +78,16 @@
     PERCENT_EMAIL = 66
     ROWS_INSERTED = 67
     HOURS_SINCE_LAST_LOAD = 68
     COUNT_READ_QUERIES = 69
     PERCENT_NOT_NULL = 70
     FRESHNESS = 71
     VOLUME = 72
-    FRESHNESS_DATA_DATE = 73
-    FRESHNESS_DATA_TIMESTAMP = 74
-    VOLUME_DATA = 75
+    FRESHNESS_DATA = 73
+    VOLUME_DATA = 74
 
 
 class FieldType(betterproto.Enum):
     FIELD_TYPE_UNSPECIFIED = 0
     FIELD_TYPE_STRING = 1
     FIELD_TYPE_UUID = 2
     FIELD_TYPE_BINARY = 3
@@ -742,20 +741,14 @@
 
 class DashboardDateAggregationType(betterproto.Enum):
     DASHBOARD_DATE_AGGREGATION_TYPE_DAY = 0
     DASHBOARD_DATE_AGGREGATION_TYPE_WEEK = 1
     DASHBOARD_DATE_AGGREGATION_TYPE_MONTH = 2
 
 
-class GroupMembershipVia(betterproto.Enum):
-    GROUP_MEMBERSHIP_VIA_UNSPECIFIED = 0
-    GROUP_MEMBERSHIP_VIA_MANUAL_ASSIGNMENT = 1
-    GROUP_MEMBERSHIP_VIA_IDP_GROUPS = 2
-
-
 class GroupUserOperation(betterproto.Enum):
     GROUP_USER_OPERATION_UNSPECIFIED = 0
     GROUP_USER_OPERATION_ADD = 1
     GROUP_USER_OPERATION_REMOVE = 2
 
 
 class RoleOperation(betterproto.Enum):
@@ -852,16 +845,14 @@
 class User(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     email: str = betterproto.string_field(3)
     role: "Role" = betterproto.enum_field(4)
     groups: List["IdAndDisplayName"] = betterproto.message_field(5)
     picture_url: str = betterproto.string_field(6)
-    idp_groups: List[str] = betterproto.string_field(7)
-    last_login_at: int = betterproto.int64_field(8)
 
 
 @dataclass
 class UserInviteRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
     email: str = betterproto.string_field(2)
     group_ids: List[int] = betterproto.int32_field(3)
@@ -3191,15 +3182,14 @@
 
 @dataclass
 class PaginationInfo(betterproto.Message):
     prev_cursor: str = betterproto.string_field(1)
     next_cursor: str = betterproto.string_field(2)
     num_records: int = betterproto.int32_field(3)
     first_sort_distinct_values: int = betterproto.int64_field(4)
-    no_num_records: bool = betterproto.bool_field(5)
 
 
 @dataclass
 class ColumnSearchRequest(betterproto.Message):
     table_id: int = betterproto.int32_field(1)
     column_ids: List[int] = betterproto.int32_field(2)
 
@@ -3427,15 +3417,14 @@
 @dataclass
 class DomainAuthMapping(betterproto.Message):
     id: int = betterproto.int32_field(1)
     domain: str = betterproto.string_field(2)
     connection_name: str = betterproto.string_field(3)
     id_provider: "IdProvider" = betterproto.enum_field(4)
     oidc_config: "OidcConfigResponse" = betterproto.message_field(5)
-    scopes: List[str] = betterproto.string_field(6)
 
 
 @dataclass
 class OidcConfigRequest(betterproto.Message):
     identity_provider_url: str = betterproto.string_field(1)
     client_id: str = betterproto.string_field(2)
     client_secret: str = betterproto.string_field(3)
@@ -3449,15 +3438,14 @@
 
 @dataclass
 class CreateDomainMappingRequest(betterproto.Message):
     domain: str = betterproto.string_field(1)
     connection_name: str = betterproto.string_field(2)
     id_provider: "IdProvider" = betterproto.enum_field(3)
     oidc_config: "OidcConfigRequest" = betterproto.message_field(4)
-    scopes: List[str] = betterproto.string_field(5)
 
 
 @dataclass
 class CreateDomainMappingResponse(betterproto.Message):
     domain_mapping: "DomainAuthMapping" = betterproto.message_field(1)
 
 
@@ -4282,33 +4270,24 @@
 
 @dataclass
 class Group(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     users: List["IdAndDisplayName"] = betterproto.message_field(3)
     roles: List["RoleV2"] = betterproto.message_field(4)
-    idp_groups: List[str] = betterproto.string_field(5)
-    memberships: List["UserGroupMembership"] = betterproto.message_field(6)
-
-
-@dataclass
-class UserGroupMembership(betterproto.Message):
-    user: "User" = betterproto.message_field(1)
-    membership_paths: List["GroupMembershipVia"] = betterproto.enum_field(2)
 
 
 @dataclass
 class GroupListResponse(betterproto.Message):
     groups: List["Group"] = betterproto.message_field(1)
 
 
 @dataclass
 class CreateOrUpdateGroupRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
-    idp_groups: List[str] = betterproto.string_field(2)
 
 
 @dataclass
 class SinglePathParamGroupIdRequest(betterproto.Message):
     group_id: int = betterproto.int32_field(1)
 
 
@@ -7882,22 +7861,19 @@
             RoleV2,
         )
 
 
 class GroupServiceStub(betterproto.ServiceStub):
     """Groups"""
 
-    async def create_group(
-        self, *, name: str = "", idp_groups: List[str] = []
-    ) -> Group:
+    async def create_group(self, *, name: str = "") -> Group:
         """Create a group"""
 
         request = CreateOrUpdateGroupRequest()
         request.name = name
-        request.idp_groups = idp_groups
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.GroupService/CreateGroup",
             request,
             Group,
         )
```

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.76/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/log/__init__.py` & `bigeye_sdk-0.4.76/bigeye_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/dbt_manifest.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/dbt_manifest.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.76/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.76/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.75/pyproject.toml` & `bigeye_sdk-0.4.76/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.75"
+version = "0.4.76"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
@@ -48,15 +48,15 @@
 pytest = "^7.1.3"
 Sphinx = { version = "^5.2.2"}
 sphinx-rtd-theme = { version = "^1.0.0"}
 
 [tool.poe.tasks]
     test = ["python_tests"]
     pre_build = ["protogen"]
-    pre_publish = ["clean"]
+    pre_publish = ["clean", "docgen"]
     pre_install = ["protogen"]
     post_install = []
     post_publish = ["clean"]
 
     [tool.poe.tasks.include_generated]
         help = "Includes generated code for the Poetry build.  Git excluded code is not included in Poetry Build"
         shell = """
```

### Comparing `bigeye_sdk-0.4.75/PKG-INFO` & `bigeye_sdk-0.4.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.75
+Version: 0.4.76
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

