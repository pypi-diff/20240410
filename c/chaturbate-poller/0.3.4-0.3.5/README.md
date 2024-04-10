# Comparing `tmp/chaturbate_poller-0.3.4.tar.gz` & `tmp/chaturbate_poller-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.4.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.5.tar", max compression
```

## Comparing `chaturbate_poller-0.3.4.tar` & `chaturbate_poller-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/README.md
--rw-r--r--   0        0        0     3129 2024-04-09 14:52:17.098888 chaturbate_poller-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      538 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     3838 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      669 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     2211 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     5578 2024-04-09 14:52:07.010776 chaturbate_poller-0.3.4/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-10 15:45:51.505478 chaturbate_poller-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-10 15:45:51.505478 chaturbate_poller-0.3.5/README.md
+-rw-r--r--   0        0        0     3129 2024-04-10 15:46:02.509504 chaturbate_poller-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     3889 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      669 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     4017 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/format_messages.py
+-rw-r--r--   0        0        0     2211 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     5578 2024-04-10 15:45:51.509478 chaturbate_poller-0.3.5/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.5/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.4/LICENSE` & `chaturbate_poller-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.4/README.md` & `chaturbate_poller-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.4/pyproject.toml` & `chaturbate_poller-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.4"
+version = "0.3.5"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.4/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.5/src/chaturbate_poller/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """chaturbate_poller package."""
 
 # Read version from installed package
 from importlib.metadata import version
 
-from .chaturbate_poller import ChaturbateClient
+from chaturbate_poller.chaturbate_poller import ChaturbateClient
 
 __version__ = version("chaturbate_poller")
 __author__ = "MountainGod2"
 __author_email__ = "admin@reid.ca"
 __maintainer__ = "MountainGod2"
 __maintainer_email__ = "admin@reid.ca"
 __license__ = "MIT"
 __url__ = "https://github.com/MountainGod2/chaturbate_poller"
 __description__ = "A Chaturbate event poller."
 
 
-__all__ = ["ChaturbateClient"]
+__all__ = ["ChaturbateClient", "format_message"]
 """List[str]: The package exports."""
```

### Comparing `chaturbate_poller-0.3.4/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.5/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from logging.config import dictConfig
 from types import TracebackType
 
 import backoff
 import httpx
 from httpx import HTTPStatusError, RequestError
 
-from .constants import BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
-from .logging_config import LOGGING_CONFIG
-from .models import EventsAPIResponse
+from chaturbate_poller.constants import BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
+from chaturbate_poller.logging_config import LOGGING_CONFIG
+from chaturbate_poller.models import EventsAPIResponse
 
 dictConfig(LOGGING_CONFIG)
 """Use the logging configuration from LOGGING_CONFIG."""
 
 logger = logging.getLogger(__name__)
 """Logger for the module."""
```

### Comparing `chaturbate_poller-0.3.4/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.5/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.4/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.5/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.4/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.5/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.4/PKG-INFO` & `chaturbate_poller-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.4
+Version: 0.3.5
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

