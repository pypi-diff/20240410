# Comparing `tmp/csvbase-client-0.0.1.tar.gz` & `tmp/csvbase-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvbase-client-0.0.1.tar", last modified: Wed Aug 30 20:20:18 2023, max compression
+gzip compressed data, was "csvbase-client-0.1.0.tar", last modified: Tue Apr  9 11:17:53 2024, max compression
```

## Comparing `csvbase-client-0.0.1.tar` & `csvbase-client-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2023-08-30 20:20:18.511463 csvbase-client-0.0.1/
--rw-r--r--   0 cal       (1000) cal       (1000)    34523 2017-09-30 07:16:25.000000 csvbase-client-0.0.1/COPYING
--rw-r--r--   0 cal       (1000) cal       (1000)       40 2023-04-05 16:09:56.000000 csvbase-client-0.0.1/MANIFEST.in
--rw-r--r--   0 cal       (1000) cal       (1000)     2234 2023-08-30 20:20:18.507463 csvbase-client-0.0.1/PKG-INFO
--rw-r--r--   0 cal       (1000) cal       (1000)     1210 2023-08-30 11:40:03.000000 csvbase-client-0.0.1/README.md
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2023-08-30 20:20:18.507463 csvbase-client-0.0.1/csvbase_client/
--rw-r--r--   0 cal       (1000) cal       (1000)        5 2023-08-29 19:59:11.000000 csvbase-client-0.0.1/csvbase_client/VERSION
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.0.1/csvbase_client/__init__.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2023-08-30 20:20:18.507463 csvbase-client-0.0.1/csvbase_client/internals/
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.0.1/csvbase_client/internals/__init__.py
--rw-r--r--   0 cal       (1000) cal       (1000)      988 2023-08-30 09:19:08.000000 csvbase-client-0.0.1/csvbase_client/internals/auth.py
--rw-r--r--   0 cal       (1000) cal       (1000)     7657 2023-08-30 19:16:49.000000 csvbase-client-0.0.1/csvbase_client/internals/cache.py
--rw-r--r--   0 cal       (1000) cal       (1000)     4358 2023-08-30 13:41:46.000000 csvbase-client-0.0.1/csvbase_client/internals/cli.py
--rw-r--r--   0 cal       (1000) cal       (1000)     1560 2023-08-29 09:47:19.000000 csvbase-client-0.0.1/csvbase_client/internals/config.py
--rw-r--r--   0 cal       (1000) cal       (1000)       77 2023-08-29 09:50:35.000000 csvbase-client-0.0.1/csvbase_client/internals/dirs.py
--rw-r--r--   0 cal       (1000) cal       (1000)      747 2023-08-29 17:38:17.000000 csvbase-client-0.0.1/csvbase_client/internals/http.py
--rw-r--r--   0 cal       (1000) cal       (1000)      946 2023-08-29 18:10:42.000000 csvbase-client-0.0.1/csvbase_client/internals/value_objs.py
--rw-r--r--   0 cal       (1000) cal       (1000)      947 2023-08-30 19:04:54.000000 csvbase-client-0.0.1/csvbase_client/internals/version.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2023-08-30 20:20:18.507463 csvbase-client-0.0.1/csvbase_client.egg-info/
--rw-r--r--   0 cal       (1000) cal       (1000)     2234 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/PKG-INFO
--rw-r--r--   0 cal       (1000) cal       (1000)      652 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/SOURCES.txt
--rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/dependency_links.txt
--rw-r--r--   0 cal       (1000) cal       (1000)       68 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/entry_points.txt
--rw-r--r--   0 cal       (1000) cal       (1000)      216 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/requires.txt
--rw-r--r--   0 cal       (1000) cal       (1000)       15 2023-08-30 20:20:18.000000 csvbase-client-0.0.1/csvbase_client.egg-info/top_level.txt
--rw-r--r--   0 cal       (1000) cal       (1000)       38 2023-08-30 20:20:18.511463 csvbase-client-0.0.1/setup.cfg
--rw-r--r--   0 cal       (1000) cal       (1000)     2108 2023-08-30 20:20:09.000000 csvbase-client-0.0.1/setup.py
-drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2023-08-30 20:20:18.507463 csvbase-client-0.0.1/tests/
--rw-r--r--   0 cal       (1000) cal       (1000)      371 2023-08-30 11:50:37.000000 csvbase-client-0.0.1/tests/test_version.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/
+-rw-r--r--   0 cal       (1000) cal       (1000)    34523 2017-09-30 07:16:25.000000 csvbase-client-0.1.0/COPYING
+-rw-r--r--   0 cal       (1000) cal       (1000)       40 2023-04-05 16:09:56.000000 csvbase-client-0.1.0/MANIFEST.in
+-rw-r--r--   0 cal       (1000) cal       (1000)     4342 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/PKG-INFO
+-rw-r--r--   0 cal       (1000) cal       (1000)     2995 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/README.md
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client/
+-rw-r--r--   0 cal       (1000) cal       (1000)        5 2024-04-05 10:39:14.000000 csvbase-client-0.1.0/csvbase_client/VERSION
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/__init__.py
+-rw-r--r--   0 cal       (1000) cal       (1000)       40 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/constants.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      530 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/exceptions.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     7318 2024-04-08 10:19:42.000000 csvbase-client-0.1.0/csvbase_client/fsspec.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client/internals/
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/internals/__init__.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      988 2024-02-03 15:57:46.000000 csvbase-client-0.1.0/csvbase_client/internals/auth.py
+-rw-r--r--   0 cal       (1000) cal       (1000)    11948 2024-04-05 10:43:06.000000 csvbase-client-0.1.0/csvbase_client/internals/cache.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     4438 2024-04-08 09:41:10.000000 csvbase-client-0.1.0/csvbase_client/internals/cli.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     1560 2023-08-29 09:47:19.000000 csvbase-client-0.1.0/csvbase_client/internals/config.py
+-rw-r--r--   0 cal       (1000) cal       (1000)       77 2023-08-29 09:50:35.000000 csvbase-client-0.1.0/csvbase_client/internals/dirs.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      866 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/csvbase_client/internals/http.py
+-rw-r--r--   0 cal       (1000) cal       (1000)     1032 2023-08-31 16:35:27.000000 csvbase-client-0.1.0/csvbase_client/internals/value_objs.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      855 2024-04-08 09:54:49.000000 csvbase-client-0.1.0/csvbase_client/internals/version.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      634 2024-02-03 12:13:20.000000 csvbase-client-0.1.0/csvbase_client/io.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/csvbase_client.egg-info/
+-rw-r--r--   0 cal       (1000) cal       (1000)     4342 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/PKG-INFO
+-rw-r--r--   0 cal       (1000) cal       (1000)      775 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)        1 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)      134 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/entry_points.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)      120 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/requires.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)       15 2024-04-09 11:17:53.000000 csvbase-client-0.1.0/csvbase_client.egg-info/top_level.txt
+-rw-r--r--   0 cal       (1000) cal       (1000)       38 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/setup.cfg
+-rw-r--r--   0 cal       (1000) cal       (1000)     2114 2024-04-09 11:16:11.000000 csvbase-client-0.1.0/setup.py
+drwxr-xr-x   0 cal       (1000) cal       (1000)        0 2024-04-09 11:17:53.839408 csvbase-client-0.1.0/tests/
+-rw-r--r--   0 cal       (1000) cal       (1000)      759 2024-04-05 10:25:59.000000 csvbase-client-0.1.0/tests/test_cache.py
+-rw-r--r--   0 cal       (1000) cal       (1000)      371 2023-08-30 11:50:37.000000 csvbase-client-0.1.0/tests/test_version.py
```

### Comparing `csvbase-client-0.0.1/COPYING` & `csvbase-client-0.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/auth.py` & `csvbase-client-0.1.0/csvbase_client/internals/auth.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/cache.py` & `csvbase-client-0.1.0/csvbase_client/fsspec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,241 +1,230 @@
-import sqlite3
+import io
+from typing import Dict, Optional, IO, Iterator
 import shutil
