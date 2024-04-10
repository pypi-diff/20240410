# Comparing `tmp/replit-3.6.1.tar.gz` & `tmp/replit-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-3.6.1.tar", max compression
+gzip compressed data, was "replit-3.6.2.tar", max compression
```

## Comparing `replit-3.6.1.tar` & `replit-3.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      720 2024-02-28 00:07:42.579003 replit-3.6.1/LICENSE
--rw-r--r--   0        0        0     1324 2024-02-28 00:07:42.579003 replit-3.6.1/README.md
--rw-r--r--   0        0        0     1487 2024-02-28 00:07:51.350993 replit-3.6.1/pyproject.toml
--rw-r--r--   0        0        0      798 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/__init__.py
--rw-r--r--   0        0        0     3028 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/__main__.py
--rw-r--r--   0        0        0      171 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/audio/Makefile
--rw-r--r--   0        0        0    13225 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/audio/__init__.py
--rw-r--r--   0        0        0     1848 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/audio/test.py
--rw-r--r--   0        0        0     3687 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/audio/types.py
--rw-r--r--   0        0        0      861 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/database/__init__.py
--rw-r--r--   0        0        0    22908 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/database/database.py
--rw-r--r--   0        0        0     1520 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/database/default_db.py
--rw-r--r--   0        0        0     2641 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/database/server.py
--rw-r--r--   0        0        0       33 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/api/__init__.py
--rw-r--r--   0        0        0     5800 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/api/client_pb2.py
--rw-r--r--   0        0        0        0 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/api/features/__init__.py
--rw-r--r--   0        0        0     1606 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/api/features/features_pb2.py
--rw-r--r--   0        0        0        0 2024-02-28 00:07:42.583003 replit-3.6.1/src/replit/goval/api/repl/__init__.py
--rw-r--r--   0        0        0     4642 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/goval/api/repl/repl_pb2.py
--rw-r--r--   0        0        0     4963 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/goval/api/signing_pb2.py
--rw-r--r--   0        0        0      174 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/identity/__init__.py
--rw-r--r--   0        0        0      159 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/identity/exceptions.py
--rw-r--r--   0        0        0     2110 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/identity/sign.py
--rw-r--r--   0        0        0    13408 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/identity/verify.py
--rw-r--r--   0        0        0     2734 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/info.py
--rw-r--r--   0        0        0      733 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/web/__init__.py
--rw-r--r--   0        0        0     2640 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/web/app.py
--rw-r--r--   0        0        0     3666 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/web/user.py
--rw-r--r--   0        0        0     8607 2024-02-28 00:07:42.587003 replit-3.6.1/src/replit/web/utils.py
--rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 replit-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0      720 2024-04-10 13:42:36.208942 replit-3.6.2/LICENSE
+-rw-r--r--   0        0        0     1491 2024-04-10 13:42:36.208942 replit-3.6.2/README.md
+-rw-r--r--   0        0        0     1487 2024-04-10 13:42:46.180993 replit-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0      798 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/__init__.py
+-rw-r--r--   0        0        0     3028 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/__main__.py
+-rw-r--r--   0        0        0      171 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/Makefile
+-rw-r--r--   0        0        0    13225 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/test.py
+-rw-r--r--   0        0        0     3687 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/audio/types.py
+-rw-r--r--   0        0        0      861 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/__init__.py
+-rw-r--r--   0        0        0    24452 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/database.py
+-rw-r--r--   0        0        0     1520 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/default_db.py
+-rw-r--r--   0        0        0     2641 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/database/server.py
+-rw-r--r--   0        0        0       33 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/__init__.py
+-rw-r--r--   0        0        0     5800 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/client_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/features/__init__.py
+-rw-r--r--   0        0        0     1606 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/features/features_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/repl/__init__.py
+-rw-r--r--   0        0        0     4642 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/repl/repl_pb2.py
+-rw-r--r--   0        0        0     4963 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/goval/api/signing_pb2.py
+-rw-r--r--   0        0        0      174 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/__init__.py
+-rw-r--r--   0        0        0      159 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/exceptions.py
+-rw-r--r--   0        0        0     2110 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/sign.py
+-rw-r--r--   0        0        0    13408 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/identity/verify.py
+-rw-r--r--   0        0        0     2734 2024-04-10 13:42:36.216942 replit-3.6.2/src/replit/info.py
+-rw-r--r--   0        0        0      733 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/app.py
+-rw-r--r--   0        0        0     3666 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/user.py
+-rw-r--r--   0        0        0     8607 2024-04-10 13:42:36.220942 replit-3.6.2/src/replit/web/utils.py
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 replit-3.6.2/PKG-INFO
```

### Comparing `replit-3.6.1/LICENSE` & `replit-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/README.md` & `replit-3.6.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### `>>> import replit`
 
