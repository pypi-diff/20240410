# Comparing `tmp/pfeed-0.0.1.dev8.tar.gz` & `tmp/pfeed-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfeed-0.0.1.dev8.tar", max compression
+gzip compressed data, was "pfeed-0.0.1.dev9.tar", max compression
```

## Comparing `pfeed-0.0.1.dev8.tar` & `pfeed-0.0.1.dev9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev8/LICENSE
--rw-r--r--   0        0        0    11225 2024-04-02 17:30:09.523671 pfeed-0.0.1.dev8/README.md
--rw-r--r--   0        0        0      326 2024-03-21 17:02:33.426143 pfeed-0.0.1.dev8/pfeed/__init__.py
--rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev8/pfeed/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev8/pfeed/cli/commands/__init__.py
--rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev8/pfeed/cli/commands/config.py
--rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev8/pfeed/cli/commands/docker_compose.py
--rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev8/pfeed/cli/commands/download.py
--rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev8/pfeed/cli/commands/stream.py
--rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev8/pfeed/cli/main.py
--rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev8/pfeed/config/logging.yml
--rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev8/pfeed/config_handler.py
--rw-r--r--   0        0        0      442 2024-04-06 07:27:27.195256 pfeed-0.0.1.dev8/pfeed/const/commons.py
--rw-r--r--   0        0        0      518 2024-04-03 07:02:18.957136 pfeed-0.0.1.dev8/pfeed/const/paths.py
--rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_polars.py
--rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pyspark.py
--rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev8/pfeed/datastore.py
--rw-r--r--   0        0        0     9172 2024-04-06 11:03:28.122162 pfeed-0.0.1.dev8/pfeed/etl.py
--rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev8/pfeed/feeds/__init__.py
--rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev8/pfeed/feeds/base_feed.py
--rw-r--r--   0        0        0     8829 2024-04-06 11:03:28.122347 pfeed-0.0.1.dev8/pfeed/feeds/bybit_feed.py
--rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev8/pfeed/feeds/custom_csv_feed.py
--rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev8/pfeed/feeds/yahoo_finance_feed.py
--rw-r--r--   0        0        0     2206 2024-04-06 11:03:28.122398 pfeed-0.0.1.dev8/pfeed/filepath.py
--rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev8/pfeed/main.py
--rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev8/pfeed/sources/__init__.py
--rw-r--r--   0        0        0      364 2024-04-02 17:44:35.831803 pfeed-0.0.1.dev8/pfeed/sources/bybit/__init__.py
--rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev8/pfeed/sources/bybit/api.py
--rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev8/pfeed/sources/bybit/const.py
--rw-r--r--   0        0        0     7248 2024-04-09 15:10:28.708592 pfeed-0.0.1.dev8/pfeed/sources/bybit/download.py
--rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev8/pfeed/sources/bybit/stream.py
--rw-r--r--   0        0        0      589 2024-04-06 07:32:59.669635 pfeed-0.0.1.dev8/pfeed/types/common_literals.py
--rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev8/pfeed/utils/monitor.py
--rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev8/pfeed/utils/utils.py
--rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev8/pfeed/utils/validate.py
--rw-r--r--   0        0        0     1304 2024-04-09 15:16:37.676727 pfeed-0.0.1.dev8/pyproject.toml
--rw-r--r--   0        0        0    12683 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev8/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev9/LICENSE
+-rw-r--r--   0        0        0    11584 2024-04-10 03:51:08.875849 pfeed-0.0.1.dev9/README.md
+-rw-r--r--   0        0        0      326 2024-04-10 06:51:55.747452 pfeed-0.0.1.dev9/pfeed/__init__.py
+-rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev9/pfeed/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev9/pfeed/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev9/pfeed/cli/commands/config.py
+-rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev9/pfeed/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev9/pfeed/cli/commands/download.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev9/pfeed/cli/commands/stream.py
+-rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev9/pfeed/cli/main.py
+-rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev9/pfeed/config/logging.yml
+-rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev9/pfeed/config_handler.py
+-rw-r--r--   0        0        0      442 2024-04-06 07:27:27.195256 pfeed-0.0.1.dev9/pfeed/const/commons.py
+-rw-r--r--   0        0        0      518 2024-04-03 07:02:18.957136 pfeed-0.0.1.dev9/pfeed/const/paths.py
+-rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev9/pfeed/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev9/pfeed/data_tools/data_tool_polars.py
+-rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev9/pfeed/data_tools/data_tool_pyspark.py
+-rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev9/pfeed/datastore.py
+-rw-r--r--   0        0        0     9490 2024-04-10 07:11:39.495105 pfeed-0.0.1.dev9/pfeed/etl.py
+-rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev9/pfeed/feeds/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev9/pfeed/feeds/base_feed.py
+-rw-r--r--   0        0        0     8829 2024-04-06 11:03:28.122347 pfeed-0.0.1.dev9/pfeed/feeds/bybit_feed.py
+-rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev9/pfeed/feeds/custom_csv_feed.py
+-rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev9/pfeed/feeds/yahoo_finance_feed.py
+-rw-r--r--   0        0        0     2206 2024-04-06 11:03:28.122398 pfeed-0.0.1.dev9/pfeed/filepath.py
+-rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev9/pfeed/main.py
+-rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev9/pfeed/sources/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-10 06:44:48.250380 pfeed-0.0.1.dev9/pfeed/sources/bybit/__init__.py
+-rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev9/pfeed/sources/bybit/api.py
+-rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev9/pfeed/sources/bybit/const.py
+-rw-r--r--   0        0        0     7248 2024-04-09 15:10:28.708592 pfeed-0.0.1.dev9/pfeed/sources/bybit/download.py
+-rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev9/pfeed/sources/bybit/stream.py
+-rw-r--r--   0        0        0      589 2024-04-06 07:32:59.669635 pfeed-0.0.1.dev9/pfeed/types/common_literals.py
+-rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev9/pfeed/utils/monitor.py
+-rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev9/pfeed/utils/utils.py
+-rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev9/pfeed/utils/validate.py
+-rw-r--r--   0        0        0     1437 2024-04-10 07:15:40.470485 pfeed-0.0.1.dev9/pyproject.toml
+-rw-r--r--   0        0        0    13118 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev9/PKG-INFO
```

### Comparing `pfeed-0.0.1.dev8/LICENSE` & `pfeed-0.0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/README.md` & `pfeed-0.0.1.dev9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,22 +64,36 @@
 - [ ] Integrates with [Prefect](https://www.prefect.io) to control data flows
 - [ ] Listens to PFund's trade engine and adds trade history to a local database [Timescaledb](https://www.timescale.com/) (optional)
 
 
 ## Installation
 ### Using [Poetry](https://python-poetry.org) (Recommended)
 ```bash
+# [RECOMMENDED]: dataframes (e.g. polars, pandas) + data storage (e.g. MinIO) + boosted performance
+poetry add "pfeed[df,data,boost]"
+
+# only for downloading data, e.g. Bybit and Yahoo Finance
 poetry add pfeed
+
+# update to the latest version:
+poetry update pfeed
 ```
 
 ### Using Pip
 ```bash
 pip install pfeed
+
+# install the latest version:
+pip install -U pfeed
 ```
 
+### Checking your installation
+```bash
+$ pfeed --version
+```
 
 ## Quick Start
 ### Main Usage: Data Feed
 1. Download bybit raw data on the fly if not stored locally
 
     ```python
     import pfeed as pe
```

### Comparing `pfeed-0.0.1.dev8/pfeed/cli/commands/config.py` & `pfeed-0.0.1.dev9/pfeed/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/cli/commands/docker_compose.py` & `pfeed-0.0.1.dev9/pfeed/cli/commands/docker_compose.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/cli/commands/download.py` & `pfeed-0.0.1.dev9/pfeed/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/cli/main.py` & `pfeed-0.0.1.dev9/pfeed/cli/main.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/config/logging.yml` & `pfeed-0.0.1.dev9/pfeed/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/config_handler.py` & `pfeed-0.0.1.dev9/pfeed/config_handler.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/const/paths.py` & `pfeed-0.0.1.dev9/pfeed/const/paths.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_pandas.py` & `pfeed-0.0.1.dev9/pfeed/data_tools/data_tool_pandas.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/data_tools/data_tool_polars.py` & `pfeed-0.0.1.dev9/pfeed/data_tools/data_tool_polars.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/datastore.py` & `pfeed-0.0.1.dev9/pfeed/datastore.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/etl.py` & `pfeed-0.0.1.dev9/pfeed/etl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 '''ETL = Extract, Transform, Load data'''
 import io
 import logging
 import importlib
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from pfeed.types.common_literals import tSUPPORTED_DATA_TOOLS, tSUPPORTED_DOWNLOAD_DATA_SOURCES, tSUPPORTED_DATA_SINKS, tSUPPORTED_DATA_TYPES, tSUPPORTED_DATA_MODES
+
 import pandas as pd
-from minio.error import MinioException
 
-from pfeed.datastore import Datastore
+try:
+    from pfeed.datastore import Datastore, MinioException
+except ImportError:
+    pass
 from pfeed.filepath import FilePath
 from pfeed.config_handler import ConfigHandler
 from pfeed.const.commons import SUPPORTED_DATA_TYPES, SUPPORTED_DATA_SINKS, SUPPORTED_DOWNLOAD_DATA_SOURCES, SUPPORTED_DATA_MODES
-from pfeed.types.common_literals import tSUPPORTED_DATA_TOOLS, tSUPPORTED_DOWNLOAD_DATA_SOURCES, tSUPPORTED_DATA_SINKS, tSUPPORTED_DATA_TYPES, tSUPPORTED_DATA_MODES
-from pfeed.utils.monitor import print_disk_usage
 from pfund.datas.resolution import Resolution
+try:
+    from pfeed.utils.monitor import print_disk_usage
+except ImportError:
+    print_disk_usage = None
 
 
 logger = logging.getLogger('pfeed')
 
 
 def _convert_raw_dtype_to_explicit(data_source: str, dtype: str):
     """Covnerts implicit dtype 'raw' to explicit one by using the first element in SUPPORTED_RAW_DATA_TYPES, e.g. 'raw_tick'."""
@@ -43,15 +51,15 @@
         dtype (Literal['raw_tick', 'raw', 'tick', 'second', 'minute', 'hour', 'daily']): The type of data to extract.
         pdt (str): product, e.g. BTC_USDT_PERP.
         date (str): The date of the data to extract.
         mode (Literal['historical', 'streaming'], optional): The mode of extraction. Defaults to 'historical'.
 
     Returns:
         bytes | None: The extracted data as bytes, or None if the data is not found.
-    """
+    """    
     for data_sink in SUPPORTED_DATA_SINKS:
         try:
             data: bytes = extract_data(data_sink, data_source, dtype, pdt, date, mode=mode)
         except MinioException:
             data = None
         if data:
             return data
@@ -169,15 +177,16 @@
     elif data_sink == 'minio':
         datastore = Datastore()
         object_name = fp.storage_path
         datastore.put_object(object_name, data, **kwargs)
         logger.info(f'loaded {data_source} data to MinIO object {object_name} {kwargs=}')
     else:
         raise NotImplementedError(f'{data_sink=}')
-    print_disk_usage(config.data_path)
+    if print_disk_usage:
+        print_disk_usage(config.data_path)
         
 
 def clean_raw_data(data_source: tSUPPORTED_DOWNLOAD_DATA_SOURCES, raw_data: bytes) -> bytes:
     module = importlib.import_module(f'pfeed.sources.{data_source.lower()}.const')
     RENAMING_COLS = getattr(module, 'RENAMING_COLS')
     MAPPING_COLS = getattr(module, 'MAPPING_COLS')
     df = pd.read_csv(io.BytesIO(raw_data), compression='gzip')
@@ -205,9 +214,13 @@
     df = pd.read_parquet(io.BytesIO(raw_tick))
     df = df.loc[:, ['ts', 'side', 'volume', 'price']]
     tick_data: bytes = df.to_parquet(compression='snappy')
     return tick_data
 
 
 def resample_data(data: bytes, resolution: str | Resolution, data_tool: tSUPPORTED_DATA_TOOLS='polars', check_if_drop_last_bar=False) -> bytes:
-    data_tool = importlib.import_module(f'pfeed.data_tools.data_tool_{data_tool.lower()}')
+    try:
+        data_tool = importlib.import_module(f'pfeed.data_tools.data_tool_{data_tool.lower()}')
+    except ImportError:
+        # fallback data_tool to pandas
+        data_tool = importlib.import_module('pfeed.data_tools.data_tool_pandas')
     return data_tool.resample_data(data, resolution, check_if_drop_last_bar=check_if_drop_last_bar)
```

### Comparing `pfeed-0.0.1.dev8/pfeed/feeds/base_feed.py` & `pfeed-0.0.1.dev9/pfeed/feeds/base_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/feeds/bybit_feed.py` & `pfeed-0.0.1.dev9/pfeed/feeds/bybit_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/feeds/yahoo_finance_feed.py` & `pfeed-0.0.1.dev9/pfeed/feeds/yahoo_finance_feed.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/filepath.py` & `pfeed-0.0.1.dev9/pfeed/filepath.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/sources/bybit/api.py` & `pfeed-0.0.1.dev9/pfeed/sources/bybit/api.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/sources/bybit/const.py` & `pfeed-0.0.1.dev9/pfeed/sources/bybit/const.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/sources/bybit/download.py` & `pfeed-0.0.1.dev9/pfeed/sources/bybit/download.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/types/common_literals.py` & `pfeed-0.0.1.dev9/pfeed/types/common_literals.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/utils/utils.py` & `pfeed-0.0.1.dev9/pfeed/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pfeed/utils/validate.py` & `pfeed-0.0.1.dev9/pfeed/utils/validate.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev8/pyproject.toml` & `pfeed-0.0.1.dev9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "pfeed"
-version = "0.0.1.dev8"
+version = "0.0.1.dev9"
 description = "Data pipeline for algo-trading, getting and storing both real-time and historical data made easy."
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfeed@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfeed"
 documentation = "https://pfeed-docs.pfund.ai"
 keywords = ["trading", "algo-trading", "data pipeline", "ETL", "data lake", "data warehouse", "data integration", "historical data", "live data", "data streaming"]
 
 [tool.poetry.dependencies]
 python = ">=3.10 <3.13"
-pfund = "^0.0.1.dev8"
+pfund = "^0.0.1.dev9"
 beautifulsoup4 = "^4.12.3"
-tqdm = "^4.66.2"
-s3fs = "^2024.3.1"
-minio = "^7.2.5"
 yfinance = "^0.2.37"
-pandas = { version = "^2.2.0", optional = true}
-polars = { version = "^0.20.16", optional = true}
-connectorx = { version = "^0.3.2", optional = true}
+psutil = { version = "^5.9.8", optional = true }
+s3fs = { version = "^2024.3.1", optional = true }
+minio = { version = "^7.2.5", optional = true }
+pandas = { version = "^2.2.0", optional = true }
+polars = { version = "^0.20.16", optional = true }
+connectorx = { version = "^0.3.2", optional = true }
 pyarrow = { version = "^15.0.0", optional = true }
-ray = { version = "^2.10.0", optional = true}
+ray = { version = "^2.10.0", optional = true }
 
 [tool.poetry.extras]
 df = ["pandas", "polars"]
+data = ["psutil", "minio", "s3fs"]
 boost = ["pyarrow", "connectorx", "ray"]
 
 [tool.poetry.scripts]
 pfeed = "pfeed.main:run_cli"
 
 [tool.poetry.group.dev.dependencies]
 pfund = {path = "../pfund", develop = true}
```

### Comparing `pfeed-0.0.1.dev8/PKG-INFO` & `pfeed-0.0.1.dev9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pfeed
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
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
 Provides-Extra: boost
+Provides-Extra: data
 Provides-Extra: df
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: connectorx (>=0.3.2,<0.4.0) ; extra == "boost"
-Requires-Dist: minio (>=7.2.5,<8.0.0)
+Requires-Dist: minio (>=7.2.5,<8.0.0) ; extra == "data"
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "df"
-Requires-Dist: pfund (>=0.0.1.dev8,<0.0.2)
+Requires-Dist: pfund (>=0.0.1.dev9,<0.0.2)
 Requires-Dist: polars (>=0.20.16,<0.21.0) ; extra == "df"
+Requires-Dist: psutil (>=5.9.8,<6.0.0) ; extra == "data"
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0) ; extra == "boost"
 Requires-Dist: ray (>=2.10.0,<3.0.0) ; extra == "boost"
-Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: s3fs (>=2024.3.1,<2025.0.0) ; extra == "data"
 Requires-Dist: yfinance (>=0.2.37,<0.3.0)
 Project-URL: Documentation, https://pfeed-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfeed
 Description-Content-Type: text/markdown
 
 # PFeed: Data Pipeline for Algo-Trading, Getting and Storing Real-Time and Historical Data Made Easy.
 
@@ -96,22 +97,36 @@
 - [ ] Integrates with [Prefect](https://www.prefect.io) to control data flows
 - [ ] Listens to PFund's trade engine and adds trade history to a local database [Timescaledb](https://www.timescale.com/) (optional)
 
 
 ## Installation
 ### Using [Poetry](https://python-poetry.org) (Recommended)
 ```bash
+# [RECOMMENDED]: dataframes (e.g. polars, pandas) + data storage (e.g. MinIO) + boosted performance
+poetry add "pfeed[df,data,boost]"
+
+# only for downloading data, e.g. Bybit and Yahoo Finance
 poetry add pfeed
+
+# update to the latest version:
+poetry update pfeed
 ```
 
 ### Using Pip
 ```bash
 pip install pfeed
+
+# install the latest version:
+pip install -U pfeed
 ```
 
+### Checking your installation
+```bash
+$ pfeed --version
+```
 
 ## Quick Start
 ### Main Usage: Data Feed
 1. Download bybit raw data on the fly if not stored locally
 
     ```python
     import pfeed as pe
```

