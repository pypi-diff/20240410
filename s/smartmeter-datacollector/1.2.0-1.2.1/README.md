# Comparing `tmp/smartmeter-datacollector-1.2.0.tar.gz` & `tmp/smartmeter-datacollector-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartmeter-datacollector-1.2.0.tar", last modified: Wed Mar 27 12:50:35 2024, max compression
+gzip compressed data, was "smartmeter-datacollector-1.2.1.tar", last modified: Wed Apr 10 10:54:53 2024, max compression
```

## Comparing `smartmeter-datacollector-1.2.0.tar` & `smartmeter-datacollector-1.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.113884 smartmeter-datacollector-1.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      321 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/bin/smartmeter-datacollector
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.113884 smartmeter-datacollector-1.2.0/smartmeter_datacollector/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/data_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/logger_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/mqtt_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/cosem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/iskraam550.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/kamstrup_han.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge360.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge450.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge570.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/meter_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/obis.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/serial_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:50:35.000000 smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:50:35.117884 smartmeter-datacollector-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_hdlc_dlms_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_iskraam550.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_lge450.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_lge570.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_meter_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_mqtt_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-27 12:50:13.000000 smartmeter-datacollector-1.2.0/tests/test_obis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.203357 smartmeter-datacollector-1.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      321 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/bin/smartmeter-datacollector
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.203357 smartmeter-datacollector-1.2.1/smartmeter_datacollector/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.203357 smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/data_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/logger_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/mqtt_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/cosem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/iskraam550.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/kamstrup_han.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge450.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge570.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/meter_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/obis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/serial_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:54:53.000000 smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:54:53.207357 smartmeter-datacollector-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_hdlc_dlms_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_iskraam550.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_lge450.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_lge570.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_meter_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_mqtt_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-10 10:54:42.000000 smartmeter-datacollector-1.2.1/tests/test_obis.py
```

### Comparing `smartmeter-datacollector-1.2.0/LICENSE` & `smartmeter-datacollector-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/PKG-INFO` & `smartmeter-datacollector-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartmeter-datacollector
-Version: 1.2.0
+Version: 1.2.1
 Summary: Smart Meter Data Collector
 Home-page: https://github.com/scs/smartmeter-datacollector
 Author: Supercomputing Systems AG
 Author-email: info@scs.ch
 Maintainer: Supercomputing Systems AG
 Maintainer-email: info@scs.ch
 License: GPLv2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.2.1 Summary:
 Smart Meter Data Collector Home-page: https://github.com/scs/smartmeter-
 datacollector Author: Supercomputing Systems AG Author-email: info@scs.ch
 Maintainer: Supercomputing Systems AG Maintainer-email: info@scs.ch License:
 GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-datacollector
 Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/
 issues Project-URL: Pull Requests, https://github.com/scs/smartmeter-
 datacollector/pulls Project-URL: SCS, https://www.scs.ch Classifier:
```

### Comparing `smartmeter-datacollector-1.2.0/README.md` & `smartmeter-datacollector-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/pyproject.toml` & `smartmeter-datacollector-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/setup.py` & `smartmeter-datacollector-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/app.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/app.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/collector.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/collector.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/config.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/config.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/factory.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/factory.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/data_sink.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/data_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/logger_sink.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/logger_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/sinks/mqtt_sink.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/sinks/mqtt_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/cosem.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/cosem.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,16 @@
         return meter_id
 
     def retrieve_time_from_dlms_registers(self, dlms_objects: Dict[OBISCode, Any]) -> Optional[datetime]:
         clock_obj = dlms_objects.get(Cosem.CLOCK_DEFAULT_OBIS, None)
         if clock_obj and isinstance(clock_obj, GXDLMSClock):
             timestamp = self._extract_datetime(clock_obj)
             if timestamp:
-                return timestamp
+                # assume local time if tzinfo is None
+                return timestamp.astimezone(timestamp.tzinfo)
         return None
 
     def get_register(self, obis: OBISCode) -> Optional[RegisterCosem]:
         return self._register_obis.get(obis, None)
 
     def _trigger_id_detect_counter(self):
         self._id_detect_countdown -= 1
