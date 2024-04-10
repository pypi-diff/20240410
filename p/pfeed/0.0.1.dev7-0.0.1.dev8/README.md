# Comparing `tmp/pfeed-0.0.1.dev7.tar.gz` & `tmp/pfeed-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfeed-0.0.1.dev7.tar", max compression
+gzip compressed data, was "pfeed-0.0.1.dev8.tar", max compression
```

## Comparing `pfeed-0.0.1.dev7.tar` & `pfeed-0.0.1.dev8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev7/LICENSE
--rw-r--r--   0        0        0    11225 2024-04-02 17:30:09.523671 pfeed-0.0.1.dev7/README.md
--rw-r--r--   0        0        0      326 2024-03-21 17:02:33.426143 pfeed-0.0.1.dev7/pfeed/__init__.py
--rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev7/pfeed/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev7/pfeed/cli/commands/__init__.py
--rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev7/pfeed/cli/commands/config.py
--rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev7/pfeed/cli/commands/docker_compose.py
--rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev7/pfeed/cli/commands/download.py
--rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev7/pfeed/cli/commands/stream.py
--rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev7/pfeed/cli/main.py
--rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev7/pfeed/config/logging.yml
--rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev7/pfeed/config_handler.py
--rw-r--r--   0        0        0      442 2024-04-06 07:27:27.195256 pfeed-0.0.1.dev7/pfeed/const/commons.py
--rw-r--r--   0        0        0      518 2024-04-03 07:02:18.957136 pfeed-0.0.1.dev7/pfeed/const/paths.py
--rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_polars.py
--rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pyspark.py
--rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev7/pfeed/datastore.py
--rw-r--r--   0        0        0     9172 2024-04-06 11:03:28.122162 pfeed-0.0.1.dev7/pfeed/etl.py
--rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev7/pfeed/feeds/__init__.py
--rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev7/pfeed/feeds/base_feed.py
--rw-r--r--   0        0        0     8829 2024-04-06 11:03:28.122347 pfeed-0.0.1.dev7/pfeed/feeds/bybit_feed.py
--rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev7/pfeed/feeds/custom_csv_feed.py
--rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev7/pfeed/feeds/yahoo_finance_feed.py
--rw-r--r--   0        0        0     2206 2024-04-06 11:03:28.122398 pfeed-0.0.1.dev7/pfeed/filepath.py
--rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev7/pfeed/main.py
--rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev7/pfeed/sources/__init__.py
--rw-r--r--   0        0        0      364 2024-04-02 17:44:35.831803 pfeed-0.0.1.dev7/pfeed/sources/bybit/__init__.py
--rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev7/pfeed/sources/bybit/api.py
--rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev7/pfeed/sources/bybit/const.py
--rw-r--r--   0        0        0     7258 2024-03-30 06:58:44.787802 pfeed-0.0.1.dev7/pfeed/sources/bybit/download.py
--rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev7/pfeed/sources/bybit/stream.py
--rw-r--r--   0        0        0      589 2024-04-06 07:32:59.669635 pfeed-0.0.1.dev7/pfeed/types/common_literals.py
--rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev7/pfeed/utils/monitor.py
--rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev7/pfeed/utils/utils.py
--rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev7/pfeed/utils/validate.py
--rw-r--r--   0        0        0     1599 2024-04-09 13:32:33.763658 pfeed-0.0.1.dev7/pyproject.toml
--rw-r--r--   0        0        0    12599 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev8/LICENSE
+-rw-r--r--   0        0        0    11225 2024-04-02 17:30:09.523671 pfeed-0.0.1.dev8/README.md
+-rw-r--r--   0        0        0      326 2024-03-21 17:02:33.426143 pfeed-0.0.1.dev8/pfeed/__init__.py
+-rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev8/pfeed/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev8/pfeed/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev8/pfeed/cli/commands/config.py
+-rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev8/pfeed/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev8/pfeed/cli/commands/download.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev8/pfeed/cli/commands/stream.py
+-rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev8/pfeed/cli/main.py
+-rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev8/pfeed/config/logging.yml
+-rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev8/pfeed/config_handler.py
+-rw-r--r--   0        0        0      442 2024-04-06 07:27:27.195256 pfeed-0.0.1.dev8/pfeed/const/commons.py
+-rw-r--r--   0        0        0      518 2024-04-03 07:02:18.957136 pfeed-0.0.1.dev8/pfeed/const/paths.py
+-rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_polars.py
+-rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pyspark.py
+-rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev8/pfeed/datastore.py
+-rw-r--r--   0        0        0     9172 2024-04-06 11:03:28.122162 pfeed-0.0.1.dev8/pfeed/etl.py
+-rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev8/pfeed/feeds/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev8/pfeed/feeds/base_feed.py
+-rw-r--r--   0        0        0     8829 2024-04-06 11:03:28.122347 pfeed-0.0.1.dev8/pfeed/feeds/bybit_feed.py
+-rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev8/pfeed/feeds/custom_csv_feed.py
+-rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev8/pfeed/feeds/yahoo_finance_feed.py
+-rw-r--r--   0        0        0     2206 2024-04-06 11:03:28.122398 pfeed-0.0.1.dev8/pfeed/filepath.py
+-rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev8/pfeed/main.py
+-rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev8/pfeed/sources/__init__.py
+-rw-r--r--   0        0        0      364 2024-04-02 17:44:35.831803 pfeed-0.0.1.dev8/pfeed/sources/bybit/__init__.py
+-rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev8/pfeed/sources/bybit/api.py
+-rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev8/pfeed/sources/bybit/const.py
+-rw-r--r--   0        0        0     7248 2024-04-09 15:10:28.708592 pfeed-0.0.1.dev8/pfeed/sources/bybit/download.py
+-rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev8/pfeed/sources/bybit/stream.py
+-rw-r--r--   0        0        0      589 2024-04-06 07:32:59.669635 pfeed-0.0.1.dev8/pfeed/types/common_literals.py
+-rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev8/pfeed/utils/monitor.py
+-rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev8/pfeed/utils/utils.py
+-rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev8/pfeed/utils/validate.py
+-rw-r--r--   0        0        0     1304 2024-04-09 15:16:37.676727 pfeed-0.0.1.dev8/pyproject.toml
+-rw-r--r--   0        0        0    12683 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev8/PKG-INFO
```

### Comparing `pfeed-0.0.1.dev7/LICENSE` & `pfeed-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/README.md` & `pfeed-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/cli/commands/config.py` & `pfeed-0.0.1.dev8/pfeed/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/cli/commands/docker_compose.py` & `pfeed-0.0.1.dev8/pfeed/cli/commands/docker_compose.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/cli/commands/download.py` & `pfeed-0.0.1.dev8/pfeed/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/cli/main.py` & `pfeed-0.0.1.dev8/pfeed/cli/main.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/config/logging.yml` & `pfeed-0.0.1.dev8/pfeed/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/config_handler.py` & `pfeed-0.0.1.dev8/pfeed/config_handler.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/const/paths.py` & `pfeed-0.0.1.dev8/pfeed/const/paths.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_pandas.py` & `pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pandas.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/data_tools/data_tool_polars.py` & `pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_polars.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/datastore.py` & `pfeed-0.0.1.dev8/pfeed/datastore.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/etl.py` & `pfeed-0.0.1.dev8/pfeed/etl.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/feeds/base_feed.py` & `pfeed-0.0.1.dev8/pfeed/feeds/base_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/feeds/bybit_feed.py` & `pfeed-0.0.1.dev8/pfeed/feeds/bybit_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/feeds/yahoo_finance_feed.py` & `pfeed-0.0.1.dev8/pfeed/feeds/yahoo_finance_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/filepath.py` & `pfeed-0.0.1.dev8/pfeed/filepath.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/sources/bybit/api.py` & `pfeed-0.0.1.dev8/pfeed/sources/bybit/api.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/sources/bybit/const.py` & `pfeed-0.0.1.dev8/pfeed/sources/bybit/const.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/sources/bybit/download.py` & `pfeed-0.0.1.dev8/pfeed/sources/bybit/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Downloads Bybit historical data"""
-import os
 import logging
 import datetime
 from collections import defaultdict
 from logging.handlers import QueueHandler, QueueListener
 
 from tqdm import tqdm
 from rich.console import Console
```

### Comparing `pfeed-0.0.1.dev7/pfeed/types/common_literals.py` & `pfeed-0.0.1.dev8/pfeed/types/common_literals.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/utils/utils.py` & `pfeed-0.0.1.dev8/pfeed/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/pfeed/utils/validate.py` & `pfeed-0.0.1.dev8/pfeed/utils/validate.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev7/PKG-INFO` & `pfeed-0.0.1.dev8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: pfeed
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Data pipeline for algo-trading, getting and storing both real-time and historical data made easy.
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: trading,algo-trading,data pipeline,ETL,data lake,data warehouse,data integration,historical data,live data,data streaming
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfeed@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: boost
+Provides-Extra: df
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: connectorx (>=0.3.2,<0.4.0) ; extra == "boost"
 Requires-Dist: minio (>=7.2.5,<8.0.0)
-Requires-Dist: pfund (>=0.0.1.dev7,<0.0.2)
-Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "df"
+Requires-Dist: pfund (>=0.0.1.dev8,<0.0.2)
+Requires-Dist: polars (>=0.20.16,<0.21.0) ; extra == "df"
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "boost"
+Requires-Dist: ray (>=2.10.0,<3.0.0) ; extra == "boost"
 Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: yfinance (>=0.2.37,<0.3.0)
 Project-URL: Documentation, https://pfeed-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfeed
 Description-Content-Type: text/markdown
```

