# Comparing `tmp/vtarget-0.8.5.tar.gz` & `tmp/vtarget-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtarget-0.8.5.tar", last modified: Mon Mar 25 18:33:41 2024, max compression
+gzip compressed data, was "vtarget-0.8.6.tar", last modified: Wed Apr 10 13:56:00 2024, max compression
```

## Comparing `vtarget-0.8.5.tar` & `vtarget-0.8.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.967155 vtarget-0.8.5/
--rw-rw-rw-   0        0        0     1494 2024-03-25 15:35:40.000000 vtarget-0.8.5/LICENSE
--rw-rw-rw-   0        0        0       58 2024-03-25 15:35:40.000000 vtarget-0.8.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2144 2024-03-25 18:33:41.965154 vtarget-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0      806 2024-03-25 15:35:52.000000 vtarget-0.8.5/README.md
--rw-rw-rw-   0        0        0      100 2024-03-25 15:35:41.000000 vtarget-0.8.5/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-03-25 15:35:52.000000 vtarget-0.8.5/requirements.txt
--rw-rw-rw-   0        0        0       96 2024-03-25 18:33:41.970155 vtarget-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      826 2024-03-25 18:33:15.000000 vtarget-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.718159 vtarget-0.8.5/vtarget/
--rw-rw-rw-   0        0        0      146 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.751155 vtarget-0.8.5/vtarget/dataprep/
--rw-rw-rw-   0        0        0     2635 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/__init__.py
--rw-rw-rw-   0        0        0    37512 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/builder.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.891155 vtarget-0.8.5/vtarget/dataprep/nodes/
--rw-rw-rw-   0        0        0     2756 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/api_rest.py
--rw-rw-rw-   0        0        0     4933 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/code.py
--rw-rw-rw-   0        0        0     4148 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/column.py
--rw-rw-rw-   0        0        0     3232 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/concat.py
--rw-rw-rw-   0        0        0     3304 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/cross_join.py
--rw-rw-rw-   0        0        0     3798 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/cumsum.py
--rw-rw-rw-   0        0        0     2318 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/cut.py
--rw-rw-rw-   0        0        0     5935 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/data_cleansing.py
--rw-rw-rw-   0        0        0     9143 2024-03-25 18:33:04.000000 vtarget-0.8.5/vtarget/dataprep/nodes/database.py
--rw-rw-rw-   0        0        0     7215 2024-03-25 18:33:04.000000 vtarget-0.8.5/vtarget/dataprep/nodes/database_write.py
--rw-rw-rw-   0        0        0     2384 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/datetime_extract.py
--rw-rw-rw-   0        0        0     2617 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/datetime_fill.py
--rw-rw-rw-   0        0        0     4641 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/datetime_formatter.py
--rw-rw-rw-   0        0        0     2465 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/datetime_range.py
--rw-rw-rw-   0        0        0     3612 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/describe.py
--rw-rw-rw-   0        0        0     1842 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/df_maker.py
--rw-rw-rw-   0        0        0     1792 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/drop_duplicates.py
--rw-rw-rw-   0        0        0     7409 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/dtype.py
--rw-rw-rw-   0        0        0     6583 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/email.py
--rw-rw-rw-   0        0        0     5993 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/excel.py
--rw-rw-rw-   0        0        0     9424 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/filter.py
--rw-rw-rw-   0        0        0     3392 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/formula.py
--rw-rw-rw-   0        0        0     5411 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/groupby.py
--rw-rw-rw-   0        0        0     4900 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/input_data.py
--rw-rw-rw-   0        0        0     4160 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/inter_row.py
--rw-rw-rw-   0        0        0     2810 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/isin.py
--rw-rw-rw-   0        0        0     1820 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/melt.py
--rw-rw-rw-   0        0        0     6490 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/merge.py
--rw-rw-rw-   0        0        0     3112 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/output.py
--rw-rw-rw-   0        0        0     4404 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/pivot.py
--rw-rw-rw-   0        0        0     3133 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/rolling.py
--rw-rw-rw-   0        0        0     3151 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/sample.py
--rw-rw-rw-   0        0        0     1212 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/shape.py
--rw-rw-rw-   0        0        0     2024 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/sort.py
--rw-rw-rw-   0        0        0     3122 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/split.py
--rw-rw-rw-   0        0        0     8644 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/switch.py
--rw-rw-rw-   0        0        0     1513 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/unique.py
--rw-rw-rw-   0        0        0      616 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/dataprep/nodes/v_output.py
--rw-rw-rw-   0        0        0     2500 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/nodes/value_counts.py
--rw-rw-rw-   0        0        0     8894 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/pipeline.py
--rw-rw-rw-   0        0        0     1542 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/dataprep/types.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.916161 vtarget-0.8.5/vtarget/handlers/
--rw-rw-rw-   0        0        0     5301 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/automl_cache.py
--rw-rw-rw-   0        0        0     6508 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/autots_cache.py
--rw-rw-rw-   0        0        0     1856 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/bug_handler.py
--rw-rw-rw-   0        0        0     9116 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/cache_handler.py
--rw-rw-rw-   0        0        0     1449 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/event_handler.py
--rw-rw-rw-   0        0        0      464 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/log_handler.py
--rw-rw-rw-   0        0        0      172 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/handlers/script_handler.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.922154 vtarget-0.8.5/vtarget/language/
--rw-rw-rw-   0        0        0    35505 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/language/app_message.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.946153 vtarget-0.8.5/vtarget/utils/
--rw-rw-rw-   0        0        0     4125 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/utils/__init__.py
--rw-rw-rw-   0        0        0     1570 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/utils/calc_metrics.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.958156 vtarget-0.8.5/vtarget/utils/database_connection/
--rw-rw-rw-   0        0        0     3311 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/utils/database_connection/field_validation.py
--rw-rw-rw-   0        0        0     7400 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/utils/database_connection/utilities.py
--rw-rw-rw-   0        0        0     3516 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/utils/email_sender.py
--rw-rw-rw-   0        0        0      838 2024-03-25 15:35:41.000000 vtarget-0.8.5/vtarget/utils/encrypter.py
--rw-rw-rw-   0        0        0    20811 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/utils/modeling.py
--rw-rw-rw-   0        0        0    13591 2024-03-25 15:35:53.000000 vtarget-0.8.5/vtarget/utils/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-25 18:33:41.962153 vtarget-0.8.5/vtarget.egg-info/
--rw-rw-rw-   0        0        0     2144 2024-03-25 18:33:41.000000 vtarget-0.8.5/vtarget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2259 2024-03-25 18:33:41.000000 vtarget-0.8.5/vtarget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 18:33:41.000000 vtarget-0.8.5/vtarget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      531 2024-03-25 18:33:41.000000 vtarget-0.8.5/vtarget.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-25 18:33:41.000000 vtarget-0.8.5/vtarget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.401853 vtarget-0.8.6/
+-rw-rw-rw-   0        0        0     1494 2024-03-25 15:35:40.000000 vtarget-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0       58 2024-03-25 15:35:40.000000 vtarget-0.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2144 2024-04-10 13:56:00.399855 vtarget-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-03-25 15:35:52.000000 vtarget-0.8.6/README.md
+-rw-rw-rw-   0        0        0      100 2024-03-25 15:35:41.000000 vtarget-0.8.6/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-03-25 15:35:52.000000 vtarget-0.8.6/requirements.txt
+-rw-rw-rw-   0        0        0       96 2024-04-10 13:56:00.403852 vtarget-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      826 2024-04-10 13:55:35.000000 vtarget-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.187866 vtarget-0.8.6/vtarget/
+-rw-rw-rw-   0        0        0      146 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.217867 vtarget-0.8.6/vtarget/dataprep/
+-rw-rw-rw-   0        0        0     2635 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/__init__.py
+-rw-rw-rw-   0        0        0    37512 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/builder.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.338857 vtarget-0.8.6/vtarget/dataprep/nodes/
+-rw-rw-rw-   0        0        0     2756 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/api_rest.py
+-rw-rw-rw-   0        0        0     4933 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/code.py
+-rw-rw-rw-   0        0        0     4148 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/column.py
+-rw-rw-rw-   0        0        0     3232 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/concat.py
+-rw-rw-rw-   0        0        0     3304 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cross_join.py
+-rw-rw-rw-   0        0        0     3798 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cumsum.py
+-rw-rw-rw-   0        0        0     2318 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/cut.py
+-rw-rw-rw-   0        0        0     5935 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/data_cleansing.py
+-rw-rw-rw-   0        0        0     9143 2024-03-25 18:33:04.000000 vtarget-0.8.6/vtarget/dataprep/nodes/database.py
+-rw-rw-rw-   0        0        0     7215 2024-03-25 18:33:04.000000 vtarget-0.8.6/vtarget/dataprep/nodes/database_write.py
+-rw-rw-rw-   0        0        0     2384 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_extract.py
+-rw-rw-rw-   0        0        0     2617 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_fill.py
+-rw-rw-rw-   0        0        0     4681 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_formatter.py
+-rw-rw-rw-   0        0        0     2465 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/datetime_range.py
+-rw-rw-rw-   0        0        0     3612 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/describe.py
+-rw-rw-rw-   0        0        0     1842 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/df_maker.py
+-rw-rw-rw-   0        0        0     1792 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/drop_duplicates.py
+-rw-rw-rw-   0        0        0     7409 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/dtype.py
+-rw-rw-rw-   0        0        0     6583 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/email.py
+-rw-rw-rw-   0        0        0     5993 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/excel.py
+-rw-rw-rw-   0        0        0     9424 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/filter.py
+-rw-rw-rw-   0        0        0     3392 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/formula.py
+-rw-rw-rw-   0        0        0     5411 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/groupby.py
+-rw-rw-rw-   0        0        0     6755 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/dataprep/nodes/input_data.py
+-rw-rw-rw-   0        0        0     4160 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/inter_row.py
+-rw-rw-rw-   0        0        0     2810 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/isin.py
+-rw-rw-rw-   0        0        0     1820 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/melt.py
+-rw-rw-rw-   0        0        0     6490 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/merge.py
+-rw-rw-rw-   0        0        0     3112 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/output.py
+-rw-rw-rw-   0        0        0     4404 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/pivot.py
+-rw-rw-rw-   0        0        0     3133 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/rolling.py
+-rw-rw-rw-   0        0        0     3151 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/sample.py
+-rw-rw-rw-   0        0        0     1212 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/shape.py
+-rw-rw-rw-   0        0        0     2024 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/sort.py
+-rw-rw-rw-   0        0        0     3122 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/split.py
+-rw-rw-rw-   0        0        0     8644 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/switch.py
+-rw-rw-rw-   0        0        0     1513 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/unique.py
+-rw-rw-rw-   0        0        0      616 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/dataprep/nodes/v_output.py
+-rw-rw-rw-   0        0        0     2500 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/nodes/value_counts.py
+-rw-rw-rw-   0        0        0     8894 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/pipeline.py
+-rw-rw-rw-   0        0        0     1542 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/dataprep/types.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.360857 vtarget-0.8.6/vtarget/handlers/
+-rw-rw-rw-   0        0        0     5301 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/automl_cache.py
+-rw-rw-rw-   0        0        0     6508 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/autots_cache.py
+-rw-rw-rw-   0        0        0     1856 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/bug_handler.py
+-rw-rw-rw-   0        0        0     9116 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/cache_handler.py
+-rw-rw-rw-   0        0        0     1449 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      464 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/log_handler.py
+-rw-rw-rw-   0        0        0      172 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/handlers/script_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.366855 vtarget-0.8.6/vtarget/language/
+-rw-rw-rw-   0        0        0    35956 2024-04-10 13:55:35.000000 vtarget-0.8.6/vtarget/language/app_message.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.384855 vtarget-0.8.6/vtarget/utils/
+-rw-rw-rw-   0        0        0     4125 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/__init__.py
+-rw-rw-rw-   0        0        0     1570 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/calc_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.393851 vtarget-0.8.6/vtarget/utils/database_connection/
+-rw-rw-rw-   0        0        0     3311 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/database_connection/field_validation.py
+-rw-rw-rw-   0        0        0     7400 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/database_connection/utilities.py
+-rw-rw-rw-   0        0        0     3516 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/email_sender.py
+-rw-rw-rw-   0        0        0      838 2024-03-25 15:35:41.000000 vtarget-0.8.6/vtarget/utils/encrypter.py
+-rw-rw-rw-   0        0        0    20811 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/modeling.py
+-rw-rw-rw-   0        0        0    13591 2024-03-25 15:35:53.000000 vtarget-0.8.6/vtarget/utils/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-10 13:56:00.397860 vtarget-0.8.6/vtarget.egg-info/
+-rw-rw-rw-   0        0        0     2144 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2259 2024-04-10 13:56:00.000000 vtarget-0.8.6/vtarget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      531 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-10 13:55:59.000000 vtarget-0.8.6/vtarget.egg-info/top_level.txt
```

### Comparing `vtarget-0.8.5/LICENSE` & `vtarget-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/PKG-INFO` & `vtarget-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtarget
-Version: 0.8.5
+Version: 0.8.6
 Summary: vtarget lib
 Author: vTarget Team
 Author-email: contact@vtarget.ai
 License: BSD
 Keywords: vtarget,dataprep
 Requires-Python: >=3.9.0,<3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `vtarget-0.8.5/README.md` & `vtarget-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/requirements.txt` & `vtarget-0.8.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/setup.py` & `vtarget-0.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         "vtarget.dataprep",
         "vtarget.dataprep.nodes",
         "vtarget.handlers",
         "vtarget.utils",
         "vtarget.utils.database_connection",
         "vtarget.language",
     ],
-    version="0.8.5",
+    version="0.8.6",
     description="vtarget lib",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="vTarget Team",
     author_email="contact@vtarget.ai",
     keywords=["vtarget", "dataprep"],
     classifiers=[],
```

