# Comparing `tmp/nrewebservices-0.2.0.tar.gz` & `tmp/nrewebservices-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nrewebservices-0.2.0.tar", last modified: Sun Dec 30 20:47:38 2018, max compression
+gzip compressed data, was "nrewebservices-0.2.1.tar", last modified: Wed Apr 10 11:50:20 2024, max compression
```

## Comparing `nrewebservices-0.2.0.tar` & `nrewebservices-0.2.1.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/
--rw-r--r--   0 gberg     (1000) users      (100)     1808 2018-12-30 20:45:19.000000 nrewebservices-0.2.0/CHANGELOG.rst
--rw-r--r--   0 gberg     (1000) users      (100)     1391 2016-08-16 11:55:08.000000 nrewebservices-0.2.0/LICENSE
--rw-r--r--   0 gberg     (1000) users      (100)      255 2016-09-09 22:52:00.000000 nrewebservices-0.2.0/MANIFEST.in
--rw-r--r--   0 gberg     (1000) users      (100)     3300 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/PKG-INFO
--rw-r--r--   0 gberg     (1000) users      (100)     1869 2018-12-30 20:26:22.000000 nrewebservices-0.2.0/README.rst
--rw-r--r--   0 gberg     (1000) users      (100)     1342 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/RELEASING.rst
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/docs/
--rw-r--r--   0 gberg     (1000) users      (100)     7638 2016-08-17 20:05:15.000000 nrewebservices-0.2.0/docs/Makefile
--rw-r--r--   0 gberg     (1000) users      (100)      203 2016-08-21 15:32:25.000000 nrewebservices-0.2.0/docs/api-hsp.rst
--rw-r--r--   0 gberg     (1000) users      (100)     2399 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/docs/api-ldbws.rst
--rw-r--r--   0 gberg     (1000) users      (100)      193 2016-08-21 15:33:38.000000 nrewebservices-0.2.0/docs/api-staff.rst
--rw-r--r--   0 gberg     (1000) users      (100)      120 2016-08-21 13:55:38.000000 nrewebservices-0.2.0/docs/api.rst
--rw-r--r--   0 gberg     (1000) users      (100)    10253 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/docs/conf.py
--rw-r--r--   0 gberg     (1000) users      (100)      227 2016-08-21 15:22:32.000000 nrewebservices-0.2.0/docs/hsp.rst
--rw-r--r--   0 gberg     (1000) users      (100)      413 2016-08-21 14:25:21.000000 nrewebservices-0.2.0/docs/index.rst
--rw-r--r--   0 gberg     (1000) users      (100)     1751 2018-12-30 20:26:22.000000 nrewebservices-0.2.0/docs/introduction.rst
--rw-r--r--   0 gberg     (1000) users      (100)     3981 2016-08-25 18:00:59.000000 nrewebservices-0.2.0/docs/ldbws.rst
--rw-r--r--   0 gberg     (1000) users      (100)     7748 2016-08-17 20:05:15.000000 nrewebservices-0.2.0/docs/make.bat
--rw-r--r--   0 gberg     (1000) users      (100)      585 2016-08-21 15:26:14.000000 nrewebservices-0.2.0/docs/staff.rst
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/examples/
--rwxr-xr-x   0 gberg     (1000) users      (100)     3175 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/examples/ldbws.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices/
--rw-r--r--   0 gberg     (1000) users      (100)      117 2016-08-31 19:10:25.000000 nrewebservices-0.2.0/nrewebservices/__init__.py
--rw-r--r--   0 gberg     (1000) users      (100)       18 2018-12-30 20:44:53.000000 nrewebservices-0.2.0/nrewebservices/__release__.py
--rw-r--r--   0 gberg     (1000) users      (100)       16 2018-12-30 20:44:53.000000 nrewebservices-0.2.0/nrewebservices/__version__.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices/common/
--rw-r--r--   0 gberg     (1000) users      (100)      217 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/nrewebservices/common/__init__.py
--rw-r--r--   0 gberg     (1000) users      (100)     1394 2018-12-30 20:10:23.000000 nrewebservices-0.2.0/nrewebservices/common/soap.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices/ldbws/
--rw-r--r--   0 gberg     (1000) users      (100)      307 2016-08-17 21:08:02.000000 nrewebservices-0.2.0/nrewebservices/ldbws/__init__.py
--rw-r--r--   0 gberg     (1000) users      (100)    40895 2018-12-30 20:12:24.000000 nrewebservices-0.2.0/nrewebservices/ldbws/responses.py
--rw-r--r--   0 gberg     (1000) users      (100)    23016 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/nrewebservices/ldbws/webservice.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/
--rw-r--r--   0 gberg     (1000) users      (100)     3300 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/PKG-INFO
--rw-r--r--   0 gberg     (1000) users      (100)     2199 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/SOURCES.txt
--rw-r--r--   0 gberg     (1000) users      (100)        1 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/dependency_links.txt
--rw-r--r--   0 gberg     (1000) users      (100)       16 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/requires.txt
--rw-r--r--   0 gberg     (1000) users      (100)       15 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/nrewebservices.egg-info/top_level.txt
--rw-r--r--   0 gberg     (1000) users      (100)       92 2016-09-01 17:43:02.000000 nrewebservices-0.2.0/requirements-dev.txt
--rw-r--r--   0 gberg     (1000) users      (100)       16 2016-08-31 18:58:25.000000 nrewebservices-0.2.0/requirements.txt
--rw-r--r--   0 gberg     (1000) users      (100)       61 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/setup.cfg
--rw-r--r--   0 gberg     (1000) users      (100)     1376 2018-12-30 20:44:53.000000 nrewebservices-0.2.0/setup.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/.cache/
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/.cache/v/
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/.cache/v/cache/
--rw-r--r--   0 gberg     (1000) users      (100)       66 2016-08-17 13:27:38.000000 nrewebservices-0.2.0/tests/.cache/v/cache/lastfailed
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/data/
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/data/ldbws/
--rw-r--r--   0 gberg     (1000) users      (100)     7200 2016-09-03 16:33:14.000000 nrewebservices-0.2.0/tests/data/ldbws/basic-fastest-departures-board-with-details.xml
--rw-r--r--   0 gberg     (1000) users      (100)     3200 2016-09-02 13:24:29.000000 nrewebservices-0.2.0/tests/data/ldbws/basic-fastest-departures-board.xml
--rw-r--r--   0 gberg     (1000) users      (100)     4392 2016-09-03 16:43:18.000000 nrewebservices-0.2.0/tests/data/ldbws/basic-service-details.xml
--rw-r--r--   0 gberg     (1000) users      (100)     7391 2016-08-16 21:08:40.000000 nrewebservices-0.2.0/tests/data/ldbws/basic-station-board-departures.xml
--rw-r--r--   0 gberg     (1000) users      (100)    21940 2016-08-06 21:06:12.000000 nrewebservices-0.2.0/tests/data/ldbws/basic-station-board-with-details-departures.xml
--rw-r--r--   0 gberg     (1000) users      (100)    15988 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/data/ldbws/departure-board-with-partial-formation-and-loading.xml
--rw-r--r--   0 gberg     (1000) users      (100)     6324 2018-11-05 18:52:55.000000 nrewebservices-0.2.0/tests/data/ldbws/service-details-with-partial-formation-and-loading.xml
--rw-r--r--   0 gberg     (1000) users      (100)     1030 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/helpers.py
--rw-r--r--   0 gberg     (1000) users      (100)     3000 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/test_ldbws_fastest_departures_board_basics.py
--rw-r--r--   0 gberg     (1000) users      (100)     4125 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/test_ldbws_fastest_departures_board_with_details.py
--rw-r--r--   0 gberg     (1000) users      (100)     3584 2018-12-30 20:12:58.000000 nrewebservices-0.2.0/tests/test_ldbws_formations.py
--rw-r--r--   0 gberg     (1000) users      (100)     3392 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/test_ldbws_service_details.py
--rw-r--r--   0 gberg     (1000) users      (100)    17547 2018-12-30 20:22:15.000000 nrewebservices-0.2.0/tests/test_ldbws_session.py
--rw-r--r--   0 gberg     (1000) users      (100)     6035 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/test_ldbws_station_board_basics.py
--rw-r--r--   0 gberg     (1000) users      (100)     4010 2018-05-13 14:27:05.000000 nrewebservices-0.2.0/tests/test_ldbws_station_board_with_details.py
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/wsdl/
-drwxr-xr-x   0 gberg     (1000) users      (100)        0 2018-12-30 20:47:38.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/
--rw-r--r--   0 gberg     (1000) users      (100)      471 2015-02-17 11:02:12.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/darwin_token_types_2013-11-28.wsdl
--rw-r--r--   0 gberg     (1000) users      (100)     1116 2015-02-17 11:02:12.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/darwin_token_types_2013-11-28.xsd
--rw-r--r--   0 gberg     (1000) users      (100)     3709 2015-02-17 11:02:12.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2007-10-10_ldb_common_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    21741 2015-02-17 11:02:12.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2012-01-13_ldb_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)     1358 2015-12-11 05:08:38.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2015-11-27_ldb_common_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    31969 2015-12-11 05:08:38.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2015-11-27_ldb_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    25467 2016-04-08 04:09:08.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb.wsdl
--rw-r--r--   0 gberg     (1000) users      (100)      658 2016-04-08 04:09:08.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb_common_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    11880 2016-04-08 04:09:08.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)     1313 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-02-02_ldb_common_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    25587 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb.wsdl
--rw-r--r--   0 gberg     (1000) users      (100)     1856 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb_common_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)    25457 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb_types.xsd
--rw-r--r--   0 gberg     (1000) users      (100)      853 2018-12-30 19:54:05.000000 nrewebservices-0.2.0/tests/wsdl/ldbws/wsdl.aspx
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.157675 nrewebservices-0.2.1/
+-rw-r--r--   0 gberg     (1000) users      (100)     1937 2024-04-10 11:49:15.000000 nrewebservices-0.2.1/CHANGELOG.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     1391 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/LICENSE
+-rw-r--r--   0 gberg     (1000) users      (100)      255 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/MANIFEST.in
+-rw-r--r--   0 gberg     (1000) users      (100)     2952 2024-04-10 11:50:20.157675 nrewebservices-0.2.1/PKG-INFO
+-rw-r--r--   0 gberg     (1000) users      (100)     1867 2024-04-10 11:47:37.000000 nrewebservices-0.2.1/README.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     1342 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/RELEASING.rst
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.151008 nrewebservices-0.2.1/docs/
+-rw-r--r--   0 gberg     (1000) users      (100)     7638 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/Makefile
+-rw-r--r--   0 gberg     (1000) users      (100)      203 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/api-hsp.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     2399 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/api-ldbws.rst
+-rw-r--r--   0 gberg     (1000) users      (100)      193 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/api-staff.rst
+-rw-r--r--   0 gberg     (1000) users      (100)      120 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/api.rst
+-rw-r--r--   0 gberg     (1000) users      (100)    10253 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/conf.py
+-rw-r--r--   0 gberg     (1000) users      (100)      227 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/hsp.rst
+-rw-r--r--   0 gberg     (1000) users      (100)      413 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/index.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     1751 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/introduction.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     3981 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/ldbws.rst
+-rw-r--r--   0 gberg     (1000) users      (100)     7748 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/make.bat
+-rw-r--r--   0 gberg     (1000) users      (100)      585 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/docs/staff.rst
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.151008 nrewebservices-0.2.1/examples/
+-rwxr-xr-x   0 gberg     (1000) users      (100)     3175 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/examples/ldbws.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/nrewebservices/
+-rw-r--r--   0 gberg     (1000) users      (100)      117 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/__init__.py
+-rw-r--r--   0 gberg     (1000) users      (100)       18 2024-04-10 11:49:15.000000 nrewebservices-0.2.1/nrewebservices/__release__.py
+-rw-r--r--   0 gberg     (1000) users      (100)       16 2024-04-10 11:49:15.000000 nrewebservices-0.2.1/nrewebservices/__version__.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/nrewebservices/common/
+-rw-r--r--   0 gberg     (1000) users      (100)      217 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/common/__init__.py
+-rw-r--r--   0 gberg     (1000) users      (100)     1394 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/common/soap.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/nrewebservices/ldbws/
+-rw-r--r--   0 gberg     (1000) users      (100)      307 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/ldbws/__init__.py
+-rw-r--r--   0 gberg     (1000) users      (100)    40895 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/ldbws/responses.py
+-rw-r--r--   0 gberg     (1000) users      (100)    23016 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/nrewebservices/ldbws/webservice.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/nrewebservices.egg-info/
+-rw-r--r--   0 gberg     (1000) users      (100)     2952 2024-04-10 11:50:20.000000 nrewebservices-0.2.1/nrewebservices.egg-info/PKG-INFO
+-rw-r--r--   0 gberg     (1000) users      (100)     2167 2024-04-10 11:50:20.000000 nrewebservices-0.2.1/nrewebservices.egg-info/SOURCES.txt
+-rw-r--r--   0 gberg     (1000) users      (100)        1 2024-04-10 11:50:20.000000 nrewebservices-0.2.1/nrewebservices.egg-info/dependency_links.txt
+-rw-r--r--   0 gberg     (1000) users      (100)       10 2024-04-10 11:50:20.000000 nrewebservices-0.2.1/nrewebservices.egg-info/requires.txt
+-rw-r--r--   0 gberg     (1000) users      (100)       15 2024-04-10 11:50:20.000000 nrewebservices-0.2.1/nrewebservices.egg-info/top_level.txt
+-rw-r--r--   0 gberg     (1000) users      (100)       92 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/requirements-dev.txt
+-rw-r--r--   0 gberg     (1000) users      (100)       10 2024-04-10 11:32:54.000000 nrewebservices-0.2.1/requirements.txt
+-rw-r--r--   0 gberg     (1000) users      (100)       61 2024-04-10 11:50:20.157675 nrewebservices-0.2.1/setup.cfg
+-rw-r--r--   0 gberg     (1000) users      (100)     1477 2024-04-10 11:49:15.000000 nrewebservices-0.2.1/setup.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/tests/
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.151008 nrewebservices-0.2.1/tests/data/
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.154341 nrewebservices-0.2.1/tests/data/ldbws/
+-rw-r--r--   0 gberg     (1000) users      (100)     7200 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/basic-fastest-departures-board-with-details.xml
+-rw-r--r--   0 gberg     (1000) users      (100)     3200 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/basic-fastest-departures-board.xml
+-rw-r--r--   0 gberg     (1000) users      (100)     4392 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/basic-service-details.xml
+-rw-r--r--   0 gberg     (1000) users      (100)     7391 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/basic-station-board-departures.xml
+-rw-r--r--   0 gberg     (1000) users      (100)    21940 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/basic-station-board-with-details-departures.xml
+-rw-r--r--   0 gberg     (1000) users      (100)    15988 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/departure-board-with-partial-formation-and-loading.xml
+-rw-r--r--   0 gberg     (1000) users      (100)     6324 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/data/ldbws/service-details-with-partial-formation-and-loading.xml
+-rw-r--r--   0 gberg     (1000) users      (100)     1030 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/helpers.py
+-rw-r--r--   0 gberg     (1000) users      (100)     3000 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_fastest_departures_board_basics.py
+-rw-r--r--   0 gberg     (1000) users      (100)     4125 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_fastest_departures_board_with_details.py
+-rw-r--r--   0 gberg     (1000) users      (100)     3584 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_formations.py
+-rw-r--r--   0 gberg     (1000) users      (100)     3392 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_service_details.py
+-rw-r--r--   0 gberg     (1000) users      (100)    17547 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_session.py
+-rw-r--r--   0 gberg     (1000) users      (100)     6035 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_station_board_basics.py
+-rw-r--r--   0 gberg     (1000) users      (100)     4010 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/test_ldbws_station_board_with_details.py
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.151008 nrewebservices-0.2.1/tests/wsdl/
+drwxr-xr-x   0 gberg     (1000) users      (100)        0 2024-04-10 11:50:20.157675 nrewebservices-0.2.1/tests/wsdl/ldbws/
+-rw-r--r--   0 gberg     (1000) users      (100)      471 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/darwin_token_types_2013-11-28.wsdl
+-rw-r--r--   0 gberg     (1000) users      (100)     1116 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/darwin_token_types_2013-11-28.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)     3709 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2007-10-10_ldb_common_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    21741 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2012-01-13_ldb_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)     1358 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2015-11-27_ldb_common_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    31969 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2015-11-27_ldb_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    25467 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb.wsdl
+-rw-r--r--   0 gberg     (1000) users      (100)      658 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb_common_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    11880 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)     1313 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-02-02_ldb_common_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    25587 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb.wsdl
+-rw-r--r--   0 gberg     (1000) users      (100)     1856 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb_common_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)    25457 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb_types.xsd
+-rw-r--r--   0 gberg     (1000) users      (100)      853 2024-04-10 11:32:39.000000 nrewebservices-0.2.1/tests/wsdl/ldbws/wsdl.aspx
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nrewebservices-0.2.0/CHANGELOG.rst` & `nrewebservices-0.2.1/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ----------
 Change Log
 ----------
 
