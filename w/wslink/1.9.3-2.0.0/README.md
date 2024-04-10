# Comparing `tmp/wslink-1.9.3.tar.gz` & `tmp/wslink-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../dist/wslink-1.9.3.tar", last modified: Mon Dec 19 17:53:11 2022, max compression
+gzip compressed data, was "wslink-2.0.0.tar", last modified: Wed Apr 10 21:41:58 2024, max compression
```

## Comparing `wslink-1.9.3.tar` & `wslink-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-12-19 17:52:31.000000 wslink-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-19 17:53:11.000000 wslink-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1448 2022-12-19 17:52:31.000000 wslink-1.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       66 2022-12-19 17:53:11.000000 wslink-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1587 2022-12-19 17:52:31.000000 wslink-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/
--rw-r--r--   0 runner    (1001) docker     (116)     1483 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2708 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/backends/
--rw-r--r--   0 runner    (1001) docker     (116)      485 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink/backends/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (116)    23509 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8445 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)    13338 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/backends/aiohttp/relay.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    21137 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)     2573 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/publish.py
--rw-r--r--   0 runner    (1001) docker     (116)       86 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/relay.py
--rw-r--r--   0 runner    (1001) docker     (116)     9394 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/ssl_context.py
--rw-r--r--   0 runner    (1001) docker     (116)      384 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/uri.py
--rw-r--r--   0 runner    (1001) docker     (116)     4574 2022-12-19 17:52:31.000000 wslink-1.9.3/src/wslink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2463 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      555 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       30 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-12-19 17:53:11.000000 wslink-1.9.3/src/wslink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 21:41:28.000000 wslink-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 21:41:58.829609 wslink-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-10 21:41:28.000000 wslink-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 21:41:58.829609 wslink-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-10 21:41:28.000000 wslink-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.821609 wslink-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.825609 wslink-2.0.0/src/wslink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.825609 wslink-2.0.0/src/wslink/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/aiohttp/relay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/generic/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/jupyter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink/backends/tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/backends/tornado/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/chunking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21170 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/ssl_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 21:41:28.000000 wslink-2.0.0/src/wslink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:41:58.829609 wslink-2.0.0/src/wslink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 21:41:58.000000 wslink-2.0.0/src/wslink.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wslink-1.9.3/PKG-INFO` & `wslink-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 1.9.3
+Version: 2.0.0
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,18 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp<4
+Requires-Dist: msgpack<2,>=1
 Provides-Extra: ssl
+Requires-Dist: cryptography; extra == "ssl"
 
 wslink
 ======
 
 Wslink allows easy, bi-directional communication between a python server and a
 javascript client over a websocket_. The client can make RPC calls to the
 server, and the server can publish messages to topics that the client can
@@ -49,14 +52,24 @@
 
 Get the whole story
 -------------------
 
 This package is just the server side of wslink. See the `github repo`_ for
 the full story - and to contribute or report issues!
 
+Configure from environment variables
+------------------------------------
+
+Those only apply for the Python server and launcher.
+
+* WSLINK_LAUNCHER_GET - If set to 1 this will enable the GET endpoint for session information
+* WSLINK_LAUNCHER_DELETE - If set to 1 this will enable the DELETE endpoint for killing a running session
+* WSLINK_MAX_MSG_SIZE - Number of bytes for a message size (default: 4194304)
+* WSLINK_HEART_BEAT - Number of seconds between heartbeats (default: 30)
+
 License
 -------
 Free to use in open-source and commercial projects, under the BSD-3-Clause license.
 
 .. _github repo: https://github.com/kitware/wslink
 .. _ParaView: https://www.paraview.org/
 .. _VTK: http://www.vtk.org/
```

### Comparing `wslink-1.9.3/README.rst` & `wslink-2.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 
 Get the whole story
 -------------------
 
 This package is just the server side of wslink. See the `github repo`_ for
 the full story - and to contribute or report issues!
 