### Comparing `vtarget-0.8.5/vtarget/dataprep/__init__.py` & `vtarget-0.8.6/vtarget/dataprep/__init__.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/builder.py` & `vtarget-0.8.6/vtarget/dataprep/builder.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/api_rest.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/api_rest.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/code.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/code.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/column.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/column.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/concat.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/concat.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/cross_join.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/cross_join.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/cumsum.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/cumsum.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/cut.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/cut.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/data_cleansing.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/data_cleansing.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/database.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/database.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/database_write.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/database_write.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/datetime_extract.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_extract.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/datetime_fill.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_fill.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/datetime_formatter.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     preconfigured_pattern = custom_pattern[1:-1]
                 else:
                     if not preconfigured_pattern:
                         msg = app_message.dataprep["nodes"]["datetime_formatter"]["pattern_required"](node_key)
                         return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
 
                 try:
-                    if df[column_to_convert].dtype == "object":
+                    if df[column_to_convert].dtype == "object" or df[column_to_convert].dtype == "str":
                         df[new_column_name] = pd.to_datetime(df[column_to_convert], format=preconfigured_pattern)
                         script.append(f"df['{new_column_name}'] = pd.to_datetime(df['{column_to_convert}'], format='{preconfigured_pattern}')")
                     else:
                         df[new_column_name] = df[column_to_convert].dt.strftime(preconfigured_pattern)
                         script.append(f"df['{new_column_name}'] = df['{column_to_convert}'].dt.strftime('{preconfigured_pattern}')")
 
                 except Exception as e:
```

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/datetime_range.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/datetime_range.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/describe.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/describe.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/df_maker.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/df_maker.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/drop_duplicates.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/drop_duplicates.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/dtype.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/dtype.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/email.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/email.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/excel.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/excel.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/filter.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/filter.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/formula.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/formula.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/groupby.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/groupby.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/input_data.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/input_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,86 @@
 import json
 import os
+from pathlib import Path
+from urllib.parse import urlparse
 
 import pandas as pd
 
 from vtarget.handlers.bug_handler import bug_handler
 from vtarget.handlers.cache_handler import cache_handler
 from vtarget.handlers.script_handler import script_handler
 from vtarget.language.app_message import app_message
 from vtarget.utils import normpath
+import requests
 
 
 class InputData:
     def exec(self, flow_id: str, node_key: str, pin: dict[str, pd.DataFrame], settings: dict):
         script = []
         script.append("\n# INPUT")
 
         encoding: str = settings["encoding"] if "encoding" in settings else "ISO-8859-1"
         dtype = str if "as_string" in settings and settings["as_string"] == True else None
         delimiter: str = settings["delimiter"] if "delimiter" in settings and settings["delimiter"] else None
         header: str = None if "has_header" in settings and settings["has_header"] == False else "infer"
-        file_path = normpath(settings["file_path"]) if "file_path" in settings else ""
-
+        file_path = settings["file_path"] if "file_path" in settings else ""
+        
+        is_external = file_path.startswith("http://") or file_path.startswith("https://")
+        if file_path and not is_external:
+            file_path = normpath(file_path)
+        
         # !! Deploy mode habilitado
         deploy_enabled: bool = settings["deploy_enabled"] if "deploy_enabled" in settings else False
 
         if deploy_enabled:
             if "deploy_file_path" not in settings or not settings["deploy_file_path"]:
                 msg = app_message.dataprep["nodes"]["deploy_enabled"](node_key)
                 return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
-
-            file_path = normpath(settings["deploy_file_path"]) if "deploy_file_path" in settings else ""
-
-        _, file_ext = os.path.splitext(file_path)
-        file_ext = file_ext[1:]
-        
-        # * check file exists
-        file_exists = os.path.exists(file_path)
+            
+            file_path = settings["deploy_file_path"] if "deploy_file_path" in settings else ""
+            
+            is_external = file_path.startswith("http://") or file_path.startswith("https://")
+            if file_path and not is_external:
+                file_path = normpath(file_path)
+            
         
-        if not file_exists:
-            msg = app_message.dataprep["nodes"]["input_data"]["file_not_exist"](node_key, file_path)
-            return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+        if not is_external:
+            # * check file exists
+            file_exists = os.path.exists(file_path)
+            
+            if not file_exists:
+                msg = app_message.dataprep["nodes"]["input_data"]["file_not_exist"](node_key, file_path)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+            # * get file extension
+            _, file_ext = os.path.splitext(file_path)
+            file_ext = file_ext[1:]
+            
+        else:
+            # * check if url exist
+            resp = requests.get(file_path)
+            if resp.status_code not in range(200, 300):
+                msg = app_message.dataprep["nodes"]["input_data"]["url_not_valid"](node_key, file_path)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
+            
+            # * get file extension from node config
+            file_ext = settings["extension"] if "extension" in settings else ""
+            if deploy_enabled:
+                file_ext = settings["deploy_extension"] if "deploy_extension" in settings else ""
+                
+            # * si la ext no existe en la config, intentar extraer del nombre del archivo
+            if not file_ext:
+                url_path = urlparse(file_path)
+                _, file_ext = os.path.splitext(Path(url_path.path))
+                file_ext = file_ext[1:]
+                
+            # * Error si no es posible extraer la extension dela archivo
+            if not file_ext:
+                msg = app_message.dataprep["nodes"]["input_data"]["missing_extension"](node_key)
+                return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
         
         try:
             bug_handler.console('Leyendo fuente "{}"...'.format(file_path), "trace", flow_id)
             if file_ext in ["csv", "txt"]:
                 df = pd.read_csv(
                     file_path,
                     dtype=dtype,
@@ -65,15 +102,16 @@
             elif file_ext == "json":
                 orient = settings["orient"] if "orient" in settings else "columns"
                 df = pd.read_json(file_path, orient=orient, encoding=encoding)
                 script.append(f"df = pd.read_json('{file_path}', orient='{orient}', encoding='{encoding}')")
                 
             elif file_ext in ["xls", "xlsx", "xlsm", "xlsb"]:
                 sheet_name = settings["sheet_name"] if "sheet_name" in settings else 0
-                df = pd.read_excel(file_path, dtype=dtype, sheet_name=sheet_name)
+                
+                df = pd.read_excel(file_path, dtype=dtype, sheet_name=sheet_name, engine=None)
                 dtype_str = 'str' if dtype != None else None
                 script.append(f"df = pd.read_excel('{file_path}', dtype={dtype_str}, sheet_name='{sheet_name}')")
                 
             else:
                 msg = app_message.dataprep["nodes"]["input_data"]["unknow_format"](node_key, file_ext)
                 return bug_handler.default_node_log(flow_id, node_key, msg, console_level="error")
```

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/inter_row.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/inter_row.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/isin.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/isin.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/melt.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/melt.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/merge.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/merge.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/output.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/output.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/pivot.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/pivot.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/rolling.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/rolling.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/sample.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/sample.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/shape.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/shape.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/sort.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/sort.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/split.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/split.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/switch.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/switch.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/unique.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/unique.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/v_output.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/v_output.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/nodes/value_counts.py` & `vtarget-0.8.6/vtarget/dataprep/nodes/value_counts.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/pipeline.py` & `vtarget-0.8.6/vtarget/dataprep/pipeline.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/dataprep/types.py` & `vtarget-0.8.6/vtarget/dataprep/types.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/handlers/automl_cache.py` & `vtarget-0.8.6/vtarget/handlers/automl_cache.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/handlers/autots_cache.py` & `vtarget-0.8.6/vtarget/handlers/autots_cache.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/handlers/bug_handler.py` & `vtarget-0.8.6/vtarget/handlers/bug_handler.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/handlers/cache_handler.py` & `vtarget-0.8.6/vtarget/handlers/cache_handler.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/handlers/event_handler.py` & `vtarget-0.8.6/vtarget/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/language/app_message.py` & `vtarget-0.8.6/vtarget/language/app_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,16 @@
                     "unknow_rule": lambda node_key, rule: f"({node_key}): No se reconoce la regla '{rule}'",
                     "failed_condition": lambda node_key: f"({node_key}): No fue posible procesar la condición",
                     "unknow_column": lambda node_key, field: f"({node_key}): No existe la columna '{field}' en el Dataframe de entrada",
                     "unknow_operator": lambda node_key, operator: f"({node_key}): Operador '{operator}' no reconocido ",
                 },
                 "group_by": {"missing_props": lambda node_key: f"({node_key}): Alguna de las propiedades para el método de agregación no ha sido proporcionada"},
                 "input_data": {
+                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' no existe o no es válida",
+                    "missing_extension": lambda node_key: f"({node_key}): No existe extensión del archivo",
                     "file_not_exist": lambda node_key, path: f"({node_key}): Archivo '{path}' no existe en disco",
                     "unknow_format": lambda node_key, format: f"({node_key}): Formato '{format}' no reconocido",
                     "end_start_spaces": lambda node_key: f"({node_key}): Archivo fuente contiene espacios al inicio o final del nombre de una o más columnas. Se ha corregido para la lectura",
                 },
                 "inter_row": {
                     "fillna": lambda node_key: f"({node_key}): La función 'fillna', debes especificar el valor para los nulos",
                 },