```

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/hdlc_dlms_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,18 @@
         LOGGER.debug("DLMS packet complete and ready for parsing.")
         self._hdlc_buffer.clear()
         return True
 
     def extract_message_time(self) -> Optional[datetime]:
         if not isinstance(self._dlms_data.time, GXDateTime):
             return None
-        if isinstance(self._dlms_data.time.value, datetime):
-            return self._dlms_data.time.value
+        dt = self._dlms_data.time.value
+        if isinstance(dt, datetime):
+            # assume local time if tzinfo is None
+            return dt.astimezone(dt.tzinfo)
         return None
 
     def parse_to_dlms_objects(self) -> List[GXDLMSObject]:
         if not isinstance(self._dlms_data.value, list) or not self._dlms_data.value:
             self._dlms_data.clear()
             LOGGER.error("DLMS data is no list or empty list. Not parsable.")
             return []
@@ -129,17 +131,16 @@
         if not timestamp:
             timestamp = message_time
         if not timestamp:
             LOGGER.warning("Unable to get timestamp from message. Falling back to system time.")
             self._use_system_time = True
             timestamp = datetime.now(timezone.utc)
 
-        if not timestamp.tzinfo:
-            # if timezone info not set, assume UTC
-            timestamp = timestamp.replace(tzinfo=timezone.utc)
+        # convert to UTC format
+        timestamp = timestamp.astimezone(timezone.utc)
 
         # Extract register data
         data_points: List[MeterDataPoint] = []
         for obis, obj in filter(lambda o: o[1].getObjectType() == ObjectType.REGISTER, obis_obj_pairs.items()):
             reg_type = self._cosem.get_register(obis)
             if reg_type and isinstance(obj, GXDLMSRegister):
                 raw_value = self._extract_register_value(obj)
```

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/iskraam550.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/iskraam550.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/kamstrup_han.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/kamstrup_han.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge360.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge360.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge450.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge450.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/lge570.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/lge570.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/meter.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/meter.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/meter_data.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/meter_data.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/obis.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/obis.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/reader.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/reader.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector/smartmeter/serial_reader.py` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector/smartmeter/serial_reader.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/PKG-INFO` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartmeter-datacollector
-Version: 1.2.0
+Version: 1.2.1
 Summary: Smart Meter Data Collector
 Home-page: https://github.com/scs/smartmeter-datacollector
 Author: Supercomputing Systems AG
 Author-email: info@scs.ch
 Maintainer: Supercomputing Systems AG
 Maintainer-email: info@scs.ch
 License: GPLv2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: smartmeter-datacollector Version: 1.2.1 Summary:
 Smart Meter Data Collector Home-page: https://github.com/scs/smartmeter-
 datacollector Author: Supercomputing Systems AG Author-email: info@scs.ch
 Maintainer: Supercomputing Systems AG Maintainer-email: info@scs.ch License:
 GPLv2 Project-URL: Source, https://github.com/scs/smartmeter-datacollector
 Project-URL: Bug Reports, https://github.com/scs/smartmeter-datacollector/
 issues Project-URL: Pull Requests, https://github.com/scs/smartmeter-
 datacollector/pulls Project-URL: SCS, https://www.scs.ch Classifier:
```

### Comparing `smartmeter-datacollector-1.2.0/smartmeter_datacollector.egg-info/SOURCES.txt` & `smartmeter-datacollector-1.2.1/smartmeter_datacollector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/tests/test_collector.py` & `smartmeter-datacollector-1.2.1/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/tests/test_config.py` & `smartmeter-datacollector-1.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/tests/test_hdlc_dlms_parser.py` & `smartmeter-datacollector-1.2.1/tests/test_hdlc_dlms_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,16 @@
 
         assert isinstance(meter_data, list)
         assert len(meter_data) == 11
         assert any(data.type == MeterDataPointTypes.ACTIVE_POWER_P.value for data in meter_data)
         assert any(data.type == MeterDataPointTypes.ACTIVE_POWER_N.value for data in meter_data)
         assert all(isinstance(data.value, float) for data in meter_data)
         assert all(data.source == "LGZ1030655933512" for data in meter_data)