+Configure from environment variables
+------------------------------------
+
+Those only apply for the Python server and launcher.
+
+* WSLINK_LAUNCHER_GET - If set to 1 this will enable the GET endpoint for session information
+* WSLINK_LAUNCHER_DELETE - If set to 1 this will enable the DELETE endpoint for killing a running session
+* WSLINK_MAX_MSG_SIZE - Number of bytes for a message size (default: 4194304)
+* WSLINK_HEART_BEAT - Number of seconds between heartbeats (default: 30)
+
 License
 -------
 Free to use in open-source and commercial projects, under the BSD-3-Clause license.
 
 .. _github repo: https://github.com/kitware/wslink
 .. _ParaView: https://www.paraview.org/
 .. _VTK: http://www.vtk.org/
```

### Comparing `wslink-1.9.3/setup.py` & `wslink-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,13 +41,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="websocket javascript rpc pubsub",
     packages=find_packages("src", exclude=("tests.*", "tests")),
     package_dir={"": "src"},
-    install_requires=["aiohttp<4"],
+    install_requires=["aiohttp<4", "msgpack>=1,<2"],
     extras_require={
         "ssl": ["cryptography"],
     },
     include_package_data=True,
 )
```

### Comparing `wslink-1.9.3/src/wslink/LICENSE` & `wslink-2.0.0/src/wslink/LICENSE`

 * *Files identical despite different names*

### Comparing `wslink-1.9.3/src/wslink/__init__.py` & `wslink-2.0.0/src/wslink/__init__.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.3/src/wslink/backends/aiohttp/launcher.py` & `wslink-2.0.0/src/wslink/backends/aiohttp/launcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-import argparse
 import asyncio
 import datetime
-import io
-import json
 import logging
 import os
-import re
-import string
-import subprocess
 import sys
-import time
-import uuid
 
 from random import choice
 
 import aiohttp.web as aiohttp_web
 
 from . import _root_handler
 
@@ -27,14 +19,24 @@
     STATUS_SERVICE_UNAVAILABLE,
     filterResponse,
     STATUS_OK,
     extractSessionId,
     STATUS_NOT_FOUND,
 )
 
+logger = logging.getLogger(__name__)
+
+# ===========================================================================
+# Launcher ENV configuration
+# ===========================================================================
+
+ENABLE_GET = int(os.environ.get("WSLINK_LAUNCHER_GET", 0))
+ENABLE_DELETE = int(os.environ.get("WSLINK_LAUNCHER_DELETE", 0))
+
+
 # ===========================================================================
 # Class to implement requests to POST, GET and DELETE methods
 # ===========================================================================
 
 
 class LauncherResource(object):
     def __init__(self, options, config):
@@ -46,15 +48,15 @@
             config, ProxyMappingManagerTXT(config["configuration"]["proxy_file"])
         )
         self.process_manager = ProcessManager(config)
 
     def __del__(self):
         try:
             # causes an exception when server is killed with Ctrl-C
-            logging.warning("Server factory shutting down. Stopping all processes")
+            logger.warning("Server factory shutting down. Stopping all processes")
         except:
             pass
 
     # ========================================================================
     # Handle POST request
     # ========================================================================
 
@@ -137,25 +139,25 @@
     # =========================================================================
 
     async def handle_get(self, request):
         id = extractSessionId(request)
 
         if not id:
             message = "id not provided in GET request"
-            logging.error(message)
+            logger.error(message)
             return aiohttp_web.json_response(
                 {"error": message}, status=STATUS_BAD_REQUEST
             )
 
-        logging.info("GET request received for id: %s" % id)
+        logger.info("GET request received for id: %s" % id)
 
         session = self.session_manager.getSession(id)
         if not session:
             message = "No session with id: %s" % id
