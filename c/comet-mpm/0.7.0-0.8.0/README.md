# Comparing `tmp/comet_mpm-0.7.0.tar.gz` & `tmp/comet_mpm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_mpm-0.7.0.tar", last modified: Wed Feb 28 22:17:51 2024, max compression
+gzip compressed data, was "comet_mpm-0.8.0.tar", last modified: Wed Apr 10 15:10:16 2024, max compression
```

## Comparing `comet_mpm-0.7.0.tar` & `comet_mpm-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.074576 comet_mpm-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 22:17:51.074576 comet_mpm-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.066576 comet_mpm-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm/_json/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/_json/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/aws_lambda/lambda_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12776 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/comet_mpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm/events/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/events/base_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/events/events_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/events/label_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/events/prediction_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/logging_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/optional_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm/sender/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/sender/asyncio_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/sender/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/sender/thread_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-28 22:17:40.000000 comet_mpm-0.7.0/src/comet_mpm/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 22:17:51.070576 comet_mpm-0.7.0/src/comet_mpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-28 22:17:51.000000 comet_mpm-0.7.0/src/comet_mpm.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:10:16.177246 comet_mpm-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.165246 comet_mpm-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_json/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/base64_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/api_key/comet_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/aws_lambda/lambda_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/comet_mpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/connection_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/events_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/label_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/events/prediction_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/logging_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/optional_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/asyncio_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/sender/thread_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 15:10:09.000000 comet_mpm-0.8.0/src/comet_mpm/settings_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:10:16.173246 comet_mpm-0.8.0/src/comet_mpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 15:10:16.000000 comet_mpm-0.8.0/src/comet_mpm.egg-info/SOURCES.txt
```

### Comparing `comet_mpm-0.7.0/MANIFEST.in` & `comet_mpm-0.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/PKG-INFO` & `comet_mpm-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_mpm
-Version: 0.7.0
+Version: 0.8.0
 Summary: Comet MPM SDK
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_mpm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_mpm-0.7.0/setup.py` & `comet_mpm-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_mpm",
     name="comet_mpm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.7.0",
+    version="0.8.0",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm/__init__.py` & `comet_mpm-0.8.0/src/comet_mpm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 __author__ = """Comet ML Inc."""
 __email__ = "mail@comet.ml"
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 __all__ = ["CometMPM"]
 
 from ._logging import _setup_comet_mpm_logging
 from .comet_mpm import CometMPM
 
 _setup_comet_mpm_logging()
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm/_json/__init__.py` & `comet_mpm-0.8.0/src/comet_mpm/_json/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/_json/numpy_encoder.py` & `comet_mpm-0.8.0/src/comet_mpm/_json/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/_logging.py` & `comet_mpm-0.8.0/src/comet_mpm/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/aws_lambda/__init__.py` & `comet_mpm-0.8.0/src/comet_mpm/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/aws_lambda/lambda_helpers.py` & `comet_mpm-0.8.0/src/comet_mpm/aws_lambda/lambda_helpers.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/batch_utils.py` & `comet_mpm-0.8.0/src/comet_mpm/batch_utils.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/cli.py` & `comet_mpm-0.8.0/src/comet_mpm/cli.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/comet_mpm.py` & `comet_mpm-0.8.0/src/comet_mpm/comet_mpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 import asyncio as asyncio_module
 import atexit
 import logging
 import os
 from typing import Any, Awaitable, Dict, Iterable, List, Optional, Union
 
 from . import constants, logging_messages, optional_update
-from .connection import MPM_BASE_PATH, REST_API_BASE_PATH, sanitize_url, url_join
+from .connection import MPM_BASE_PATH, REST_API_BASE_PATH
+from .connection_helpers import sanitize_url, url_join
 from .environment import check_environment
 from .events import events_from_dataframe
 from .events.label_event import LabelEvent
 from .events.prediction_event import PredictionEvent
 from .logging_messages import MPM_JOIN_DEPRECATED_WARNING
 from .sender import get_sender
 from .settings import MPMSettings, get_model
+from .settings_helper import extract_comet_url
 
 LOGGER = logging.getLogger(__name__)
 
 LogEventsResult = Union[List[Any], Awaitable[List[Any]]]
 
 
 class CometMPM:
@@ -81,16 +83,18 @@
         )
         if disabled:
             self.disabled = disabled  # type: bool
         else:
             self.disabled = bool(os.getenv("COMET_MPM_DISABLED"))
         self._asyncio = asyncio
 
