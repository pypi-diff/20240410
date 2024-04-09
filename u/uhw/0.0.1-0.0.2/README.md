# Comparing `tmp/uhw-0.0.1.tar.gz` & `tmp/uhw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uhw-0.0.1.tar", last modified: Sun Apr  7 19:46:21 2024, max compression
+gzip compressed data, was "uhw-0.0.2.tar", last modified: Tue Apr  9 23:04:59 2024, max compression
```

## Comparing `uhw-0.0.1.tar` & `uhw-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:46:21.774075 uhw-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-07 19:46:17.000000 uhw-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-07 19:46:17.000000 uhw-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-07 19:46:21.774075 uhw-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-07 19:46:17.000000 uhw-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-07 19:46:17.000000 uhw-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:46:21.774075 uhw-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:46:21.774075 uhw-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 19:46:17.000000 uhw-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-07 19:46:17.000000 uhw-0.0.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-07 19:46:17.000000 uhw-0.0.1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-07 19:46:17.000000 uhw-0.0.1/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:46:21.774075 uhw-0.0.1/uhw/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 19:46:17.000000 uhw-0.0.1/uhw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-07 19:46:17.000000 uhw-0.0.1/uhw/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-07 19:46:17.000000 uhw-0.0.1/uhw/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-07 19:46:17.000000 uhw-0.0.1/uhw/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:46:21.774075 uhw-0.0.1/uhw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-07 19:46:21.000000 uhw-0.0.1/uhw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-07 19:46:21.000000 uhw-0.0.1/uhw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:46:21.000000 uhw-0.0.1/uhw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 19:46:21.000000 uhw-0.0.1/uhw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 19:46:21.000000 uhw-0.0.1/uhw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:59.081846 uhw-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 23:04:54.000000 uhw-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 23:04:54.000000 uhw-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-09 23:04:59.077846 uhw-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-09 23:04:54.000000 uhw-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 23:04:54.000000 uhw-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:04:59.081846 uhw-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:59.077846 uhw-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:54.000000 uhw-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 23:04:54.000000 uhw-0.0.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-09 23:04:54.000000 uhw-0.0.2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 23:04:54.000000 uhw-0.0.2/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:59.077846 uhw-0.0.2/uhw/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 23:04:54.000000 uhw-0.0.2/uhw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 23:04:54.000000 uhw-0.0.2/uhw/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-09 23:04:54.000000 uhw-0.0.2/uhw/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-09 23:04:54.000000 uhw-0.0.2/uhw/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:04:59.077846 uhw-0.0.2/uhw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-09 23:04:59.000000 uhw-0.0.2/uhw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 23:04:59.000000 uhw-0.0.2/uhw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:04:59.000000 uhw-0.0.2/uhw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 23:04:59.000000 uhw-0.0.2/uhw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 23:04:59.000000 uhw-0.0.2/uhw.egg-info/top_level.txt
```

### Comparing `uhw-0.0.1/LICENSE` & `uhw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/PKG-INFO` & `uhw-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uhw
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lightweight asynchronous command parsing and serving framework.
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Michael Czigler
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `uhw-0.0.1/README.md` & `uhw-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/pyproject.toml` & `uhw-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/tests/test_parser.py` & `uhw-0.0.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/tests/test_protocol.py` & `uhw-0.0.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/tests/test_server.py` & `uhw-0.0.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/uhw/parser.py` & `uhw-0.0.2/uhw/parser.py`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/uhw/protocol.py` & `uhw-0.0.2/uhw/protocol.py`

 * *Files identical despite different names*

### Comparing `uhw-0.0.1/uhw/server.py` & `uhw-0.0.2/uhw/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from asyncio import AbstractEventLoop
 from asyncio import get_running_loop
 from asyncio import run as asyncio_run
-from ssl import SSLContext
 from typing import Any
 from typing import Callable
 
 from .parser import command_to_compiled_regex
 from .protocol import ProtocolFactory
 
 
@@ -44,15 +43,15 @@
             if not self.commands.get(name, None):
                 regex = command_to_compiled_regex(name)
                 self.commands[name] = dict(regex=regex)
             self.commands[name]["pull"] = func
 
         return wrapper
 
-    async def serve(self, host: str, port: int, ssl: SSLContext | None = None) -> None:
+    async def serve(self, host: str, port: int) -> None:
         """
         Create and start server.
         """
 
         loop = get_running_loop()
         protocol_factory = lambda: ProtocolFactory(self.commands)
         server = await loop.create_server(protocol_factory, host, port)
@@ -60,17 +59,16 @@
             await server.serve_forever()
 
     def run(
         self,
         host: str = "0.0.0.0",
         port: int = 5000,
         debug: bool | None = None,
-        loop: AbstractEventLoop | None = None,
-        ssl: SSLContext | None = None,
+        loop_factory: AbstractEventLoop | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Run asynchronous service.
         """
 
-        coro = self.serve(host, port, ssl)
-        asyncio_run(coro, debug=debug)
+        coro = self.serve(host, port)
+        asyncio_run(coro, debug=debug, loop_factory=loop_factory)
```

### Comparing `uhw-0.0.1/uhw.egg-info/PKG-INFO` & `uhw-0.0.2/uhw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uhw
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lightweight asynchronous command parsing and serving framework.
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Michael Czigler
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