-        assert all(data.timestamp.strftime(r"%m/%d/%y %H:%M:%S") == "07/06/21 14:58:18" for data in meter_data)
+        assert all(data.timestamp.astimezone().strftime(r"%m/%d/%y %H:%M:%S")
+                   == "07/06/21 14:58:18" for data in meter_data)
 
     def test_parse_dlms_to_meter_data2(self, unencrypted_valid_data_lg2: List[bytes], cosem_config_lg: Cosem):
         parser = prepare_parser(unencrypted_valid_data_lg2, cosem_config_lg)
         dlms_objects = parser.parse_to_dlms_objects()
         meter_data = parser.convert_dlms_bundle_to_reader_data(dlms_objects)
 
         assert isinstance(meter_data, list)
```

### Comparing `smartmeter-datacollector-1.2.0/tests/test_iskraam550.py` & `smartmeter-datacollector-1.2.1/tests/test_iskraam550.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,8 +61,9 @@
     assert any(data.type == MeterDataPointTypes.ACTIVE_ENERGY_N.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q1.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q2.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q3.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q4.value for data in values)
     assert any(data.type == MeterDataPointTypes.POWER_FACTOR.value for data in values)
     assert all(data.source == "ISK1030775213859" for data in values)
-    assert all(data.timestamp.strftime(r"%m/%d/%y %H:%M:%S") == "08/15/20 06:19:45" for data in values)
+    # message time comes with timezone info (+02:00)
+    assert all(data.timestamp.strftime(r"%m/%d/%y %H:%M:%S") == "08/15/20 04:19:45" for data in values)
```

### Comparing `smartmeter-datacollector-1.2.0/tests/test_lge450.py` & `smartmeter-datacollector-1.2.1/tests/test_lge450.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     assert any(data.type == MeterDataPointTypes.ACTIVE_ENERGY_N.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q1.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q2.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q3.value for data in values)
     assert any(data.type == MeterDataPointTypes.REACTIVE_ENERGY_Q4.value for data in values)
     assert any(data.type == MeterDataPointTypes.POWER_FACTOR.value for data in values)
     assert all(data.source == "LGZ1030655933512" for data in values)
-    assert all(data.timestamp.strftime(r"%m/%d/%y %H:%M:%S") == "07/06/21 14:58:18" for data in values)
+    assert all(data.timestamp.astimezone().strftime(r"%m/%d/%y %H:%M:%S") == "07/06/21 14:58:18" for data in values)
 
 
 @pytest.mark.asyncio
 async def test_lge450_do_not_provide_invalid_data(mocker: MockerFixture,
                                                   unencrypted_invalid_data_lg: List[bytes]):
     observer = mocker.stub("collector_mock")
     observer.mock_add_spec(['notify'])
```

### Comparing `smartmeter-datacollector-1.2.0/tests/test_lge570.py` & `smartmeter-datacollector-1.2.1/tests/test_lge570.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from smartmeter_datacollector.smartmeter.lge570 import LGE570
 from smartmeter_datacollector.smartmeter.meter_data import MeterDataPointTypes
 
 from .utils import *
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="Python3.7 does not support AsyncMock.")
 @pytest.mark.asyncio
 async def test_lge570_parse_and_provide_encrypted_data(mocker: MockerFixture,
                                                        encrypted_valid_data_lge570: List[bytes]):
     observer = mocker.stub("collector_mock")
     observer.mock_add_spec(['notify'])
     serial_mock = mocker.patch("smartmeter_datacollector.smartmeter.meter.SerialReader",
                                autospec=True).return_value
```

### Comparing `smartmeter-datacollector-1.2.0/tests/test_meter_data.py` & `smartmeter-datacollector-1.2.1/tests/test_meter_data.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/tests/test_mqtt_sink.py` & `smartmeter-datacollector-1.2.1/tests/test_mqtt_sink.py`

 * *Files identical despite different names*

### Comparing `smartmeter-datacollector-1.2.0/tests/test_obis.py` & `smartmeter-datacollector-1.2.1/tests/test_obis.py`

 * *Files identical despite different names*