+v0.2.1
+==========
+
+* Switch from suds-jurko to suds
+* Discontinue support for python < 3.5, and add support for python to 3.12
+
+
 v0.2.0
 ======
 
 * Discontinue support for Python 2.6 and 3.3, and officially add support for Python 3.6 & 3.7.
 * Update to the 2017-10-01 version of the LDBWS schema. This introduces Formations for services.
 
 v0.1.4
```

### Comparing `nrewebservices-0.2.0/LICENSE` & `nrewebservices-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/README.rst` & `nrewebservices-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 .. image:: https://img.shields.io/pypi/l/nrewebservices.svg?maxAge=2592000
     :target: https://github.com/grundleborg/nrewebservices/blob/master/LICENSE
     :alt: License
 
 NREWebServices
 ==============
 
-A Python 2/3 client for the National Rail Enquiries web services.
+A Python 3 client for the National Rail Enquiries web services.
 
 Supported Web Services
 ----------------------
 
 The following NRE web services are currently supported by this library.
 
 * Darwin Live Departure Boards (ldbws).
```

### Comparing `nrewebservices-0.2.0/RELEASING.rst` & `nrewebservices-0.2.1/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/Makefile` & `nrewebservices-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/api-ldbws.rst` & `nrewebservices-0.2.1/docs/api-ldbws.rst`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/conf.py` & `nrewebservices-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/introduction.rst` & `nrewebservices-0.2.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/ldbws.rst` & `nrewebservices-0.2.1/docs/ldbws.rst`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/make.bat` & `nrewebservices-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/docs/staff.rst` & `nrewebservices-0.2.1/docs/staff.rst`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/examples/ldbws.py` & `nrewebservices-0.2.1/examples/ldbws.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/nrewebservices/common/soap.py` & `nrewebservices-0.2.1/nrewebservices/common/soap.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/nrewebservices/ldbws/responses.py` & `nrewebservices-0.2.1/nrewebservices/ldbws/responses.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/nrewebservices/ldbws/webservice.py` & `nrewebservices-0.2.1/nrewebservices/ldbws/webservice.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/nrewebservices.egg-info/SOURCES.txt` & `nrewebservices-0.2.1/nrewebservices.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 tests/test_ldbws_fastest_departures_board_basics.py
 tests/test_ldbws_fastest_departures_board_with_details.py
 tests/test_ldbws_formations.py
 tests/test_ldbws_service_details.py
 tests/test_ldbws_session.py
 tests/test_ldbws_station_board_basics.py
 tests/test_ldbws_station_board_with_details.py
-tests/.cache/v/cache/lastfailed
 tests/data/ldbws/basic-fastest-departures-board-with-details.xml
 tests/data/ldbws/basic-fastest-departures-board.xml
 tests/data/ldbws/basic-service-details.xml
 tests/data/ldbws/basic-station-board-departures.xml
 tests/data/ldbws/basic-station-board-with-details-departures.xml
 tests/data/ldbws/departure-board-with-partial-formation-and-loading.xml
 tests/data/ldbws/service-details-with-partial-formation-and-loading.xml
```

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/basic-fastest-departures-board-with-details.xml` & `nrewebservices-0.2.1/tests/data/ldbws/basic-fastest-departures-board-with-details.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/basic-fastest-departures-board.xml` & `nrewebservices-0.2.1/tests/data/ldbws/basic-fastest-departures-board.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/basic-service-details.xml` & `nrewebservices-0.2.1/tests/data/ldbws/basic-service-details.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/basic-station-board-departures.xml` & `nrewebservices-0.2.1/tests/data/ldbws/basic-station-board-departures.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/basic-station-board-with-details-departures.xml` & `nrewebservices-0.2.1/tests/data/ldbws/basic-station-board-with-details-departures.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/departure-board-with-partial-formation-and-loading.xml` & `nrewebservices-0.2.1/tests/data/ldbws/departure-board-with-partial-formation-and-loading.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/data/ldbws/service-details-with-partial-formation-and-loading.xml` & `nrewebservices-0.2.1/tests/data/ldbws/service-details-with-partial-formation-and-loading.xml`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/helpers.py` & `nrewebservices-0.2.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_fastest_departures_board_basics.py` & `nrewebservices-0.2.1/tests/test_ldbws_fastest_departures_board_basics.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_fastest_departures_board_with_details.py` & `nrewebservices-0.2.1/tests/test_ldbws_fastest_departures_board_with_details.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_formations.py` & `nrewebservices-0.2.1/tests/test_ldbws_formations.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_service_details.py` & `nrewebservices-0.2.1/tests/test_ldbws_service_details.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_session.py` & `nrewebservices-0.2.1/tests/test_ldbws_session.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_station_board_basics.py` & `nrewebservices-0.2.1/tests/test_ldbws_station_board_basics.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/test_ldbws_station_board_with_details.py` & `nrewebservices-0.2.1/tests/test_ldbws_station_board_with_details.py`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/darwin_token_types_2013-11-28.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/darwin_token_types_2013-11-28.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2007-10-10_ldb_common_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2007-10-10_ldb_common_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2012-01-13_ldb_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2012-01-13_ldb_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2015-11-27_ldb_common_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2015-11-27_ldb_common_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2015-11-27_ldb_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2015-11-27_ldb_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb.wsdl` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb.wsdl`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb_common_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb_common_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2016-02-16_ldb_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2016-02-16_ldb_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-02-02_ldb_common_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-02-02_ldb_common_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb.wsdl` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb.wsdl`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb_common_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb_common_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/rtti_2017-10-01_ldb_types.xsd` & `nrewebservices-0.2.1/tests/wsdl/ldbws/rtti_2017-10-01_ldb_types.xsd`

 * *Files identical despite different names*

### Comparing `nrewebservices-0.2.0/tests/wsdl/ldbws/wsdl.aspx` & `nrewebservices-0.2.1/tests/wsdl/ldbws/wsdl.aspx`

 * *Files identical despite different names*

