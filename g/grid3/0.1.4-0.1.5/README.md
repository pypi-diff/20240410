# Comparing `tmp/grid3-0.1.4.tar.gz` & `tmp/grid3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid3-0.1.4.tar", max compression
+gzip compressed data, was "grid3-0.1.5.tar", max compression
```

## Comparing `grid3-0.1.4.tar` & `grid3-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    11350 2023-10-31 23:30:25.227865 grid3-0.1.4/LICENSE
--rw-r--r--   0        0        0     1598 2023-11-01 20:49:25.182303 grid3-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-03 01:26:02.905821 grid3-0.1.4/grid3/__init__.py
--rw-r--r--   0        0        0     7600 2023-05-05 23:39:20.557684 grid3-0.1.4/grid3/graphql.py
--rw-r--r--   0        0        0     1831 2023-10-31 20:59:05.691085 grid3-0.1.4/grid3/network.py
--rw-r--r--   0        0        0     1919 2023-10-31 21:00:20.491570 grid3-0.1.4/grid3/proxy.py
--rw-r--r--   0        0        0     4492 2023-07-20 03:43:32.243551 grid3-0.1.4/grid3/rmb.py
--rw-r--r--   0        0        0     4216 2023-07-18 23:52:01.722433 grid3-0.1.4/grid3/types.py
--rw-r--r--   0        0        0      436 2023-11-01 23:07:07.976685 grid3-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 grid3-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-10-31 23:30:25.227865 grid3-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1598 2023-11-01 20:49:25.182303 grid3-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 01:26:02.905821 grid3-0.1.5/grid3/__init__.py
+-rw-r--r--   0        0        0     7600 2023-05-05 23:39:20.557684 grid3-0.1.5/grid3/graphql.py
+-rw-r--r--   0        0        0     1916 2024-02-10 08:21:26.935548 grid3-0.1.5/grid3/grid_cli.py
+-rw-r--r--   0        0        0     1831 2023-10-31 20:59:05.691085 grid3-0.1.5/grid3/network.py
+-rw-r--r--   0        0        0     1919 2023-10-31 21:00:20.491570 grid3-0.1.5/grid3/proxy.py
+-rw-r--r--   0        0        0     4739 2024-02-12 23:59:39.914194 grid3-0.1.5/grid3/rmb.py
+-rw-r--r--   0        0        0     5001 2024-04-10 01:35:38.348865 grid3-0.1.5/grid3/tfchain.py
+-rw-r--r--   0        0        0     4216 2023-07-18 23:52:01.722433 grid3-0.1.5/grid3/types.py
+-rw-r--r--   0        0        0      614 2024-04-10 02:14:49.500392 grid3-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 grid3-0.1.5/PKG-INFO
```

### Comparing `grid3-0.1.4/LICENSE` & `grid3-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/README.md` & `grid3-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/grid3/graphql.py` & `grid3-0.1.5/grid3/graphql.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/grid3/network.py` & `grid3-0.1.5/grid3/network.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/grid3/proxy.py` & `grid3-0.1.5/grid3/proxy.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/grid3/rmb.py` & `grid3-0.1.5/grid3/rmb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import redis, json, base64, time, subprocess, socket
+import redis, json, base64, time, subprocess, socket, shutil
 
 class RmbClient:
     """
     A simple wrapper to use the Reliable Message Bus via rmb-peer over Redis. Be sure to start up redis-server and rmb-peer before attempting to use this class.
 
     For more info on RMB and rmb-peer, see: https://github.com/threefoldtech/rmb-rs
     """
@@ -60,15 +60,15 @@
                     'test': 'wss://relay.test.grid.tf:443',
                     'qa': 'wss://relay.qa.grid.tf:443', 
                     'dev': 'wss://relay.dev.grid.tf:443'}
 
     def __init__(self, secret, network='main', peer_logfile='rmb-peer.log', 
                  redis_port=6379, key_type='sr25519', tfchain_url=None, 
                  relay_url=None, redis_url=None, debug=False,
-                 path='./rmb-peer', spawn_redis=False, 
+                 path=None, spawn_redis=False, 
                  redis_logfile='redis.log'):
 
         self.redis_port = redis_port
 
         if spawn_redis:
             if redis_port is None:
                 # We ask the OS for a free port if None is given, then close the socket immediately so we can use it
@@ -93,14 +93,22 @@
             relay_url = self.relay_urls[network]
 
         if redis_url is None:
             if self.redis_port is None:
                 raise Exception('Redis port of None only valid when spawning redis')
             redis_url = 'redis://localhost:' + str(self.redis_port)
 
+        if path is None:
+            for p in ['rmb-peer', './rmb-peer']:
+                if shutil.which(p):
+                    path = p
+
+            if path is None:
+                raise Exception('rmb-peer binary not found')
+                
         call = [path]
 
         if debug:
             call.append('-d')
 
         call.extend(['-s', tfchain_url, '--relay', relay_url, 
                      '-r', redis_url, '--mnemonic', secret, '-k', key_type])
```

### Comparing `grid3-0.1.4/grid3/types.py` & `grid3-0.1.5/grid3/types.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.4/PKG-INFO` & `grid3-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: grid3
-Version: 0.1.4
+Version: 0.1.5
 Summary: Modules for interacting with ThreeFold Grid v3.
 License: Apache-2.0
 Author: Scott Yeager
 Author-email: scott@threefold.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: rmb
+Provides-Extra: tfchain
 Requires-Dist: gql[requests] (>=3.4.1,<4.0.0)
+Requires-Dist: redis (>=5.0.0,<6.0.0) ; extra == "rmb"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: substrate-interface (>=1.7.7,<2.0.0) ; extra == "tfchain"
 Description-Content-Type: text/markdown
 
 # Grid3.py
 
 This is a collection of Python modules for working with ThreeFold Grid v3. It's designed foremostly for interactive use on the REPL and joyful scripting. We value conciseness and trying to do what you *meant*, even at the expense of a few extra CPU cycles.
 
 If you're looking for a Grid v3 SDK for writing efficient and maintainable code bases, check out [Go](https://github.com/threefoldtech/tfgrid-sdk-go). For code that must execute in the user's browser, see [Typescript](https://github.com/threefoldtech/tfgrid-sdk-ts).
```

