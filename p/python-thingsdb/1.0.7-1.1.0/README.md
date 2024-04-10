# Comparing `tmp/python-thingsdb-1.0.7.tar.gz` & `tmp/python-thingsdb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-thingsdb-1.0.7.tar", last modified: Fri Jan 26 11:48:33 2024, max compression
+gzip compressed data, was "python-thingsdb-1.1.0.tar", last modified: Wed Apr 10 11:13:21 2024, max compression
```

## Comparing `python-thingsdb-1.0.7.tar` & `python-thingsdb-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.892247 python-thingsdb-1.0.7/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.892247 python-thingsdb-1.0.7/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      679 2024-01-26 11:10:22.000000 python-thingsdb-1.0.7/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)      119 2021-09-14 09:36:12.000000 python-thingsdb-1.0.7/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)     1066 2019-12-20 12:14:05.000000 python-thingsdb-1.0.7/LICENSE
--rw-r--r--   0 joente    (1000) joente    (1000)    16641 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)    15886 2022-11-11 21:53:28.000000 python-thingsdb-1.0.7/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.892247 python-thingsdb-1.0.7/examples/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.892247 python-thingsdb-1.0.7/examples/bookstore/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3377 2022-02-23 09:48:18.000000 python-thingsdb-1.0.7/examples/bookstore/webserver.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/python_thingsdb.egg-info/
--rw-r--r--   0 joente    (1000) joente    (1000)    16641 2024-01-26 11:48:33.000000 python-thingsdb-1.0.7/python_thingsdb.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      741 2024-01-26 11:48:33.000000 python-thingsdb-1.0.7/python_thingsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-01-26 11:48:33.000000 python-thingsdb-1.0.7/python_thingsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       20 2024-01-26 11:48:33.000000 python-thingsdb-1.0.7/python_thingsdb.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        9 2024-01-26 11:48:33.000000 python-thingsdb-1.0.7/python_thingsdb.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       27 2019-12-17 14:25:00.000000 python-thingsdb-1.0.7/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2023-02-10 12:47:09.000000 python-thingsdb-1.0.7/setup.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      800 2022-11-11 21:22:06.000000 python-thingsdb-1.0.7/test_thingsdb.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.892247 python-thingsdb-1.0.7/thingsdb/
--rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.0.7/thingsdb/__init__.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/thingsdb/client/
--rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.0.7/thingsdb/client/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    16343 2024-01-26 11:10:22.000000 python-thingsdb-1.0.7/thingsdb/client/buildin.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    24589 2023-07-20 17:59:07.000000 python-thingsdb-1.0.7/thingsdb/client/client.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1851 2023-07-20 17:58:48.000000 python-thingsdb-1.0.7/thingsdb/client/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8317 2021-09-22 12:02:58.000000 python-thingsdb-1.0.7/thingsdb/client/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.0.7/thingsdb/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/thingsdb/room/
--rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.0.7/thingsdb/room/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.0.7/thingsdb/room/event.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.0.7/thingsdb/room/room.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     8704 2023-07-20 17:58:48.000000 python-thingsdb-1.0.7/thingsdb/room/roombase.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-01-26 11:48:33.896247 python-thingsdb-1.0.7/thingsdb/util/
--rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.0.7/thingsdb/util/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.0.7/thingsdb/util/access.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.0.7/thingsdb/util/cleancode.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.0.7/thingsdb/util/cnscope.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      501 2023-07-20 17:58:21.000000 python-thingsdb-1.0.7/thingsdb/util/id.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2024-01-26 11:10:45.000000 python-thingsdb-1.0.7/thingsdb/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      679 2024-01-26 11:10:22.000000 python-thingsdb-1.1.0/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)      119 2021-09-14 09:36:12.000000 python-thingsdb-1.1.0/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1066 2019-12-20 12:14:05.000000 python-thingsdb-1.1.0/LICENSE
+-rw-r--r--   0 joente    (1000) joente    (1000)    18778 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)    18022 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/examples/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/examples/bookstore/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3377 2022-02-23 09:48:18.000000 python-thingsdb-1.1.0/examples/bookstore/webserver.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/python_thingsdb.egg-info/
+-rw-r--r--   0 joente    (1000) joente    (1000)    18778 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      741 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       20 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        9 2024-04-10 11:13:21.000000 python-thingsdb-1.1.0/python_thingsdb.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       59 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2002 2023-02-10 12:47:09.000000 python-thingsdb-1.1.0/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      776 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/test_thingsdb.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       33 2021-08-06 17:41:51.000000 python-thingsdb-1.1.0/thingsdb/__init__.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/client/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       70 2021-09-22 12:02:58.000000 python-thingsdb-1.1.0/thingsdb/client/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    16343 2024-01-26 11:10:22.000000 python-thingsdb-1.1.0/thingsdb/client/buildin.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    25656 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/client.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2247 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    11933 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/client/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1668 2021-01-25 17:31:46.000000 python-thingsdb-1.1.0/thingsdb/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.567901 python-thingsdb-1.1.0/thingsdb/room/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       48 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/room/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       93 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/room/event.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1797 2021-12-08 10:35:31.000000 python-thingsdb-1.1.0/thingsdb/room/room.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8704 2023-07-20 17:58:48.000000 python-thingsdb-1.1.0/thingsdb/room/roombase.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2024-04-10 11:13:21.571901 python-thingsdb-1.1.0/thingsdb/util/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       90 2021-12-07 13:10:39.000000 python-thingsdb-1.1.0/thingsdb/util/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      141 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/util/access.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      303 2021-12-07 13:10:39.000000 python-thingsdb-1.1.0/thingsdb/util/cleancode.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      699 2021-09-10 14:49:48.000000 python-thingsdb-1.1.0/thingsdb/util/cnscope.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      501 2023-07-20 17:58:21.000000 python-thingsdb-1.1.0/thingsdb/util/id.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2024-04-10 11:12:35.000000 python-thingsdb-1.1.0/thingsdb/version.py
```

### Comparing `python-thingsdb-1.0.7/.github/workflows/ci.yml` & `python-thingsdb-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/LICENSE` & `python-thingsdb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/PKG-INFO` & `python-thingsdb-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-thingsdb
-Version: 1.0.7
+Version: 1.1.0
 Summary: ThingsDB Connector
 Home-page: https://github.com/thingsdb/python-thingsdb
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: MIT
 Keywords: database connector
 Classifier: Development Status :: 4 - Beta