-        self._mpm_url = url_join(sanitize_url(self._settings.url), MPM_BASE_PATH)
-        self._api_url = url_join(sanitize_url(self._settings.url), REST_API_BASE_PATH)
+        comet_url = sanitize_url(extract_comet_url(self._settings))
+
+        self._mpm_url = url_join(comet_url, MPM_BASE_PATH)
+        self._api_url = url_join(comet_url, REST_API_BASE_PATH)
 
         if self.disabled:
             self._sender = None
         else:
             self._sender = get_sender(
                 api_key=self._settings.api_key,
                 server_address=self._mpm_url,
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm/connection.py` & `comet_mpm-0.8.0/src/comet_mpm/connection.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import logging
 from typing import Any, Optional
-from urllib.parse import urljoin, urlparse, urlunparse
 
 import aiohttp
 from requests import Session
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .logging_messages import BATCH_SENDING_ERROR
@@ -83,39 +82,7 @@
         headers = {"Authorization": api_key}
         response = await session.post(
             url_endpoint, headers=headers, json=batch, timeout=batch_sending_timeout
         )
         response.raise_for_status()
     except Exception:
         LOGGER.error(BATCH_SENDING_ERROR, exc_info=True)
-
-
-def sanitize_url(url: str) -> str:
-    """Sanitize an URL, checking that it is a valid URL and ensure it contains an ending slash /"""
-    parts = urlparse(url)
-    scheme, netloc, path, params, query, fragment = parts
-
-    # TODO: Raise an exception if params, query and fragment are not empty?
-
-    # Ensure the leading slash
-    if path and not path.endswith("/"):
-        path = path + "/"
-    elif not path and not netloc.endswith("/"):
-        netloc = netloc + "/"
-
-    return urlunparse((scheme, netloc, path, params, query, fragment))
-
-
-def url_join(base: str, *parts: str) -> str:
-    """Given a base and url parts (for example [workspace, project, id]) returns a full URL"""
-    # TODO: Enforce base to have a scheme and netloc?
-    result = base
-
-    for part in parts[:-1]:
-        if not part.endswith("/"):
-            raise ValueError("Intermediary part not ending with /")
-
-        result = urljoin(result, part)
-
-    result = urljoin(result, parts[-1])
-
-    return result
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm/constants.py` & `comet_mpm-0.8.0/src/comet_mpm/constants.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/data_series.py` & `comet_mpm-0.8.0/src/comet_mpm/data_series.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/environment.py` & `comet_mpm-0.8.0/src/comet_mpm/environment.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/events/__init__.py` & `comet_mpm-0.8.0/src/comet_mpm/events/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/events/base_event.py` & `comet_mpm-0.8.0/src/comet_mpm/events/base_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/events/events_from_dataframe.py` & `comet_mpm-0.8.0/src/comet_mpm/events/events_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/events/label_event.py` & `comet_mpm-0.8.0/src/comet_mpm/events/label_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/events/prediction_event.py` & `comet_mpm-0.8.0/src/comet_mpm/events/prediction_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/exceptions.py` & `comet_mpm-0.8.0/src/comet_mpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/logging_messages.py` & `comet_mpm-0.8.0/src/comet_mpm/logging_messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,17 @@
 DEPRECATED_DATAFRAME_OUTPUT_VALUE_AND_PROBABILITY = "You are using the deprecated fields `output_value_column` and `output_probability_column`,you should specify `output_features_columns with value and probability columns`"
 
 MPM_ALREADY_CLOSED_LOG_DATA_WARNING = "This MPM instance has already been closed. Create a new instance to log additional data."
 
 MPM_IN_AWS_LAMBDA_NEEDS_END = "As you are running in a Lambda function, you will need to call 'mpm.end()' when finished to ensure all data is logged before exiting."
 
 MPM_JOIN_DEPRECATED_WARNING = "MPM.join is deprecated, use MPM.end instead."
+
+PARSE_API_KEY_EMPTY_KEY = "Can not parse empty Comet API key"
+
+PARSE_API_KEY_EMPTY_EXPECTED_ATTRIBUTES = (
+    "Expected attributes not found in the Comet API key: %r"
+)
+
+PARSE_API_KEY_TOO_MANY_PARTS = "Too many parts (%d) found in the Comet API key: %r"
+
+BASE_URL_MISMATCH_CONFIG_API_KEY = "Comet URL conflict detected between config (%r) and API Key (%r). MPM SDK will use config URL. Resolve by either removing config URL or set it to the same value."
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm/optional_update.py` & `comet_mpm-0.8.0/src/comet_mpm/optional_update.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/sender/__init__.py` & `comet_mpm-0.8.0/src/comet_mpm/sender/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/sender/asyncio_sender.py` & `comet_mpm-0.8.0/src/comet_mpm/sender/asyncio_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/sender/base.py` & `comet_mpm-0.8.0/src/comet_mpm/sender/base.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/sender/thread_sender.py` & `comet_mpm-0.8.0/src/comet_mpm/sender/thread_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.7.0/src/comet_mpm/settings.py` & `comet_mpm-0.8.0/src/comet_mpm/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     class Config:
         env_prefix = "comet_"
 
 
 class MPMSettings(BaseSettings):
     # Use same names as the Python SDK to ease configuration
     api_key: str
-    url: AnyHttpUrl = "https://www.comet.com/"
+    url: Optional[AnyHttpUrl]
 
     mpm_workspace_name: str
     mpm_model_name: str
     mpm_model_version: str
 
     mpm_max_batch_size: PositiveInt = 1000
     mpm_max_batch_time: PositiveInt = 60
```

### Comparing `comet_mpm-0.7.0/src/comet_mpm.egg-info/SOURCES.txt` & `comet_mpm-0.8.0/src/comet_mpm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 setup.py
 src/comet_mpm/__init__.py
 src/comet_mpm/_logging.py
 src/comet_mpm/batch_utils.py
 src/comet_mpm/cli.py
 src/comet_mpm/comet_mpm.py
 src/comet_mpm/connection.py
+src/comet_mpm/connection_helpers.py
 src/comet_mpm/constants.py
 src/comet_mpm/data_series.py
 src/comet_mpm/environment.py
 src/comet_mpm/exceptions.py
 src/comet_mpm/logging_messages.py
 src/comet_mpm/optional_update.py
 src/comet_mpm/settings.py
+src/comet_mpm/settings_helper.py
 src/comet_mpm/_json/__init__.py
 src/comet_mpm/_json/numpy_encoder.py
+src/comet_mpm/api_key/__init__.py
+src/comet_mpm/api_key/base64_helper.py
+src/comet_mpm/api_key/comet_api_key.py
 src/comet_mpm/aws_lambda/__init__.py
 src/comet_mpm/aws_lambda/lambda_helpers.py
 src/comet_mpm/events/__init__.py
 src/comet_mpm/events/base_event.py
 src/comet_mpm/events/events_from_dataframe.py
 src/comet_mpm/events/label_event.py
 src/comet_mpm/events/prediction_event.py
```