-from contextlib import closing
 from logging import getLogger
-from pathlib import Path
-from typing import List, Optional, IO, Any, Dict, Iterable, Tuple
-from io import BytesIO
 from urllib.parse import urljoin
-from datetime import datetime, timezone
+from threading import Lock
+import contextlib
 
-from pyappcache.keys import BaseKey, Key
-from pyappcache.sqlite_lru import SqliteCache
-from pyappcache.serialisation import Serialiser
-
-from .config import Config
-from .http import get_http_sesh
-from .dirs import dirs
-from .value_objs import Auth, ContentType
+import requests
+from pyappcache.keys import Key
+from pyappcache.fs import FilesystemCache
+from fsspec.spec import AbstractFileSystem, AbstractBufferedFile
+
+from .io import rewind
+from .internals.cache import get_fs_cache, get_last_etag, set_etag, RepKey
+from .internals.value_objs import Auth, ContentType
+from .internals.auth import get_auth
+from .internals.http import get_http_sesh, HTTP_TIMEOUT
+from .constants import CSVBASE_DOT_COM
+from .exceptions import http_error_to_user_message, CSVBaseException
 
 logger = getLogger(__name__)
 
-HTTP_TIMEOUTS = (5, 60)
 
-ETAGS_DDL = """
-CREATE TABLE IF NOT EXISTS etags (
-    ref text,
-    etag text NOT NULL,
-    content_type text NOT NULL,
-    last_modified text NOT NULL,
-    PRIMARY KEY (ref, content_type)
-);
-"""
-
-GET_ETAG_DQL = """
-SELECT
-    etag
-FROM
-    etags
-WHERE
-    ref = ?
-AND
-    content_type = ?
-"""
-
-#
-SET_ETAG_DML = """
-INSERT INTO etags (ref, etag, content_type, last_modified)
-VALUES (?, ?, ?, ?)
-ON CONFLICT(ref, content_type) DO UPDATE SET
-    etag = excluded.etag,
-    last_modified = excluded.last_modified;
-
-"""
-
-GET_CACHE_INFO_DQL = """
-SELECT
-   ref, etag, content_type, last_modified
-FROM etags
-JOIN
-   pyappcache
-ON key = 'pyappcache/' || etag
-"""
-
-
-class ETagKey(BaseKey):
-    def __init__(self, ref):
-        self.ref = ref
-
-    def cache_key_segments(self) -> List[str]:
-        return [self.ref]  # FIXME: correct this in the docs
-
-    def should_compress(self, python_obj, as_bytes) -> bool:
-        # csv files are highly compressible
-        return True
-
-
-def cache_path() -> Path:
-    return Path(dirs.user_cache_dir) / "cache.db"
-
-
-class TableCache:
-    """A read-through cache of tables."""
-
-    def __init__(self, config: Config) -> None:
-        cache_db_path = cache_path()
-        logger.info("cache db path = %s", cache_db_path)
-        cache_db_path.parent.mkdir(parents=True, exist_ok=True)
-        self._sqlite_conn = sqlite3.connect(cache_db_path)
-        self._create_etags_table()
-        self._lru_cache = SqliteCache(max_size=100, connection=self._sqlite_conn)
-        self._lru_cache.prefix = (
-            "pyappcache"  # FIXME: necessary because of a bug upstream
-        )
-        self._http_client = get_http_sesh()
-
-    def base_url(self) -> str:
-        return "https://csvbase.com/"
-
-    def check_creds(self, config: Config) -> bool:
-        if config.username is None or config.api_key is None:
-            return False
-        response = self._http_client.get(urljoin(self.base_url(), config.username))
-        if 400 <= response.status_code < 500:
-            return False
-        elif 200 <= response.status_code < 300:
-            return True
+def get_rep(
+    http_sesh: requests.Session,
+    cache: FilesystemCache,
+    base_url: str,
+    ref: str,
+    content_type: ContentType,
+    auth: Optional[Auth] = None,
+) -> IO[bytes]:
+    headers = {"Accept": "text/csv"}
+    if auth is not None:
+        headers["Authorization"] = auth.as_basic_auth()
+    # breakpoint()
+    url = url_for_rep(base_url, ref, content_type)
+    etag = get_last_etag(cache, base_url, ref, content_type)
+    rep_key: Key[IO[bytes]] = RepKey(base_url, ref, content_type)
+
+    if etag is not None:
+        rep = cache.get(rep_key)
+        if rep is not None:
+            logger.debug("last known etag found: '%s' ('%s')", ref, etag)
+            headers["If-None-Match"] = etag
         else:
-            response.raise_for_status()
-            # this (should be) unreachable but typechecker doesn't know that
-            return False
-
-    def get_table(
-        self, ref: str, auth: Optional[Auth] = None, force_miss: bool = False
-    ) -> IO[bytes]:
-        content_type = ContentType.CSV
-        headers = {"Accept": content_type.mimetype()}
-        if auth is not None:
-            headers["Authorization"] = auth.as_basic_auth()
-        url = self._build_url_for_table_ref(ref, content_type)
-        canon_url = self._build_url_for_table_ref(ref)
-        etag = self._get_etag(canon_url)
-        if etag is not None:
-            logger.debug("etag found: %s", etag)
-            key: Key[IO[bytes]] = ETagKey(etag)
-            table = self._lru_cache.get(key)
-            if table is not None:
-                logger.debug("cache HIT: %s", ref)
-                if force_miss:
-                    logger.info("cache HIT but forcing MISS")
-                else:
-                    headers["If-None-Match"] = etag
-            else:
-                logger.debug("etag known but cache MISS: %s", ref)
-
-        response = self._http_client.get(url, headers=headers, stream=True)
-
-        if response.status_code >= 400:
-            logger.error(
-                "got status_code: %d, %s", response.status_code, response.content
+            logger.debug("an etag is known but cache MISS: '%s'", ref)
+    else:
+        logger.debug("no etag known")
+
+    response = http_sesh.get(url, headers=headers, stream=True, timeout=HTTP_TIMEOUT)
+    logger.info("got response code: %d", response.status_code)
+
+    # make sure to log all 500s to make it clear a real error has occurred
+    if response.status_code >= 500:
+        logger.error("got status_code: %d, %s", response.status_code, response.content)
+
+    # 400s and 500s are raised as exceptions
+    if response.status_code >= 400:
+        message = http_error_to_user_message(ref, response)
+        raise CSVBaseException(message)
+
+    if response.status_code == 304:
+        # FIXME: a rejig is required here for type safety
+        return rep  # type: ignore
+    else:
+        etag = response.headers["ETag"]
+        set_etag(cache, base_url, ref, content_type, etag)
+        rep = io.BytesIO()
+        with rewind(rep):
+            shutil.copyfileobj(response.raw, rep)
+            response.close()
+        with rewind(rep):
+            cache.set(rep_key, rep)
+
+    return rep
+
+
+def send_rep(
+    http_sesh: requests.Session,
+    cache: FilesystemCache,
+    base_url: str,
+    ref: str,
+    content_type: ContentType,
+    rep: IO[bytes],
+    auth: Optional[Auth] = None,
+) -> None:
+    headers = {"Content-Type": content_type.mimetype()}
+    if auth is not None:
+        headers["Authorization"] = auth.as_basic_auth()
+    url = url_for_rep(base_url, ref, content_type)
+    response = http_sesh.put(url, data=rep, headers=headers, timeout=HTTP_TIMEOUT)
+    response.raise_for_status()
+
+
+def url_for_rep(base_url: str, ref: str, content_type: ContentType) -> str:
+    url = urljoin(base_url, ref)
+    return url
+
+
+class CSVBaseFileSystem(AbstractFileSystem):
+    def __init__(self, *args, **kwargs):
+        kwargs["use_listings_cache"] = False
+        self._base_url = CSVBASE_DOT_COM
+        self._cache_lock = Lock()
+
+        super().__init__(*args, **kwargs)
+
+    def fsid(self):
+        raise NotImplementedError
+
+    def _open(
+        self,
+        path,
+        mode="rb",
+        block_size=None,
+        autocommit=True,
+        cache_options=None,
+        **kwargs
+    ):
+        f = CSVBaseFile(self, path, mode)
+        return f
+
+    def created(self, path):
+        raise NotImplementedError
+
+    def modified(self, path):
+        raise NotImplementedError
+
+    def cp_file(self, path1, path2, **kwargs):
+        raise NotImplementedError
+
+    def touch(self, path, truncate=True, **kwargs):
+        # This will never be implemented
+        raise NotImplementedError
+
+    def ls(self, path, detail: bool = True):
+        # FIXME: need a way to list a users' tables
+        return []
+
+    def _rm(self, path):
+        raise NotImplementedError
+
+    def info(self, path: str) -> Dict:
+        # FIXME: implement a proper HEAD method for csvbase, avoid fetching the
+        # whole file: https://github.com/calpaterson/csvbase/issues/71
+        with self.open(path, "rb") as table_f:
+            size = table_f.size
+        return {
+            "name": path,
+            "size": size,
+            "type": "file" if "/" in path else "directory",
+        }
+
+    def _get_rep(self, ref: str, content_type: ContentType) -> IO[bytes]:
+        _http_sesh = get_http_sesh()
+        with self._get_fs_cache() as cache:
+            return get_rep(
+                _http_sesh,
+                cache,
+                self._base_url,
+                ref,
+                content_type,
+                self._get_auth(),
             )
 
-            response.raise_for_status()
+    def _send_rep(self, ref: str, content_type: ContentType, rep: IO[bytes]) -> None:
+        _http_sesh = get_http_sesh()
+        with self._get_fs_cache() as cache:
+            send_rep(
+                _http_sesh,
+                cache,
+                self._base_url,
+                ref,
+                content_type,
+                rep,
+                self._get_auth(),
+            )
 
-        if response.status_code == 304:
-            logger.debug("server says cache still valid")
-            # typechecker thinks this is still optional but it can't be if we
-            # got here
-            return table  # type: ignore
-        else:
-            received_etag = response.headers["ETag"]
-            received_etag_key = ETagKey(received_etag)
-            self._set_etag(canon_url, received_etag, ContentType.CSV)
-            buf: BytesIO = BytesIO()
-            shutil.copyfileobj(response.raw, buf)
-            response.close()
-            buf.seek(0)
-            self._lru_cache.set(received_etag_key, buf)
-            buf.seek(0)
-            return buf
-
-    def metadata(self, ref: str) -> Dict[str, Any]:
-        headers = {"Accept": "application/json"}
-        response = self._http_client.get(
-            self._build_url_for_table_ref(ref), headers=headers
-        )
-
-        response.raise_for_status()
-        rv = {"etag": response.headers["ETag"]}
-        rv.update(response.json())
-        return rv
-
-    def set_table(
-        self, ref: str, file_obj: IO[str], auth: Optional[Auth] = None
-    ) -> None:
-        headers = {"Content-Type": "text/csv"}
-        if auth is not None:
-            headers["Authorization"] = auth.as_basic_auth()
-        url = self._build_url_for_table_ref(ref)
-        response = self._http_client.put(url, data=file_obj, headers=headers)
-        response.raise_for_status()
-
-    def _build_url_for_table_ref(
-        self, ref: str, content_type: Optional[ContentType] = None
-    ) -> str:
-        url = urljoin(self.base_url(), ref)
-        if content_type is not None:
-            url += content_type.file_extension()
-        return url
-
-    def _get_etag(self, ref: str) -> Optional[str]:
-        # FIXME: This still isn't quite right as etags need to take account of
-        # Vary, but we aren't.
-        with closing(self._sqlite_conn.cursor()) as cursor:
-            cursor.execute(GET_ETAG_DQL, (ref, "text/csv"))
-            rs = cursor.fetchone()
-        if rs is not None:
-            return rs[0]
+    def _get_auth(self) -> Optional[Auth]:
+        # this can't be done on an instance level for testing reasons - fsspec
+        # appears to re-use instances
+        return get_auth()
+
+    @contextlib.contextmanager
+    def _get_fs_cache(self) -> Iterator[FilesystemCache]:
+        # Dask requires these fsspec objects to be thread safe.  However the
+        # FilesystemCache was not designed with that in mind.  As a temporary
+        # solution, lock it.
+        with self._cache_lock:
+            yield get_fs_cache()
+
+
+class CSVBaseFile(AbstractBufferedFile):
+    def __init__(self, fs: CSVBaseFileSystem, path, mode, **kwargs) -> None:
+        self.fs = fs
+        self.path = path
+        self._staging_buffer = io.BytesIO()
+        # this is necessary because we have no way to get size of the file
+        if mode == "rb":
+            with rewind(self._staging_buffer):
+                shutil.copyfileobj(
+                    fs._get_rep(path, ContentType.CSV), self._staging_buffer
+                )
+                size = self._staging_buffer.tell()
         else:
-            return None
+            size = 0
 
-    def _set_etag(self, url: str, etag: str, content_type: ContentType) -> None:
-        with closing(self._sqlite_conn.cursor()) as cursor:
-            cursor.execute(
-                SET_ETAG_DML,
-                (
-                    url,
-                    etag,
-                    content_type.mimetype(),
-                    datetime.now(timezone.utc).isoformat(),
-                ),
-            )
-            self._sqlite_conn.commit()
+        # currently this value is used only for test multi-chunk uploads
+        self._chunk_count = 0
 
-    def _create_etags_table(self):
-        with closing(self._sqlite_conn.cursor()) as cursor:
-            cursor.execute(ETAGS_DDL)
-            self._sqlite_conn.commit()
-
-    def entries(self) -> Iterable[Tuple[str, str, ContentType, datetime]]:
-        def parse_row(
-            url, etag, content_type_str, last_modified_str
-        ) -> Tuple[str, str, ContentType, datetime]:
-            content_type = ContentType.from_mimetype(content_type_str)
-            last_modified = datetime.fromisoformat(last_modified_str)
-            return (url, etag, content_type, last_modified)
-
-        with closing(self._sqlite_conn.cursor()) as cursor:
-            cursor.execute(GET_CACHE_INFO_DQL)
-            yield from (parse_row(*row) for row in cursor)
-
-    def clear(self) -> None:
-        if cache_path().exists():
-            cache_path().unlink()
-
-
-class StreamSerialiser(Serialiser):
-    def dump(self, obj: Any) -> IO[bytes]:
-        return obj
+        super().__init__(fs, path, mode, size=size, cache_type="none", **kwargs)
 
-    def load(self, data: IO[bytes]) -> Any:
-        return data
+    def _fetch_range(self, start: int, end: int) -> bytes:
+        self._staging_buffer.seek(start)
+        count = end - start
+        return self._staging_buffer.read(count)
+
+    def _initiate_upload(self) -> None:
+        # FIXME: possibly truncate the staging buffer
+        pass
+
+    def _upload_chunk(self, final=False) -> None:
+        # we send it all in one go at the moment
+        self.buffer.seek(0)
+        shutil.copyfileobj(self.buffer, self._staging_buffer)
+        self._chunk_count += 1
+        if final:
+            self._staging_buffer.seek(0)
+            self.fs._send_rep(self.path, ContentType.CSV, self._staging_buffer)
```

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/cli.py` & `csvbase-client-0.1.0/csvbase_client/internals/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,153 +1,153 @@
 import shutil
-import io
 import sys
 from logging import DEBUG, basicConfig, WARNING
 from typing import IO
-import csv
 
-import toml
+import humanize
+import fsspec
 import click
+from rich.console import Console as RichConsole
+from rich.table import Table as RichTable
 
-from .auth import get_auth
-from .cache import TableCache, cache_path
-from .config import get_config, write_config, config_path
+from .config import config_path
 from .version import get_version
+from .cache import cache_path, get_fs_cache, cache_contents
+from ..exceptions import CSVBaseException
 
 
 @click.group("csvbase-client")
 @click.version_option(version=get_version())
 @click.option("--verbose", is_flag=True, help="Enable more verbose output (to stderr).")
 def cli(verbose: bool):
     """A cli client for csvbase."""
     if verbose:
         level = DEBUG
     else:
         level = WARNING
     basicConfig(level=level, stream=sys.stderr, format="%(levelname)s: %(message)s")
 
 
-@cli.group("table", help="Read and write from tables.")
-def table():
-    ...
+@cli.group("table", help="Interact with tables")
+def table(): ...
 
 
 @cli.command()
-def config():
+def info():
     """Show the configuration file location, and the contents"""
     exist_str = "" if config_path().exists() else " (does not exist)"
     click.echo(f"config path: {config_path()}{exist_str}")
     exist_str = "" if cache_path().exists() else " (does not exist)"
-    click.echo(f"config path: {cache_path()}{exist_str}")
+    click.echo(f"cache path: {cache_path()}{exist_str}")
 
 
 @cli.group(help="Manage the local cache")
-def cache():
-    ...
+def cache(): ...
 
 
 @cache.command("show", help="Show cache location and contents")
-@click.option(
-    "--full-urls",
-    default=False,
-    is_flag=True,
-    help="Show full urls (hint: some terminals make them clickable)",
-)
-def cache_show(full_urls: bool):
-    table_cache = TableCache(get_config())
-    tsv_writer = csv.writer(sys.stdout, dialect="excel-tab")
-    common_cols = ["last_modified", "content_type", "etag (prefix)"]
-    if full_urls:
-        header = ["url"]
-    else:
-        header = ["ref"]
-    header.extend(common_cols)
-    tsv_writer.writerow(header)
-
-    prefix_length = len(table_cache.base_url())
-    for url, etag, content_type, last_modified in table_cache.entries():
-        # FIXME: not quite a ref - includes file extension
-        if full_urls:
-            a = url
-        else:
-            a = url[prefix_length:]
-        etag_prefix = etag[3:13]
-        tsv_writer.writerow([a, last_modified, content_type.mimetype(), etag_prefix])
-
+def cache_show() -> None:
+    table = RichTable(
+        title="csvbase-client cache", caption=f"Cache path: {cache_path()}"
+    )
+    table.add_column("Ref")
+    table.add_column("ETag prefix")
+    table.add_column("Last read")
+    table.add_column("Size")
+
+    for ce in cache_contents(get_fs_cache()):
+        # for now, only some of the CacheEntry data is surfaced
+        table.add_row(
+            ce.ref,
+            ce.etag_prefix(),
+            humanize.naturaltime(ce.last_read),
+            humanize.naturalsize(ce.size_bytes, gnu=True),
+        )
 
-@cache.command("clear", help="Wipe the cache")
-def clear():
-    table_cache = TableCache(get_config())
-    table_cache.clear()
+    console = RichConsole()
+    console.print(table)
 
 
-@cli.command()
-def login():
-    """Write API credentials to config file, creating it if necessary."""
-    config = get_config()
-    username = click.prompt(
-        "Please enter your username", default=config.username, show_default=True
-    )
-    api_key = click.prompt("Please enter your API key", hide_input=True)
-    config.username = username
-    config.api_key = api_key
-
-    table_cache = TableCache()
-    are_valid = table_cache.check_creds(config)
-    if are_valid:
-        write_config(config)
-        click.echo(f"Wrote {config_path()}")
-    else:
-        click.echo(
-            click.style(
-                "ERROR: Username or API key rejected by server - double check"
-                " they're both correct!",
-                fg="red",
-            )
-        )
-        exit(1)
+@cache.command("clear", help="Wipe the cache")
+def clear() -> None:
+    fs_cache = get_fs_cache()
+    fs_cache.clear()
+    # FIXME: it should be pyappcache that does this:
+    for path in fs_cache.directory.glob("*.csv"):
+        path.unlink()
+
+
+# @cli.command()
+# def login():
+#     """Write API credentials to config file, creating it if necessary."""
+#     config = get_config()
+#     username = click.prompt(
+#         "Please enter your username", default=config.username, show_default=True
+#     )
+#     api_key = click.prompt("Please enter your API key", hide_input=True)
+#     config.username = username
+#     config.api_key = api_key
+
+#     table_cache = TableCache()
+#     are_valid = table_cache.check_creds(config)
+#     if are_valid:
+#         write_config(config)
+#         click.echo(f"Wrote {config_path()}")
+#     else:
+#         click.echo(
+#             click.style(
+#                 "ERROR: Username or API key rejected by server - double check"
+#                 " they're both correct!",
+#                 fg="red",
+#             )
+#         )
+#         exit(1)
 
 
 @table.command(help="Get a table.")
 @click.argument("ref")
 @click.option(
     "--force-cache-miss",
     is_flag=True,
     default=False,
     help="Always download the table again, even if it hasn't changed",
 )
 def get(ref: str, force_cache_miss: bool):
-    table_cache = TableCache(get_config())
-    table_buf = table_cache.get_table(ref, force_miss=force_cache_miss, auth=get_auth())
-    text_buf = io.TextIOWrapper(table_buf, encoding="utf-8")
-    shutil.copyfileobj(text_buf, sys.stdout)
-
-
-@table.command(help="Show metadata about a table")
-@click.argument("ref")
-def table_show(ref: str):
-    table_cache = TableCache(get_config())
-    metadata = table_cache.metadata(ref)
-    rv = {
-        ref: {
-            "caption": metadata["caption"],
-            "created": metadata["created"],
-            "last_changed": metadata["last_changed"],
-            "etag": metadata["etag"],
-        }
-    }
+    fs = fsspec.filesystem("csvbase")
+    try:
+        table_buf = fs.open(ref, "r")
+    except CSVBaseException as e:
+        error_console = RichConsole(stderr=True, style="bold red")
+        error_console.print(str(e))
+        sys.exit(1)
+    shutil.copyfileobj(table_buf, sys.stdout)
+
+
+# @table.command("show", help="Show metadata about a table")
+# @click.argument("ref")
+# def table_show(ref: str):
+#     table_cache = TableCache(get_config())
+#     metadata = table_cache.metadata(ref, auth=get_auth())
+#     rv = {
+#         ref: {
+#             "caption": metadata["caption"],
+#             "created": metadata["created"],
+#             "last_changed": metadata["last_changed"],
+#         }
+#     }
 
-    toml.dump(rv, sys.stdout)
+#     click.echo(toml.dumps(rv))
 
 
-@table.command(help="Upsert a table.")
+@table.command("set", help="Create or upsert a table.")
 @click.argument("ref")
 @click.argument("file", type=click.File("rb"))
 def set(ref: str, file: IO[str]):
-    table_cache = TableCache(get_config())
-    table_cache.set_table(ref, file, auth=get_auth())
+    fs = fsspec.filesystem("csvbase")
+    with fs.open(ref, "wb") as table_buf:
+        shutil.copyfileobj(file, table_buf)
 
 
 # NOTE: This is for convenience only, the cli is actually called by setup.py
 # entry_points
 if __name__ == "__main__":
     cli()
```

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/config.py` & `csvbase-client-0.1.0/csvbase_client/internals/config.py`

 * *Files identical despite different names*

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/http.py` & `csvbase-client-0.1.0/csvbase_client/internals/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from urllib.parse import urljoin
 import requests
 
 from .value_objs import ContentType
 
+# Wait 5 secs to connect, 60s to read.  Sadly no way to set this on
+# requests.Session objects
+HTTP_TIMEOUT = (5, 60)
+
 
 def _get_http_sesh() -> requests.Session:
     """This internal function exists only for testing/mocking reasons."""
     return requests.Session()
 
 
 def get_http_sesh() -> requests.Session:
```

### Comparing `csvbase-client-0.0.1/csvbase_client/internals/value_objs.py` & `csvbase-client-0.1.0/csvbase_client/internals/value_objs.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         return f"Basic {encoded}"
 
 
 @enum.unique
 class ContentType(enum.Enum):
     PARQUET = 1
     CSV = 2
+    JSON = 3
 
     def mimetype(self):
         return MIMETYPE_MAP[self]
 
     @staticmethod
     def from_mimetype(mimetype) -> "ContentType":
         return BACKWARD_MIMETYPE_MAP[mimetype]
@@ -29,15 +30,17 @@
     def file_extension(self) -> str:
         return FILE_EXTENSION_MAP[self]
 
 
 MIMETYPE_MAP = {
     ContentType.PARQUET: "application/parquet",  # unofficial, but convenient
     ContentType.CSV: "text/csv",
+    ContentType.JSON: "application/json",
 }
 
 BACKWARD_MIMETYPE_MAP = {v: k for k, v in MIMETYPE_MAP.items()}
 
 FILE_EXTENSION_MAP = {
     ContentType.CSV: ".csv",
     ContentType.PARQUET: ".parquet",
+    ContentType.JSON: ".json",
 }
```

### Comparing `csvbase-client-0.0.1/csvbase_client.egg-info/SOURCES.txt` & `csvbase-client-0.1.0/csvbase_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 COPYING
 MANIFEST.in
 README.md
 setup.py
 csvbase_client/VERSION
 csvbase_client/__init__.py
+csvbase_client/constants.py
+csvbase_client/exceptions.py
+csvbase_client/fsspec.py
+csvbase_client/io.py
 csvbase_client.egg-info/PKG-INFO
 csvbase_client.egg-info/SOURCES.txt
 csvbase_client.egg-info/dependency_links.txt
 csvbase_client.egg-info/entry_points.txt
 csvbase_client.egg-info/requires.txt
 csvbase_client.egg-info/top_level.txt
 csvbase_client/internals/__init__.py
@@ -15,8 +19,9 @@
 csvbase_client/internals/cache.py
 csvbase_client/internals/cli.py
 csvbase_client/internals/config.py
 csvbase_client/internals/dirs.py
 csvbase_client/internals/http.py
 csvbase_client/internals/value_objs.py
 csvbase_client/internals/version.py
+tests/test_cache.py
 tests/test_version.py
```