-[![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/)
+[![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/) [![Read the Docs](https://img.shields.io/readthedocs/replit-py/latest?logo=readthedocs&label=ReadTheDocs)](https://replit-py.readthedocs.io/)
 
 This repository is the home for the `replit` Python package, which provides:
 
 - A fully-featured database client for [Replit DB](https://docs.replit.com/category/databases).
-- A Flask–based application framework for accelerating development on the platform.
+- Tools and utilities for Flask Web Development, including an interface to Replit's User Authetication service
 - Replit user profile metadata retrieval (more coming here!).
 - A simple audio library that can play tones and audio files!
 
 ### Open Source License
 
 This library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `replit-3.6.1/pyproject.toml` & `replit-3.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit"
-version = "3.6.1"  # Set by GitHub Actions
+version = "3.6.2"  # Set by GitHub Actions
 description = "A library for interacting with features of Replit"
 authors = ["Replit <contact@replit.com>", "mat <pypi@matdoes.dev>", "kennethreitz <me@kennethreitz.org>", "Scoder12 <pypi@scoder12.ml>", "AllAwesome497", ]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/replit/replit-py"
 homepage = "https://github.com/replit/replit-py"
 documentation = "https://replit-py.readthedocs.org/"
```

### Comparing `replit-3.6.1/src/replit/__init__.py` & `replit-3.6.2/src/replit/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/__main__.py` & `replit-3.6.2/src/replit/__main__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/audio/__init__.py` & `replit-3.6.2/src/replit/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/audio/test.py` & `replit-3.6.2/src/replit/audio/test.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/audio/types.py` & `replit-3.6.2/src/replit/audio/types.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/database/__init__.py` & `replit-3.6.2/src/replit/database/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/database/database.py` & `replit-3.6.2/src/replit/database/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Async and dict-like interfaces for interacting with Replit Database."""
 
+import asyncio
 from collections import abc
 import json
 import threading
 from typing import (
     Any,
     Callable,
     Dict,
@@ -78,16 +79,25 @@
 
     :param str db_url: The Database URL to connect to
     :param int retry_count: How many retry attempts we should make
     :param get_db_url Callable: A callback that returns the current db_url
     :param unbind Callable: Permit additional behavior after Database close
     """
 
-    __slots__ = ("db_url", "sess", "client", "_get_db_url", "_unbind", "_refresh_timer")
+    __slots__ = (
+        "db_url",
+        "sess",
+        "client",
+        "_get_db_url",
+        "_unbind",
+        "_refresh_timer",
+        "_watchdog_timer",
+    )
     _refresh_timer: Optional[threading.Timer]
+    _watchdog_timer: Optional[threading.Timer]
 
     def __init__(
         self,
         db_url: str,
         retry_count: int = 5,
         get_db_url: Optional[Callable[[], Optional[str]]] = None,
         unbind: Optional[Callable[[], None]] = None,
@@ -109,26 +119,37 @@
 
         retry_options = ExponentialRetry(attempts=retry_count)
         self.client = RetryClient(client_session=self.sess, retry_options=retry_options)
 
         if self._get_db_url:
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
+        watched_thread = threading.main_thread()
+        self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
+        self._watchdog_timer.start()
 
     def _refresh_db(self) -> None:
         if self._refresh_timer:
             self._refresh_timer.cancel()
             self._refresh_timer = None
         if self._get_db_url:
             db_url = self._get_db_url()
             if db_url:
                 self.update_db_url(db_url)
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
 
+    def _watchdog(self, watched_thread: threading.Thread) -> None:
+        if not watched_thread.is_alive():
+            return asyncio.run(self.close())
+        if self._watchdog_timer:
+            self._watchdog_timer.cancel()
+        self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
+        self._watchdog_timer.start()
+
     def update_db_url(self, db_url: str) -> None:
         """Update the database url.
 
         Args:
             db_url (str): Database url to use.
         """
         self.db_url = db_url
@@ -288,14 +309,17 @@
 
     async def close(self) -> None:
         """Closes the database client connection."""
         await self.sess.close()
         if self._refresh_timer:
             self._refresh_timer.cancel()
             self._refresh_timer = None
+        if self._watchdog_timer:
+            self._watchdog_timer.cancel()
+            self._watchdog_timer = None
         if self._unbind:
             # Permit signaling to surrounding scopes that we have closed
             self._unbind()
 
     def __repr__(self) -> str:
         """A representation of the database.
 
@@ -481,16 +505,24 @@
 
     :param str db_url: The Database URL to connect to
     :param int retry_count: How many retry attempts we should make
     :param get_db_url Callable: A callback that returns the current db_url
     :param unbind Callable: Permit additional behavior after Database close
     """
 
-    __slots__ = ("db_url", "sess", "_get_db_url", "_unbind", "_refresh_timer")
+    __slots__ = (
+        "db_url",
+        "sess",
+        "_get_db_url",
+        "_unbind",
+        "_refresh_timer",
+        "_watchdog_timer",
+    )
     _refresh_timer: Optional[threading.Timer]
+    _watchdog_timer: Optional[threading.Timer]
 
     def __init__(
         self,
         db_url: str,
         retry_count: int = 5,
         get_db_url: Optional[Callable[[], Optional[str]]] = None,
         unbind: Optional[Callable[[], None]] = None,
@@ -514,26 +546,37 @@
         )
         self.sess.mount("http://", HTTPAdapter(max_retries=retries))
         self.sess.mount("https://", HTTPAdapter(max_retries=retries))
 
         if self._get_db_url:
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
+        watched_thread = threading.main_thread()
+        self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
+        self._watchdog_timer.start()
 
     def _refresh_db(self) -> None:
         if self._refresh_timer:
             self._refresh_timer.cancel()
             self._refresh_timer = None
         if self._get_db_url:
             db_url = self._get_db_url()
             if db_url:
                 self.update_db_url(db_url)
             self._refresh_timer = threading.Timer(3600, self._refresh_db)
             self._refresh_timer.start()
 
+    def _watchdog(self, watched_thread: threading.Thread) -> None:
+        if not watched_thread.is_alive():
+            return self.close()
+        if self._watchdog_timer:
+            self._watchdog_timer.cancel()
+        self._watchdog_timer = threading.Timer(1, self._watchdog, args=[watched_thread])
+        self._watchdog_timer.start()
+
     def update_db_url(self, db_url: str) -> None:
         """Update the database url.
 
         Args:
             db_url (str): Database url to use.
         """
         self.db_url = db_url
@@ -716,10 +759,13 @@
 
     def close(self) -> None:
         """Closes the database client connection."""
         self.sess.close()
         if self._refresh_timer:
             self._refresh_timer.cancel()
             self._refresh_timer = None
+        if self._watchdog_timer:
+            self._watchdog_timer.cancel()
+            self._watchdog_timer = None
         if self._unbind:
             # Permit signaling to surrounding scopes that we have closed
             self._unbind()
```

### Comparing `replit-3.6.1/src/replit/database/default_db.py` & `replit-3.6.2/src/replit/database/default_db.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/database/server.py` & `replit-3.6.2/src/replit/database/server.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/goval/api/client_pb2.py` & `replit-3.6.2/src/replit/goval/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/goval/api/features/features_pb2.py` & `replit-3.6.2/src/replit/goval/api/features/features_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/goval/api/repl/repl_pb2.py` & `replit-3.6.2/src/replit/goval/api/repl/repl_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/goval/api/signing_pb2.py` & `replit-3.6.2/src/replit/goval/api/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/identity/sign.py` & `replit-3.6.2/src/replit/identity/sign.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/identity/verify.py` & `replit-3.6.2/src/replit/identity/verify.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/info.py` & `replit-3.6.2/src/replit/info.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/web/__init__.py` & `replit-3.6.2/src/replit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/web/app.py` & `replit-3.6.2/src/replit/web/app.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/web/user.py` & `replit-3.6.2/src/replit/web/user.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/src/replit/web/utils.py` & `replit-3.6.2/src/replit/web/utils.py`

 * *Files identical despite different names*

### Comparing `replit-3.6.1/PKG-INFO` & `replit-3.6.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit
-Version: 3.6.1
+Version: 3.6.2
 Summary: A library for interacting with features of Replit
 Home-page: https://github.com/replit/replit-py
 License: ISC
 Author: Replit
 Author-email: contact@replit.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
@@ -24,20 +24,20 @@
 Requires-Dist: urllib3 (>=1.26,<3)
 Project-URL: Documentation, https://replit-py.readthedocs.org/
 Project-URL: Repository, https://github.com/replit/replit-py
 Description-Content-Type: text/markdown
 
 ### `>>> import replit`
 
-[![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/)
+[![Run on Repl.it](https://img.shields.io/badge/run-on_Replit-f26208?logo=replit)](https://repl.it/github/replit/replit-py) [![pypi: replit](https://img.shields.io/pypi/v/replit)](https://pypi.org/project/replit/) [![Read the Docs](https://img.shields.io/readthedocs/replit-py/latest?logo=readthedocs&label=ReadTheDocs)](https://replit-py.readthedocs.io/)
 
 This repository is the home for the `replit` Python package, which provides:
 
 - A fully-featured database client for [Replit DB](https://docs.replit.com/category/databases).
-- A Flask–based application framework for accelerating development on the platform.
+- Tools and utilities for Flask Web Development, including an interface to Replit's User Authetication service
 - Replit user profile metadata retrieval (more coming here!).
 - A simple audio library that can play tones and audio files!
 
 ### Open Source License
 
 This library is licensed under the [ISC License](https://en.wikipedia.org/wiki/ISC_license) and is free for you to use, change, or even profit from!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