@@ -377,14 +379,16 @@
                     "unknow_rule": lambda node_key, rule: f"({node_key}): The rule is not recognized '{rule}'",
                     "failed_condition": lambda node_key: f"({node_key}): Condition could not be processed",
                     "unknow_column": lambda node_key, field: f"({node_key}): Column '{field}' does not exist in the input Dataframe",
                     "unknow_operator": lambda node_key, operator: f"({node_key}): Operator '{operator}' not recognized",
                 },
                 "group_by": {"missing_props": lambda node_key: f"({node_key}): Some of the properties of aggregate method have not been provided"},
                 "input_data": {
+                    "url_not_valid": lambda node_key, path: f"({node_key}): Url '{path}' does not exist or does not valid",
+                    "missing_extension": lambda node_key: f"({node_key}): Does not exist extension",
                     "file_not_exist": lambda node_key, path: f"({node_key}): File '{path}' does not exist on disk",
                     "unknow_format": lambda node_key, format: f"({node_key}): Format '{format}' not recognized",
                     "end_start_spaces": lambda node_key: f"({node_key}): Source file contains spaces at the beginning or end of the name of one or more columns. It has been corrected for reading",
                 },
                 "inter_row": {
                     "fillna": lambda node_key: f"({node_key}): 'fillna' function, must specify the value for nulls",
                 },
