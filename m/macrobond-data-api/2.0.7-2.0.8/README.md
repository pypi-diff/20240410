# Comparing `tmp/macrobond-data-api-2.0.7.tar.gz` & `tmp/macrobond-data-api-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrobond-data-api-2.0.7.tar", last modified: Mon Mar 25 09:15:47 2024, max compression
+gzip compressed data, was "macrobond-data-api-2.0.8.tar", last modified: Wed Apr 10 08:18:22 2024, max compression
```

## Comparing `macrobond-data-api-2.0.7.tar` & `macrobond-data-api-2.0.8.tar`

### file list

```diff
@@ -1,158 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.172899 macrobond-data-api-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-03-25 09:15:47.172899 macrobond-data-api-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.144899 macrobond-data-api-2.0.7/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.144899 macrobond-data-api-2.0.7/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_in_house_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16705 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_error_message_to_status_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_fix_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.148899 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.148899 macrobond-data-api-2.0.7/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25069 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.148899 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_weekdays.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.152899 macrobond-data-api-2.0.7/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/_parse_iso8601.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/values_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.156899 macrobond-data-api-2.0.7/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/util/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/util/save_credentials_to_keyring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/util/save_proxy_to_keyring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/util/transfer_performance_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.156899 macrobond-data-api-2.0.7/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_in_house_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/data_package_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.164899 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_pacakge_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/in_house_series_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.164899 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.164899 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_storage_location_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.168899 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 09:15:47.168899 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7177 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 09:15:47.000000 macrobond-data-api-2.0.7/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-25 09:15:47.172899 macrobond-data-api-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-25 09:14:27.000000 macrobond-data-api-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.094125 macrobond-data-api-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-10 08:18:22.094125 macrobond-data-api-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.062125 macrobond-data-api-2.0.8/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.066125 macrobond-data-api-2.0.8/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_in_house_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16705 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_error_message_to_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_fix_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.070125 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.070125 macrobond-data-api-2.0.8/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25069 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.070125 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_weekdays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.074125 macrobond-data-api-2.0.8/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/_parse_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.078125 macrobond-data-api-2.0.8/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25407 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/_diagnostic_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/save_credentials_to_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/save_proxy_to_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/util/transfer_performance_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.082125 macrobond-data-api-2.0.8/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_in_house_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/data_package_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.086125 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_pacakge_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/in_house_series_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.086125 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.090125 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_storage_location_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.090125 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:18:22.090125 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 08:18:22.000000 macrobond-data-api-2.0.8/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 08:18:22.094125 macrobond-data-api-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-10 08:16:53.000000 macrobond-data-api-2.0.8/setup.py
```

### Comparing `macrobond-data-api-2.0.7/LICENSE` & `macrobond-data-api-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/PKG-INFO` & `macrobond-data-api-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 2.0.7
+Version: 2.0.8
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.7 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.8 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-2.0.7/README.md` & `macrobond-data-api-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/__init__.py` & `macrobond-data-api-2.0.8/macrobond_data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/_generated.py` & `macrobond-data-api-2.0.8/macrobond_data_api/_generated.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/_get_api.py` & `macrobond-data-api-2.0.8/macrobond_data_api/_get_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_in_house_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_in_house_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_com_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/_metadata_directory.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_api.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_client.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 import sys
 
-from typing import TYPE_CHECKING, List, Optional, Tuple, cast
+from typing import TYPE_CHECKING, List, Optional, Tuple, cast, Any
 
 from macrobond_data_api.common import Client
 
 from .com_api import ComApi
 
 if TYPE_CHECKING:  # pragma: no cover
     from .com_types import Connection
 
 _win32com_import_error: Optional[ImportError] = None
-try:
-    from win32com import client as _client
-except ImportError as ex:
-    _win32com_import_error = ex
-
 _pywintypes_import_error: Optional[ImportError] = None
-try:
-    from pywintypes import com_error
-except ImportError as ex:
-    _pywintypes_import_error = ex
-
-try:
-    # winreg is not available on linux so mypy will fail on build server as it is runiong on linux
-    from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT, HKEY_CURRENT_USER  # type: ignore
-except ImportError:
-    pass
+
+if sys.platform == "win32":
+    try:
+        from win32com import client as _client
+    except ImportError as ex:
+        _win32com_import_error = ex
+
+    try:
+        from pywintypes import com_error
+    except ImportError as ex:
+        _pywintypes_import_error = ex
+
+    import winreg  # pylint: disable = E0401
+else:
+    _client: Any = None
+    com_error: Any = None
+    winreg: Any = None
 
 
 def _test_regedit_assembly() -> Optional[str]:
     sub_key = "CLSID\\{F22A9A5C-E6F2-4FA8-8D1B-E928AB5DDF9B}\\InprocServer32"
     try:
-        with OpenKey(HKEY_CLASSES_ROOT, sub_key) as regkey:
-            QueryValueEx(regkey, "Assembly")
+        with winreg.OpenKey(winreg.HKEY_CLASSES_ROOT, sub_key) as regkey:
+            winreg.QueryValueEx(regkey, "Assembly")
     except OSError:
         return (
             "The Macrobond application is probably not installed.\n"
             + '(Could not find the registry key "HKEY_CLASSES_ROOT\\'
             + sub_key
             + '\\Assembly")\n'
         )
     return None
 
 
 def _test_regedit_username() -> Optional[str]:
     sub_key = "Software\\Macrobond Financial\\Communication\\Connector"
     try:
-        with OpenKey(HKEY_CURRENT_USER, sub_key) as regkey:
-            QueryValueEx(regkey, "UserName")
+        with winreg.OpenKey(winreg.HKEY_CURRENT_USER, sub_key) as regkey:
+            winreg.QueryValueEx(regkey, "UserName")
     except OSError:
         return (
             "The Macrobond application does not seem to be logged in. Please start the application and verify that "
             + "it works properly.\n"
             + '(Could not find the registry key "HKEY_CURRENT_USER\\'
             + sub_key
             + '\\UserName")\n'
```

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/connection.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-2.0.8/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/api.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/client.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/__init__.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/metadata_attribute_type.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/metadata_attribute_type.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/_parse_iso8601.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/_parse_iso8601.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/get_entity_error.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/get_entity_error.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/revision_info.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/search_result_long.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_observation_history.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/unified_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/common/types/vintage_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/util/diagnostic.py` & `macrobond-data-api-2.0.8/macrobond_data_api/util/diagnostic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,138 @@
+#!/usr/bin/env python3
+from dataclasses import dataclass
 import importlib.metadata
 import os
 import platform
+import sys
+from typing import Optional, List
 
-try:
-    # winreg is not available on linux so mypy will fail on build server as it is runiong on linux
-    from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT, HKEY_CURRENT_USER  # type: ignore
-except ImportError:
-    pass
+from macrobond_data_api.util._diagnostic_winreg import _test_regedit_assembly, _test_regedit_username, _test_winreg
+from macrobond_data_api.util._common import SaveOutputToFile
 
 
-def _test_regedit_assembly() -> None:
-    sub_key = "CLSID\\{F22A9A5C-E6F2-4FA8-8D1B-E928AB5DDF9B}\\InprocServer32"
-    try:
-        with OpenKey(HKEY_CLASSES_ROOT, sub_key) as regkey:
-            QueryValueEx(regkey, "Assembly")
-        print("HKEY_CLASSES_ROOT", sub_key, "is ok")
-    except OSError as e:
-        print(
-            "The Macrobond application is probably not installed.\n"
-            + '(Could not find the registry key "HKEY_CLASSES_ROOT\\'
-            + sub_key
-            + '\\Assembly")\n',
-            e,
-        )
+@dataclass
+class _PackagesInfo:
+    exception: Optional[Exception]
+    requirement: str
+    name: str
+    verison: str
 
 
-def _test_regedit_username() -> None:
-    sub_key = "Software\\Macrobond Financial\\Communication\\Connector"
-    try:
-        with OpenKey(HKEY_CURRENT_USER, sub_key) as regkey:
-            QueryValueEx(regkey, "UserName")
-        print("HKEY_CURRENT_USER", sub_key, "is ok")
-    except OSError as e:
-        print(
-            "The Macrobond application does not seem to be logged in. Please start the application and verify that "
-            + "it works properly.\n"
-            + '(Could not find the registry key "HKEY_CURRENT_USER\\'
-            + sub_key
-            + '\\UserName")\n',
-            e,
-        )
-
-
-def print_system_information() -> None:
-
-    print("-- system_information --")
-
-    print("Platform information:", platform.platform())
-    print("Python compiler:", platform.python_compiler())
-    print("Python implementation:", platform.python_implementation())
-    print("Python version:", platform.python_version())
-    print("Python architecture:", platform.architecture())
-
+# This code is a sin against all people on earth, cooder jesus forgive me.
+def _list_packages() -> None:
     try:
+        packages_list: List[_PackagesInfo] = []
         requirements = importlib.metadata.requires("macrobond-data-api")
         if requirements is None:
             raise Exception("No requirements found for macrobond-data-api")
+
+        new_model = any(x for x in requirements if x.startswith("keyring "))
+
         for r in requirements:
             try:
-                print(r, "installed", importlib.metadata.version(r.split(" ")[0]))
+                if new_model:
+                    n = r.split(" ")[0]
+                else:
+                    n = r.split("==")[0]
+                    if len(n) > len(r.split(">=")[0]):
+                        n = r.split(">=")[0]
+
+                    if len(n) > len(r.split(";")[0]):
+                        n = r.split(";")[0]
+
+                if n.endswith("]"):
+                    continue
+
+                packages_list.append(_PackagesInfo(None, r, n, importlib.metadata.version(n)))
             except Exception as e:  # pylint: disable=broad-exception-caught
-                print("can't get versions", e)
+                packages_list.append(_PackagesInfo(e, r, "", ""))
+
+        pad = max(len(f"{p.name} == {p.verison}") for p in packages_list)
+
+        for p in packages_list:
+            if p.exception is None:
+                print("installed:", f"{p.name} == {p.verison}".ljust(pad), "requirement:", p.requirement)
+
+        for p in packages_list:
+            if p.exception is not None:
+                print(f"Can't get {p.requirement} version", p.exception)
+
     except Exception as e:  # pylint: disable=broad-exception-caught
         print("can't get macrobond-data-api depdensys versions", e)
 
+
+def _print_system_information() -> None:
+
+    print("\n-- System information --\n")
+
+    print("platform.platform():", platform.platform())
+    print("sys.platform:", sys.platform)
+    print("sys.executable:", sys.executable)
+    print("platform.python_compiler():", platform.python_compiler())
+    print("platform.python_implementation():", platform.python_implementation())
+    print("platform.python_version():", platform.python_version())
+    print("platform.architecture():", platform.architecture())
+
+    print("\n-- Python packages info --\n")
+    try:
+        _list_packages()
+    except Exception as e:  # pylint: disable=broad-exception-caught
+        print("can't get macrobond-data-api depdensys versions", e)
+
+    print("\n-- macrobond-data-api version --\n")
     try:
         import macrobond_data_api.__version__ as apiInfo  # pylint: disable=import-outside-toplevel
 
         print("macrobond-data-api version:", apiInfo.__version__)
     except Exception as e:  # pylint: disable=broad-exception-caught
         print("can't get macrobond-data-api version", e)
 
+    print("\n-- keyring info --\n")
     try:
         import keyring  # pylint: disable=import-outside-toplevel
 
         print("keyring.get_keyring().name:", keyring.get_keyring().name)
     except Exception as e:  # pylint: disable=broad-exception-caught
         print("can't get keyring.get_keyring().name", e)
 
     if os.name == "nt":
-        print("-- running on windows --")
+
+        print("\n-- Windows tests --")
+
+        print("\n-- Test regedit assembly --\n")
 
         _test_regedit_assembly()
 
+        print("\n-- Test regedit username --\n")
+
         _test_regedit_username()
 
+        print("\n-- Test ComClient.connection.Version --\n")
+
         try:
             from macrobond_data_api.com import ComClient  # pylint: disable=import-outside-toplevel
 
             with ComClient() as api:
                 print("Com version:", api.connection.Version)
         except Exception as e:  # pylint: disable=broad-exception-caught
             print("can't get Com version", e)
 
+        print("\n-- Test regedit --\n")
+
+        _test_winreg()
+
+
+def print_system_information() -> None:
+    # fmt: off
+    # pylint: disable=line-too-long
+    """
+    Tests and prints system info, for troubleshooting.
+    """
+    # pylint: enable=line-too-long
+    # fmt: on
+    with SaveOutputToFile("system_information"):
+        _print_system_information()
+
 
 if __name__ == "__main__":
     print_system_information()
```

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/util/save_credentials_to_keyring.py` & `macrobond-data-api-2.0.8/macrobond_data_api/util/save_credentials_to_keyring.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,15 @@
 
 import keyring
 from keyring.backends.fail import Keyring as fail_keyring_backend
 from keyring.backends.null import Keyring as null_keyring_backend
 from macrobond_data_api.web.configuration import Configuration
 from macrobond_data_api.web.web_client import WebClient
 
-
-def _inquiry(question: str, default: str = "yes") -> bool:
-    valid = {"yes": True, "y": True, "no": False, "n": False}
-    if default is None:
-        prompt = " [y/n] "
-    elif default == "yes":
-        prompt = " [Y/n] "
-    elif default == "no":
-        prompt = " [y/N] "
-
-    while True:
-        sys.stdout.write(question + prompt)
-        choice = input().lower()
-        if default is not None and choice == "":
-            return valid[default]
-        if choice in valid:
-            return valid[choice]
-        sys.stdout.write("Please respond with 'yes' or 'no' (or 'y' or 'n').\n")
+from macrobond_data_api.util._common import _inquiry
 
 
 def _remove_duplicates(service_name: str, username: str, warn_before_removing: bool) -> bool:
     old_credential = keyring.get_credential(service_name, username)
     while old_credential:
         if warn_before_removing and not _inquiry(
             'Warning - There is already a key with the same service name, it has the username "'
```

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/util/save_proxy_to_keyring.py` & `macrobond-data-api-2.0.8/macrobond_data_api/util/save_proxy_to_keyring.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/util/transfer_performance_test.py` & `macrobond-data-api-2.0.8/macrobond_data_api/util/transfer_performance_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from time import perf_counter
 from typing import List, Optional, Sequence
 from datetime import timedelta
 
 import requests
 
+from macrobond_data_api.util._common import SaveOutputToFile
+
 
 def _format_speed_kB_sec(kB: float) -> str:
     return _format_kB(kB) + "/s"
 
 
 def _format_kB(kB: float) -> str:
     if kB < 1:
@@ -202,22 +204,41 @@
     print("")
 
     for result_list in result_lists:
         result_list.display_results()
 
 
 def transfer_performance_test(sizes_kB: Optional[Sequence[int]] = None, times: int = 4, indicator: bool = True) -> None:
-    # Run speed and integrity test.
-    # The integrity test verifies that data is transferred correctly.
-    print("- transfer performance test beginning -\n")
+    # fmt: off
+    # pylint: disable=line-too-long
+    """
+    Testing connection the Macrobond Web Api.
+
+    Parameters
+    ----------
+    sizes_kB : Sequence[int], Optional
+        Optional bool whether the method should ask before removing keys, default to `[10, 100, 1024, 10240]`.
+
+    times : int, Optional
+        Optional bool whether the method should ask for a service name to use, default to `4`.
+
+    indicator: bool, Optional
+        Optional default to `True`.
+    """
+    # pylint: enable=line-too-long
+    # fmt: on
+    with SaveOutputToFile("transfer_performance_test"):
+        # Run speed and integrity test.
+        # The integrity test verifies that data is transferred correctly.
+        print("- transfer performance test beginning -\n")
 
-    print("- Running speed test -")
-    _speed_test()
+        print("- Running speed test -")
+        _speed_test()
 
-    print("- Running integrity test -")
-    _integrity_test(sizes_kB if sizes_kB else [10, 100, 1024, 10 * 1024], times, indicator)
+        print("- Running integrity test -")
+        _integrity_test(sizes_kB if sizes_kB else [10, 100, 1024, 10 * 1024], times, indicator)
 
-    print("- transfer performance test end -")
+        print("- transfer performance test end -")
 
 
 if __name__ == "__main__":
     transfer_performance_test()
```

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_in_house_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_in_house_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/_web_only_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/configuration.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/configuration.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/data_package_list_poller.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/data_package_list_poller.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/session.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/session.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/subscription_list.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/subscription_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_api.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_client.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_body.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_body.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list_context.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list_context.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/data_package_list_state.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/data_package_list_state.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/in_house_series_methods.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/in_house_series_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/search_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_request.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/status_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-2.0.8/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-2.0.8/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 2.0.7
+Version: 2.0.8
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.7 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.8 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-2.0.7/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-2.0.8/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 macrobond_data_api/common/types/series_observation_history.py
 macrobond_data_api/common/types/series_with_vintages.py
 macrobond_data_api/common/types/start_or_end_point.py
 macrobond_data_api/common/types/unified_series.py
 macrobond_data_api/common/types/values_metadata.py
 macrobond_data_api/common/types/vintage_series.py
 macrobond_data_api/util/__init__.py
+macrobond_data_api/util/_common.py
+macrobond_data_api/util/_diagnostic_winreg.py
 macrobond_data_api/util/diagnostic.py
 macrobond_data_api/util/save_credentials_to_keyring.py
 macrobond_data_api/util/save_proxy_to_keyring.py
 macrobond_data_api/util/transfer_performance_test.py
 macrobond_data_api/web/__init__.py
 macrobond_data_api/web/_metadata.py
 macrobond_data_api/web/_metadata_directory.py
```

### Comparing `macrobond-data-api-2.0.7/setup.cfg` & `macrobond-data-api-2.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-2.0.7/setup.py` & `macrobond-data-api-2.0.8/setup.py`

 * *Files identical despite different names*

