# Comparing `tmp/mozilla-metric-config-parser-2024.3.2.tar.gz` & `tmp/mozilla-metric-config-parser-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2024.3.2.tar", last modified: Thu Mar 21 20:06:52 2024, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2024.4.1.tar", last modified: Wed Apr 10 13:23:58 2024, max compression
```

## Comparing `mozilla-metric-config-parser-2024.3.2.tar` & `mozilla-metric-config-parser-2024.4.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.135158 mozilla-metric-config-parser-2024.3.2/
--rw-r--r--   0 root         (0) root         (0)    16725 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1590 2024-03-21 20:06:52.131158 mozilla-metric-config-parser-2024.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.123158 mozilla-metric-config-parser-2024.3.2/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7137 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    27979 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    15847 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.127158 mozilla-metric-config-parser-2024.3.2/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      143 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.127158 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.127158 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     6657 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    26303 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    16931 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    11571 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    12162 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 20:06:52.131158 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1590 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      274 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 20:06:52.000000 mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-21 20:06:52.135158 mozilla-metric-config-parser-2024.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1574 2024-03-21 20:06:42.000000 mozilla-metric-config-parser-2024.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/
+-rw-r--r--   0 root         (0) root         (0)    16725 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.654162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7137 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    27979 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    15859 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.654162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      143 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     6657 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    26303 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    16931 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    11572 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    12162 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 13:23:58.000000 mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-10 13:23:58.658162 mozilla-metric-config-parser-2024.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-04-10 13:23:49.000000 mozilla-metric-config-parser-2024.4.1/setup.py
```

### Comparing `mozilla-metric-config-parser-2024.3.2/LICENSE` & `mozilla-metric-config-parser-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/PKG-INFO` & `mozilla-metric-config-parser-2024.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/config.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/function.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 
 
 class AnalysisPeriod(Enum):
     DAY = "day"
     WEEK = "week"
     DAYS_28 = "days28"
     OVERALL = "overall"
-    WEEK_PREENROLLMENT = "week_preenrollment"
-    DAYS_28_PREENROLLMENT = "days28_preenrollment"
+    PREENROLLMENT_WEEK = "preenrollment_week"
+    PREENROLLMENT_DAYS_28 = "preenrollment_days28"
 
     @property
     def mozanalysis_label(self) -> str:
         d = {
             "day": "daily",
             "week": "weekly",
             "days28": "28_day",
             "overall": "overall",
-            "week_preenrollment": "week_preenrollment",
-            "days28_preenrollment": "days28_preenrollment",
+            "preenrollment_week": "preenrollment_weekly",
+            "preenrollment_days28": "preenrollment_days28",
         }
         return d[self.value]
 
     @property
     def table_suffix(self) -> str:
         d = {
             "day": "daily",
             "week": "weekly",
             "days28": "days28",
             "overall": "overall",
-            "week_preenrollment": "week_preenrollment",
-            "days28_preenrollment": "days28_preenrollment",
+            "preenrollment_week": "preenrollment_weekly",
+            "preenrollment_days28": "preenrollment_days28",
         }
         return d[self.value]
 
 
 class MetricLevel(Enum):
     GOLD = "gold"
     SILVER = "silver"
@@ -336,16 +336,16 @@
 class MetricsSpec:
     """Describes the interface for the metrics section in configuration."""
 
     daily: List[MetricReference] = attr.Factory(list)
     weekly: List[MetricReference] = attr.Factory(list)
     days28: List[MetricReference] = attr.Factory(list)
     overall: List[MetricReference] = attr.Factory(list)
-    week_preenrollment: List[MetricReference] = attr.Factory(list)
-    days28_preenrollment: List[MetricReference] = attr.Factory(list)
+    preenrollment_weekly: List[MetricReference] = attr.Factory(list)
+    preenrollment_days28: List[MetricReference] = attr.Factory(list)
     definitions: Dict[str, MetricDefinition] = attr.Factory(dict)
 
     @classmethod
     def from_dict(cls, d: dict) -> "MetricsSpec":
         params: Dict[str, Any] = {}
         known_keys = {f.name for f in attr.fields(cls)}
         for k in known_keys:
@@ -400,16 +400,16 @@
 
         The `other` MetricsSpec overwrites existing metrics.
         """
         self.daily = other.daily + self.daily
         self.weekly = other.weekly + self.weekly
         self.days28 = other.days28 + self.days28
         self.overall = other.overall + self.overall
-        self.week_preenrollment = other.week_preenrollment + self.week_preenrollment
-        self.days28_preenrollment = other.days28_preenrollment + self.days28_preenrollment
+        self.preenrollment_weekly = other.preenrollment_weekly + self.preenrollment_weekly
+        self.preenrollment_days28 = other.preenrollment_days28 + self.preenrollment_days28
 
         seen = []
         for key, _ in self.definitions.items():
             if key in other.definitions:
                 self.definitions[key].merge(other.definitions[key])
             seen.append(key)
         for key, definition in other.definitions.items():
```

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/population.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/project.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,40 +173,40 @@
         overall_pre_treatments = [
             m for m in cfg.metrics[AnalysisPeriod.OVERALL] if m.metric.name == "spam"
         ][0].pre_treatments
 
         assert len(overall_pre_treatments) == 1
         assert overall_pre_treatments[0].name == "remove_nulls"
 
-    def test_preenrollmennt(self, experiments, config_collection):
+    def test_preenrollment(self, experiments, config_collection):
         config_str = dedent(
             """
             [metrics]
-            days28_preenrollment = ["spam"]
-            week_preenrollment = ["spam"]
+            preenrollment_days28 = ["spam"]
+            preenrollment_weekly = ["spam"]
 
             [metrics.spam]
             data_source = "main"
             select_expression = "1"
 
             [metrics.spam.statistics.binomial]
             """
         )
 
         spec = AnalysisSpec.from_dict(toml.loads(config_str))
         cfg = spec.resolve(experiments[0], config_collection)
         week_metrics = [
-            m for m in cfg.metrics[AnalysisPeriod.WEEK_PREENROLLMENT] if m.metric.name == "spam"
+            m for m in cfg.metrics[AnalysisPeriod.PREENROLLMENT_WEEK] if m.metric.name == "spam"
         ]
 
         assert len(week_metrics) == 1
         assert week_metrics[0].metric.name == "spam"
 
         days28_metrics = [
-            m for m in cfg.metrics[AnalysisPeriod.DAYS_28_PREENROLLMENT] if m.metric.name == "spam"
+            m for m in cfg.metrics[AnalysisPeriod.PREENROLLMENT_DAYS_28] if m.metric.name == "spam"
         ]
 
         assert len(days28_metrics) == 1
         assert days28_metrics[0].metric.name == "spam"
 
 
 class TestExperimentConf:
```

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_metric.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from metric_config_parser.metric import MetricDefinition
+from metric_config_parser.metric import AnalysisPeriod, MetricDefinition
 from metric_config_parser.parameter import ParameterDefinition
 
 
 class TestMetricDefinition:
     @pytest.mark.parametrize(
         "input,expected",
         (
@@ -71,7 +71,12 @@
 
         param_definition, select_template = input
 
         actual = MetricDefinition.generate_select_expression(
             param_definition, select_template, config_collection
         )
         assert expected == actual
+
+    def test_analysis_periods_conflicts(self):
+        for test_period in AnalysisPeriod:
+            for period in [p for p in AnalysisPeriod if p != test_period]:
+                assert not period.value.startswith(f"{test_period.value}_")
```

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/metric_config_parser/util.py` & `mozilla-metric-config-parser-2024.4.1/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mozilla-metric-config-parser-2024.3.2/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2024.4.1/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2024.3.2/setup.py` & `mozilla-metric-config-parser-2024.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,9 +61,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2024.3.2",
+    version="2024.4.1",
 )
```