-            logging.error(message)
+            logger.error(message)
             return aiohttp_web.json_response(
                 {"error": message}, status=STATUS_BAD_REQUEST
             )
 
         # Return session meta-data
         return aiohttp_web.json_response(
             filterResponse(session, self.field_filter), status=STATUS_OK
@@ -166,35 +168,35 @@
     # =========================================================================
 
     async def handle_delete(self, request):
         id = extractSessionId(request)
 
         if not id:
             message = "id not provided in DELETE request"
-            logging.error(message)
+            logger.error(message)
             return aiohttp_web.json_response(
                 {"error": message}, status=STATUS_BAD_REQUEST
             )
 
-        logging.info("DELETE request received for id: %s" % id)
+        logger.info("DELETE request received for id: %s" % id)
 
         session = self.session_manager.getSession(id)
         if not session:
             message = "No session with id: %s" % id
-            logging.error(message)
+            logger.error(message)
             return aiohttp_web.json_response(
                 {"error": message}, status=STATUS_NOT_FOUND
             )
 
         # Remove session
         self.session_manager.deleteSession(id)
         self.process_manager.stopProcess(id)
 
         message = "Deleted session with id: %s" % id
-        logging.info(message)
+        logger.info(message)
 
         return aiohttp_web.json_response(session, status=STATUS_OK)
 
 
 # =============================================================================
 # Start the web server
 # =============================================================================
@@ -209,37 +211,45 @@
     host = str(config["configuration"]["host"])
     port = int(config["configuration"]["port"])
     sanitize = config["configuration"]["sanitize"]
 
     # Setup logging
     logFileName = log_dir + os.sep + "launcherLog.log"
     formatting = "%(asctime)s:%(levelname)s:%(name)s:%(message)s"
-    logging.basicConfig(
-        level=logging.DEBUG, filename=logFileName, filemode="w", format=formatting
-    )
+    # create file handler which logs even debug messages
+    fh = logging.FileHandler(logFileName, mode="w")
+    fh.setLevel(logging.DEBUG)
+    fh.setFormatter(logging.Formatter(formatting))
+    logging.getLogger("wslink").addHandler(fh)
     if options.debug:
         console = logging.StreamHandler(sys.stdout)
         console.setLevel(logging.INFO)
         formatter = logging.Formatter(formatting)
         console.setFormatter(formatter)
-        logging.getLogger("").addHandler(console)
+        logging.getLogger("wslink").addHandler(console)
 
     web_app = aiohttp_web.Application()
 
     launcher_resource = LauncherResource(options, config)
 
     if not endpoint.startswith("/"):
         endpoint = "/{0}/".format(endpoint)
 
-    web_app.add_routes(
-        [
-            aiohttp_web.post(endpoint, launcher_resource.handle_post),
-            aiohttp_web.get(endpoint + "{id}", launcher_resource.handle_get),
-            aiohttp_web.delete(endpoint + "{id}", launcher_resource.handle_delete),
-        ]
-    )
+    routes = [
+        aiohttp_web.post(endpoint, launcher_resource.handle_post),
+    ]
+
+    if ENABLE_GET:
+        routes.append(aiohttp_web.get(endpoint + "{id}", launcher_resource.handle_get))
+
+    if ENABLE_DELETE:
+        routes.append(
+            aiohttp_web.delete(endpoint + "{id}", launcher_resource.handle_delete)
+        )
+
+    web_app.add_routes(routes)
 
     if len(content) > 0:
         web_app.router.add_route("GET", "/", _root_handler)
         web_app.add_routes([aiohttp_web.static("/", content)])
 
     aiohttp_web.run_app(web_app, host=host, port=port)
```

### Comparing `wslink-1.9.3/src/wslink/backends/aiohttp/relay.py` & `wslink-2.0.0/src/wslink/backends/aiohttp/relay.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,16 +373,14 @@
 
     if www_path is None:
         www_path = args.www_path
 
     if proxy_route is None:
         proxy_route = args.proxy_route
 
-    logging.basicConfig()
-
     # Manage routes
     routes = []
 
     # Need to be first: static delivery should be a fallback
     if proxy_route is not None:
         logger.info("Proxy route: %s", proxy_route)
         routes.append(web.get(proxy_route, wsRelay.get_handler(mode)))
```

### Comparing `wslink-1.9.3/src/wslink/launcher.py` & `wslink-2.0.0/src/wslink/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import time
 import uuid
 
 from random import choice
 
 from wslink import backends
 
+logger = logging.getLogger(__name__)
+
 STATUS_OK = 200
 STATUS_BAD_REQUEST = 400
 STATUS_NOT_FOUND = 404
 STATUS_SERVICE_UNAVAILABLE = 503
 
 sample_config_file = """
 Here is a sample of what a configuration file could look like:
@@ -201,24 +203,24 @@
         return
     for key in sanitize:
         if key in key_pair:
             checkItem = sanitize[key]
             value = key_pair[key]
             if checkItem["type"] == "inList":
                 if not value in checkItem["list"]:
-                    logging.warning(
+                    logger.warning(
                         "key %s: sanitize %s with default" % (key, key_pair[key])
                     )
                     key_pair[key] = checkItem["default"]
             elif checkItem["type"] == "regexp":
                 if not "compiled" in checkItem:
                     # User is responsible to add begin- and end- string symbols, to make sure entire string is matched.
                     checkItem["compiled"] = re.compile(checkItem["regexp"])
                 if checkItem["compiled"].match(value) == None:
-                    logging.warning(
+                    logger.warning(
                         "key %s: sanitize %s with default" % (key, key_pair[key])
                     )
                     key_pair[key] = checkItem["default"]
 
 
 # -----------------------------------------------------------------------------
 # guard against malicious clients - make sure substitution is expected, if 'sanitize' is provided
@@ -228,15 +230,15 @@
 def replaceVariables(template_str, variable_list, sanitize):
     for key_pair in variable_list:
         checkSanitize(key_pair, sanitize)
         item_template = string.Template(template_str)
         template_str = item_template.safe_substitute(key_pair)
 
     if "$" in template_str:
-        logging.error("Some properties could not be resolved: " + template_str)
+        logger.error("Some properties could not be resolved: " + template_str)
 
     return template_str
 
 
 # -----------------------------------------------------------------------------
 
 
@@ -437,16 +439,16 @@
         with io.open(logFilePath, mode="a+", buffering=1, encoding="utf-8") as log_file:
             try:
                 proc = subprocess.Popen(
                     session["cmd"], stdout=log_file, stderr=log_file
                 )
                 self.processes[session["id"]] = proc
             except:
-                logging.error("The command line failed")
-                logging.error(" ".join(map(str, session["cmd"])))
+                logger.error("The command line failed")
+                logger.error(" ".join(map(str, session["cmd"])))
                 return None
 
         return proc
 
     def stopProcess(self, id):
         proc = self.processes[id]
         del self.processes[id]
```

### Comparing `wslink-1.9.3/src/wslink/server.py` & `wslink-2.0.0/src/wslink/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,19 +275,20 @@
     if hasattr(wslinkServer, "set_server"):
         wslinkServer.set_server(ws_server)
 
     def create_coroutine():
         return ws_server.start(port_callback)
 
     def main_exec():
-        # Block until the loop finishes and then close the loop
+        # Block until webapp exits
         try:
             loop.run_until_complete(create_coroutine())
-        finally:
-            loop.close()
+        except SystemExit:
+            # backend gracefully exit (due to timeout or SIGINT/SIGTERM)
+            pass
 
     def task_exec():
         return loop.create_task(create_coroutine())
 
     exec_modes = {
         "main": main_exec,
         "task": task_exec,
```

### Comparing `wslink-1.9.3/src/wslink/ssl_context.py` & `wslink-2.0.0/src/wslink/ssl_context.py`

 * *Files identical despite different names*

### Comparing `wslink-1.9.3/src/wslink/websocket.py` & `wslink-2.0.0/src/wslink/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 """
 
 import logging
 
 from . import register as exportRpc
 from . import schedule_callback
 
+logger = logging.getLogger(__name__)
+
 
 # =============================================================================
 #
 # Base class for objects that can accept RPC calls or publish over wslink
 #
 # =============================================================================
 
@@ -110,15 +112,15 @@
     # the RPC methods in the protocol.
     def unregisterLinkProtocol(self, protocol):
         assert isinstance(protocol, LinkProtocol)
         protocol.coreServer = None
         try:
             self.linkProtocols.remove(protocol)
         except ValueError as e:
-            logging.error("Link protocol missing from registered list.")
+            logger.error("Link protocol missing from registered list.")
 
     def getLinkProtocols(self):
         return self.linkProtocols
 
     def updateSecret(self, newSecret):
         self.secret = newSecret
```

### Comparing `wslink-1.9.3/src/wslink.egg-info/PKG-INFO` & `wslink-2.0.0/src/wslink.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslink
-Version: 1.9.3
+Version: 2.0.0
 Summary: Python/JavaScript library for communicating over WebSocket
 Home-page: https://github.com/kitware/wslink
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: BSD-3-Clause
 Keywords: websocket javascript rpc pubsub
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,18 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp<4
+Requires-Dist: msgpack<2,>=1
 Provides-Extra: ssl
+Requires-Dist: cryptography; extra == "ssl"
 
 wslink
 ======
 
 Wslink allows easy, bi-directional communication between a python server and a
 javascript client over a websocket_. The client can make RPC calls to the
 server, and the server can publish messages to topics that the client can
@@ -49,14 +52,24 @@
 
 Get the whole story
 -------------------
 
 This package is just the server side of wslink. See the `github repo`_ for
 the full story - and to contribute or report issues!
 
+Configure from environment variables
+------------------------------------
+
+Those only apply for the Python server and launcher.
+
+* WSLINK_LAUNCHER_GET - If set to 1 this will enable the GET endpoint for session information
+* WSLINK_LAUNCHER_DELETE - If set to 1 this will enable the DELETE endpoint for killing a running session
+* WSLINK_MAX_MSG_SIZE - Number of bytes for a message size (default: 4194304)
+* WSLINK_HEART_BEAT - Number of seconds between heartbeats (default: 30)
+
 License
 -------
 Free to use in open-source and commercial projects, under the BSD-3-Clause license.
 
 .. _github repo: https://github.com/kitware/wslink
 .. _ParaView: https://www.paraview.org/
 .. _VTK: http://www.vtk.org/
```

### Comparing `wslink-1.9.3/src/wslink.egg-info/SOURCES.txt` & `wslink-2.0.0/src/wslink.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/wslink/LICENSE
 src/wslink/__init__.py
+src/wslink/chunking.py
 src/wslink/launcher.py
+src/wslink/protocol.py
 src/wslink/publish.py
 src/wslink/relay.py
 src/wslink/server.py
 src/wslink/ssl_context.py
 src/wslink/uri.py
 src/wslink/websocket.py
 src/wslink.egg-info/PKG-INFO
 src/wslink.egg-info/SOURCES.txt
 src/wslink.egg-info/dependency_links.txt
 src/wslink.egg-info/requires.txt
 src/wslink.egg-info/top_level.txt
 src/wslink/backends/__init__.py
 src/wslink/backends/aiohttp/__init__.py
 src/wslink/backends/aiohttp/launcher.py
-src/wslink/backends/aiohttp/relay.py
+src/wslink/backends/aiohttp/relay.py
+src/wslink/backends/generic/__init__.py
+src/wslink/backends/generic/core.py
+src/wslink/backends/jupyter/__init__.py
+src/wslink/backends/jupyter/core.py
+src/wslink/backends/tornado/__init__.py
+src/wslink/backends/tornado/core.py
```