@@ -30,33 +30,36 @@
 ---------------------------------------
 
   * [Installation](#installation)
   * [Quick usage](#quick-usage)
   * [Client](#client)
     * [authenticate](#authenticate)
     * [close](#close)
+    * [close_and_wait](#close_and_wait)
     * [connect](#connect)
     * [connect_pool](#connect_pool)
     * [get_default_scope](#get_default_scope)
     * [get_event_loop](#get_event_loop)
     * [get_rooms](#get_rooms)
     * [is_connected](#is_connected)
+    * [is_websocket](#is_websocket)
     * [query](#query)
     * [reconnect](#reconnect)
     * [run](#run)
     * [set_default_scope](#set_default_scope)
     * [wait_closed](#wait_closed)
   * [Room](#room)
     * [methods](#room-methods)
     * [properties](#room-properties)
     * [join](#join)
     * [leave](#leave)
     * [emit](#emit)
     * [no_join](#no_join)
   * [Failed packages](#failed-packages)
+  * [WebSockets](#websockets)
 ---------------------------------------
 
 ## Installation
 
 Just use pip:
 
 ```
@@ -89,16 +92,15 @@
         # perform the hello world code...
         print(await client.query('''
             "Hello World!";
         ''')
 
     finally:
         # the will close the client in a nice way
-        client.close()
-        await client.wait_closed()
+        await client.close_and_wait()
 
 # run the hello world example
 asyncio.get_event_loop().run_until_complete(hello_world())
 ```
 
 ## Client
 
@@ -166,14 +168,24 @@
 
 Close the ThingsDB connection.
 
 This method will return immediately so the connection may not be
 closed yet after a call to `close()`. Use the [wait_closed()](#wait_closed) method
 after calling this method if this is required.
 
+### close_and_wait
+
+```python
+async Client().close_and_wait() -> None
+```
+
+Close and wait for the the connection to be closed.
+
+This is equivalent of combining [close()](#close)) and [wait_closed()](#wait_closed).
+
 ### connect
 
 ```python
 Client().connect(
     host: str,
     port: int = 9200,
     timeout: Optional[int] = 5
@@ -185,19 +197,20 @@
 This method will *only* create a connection, so the connection is not
 authenticated yet. Use the [authenticate(..)](#authenticate) method after creating a
 connection before using the connection.
 
 #### Args
 
 - *host (str)*:
-    A hostname, IP address, FQDN to connect to.
+    A hostname, IP address, FQDN or URI _(for WebSockets)_ to connect to.
 - *port (int, optional)*:
     Integer value between 0 and 65535 and should be the port number
     where a ThingsDB node is listening to for client connections.
-    Defaults to 9200.
+    Defaults to 9200. For WebSocket connections the port must be
+    provided with the URI _(see host argument)_.
 - *timeout (int, optional)*:
     Can be be used to control the maximum time the client will
     attempt to create a connection. The timeout may be set to
     `None` in which case the client will wait forever on a
     response. Defaults to 5.
 
 ### Returns
@@ -225,25 +238,26 @@
 automatically authenticate so the connection pool requires credentials
 to perform the authentication.
 
 #### Examples
 
 ```python
 await connect_pool([
-    'node01.local',             # address as string
-    'node02.local',             # port will default to 9200
-    ('node03.local', 9201),     # ..or with an explicit port
+    'node01.local',             # address or WebSocket URI as string
+    'node02.local',             # port will default to 9200 or ignored for URI
+    ('node03.local', 9201),     # ..or with an explicit port (ignored for URI)
 ], "admin", "pass")
 ```
 
 #### Args
 
 - *pool (list of addresses)*:
     Should be an iterable with node address strings, or tuples
-    with `address` and `port` combinations in a tuple or list.
+    with `address` and `port` combinations in a tuple or list. For WebSockets,
+    the address must be an URI with the port included. (e.g: `"ws://host:9270"`)
 - *\*auth (str or (str, str))*:
     Argument `auth` can be be either a string with a token or a
     tuple with username and password. (the latter may be provided
     as two separate arguments
 
 ### Returns
 
@@ -300,14 +314,26 @@
 ```
 
 Can be used to check if the client is connected.
 
 #### Returns
 `True` when the client is connected else `False`.
 
+
+### is_websocket
+
+```python
+Client().is_websocket() -> bool
+```
+
+Can be used to check if the client is using a WebSocket connection.
+
+#### Returns
+`True` when the client is connected else `False`.
+
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
@@ -613,7 +639,56 @@
 from thingsdb.client import set_package_fail_file
 
 set_package_fail_file('/tmp/thingsdb-invalid-data.mp')
 
 # When a package is received which fails to unpack, the data from this package
 # will be stored to file.
 ```
+
+
+## WebSockets
+
+Since ThingsDB 1.6 has received WebSocket support. The Python client is able to use the WebSockets protocol by providing the `host` as URI.
+For WebSocket connections,the `port` argument will be ignored and must be specified with the URI instead.
+
+Default the `websockets` package is **not included** when installing this connector.
+
+If you want to use WebSockets, make sure to install the package:
+
+```
+pip install websockets
+```
+
+For example:
+
+```python
+import asyncio
+from thingsdb.client import Client
+
+async def hello_world():
+    client = Client()
+
+    # replace `ws://localhost:9270` with your URI
+    await client.connect('ws://localhost:9270')
+
+    # for a secure connection, use wss:// and provide an SSL context, example:
+    # (ssl can be set either to True or False, or an SSLContext)
+    #
+    #   await client.connect('wss://localhost:9270', ssl=True)
+
+    try:
+        # replace `admin` and `pass` with your username and password
+        # or use a valid token string
+        await client.authenticate('admin', 'pass')
+
+        # perform the hello world code...
+        print(await client.query('''
+            "Hello World!";
+        ''')
+
+    finally:
+        # the will close the client in a nice way
+        await client.close_and_wait()
+
+# run the hello world example
+asyncio.get_event_loop().run_until_complete(hello_world())
+```
```

### Comparing `python-thingsdb-1.0.7/README.md` & `python-thingsdb-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 ---------------------------------------
 
   * [Installation](#installation)
   * [Quick usage](#quick-usage)
   * [Client](#client)
     * [authenticate](#authenticate)
     * [close](#close)
+    * [close_and_wait](#close_and_wait)
     * [connect](#connect)
     * [connect_pool](#connect_pool)
     * [get_default_scope](#get_default_scope)
     * [get_event_loop](#get_event_loop)
     * [get_rooms](#get_rooms)
     * [is_connected](#is_connected)
+    * [is_websocket](#is_websocket)
     * [query](#query)
     * [reconnect](#reconnect)
     * [run](#run)
     * [set_default_scope](#set_default_scope)
     * [wait_closed](#wait_closed)
   * [Room](#room)
     * [methods](#room-methods)
     * [properties](#room-properties)
     * [join](#join)
     * [leave](#leave)
     * [emit](#emit)
     * [no_join](#no_join)
   * [Failed packages](#failed-packages)
+  * [WebSockets](#websockets)
 ---------------------------------------
 
 ## Installation
 
 Just use pip:
 
 ```
@@ -67,16 +70,15 @@
         # perform the hello world code...
         print(await client.query('''
             "Hello World!";
         ''')
 
     finally:
         # the will close the client in a nice way
-        client.close()
-        await client.wait_closed()
+        await client.close_and_wait()
 
 # run the hello world example
 asyncio.get_event_loop().run_until_complete(hello_world())
 ```
 
 ## Client
 
@@ -144,14 +146,24 @@
 
 Close the ThingsDB connection.
 
 This method will return immediately so the connection may not be
 closed yet after a call to `close()`. Use the [wait_closed()](#wait_closed) method
 after calling this method if this is required.
 
+### close_and_wait
+
+```python
+async Client().close_and_wait() -> None
+```
+
+Close and wait for the the connection to be closed.
+
+This is equivalent of combining [close()](#close)) and [wait_closed()](#wait_closed).
+
 ### connect
 
 ```python
 Client().connect(
     host: str,
     port: int = 9200,
     timeout: Optional[int] = 5
@@ -163,19 +175,20 @@
 This method will *only* create a connection, so the connection is not
 authenticated yet. Use the [authenticate(..)](#authenticate) method after creating a
 connection before using the connection.
 
 #### Args
 
 - *host (str)*:
-    A hostname, IP address, FQDN to connect to.
+    A hostname, IP address, FQDN or URI _(for WebSockets)_ to connect to.
 - *port (int, optional)*:
     Integer value between 0 and 65535 and should be the port number
     where a ThingsDB node is listening to for client connections.
-    Defaults to 9200.
+    Defaults to 9200. For WebSocket connections the port must be
+    provided with the URI _(see host argument)_.
 - *timeout (int, optional)*:
     Can be be used to control the maximum time the client will
     attempt to create a connection. The timeout may be set to
     `None` in which case the client will wait forever on a
     response. Defaults to 5.
 
 ### Returns
@@ -203,25 +216,26 @@
 automatically authenticate so the connection pool requires credentials
 to perform the authentication.
 
 #### Examples
 
 ```python
 await connect_pool([
-    'node01.local',             # address as string
-    'node02.local',             # port will default to 9200
-    ('node03.local', 9201),     # ..or with an explicit port
+    'node01.local',             # address or WebSocket URI as string
+    'node02.local',             # port will default to 9200 or ignored for URI
+    ('node03.local', 9201),     # ..or with an explicit port (ignored for URI)
 ], "admin", "pass")
 ```
 
 #### Args
 
 - *pool (list of addresses)*:
     Should be an iterable with node address strings, or tuples
-    with `address` and `port` combinations in a tuple or list.
+    with `address` and `port` combinations in a tuple or list. For WebSockets,
+    the address must be an URI with the port included. (e.g: `"ws://host:9270"`)
 - *\*auth (str or (str, str))*:
     Argument `auth` can be be either a string with a token or a
     tuple with username and password. (the latter may be provided
     as two separate arguments
 
 ### Returns
 
@@ -278,14 +292,26 @@
 ```
 
 Can be used to check if the client is connected.
 
 #### Returns
 `True` when the client is connected else `False`.
 
+
+### is_websocket
+
+```python
+Client().is_websocket() -> bool
+```
+
+Can be used to check if the client is using a WebSocket connection.
+
+#### Returns
+`True` when the client is connected else `False`.
+
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
@@ -591,7 +617,56 @@
 from thingsdb.client import set_package_fail_file
 
 set_package_fail_file('/tmp/thingsdb-invalid-data.mp')
 
 # When a package is received which fails to unpack, the data from this package
 # will be stored to file.
 ```
+
+
+## WebSockets
+
+Since ThingsDB 1.6 has received WebSocket support. The Python client is able to use the WebSockets protocol by providing the `host` as URI.
+For WebSocket connections,the `port` argument will be ignored and must be specified with the URI instead.
+
+Default the `websockets` package is **not included** when installing this connector.
+
+If you want to use WebSockets, make sure to install the package:
+
+```
+pip install websockets
+```
+
+For example:
+
+```python
+import asyncio
+from thingsdb.client import Client
+
+async def hello_world():
+    client = Client()
+
+    # replace `ws://localhost:9270` with your URI
+    await client.connect('ws://localhost:9270')
+
+    # for a secure connection, use wss:// and provide an SSL context, example:
+    # (ssl can be set either to True or False, or an SSLContext)
+    #
+    #   await client.connect('wss://localhost:9270', ssl=True)
+
+    try:
+        # replace `admin` and `pass` with your username and password
+        # or use a valid token string
+        await client.authenticate('admin', 'pass')
+
+        # perform the hello world code...
+        print(await client.query('''
+            "Hello World!";
+        ''')
+
+    finally:
+        # the will close the client in a nice way
+        await client.close_and_wait()
+
+# run the hello world example
+asyncio.get_event_loop().run_until_complete(hello_world())
+```
```

### Comparing `python-thingsdb-1.0.7/examples/bookstore/webserver.py` & `python-thingsdb-1.1.0/examples/bookstore/webserver.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/python_thingsdb.egg-info/PKG-INFO` & `python-thingsdb-1.1.0/python_thingsdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-thingsdb
-Version: 1.0.7
+Version: 1.1.0
 Summary: ThingsDB Connector
 Home-page: https://github.com/thingsdb/python-thingsdb
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: MIT
 Keywords: database connector
 Classifier: Development Status :: 4 - Beta
@@ -30,33 +30,36 @@
 ---------------------------------------
 
   * [Installation](#installation)
   * [Quick usage](#quick-usage)
   * [Client](#client)
     * [authenticate](#authenticate)
     * [close](#close)
+    * [close_and_wait](#close_and_wait)
     * [connect](#connect)
     * [connect_pool](#connect_pool)
     * [get_default_scope](#get_default_scope)
     * [get_event_loop](#get_event_loop)
     * [get_rooms](#get_rooms)
     * [is_connected](#is_connected)
+    * [is_websocket](#is_websocket)
     * [query](#query)
     * [reconnect](#reconnect)
     * [run](#run)
     * [set_default_scope](#set_default_scope)
     * [wait_closed](#wait_closed)
   * [Room](#room)
     * [methods](#room-methods)
     * [properties](#room-properties)
     * [join](#join)
     * [leave](#leave)
     * [emit](#emit)
     * [no_join](#no_join)
   * [Failed packages](#failed-packages)
+  * [WebSockets](#websockets)
 ---------------------------------------
 
 ## Installation
 
 Just use pip:
 
 ```
@@ -89,16 +92,15 @@
         # perform the hello world code...
         print(await client.query('''
             "Hello World!";
         ''')
 
     finally:
         # the will close the client in a nice way
-        client.close()
-        await client.wait_closed()
+        await client.close_and_wait()
 
 # run the hello world example
 asyncio.get_event_loop().run_until_complete(hello_world())
 ```
 
 ## Client
 
@@ -166,14 +168,24 @@
 
 Close the ThingsDB connection.
 
 This method will return immediately so the connection may not be
 closed yet after a call to `close()`. Use the [wait_closed()](#wait_closed) method
 after calling this method if this is required.
 
+### close_and_wait
+
+```python
+async Client().close_and_wait() -> None
+```
+
+Close and wait for the the connection to be closed.
+
+This is equivalent of combining [close()](#close)) and [wait_closed()](#wait_closed).
+
 ### connect
 
 ```python
 Client().connect(
     host: str,
     port: int = 9200,
     timeout: Optional[int] = 5
@@ -185,19 +197,20 @@
 This method will *only* create a connection, so the connection is not
 authenticated yet. Use the [authenticate(..)](#authenticate) method after creating a
 connection before using the connection.
 
 #### Args
 
 - *host (str)*:
-    A hostname, IP address, FQDN to connect to.
+    A hostname, IP address, FQDN or URI _(for WebSockets)_ to connect to.
 - *port (int, optional)*:
     Integer value between 0 and 65535 and should be the port number
     where a ThingsDB node is listening to for client connections.
-    Defaults to 9200.
+    Defaults to 9200. For WebSocket connections the port must be
+    provided with the URI _(see host argument)_.
 - *timeout (int, optional)*:
     Can be be used to control the maximum time the client will
     attempt to create a connection. The timeout may be set to
     `None` in which case the client will wait forever on a
     response. Defaults to 5.
 
 ### Returns
@@ -225,25 +238,26 @@
 automatically authenticate so the connection pool requires credentials
 to perform the authentication.
 
 #### Examples
 
 ```python
 await connect_pool([
-    'node01.local',             # address as string
-    'node02.local',             # port will default to 9200
-    ('node03.local', 9201),     # ..or with an explicit port
+    'node01.local',             # address or WebSocket URI as string
+    'node02.local',             # port will default to 9200 or ignored for URI
+    ('node03.local', 9201),     # ..or with an explicit port (ignored for URI)
 ], "admin", "pass")
 ```
 
 #### Args
 
 - *pool (list of addresses)*:
     Should be an iterable with node address strings, or tuples
-    with `address` and `port` combinations in a tuple or list.
+    with `address` and `port` combinations in a tuple or list. For WebSockets,
+    the address must be an URI with the port included. (e.g: `"ws://host:9270"`)
 - *\*auth (str or (str, str))*:
     Argument `auth` can be be either a string with a token or a
     tuple with username and password. (the latter may be provided
     as two separate arguments
 
 ### Returns
 
@@ -300,14 +314,26 @@
 ```
 
 Can be used to check if the client is connected.
 
 #### Returns
 `True` when the client is connected else `False`.
 
+
+### is_websocket
+
+```python
+Client().is_websocket() -> bool
+```
+
+Can be used to check if the client is using a WebSocket connection.
+
+#### Returns
+`True` when the client is connected else `False`.
+
 ### query
 
 ```python
 Client().query(
         code: str,
         scope: Optional[str] = None,
         timeout: Optional[int] = None,
@@ -613,7 +639,56 @@
 from thingsdb.client import set_package_fail_file
 
 set_package_fail_file('/tmp/thingsdb-invalid-data.mp')
 
 # When a package is received which fails to unpack, the data from this package
 # will be stored to file.
 ```
+
+
+## WebSockets
+
+Since ThingsDB 1.6 has received WebSocket support. The Python client is able to use the WebSockets protocol by providing the `host` as URI.
+For WebSocket connections,the `port` argument will be ignored and must be specified with the URI instead.
+
+Default the `websockets` package is **not included** when installing this connector.
+
+If you want to use WebSockets, make sure to install the package:
+
+```
+pip install websockets
+```
+
+For example:
+
+```python
+import asyncio
+from thingsdb.client import Client
+
+async def hello_world():
+    client = Client()
+
+    # replace `ws://localhost:9270` with your URI
+    await client.connect('ws://localhost:9270')
+
+    # for a secure connection, use wss:// and provide an SSL context, example:
+    # (ssl can be set either to True or False, or an SSLContext)
+    #
+    #   await client.connect('wss://localhost:9270', ssl=True)
+
+    try:
+        # replace `admin` and `pass` with your username and password
+        # or use a valid token string
+        await client.authenticate('admin', 'pass')
+
+        # perform the hello world code...
+        print(await client.query('''
+            "Hello World!";
+        ''')
+
+    finally:
+        # the will close the client in a nice way
+        await client.close_and_wait()
+
+# run the hello world example
+asyncio.get_event_loop().run_until_complete(hello_world())
+```
```

### Comparing `python-thingsdb-1.0.7/python_thingsdb.egg-info/SOURCES.txt` & `python-thingsdb-1.1.0/python_thingsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/setup.py` & `python-thingsdb-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/test_thingsdb.py` & `python-thingsdb-1.1.0/test_thingsdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,15 @@
             data = await client.query(
                 code='.greetings[index];',
                 index=1,
                 scope='//Doc')
             self.assertEqual(data, want)
 
         finally:
-            client.close()
-            await client.wait_closed()
+            await client.close_and_wait()
 
     def test_playground(self):
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self.async_test_playground())
 
 
 TestPlayground().test_playground()
```

### Comparing `python-thingsdb-1.0.7/thingsdb/client/buildin.py` & `python-thingsdb-1.1.0/thingsdb/client/buildin.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/thingsdb/client/client.py` & `python-thingsdb-1.1.0/thingsdb/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 import ssl
 from collections import defaultdict
 from ssl import SSLContext, PROTOCOL_TLS
 from typing import Optional, Union, Any
 from concurrent.futures import CancelledError
 from .buildin import Buildin
-from .protocol import Proto, Protocol
+from .protocol import Proto, Protocol, ProtocolWS
 from ..exceptions import NodeError, AuthError
 from ..util import strip_code
 
 
 class Client(Buildin):
 
     MAX_RECONNECT_WAIT_TIME = 60
@@ -81,15 +81,15 @@
 
     def is_connected(self) -> bool:
         """Can be used to check if the client is connected.
 
         Returns:
             bool: `True` when the client is connected else `False`.
         """
-        return bool(self._protocol and self._protocol.transport)
+        return bool(self._protocol and self._protocol.is_connected())
 
     def set_default_scope(self, scope: str) -> None:
         """Set the default scope.
 
         Can be used to change the default scope which is initially set to `@t`.
 
         Args:
@@ -115,30 +115,30 @@
     def close(self) -> None:
         """Close the ThingsDB connection.
 
         This method will return immediately so the connection may not be
         closed yet after a call to `close()`. Use the `wait_closed()` method
         after calling this method if this is required.
         """
-        if self._protocol and self._protocol.transport:
-            self._reconnect = False
-            self._protocol.transport.close()
+        self._reconnect = False
+        if self._protocol:
+            self._protocol.close()
 
     def connection_info(self) -> str:
         """Returns the current connection info as a string.
 
         Even with a connection pool, the client has still one active node
         connection at the time, and info for this active connection will be
         returned.
 
         example: "node0.local:9200"
         """
         if not self.is_connected():
             return 'disconnected'
-        socket = self._protocol.transport.get_extra_info('socket', None)
+        socket = self._protocol.info()
         if socket is None:
             return 'unknown_addr'
         addr, port = socket.getpeername()[:2]
         return f'{addr}:{port}'
 
     def connect_pool(
             self,
@@ -201,19 +201,21 @@
 
         This method will *only* create a connection, so the connection is not
         authenticated yet. Use the `authenticate(..)` method after creating a
         connection before using the connection.
 
         Args:
             host (str):
-                A hostname, IP address, FQDN to connect to.
+                A hostname, IP address, FQDN or URI (for WebSockets) to connect
+                to.
             port (int, optional):
                 Integer value between 0 and 65535 and should be the port number
                 where a ThingsDB node is listening to for client connections.
-                Defaults to 9200.
+                Defaults to 9200. For WebSocket connections the port must be
+                provided with the URI (see host argument).
             timeout (int, optional):
                 Can be be used to control the maximum time the client will
                 attempt to create a connection. The timeout may be set to
                 `None` in which case the client will wait forever on a
                 response. Defaults to 5.
 
         Returns:
@@ -246,16 +248,27 @@
 
     async def wait_closed(self) -> None:
         """Wait for a connection to close.
 
         Can be used after calling the `close()` method to determine when the
         connection is actually closed.
         """
-        if self._protocol and self._protocol.close_future:
-            await self._protocol.close_future
+        if self._protocol and self._protocol.is_closing():
+            await self._protocol.wait_closed()
+
+    async def close_and_wait(self) -> None:
+        """Close and wait for the connection to be closed.
+
+        This is equivalent to calling close() and await wait_closed()
+        """
+        if self._protocol:
+            await self._protocol.close_and_wait()
+
+    def is_websocket(self) -> bool:
+        return self._protocol.__class__ is ProtocolWS
 
     async def authenticate(
             self,
             *auth: Union[str, tuple],
             timeout: Optional[int] = 5
     ) -> None:
         """Authenticate a ThingsDB connection.
@@ -534,28 +547,40 @@
             isinstance(auth, str)
         )), (
             'expecting the authentication argument to be a "token-string" '
             'or a tuple like ("username", "password").'
         )
         return auth
 
+    @staticmethod
+    def _is_websocket_host(host):
+        return host.startswith('ws://') or host.startswith('wss://')
+
     async def _connect(self, timeout=5):
         host, port = self._pool[self._pool_idx]
         try:
-            conn = self._loop.create_connection(
-                lambda: Protocol(
+            if self._is_websocket_host(host):
+                conn = ProtocolWS(
                     on_connection_lost=self._on_connection_lost,
-                    on_event=self._on_event,
-                    loop=self._loop),
-                host=host,
-                port=port,
-                ssl=self._ssl)
-            _, self._protocol = await asyncio.wait_for(
-                conn,
-                timeout=timeout)
+                    on_event=self._on_event).connect(uri=host, ssl=self._ssl)
+                self._protocol = await asyncio.wait_for(
+                    conn,
+                    timeout=timeout)
+            else:
+                conn = self._loop.create_connection(
+                    lambda: Protocol(
+                        on_connection_lost=self._on_connection_lost,
+                        on_event=self._on_event,
+                        loop=self._loop),
+                    host=host,
+                    port=port,
+                    ssl=self._ssl)
+                _, self._protocol = await asyncio.wait_for(
+                    conn,
+                    timeout=timeout)
         finally:
             self._pool_idx += 1
             self._pool_idx %= len(self._pool)
 
     async def _on_room(self, room_id, pkg):
         async with self._rooms_lock:
             try:
@@ -610,23 +635,25 @@
                 host, port = self._pool[self._pool_idx]
                 try:
                     await self._connect(timeout=timeout)
                     await self._ping(timeout=2)
                     await self._authenticate(timeout=5)
                     await self._rejoin()
                 except Exception as e:
+                    name = host if self._is_websocket_host(host) else \
+                        f'{host}:{port}'
                     logging.error(
-                        f'Connecting to {host}:{port} failed: '
+                        f'Connecting to {name} failed: '
                         f'{e}({e.__class__.__name__}), '
                         f'Try next connect in {wait_time} seconds'
                     )
                 else:
-                    if protocol and protocol.transport:
+                    if protocol and protocol.is_connected():
                         # make sure the `old` connection will be dropped
-                        self._loop.call_later(10.0, protocol.transport.close)
+                        self._loop.call_later(10.0, protocol.close)
                     break
 
                 await asyncio.sleep(wait_time)
                 wait_time *= 2
                 wait_time = min(wait_time, self.MAX_RECONNECT_WAIT_TIME)
                 timeout = min(timeout+1, self.MAX_RECONNECT_TIMEOUT)
         finally:
```

### Comparing `python-thingsdb-1.0.7/thingsdb/client/package.py` & `python-thingsdb-1.1.0/thingsdb/client/package.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,30 +29,43 @@
 
     def __init__(self, barray: bytearray) -> None:
         self.length, self.pid, self.tp, self.checkbit = \
             self.__class__.st_package.unpack_from(barray, offset=0)
         self.total = self.__class__.st_package.size + self.length
         self.data = None
 
+    def _handle_fail_file(self, message: bytes):
+        if _fail_file:
+            try:
+                with open(_fail_file, 'wb') as f:
+                    f.write(
+                        message[self.__class__.st_package.size:self.total])
+            except Exception:
+                logging.exception('')
+            else:
+                logging.warning(
+                    f'Wrote the content from {self} to `{_fail_file}`')
+
     def extract_data_from(self, barray: bytearray) -> None:
         try:
             self.data = msgpack.unpackb(
                 barray[self.__class__.st_package.size:self.total],
                 raw=False) \
                 if self.length else None
         except Exception as e:
-            if _fail_file:
-                try:
-                    with open(_fail_file, 'wb') as f:
-                        f.write(
-                            barray[self.__class__.st_package.size:self.total])
-                except Exception:
-                    logging.exception('')
-                else:
-                    logging.warning(
-                        f'Wrote the content from {self} to `{_fail_file}`')
+            self._handle_fail_file(barray)
             raise e
         finally:
             del barray[:self.total]
 
+    def read_data_from(self, message: bytes) -> None:
+        try:
+            self.data = msgpack.unpackb(
+                message[self.__class__.st_package.size:self.total],
+                raw=False) \
+                if self.length else None
+        except Exception as e:
+            self._handle_fail_file(message)
+            raise e
+
     def __repr__(self) -> str:
         return '<id: {0.pid} size: {0.length} tp: {0.tp}>'.format(self)
```

### Comparing `python-thingsdb-1.0.7/thingsdb/exceptions.py` & `python-thingsdb-1.1.0/thingsdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/thingsdb/room/room.py` & `python-thingsdb-1.1.0/thingsdb/room/room.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/thingsdb/room/roombase.py` & `python-thingsdb-1.1.0/thingsdb/room/roombase.py`

 * *Files identical despite different names*

### Comparing `python-thingsdb-1.0.7/thingsdb/util/cnscope.py` & `python-thingsdb-1.1.0/thingsdb/util/cnscope.py`

 * *Files identical despite different names*