```

### Comparing `vtarget-0.8.5/vtarget/utils/__init__.py` & `vtarget-0.8.6/vtarget/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/calc_metrics.py` & `vtarget-0.8.6/vtarget/utils/calc_metrics.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/database_connection/field_validation.py` & `vtarget-0.8.6/vtarget/utils/database_connection/field_validation.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/database_connection/utilities.py` & `vtarget-0.8.6/vtarget/utils/database_connection/utilities.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/email_sender.py` & `vtarget-0.8.6/vtarget/utils/email_sender.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/encrypter.py` & `vtarget-0.8.6/vtarget/utils/encrypter.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/modeling.py` & `vtarget-0.8.6/vtarget/utils/modeling.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget/utils/utilities.py` & `vtarget-0.8.6/vtarget/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget.egg-info/PKG-INFO` & `vtarget-0.8.6/vtarget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtarget
-Version: 0.8.5
+Version: 0.8.6
 Summary: vtarget lib
 Author: vTarget Team
 Author-email: contact@vtarget.ai
 License: BSD
 Keywords: vtarget,dataprep
 Requires-Python: >=3.9.0,<3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `vtarget-0.8.5/vtarget.egg-info/SOURCES.txt` & `vtarget-0.8.6/vtarget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vtarget-0.8.5/vtarget.egg-info/requires.txt` & `vtarget-0.8.6/vtarget.egg-info/requires.txt`

 * *Files identical despite different names*

