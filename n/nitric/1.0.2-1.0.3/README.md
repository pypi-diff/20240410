# Comparing `tmp/nitric-1.0.2.tar.gz` & `tmp/nitric-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-1.0.2.tar", last modified: Wed Apr  3 23:01:30 2024, max compression
+gzip compressed data, was "nitric-1.0.3.tar", last modified: Wed Apr 10 07:09:14 2024, max compression
```

## Comparing `nitric-1.0.2.tar` & `nitric-1.0.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.455870 nitric-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 23:01:30.455870 nitric-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 23:00:51.000000 nitric-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/bidi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/KeyValue/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/KeyValue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/KeyValue/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/KeyValue/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/apis/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/apis/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/deployments/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/deployments/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/http/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/http/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/http/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/kvstore/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/kvstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/kvstore/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/kvstore/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/queues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/queues/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/queues/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/resources/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/schedules/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/schedules/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/secrets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/secrets/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/topics/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/topics/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/websockets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.451870 nitric-1.0.2/nitric/proto/websockets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/proto/websockets/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:00:51.000000 nitric-1.0.2/nitric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.455870 nitric-1.0.2/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/resources/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-03 23:01:26.000000 nitric-1.0.2/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:01:30.447870 nitric-1.0.2/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 23:01:30.000000 nitric-1.0.2/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 23:00:51.000000 nitric-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:01:30.455870 nitric-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 23:00:51.000000 nitric-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 07:09:14.691824 nitric-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-10 07:08:34.000000 nitric-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/bidi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/KeyValue/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/KeyValue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/KeyValue/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/KeyValue/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/apis/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/apis/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/deployments/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/deployments/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/http/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/http/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/kvstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/kvstore/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/kvstore/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/queues/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/queues/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/queues/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/resources/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/schedules/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/schedules/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/secrets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/secrets/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/topics/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/websockets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/websockets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/websockets/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:08:34.000000 nitric-1.0.3/nitric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 07:08:34.000000 nitric-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:09:14.691824 nitric-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-10 07:08:34.000000 nitric-1.0.3/setup.py
```

### Comparing `nitric-1.0.2/PKG-INFO` & `nitric-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -22,21 +22,21 @@
 </h2>
 
 <p align="center">
   <a href="https://actions-badge.atrox.dev/nitrictech/python-sdk/goto?ref=main"><img alt="Build Status" src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fnitrictech%2Fpython-sdk%2Fbadge%3Fref%3Dmain&style=for-the-badge" /></a>
   <a href="https://codecov.io/gh/nitrictech/python-sdk">
     <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/nitrictech/python-sdk?style=for-the-badge&token=SBFRNSZ4ZF">
   </a>
-  <a href="https://npmjs.org/package/@nitric/sdk">
+  <a href="https://pypi.org/project/nitric">
     <img alt="Version" src="https://img.shields.io/pypi/v/nitric?style=for-the-badge">
   </a>
   <a href="https://pypi.org/project/nitric">
     <img alt="Downloads/week" src="https://img.shields.io/pypi/dw/nitric?style=for-the-badge">
   </a>
-  <a href="https://discord.gg/Webemece5C"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
+  <a href="https://nitric.io/chat"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
 </p>
 
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework with Python 3.10+. For more information check out the main [Nitric repo](https://github.com/nitrictech/nitric).
 
 Python SDKs provide an infrastructure-from-code style that lets you define resources in code. You can also write the functions that support the logic behind APIs, subscribers and schedules.
 
 You can request the type of access you need to resources such as publishing for topics, without dealing directly with IAM or policy documents.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.2 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.3 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.2/README.md` & `nitric-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 </h2>
 
 <p align="center">
   <a href="https://actions-badge.atrox.dev/nitrictech/python-sdk/goto?ref=main"><img alt="Build Status" src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fnitrictech%2Fpython-sdk%2Fbadge%3Fref%3Dmain&style=for-the-badge" /></a>
   <a href="https://codecov.io/gh/nitrictech/python-sdk">
     <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/nitrictech/python-sdk?style=for-the-badge&token=SBFRNSZ4ZF">
   </a>
-  <a href="https://npmjs.org/package/@nitric/sdk">
+  <a href="https://pypi.org/project/nitric">
     <img alt="Version" src="https://img.shields.io/pypi/v/nitric?style=for-the-badge">
   </a>
   <a href="https://pypi.org/project/nitric">
     <img alt="Downloads/week" src="https://img.shields.io/pypi/dw/nitric?style=for-the-badge">
   </a>
-  <a href="https://discord.gg/Webemece5C"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
+  <a href="https://nitric.io/chat"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
 </p>
 
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework with Python 3.10+. For more information check out the main [Nitric repo](https://github.com/nitrictech/nitric).
 
 Python SDKs provide an infrastructure-from-code style that lets you define resources in code. You can also write the functions that support the logic behind APIs, subscribers and schedules.
 
 You can request the type of access you need to resources such as publishing for topics, without dealing directly with IAM or policy documents.
```

### Comparing `nitric-1.0.2/nitric/__init__.py` & `nitric-1.0.3/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/application.py` & `nitric-1.0.3/nitric/application.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/bidi.py` & `nitric-1.0.3/nitric/bidi.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/config/__init__.py` & `nitric-1.0.3/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/context.py` & `nitric-1.0.3/nitric/context.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/exception.py` & `nitric-1.0.3/nitric/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/KeyValue/__init__.py` & `nitric-1.0.3/nitric/proto/KeyValue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/KeyValue/v1/__init__.py` & `nitric-1.0.3/nitric/proto/KeyValue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/__init__.py` & `nitric-1.0.3/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/apis/__init__.py` & `nitric-1.0.3/nitric/proto/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/apis/v1/__init__.py` & `nitric-1.0.3/nitric/proto/apis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/deployments/__init__.py` & `nitric-1.0.3/nitric/proto/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/deployments/v1/__init__.py` & `nitric-1.0.3/nitric/proto/deployments/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/http/__init__.py` & `nitric-1.0.3/nitric/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/http/v1/__init__.py` & `nitric-1.0.3/nitric/proto/http/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/kvstore/__init__.py` & `nitric-1.0.3/nitric/proto/kvstore/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/kvstore/v1/__init__.py` & `nitric-1.0.3/nitric/proto/kvstore/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/queues/__init__.py` & `nitric-1.0.3/nitric/proto/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/queues/v1/__init__.py` & `nitric-1.0.3/nitric/proto/queues/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/resources/__init__.py` & `nitric-1.0.3/nitric/proto/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/resources/v1/__init__.py` & `nitric-1.0.3/nitric/proto/resources/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/schedules/__init__.py` & `nitric-1.0.3/nitric/proto/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/schedules/v1/__init__.py` & `nitric-1.0.3/nitric/proto/schedules/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/secrets/__init__.py` & `nitric-1.0.3/nitric/proto/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/secrets/v1/__init__.py` & `nitric-1.0.3/nitric/proto/secrets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/storage/__init__.py` & `nitric-1.0.3/nitric/proto/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/storage/v1/__init__.py` & `nitric-1.0.3/nitric/proto/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/topics/__init__.py` & `nitric-1.0.3/nitric/proto/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/topics/v1/__init__.py` & `nitric-1.0.3/nitric/proto/topics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/websockets/__init__.py` & `nitric-1.0.3/nitric/proto/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/proto/websockets/v1/__init__.py` & `nitric-1.0.3/nitric/proto/websockets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/__init__.py` & `nitric-1.0.3/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/apis.py` & `nitric-1.0.3/nitric/resources/apis.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/buckets.py` & `nitric-1.0.3/nitric/resources/buckets.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import Enum
-from typing import Callable, List, Literal, Optional, Union
+from typing import Callable, List, Literal, Optional, Union, cast
 from warnings import warn
 
 import betterproto
 import grpclib
 from grpclib import GRPCError
 from grpclib.client import Channel
 
@@ -142,41 +142,79 @@
         try:
             await self._bucket._storage_stub.delete(  # type: ignore pylint: disable=protected-access
                 storage_delete_request=StorageDeleteRequest(bucket_name=self._bucket.name, key=self.key)
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
-    async def upload_url(self, expiry: Optional[timedelta] = None):
-        """Get a temporary writable URL to this file."""
-        return await self.sign_url(mode=FileMode.WRITE, expiry=expiry)
-
-    async def download_url(self, expiry: Optional[timedelta] = None):
-        """Get a temporary readable URL to this file."""
-        return await self.sign_url(mode=FileMode.READ, expiry=expiry)
+    async def upload_url(self, expiry: Optional[Union[timedelta, int]] = None):
+        """
+        Get a temporary writable URL to this file.
 
-    async def sign_url(self, mode: FileMode = FileMode.READ, expiry: Optional[timedelta] = None):
-        """Generate a signed URL for reading or writing to a file."""
-        warn("File.sign_url() is deprecated, use upload_url() or download_url() instead", DeprecationWarning)
+        Parameters:
+
+        expiry (timedelta or int, optional): The expiry time for the signed URL.
+        If an integer is provided, it is treated as seconds. Default is 600 seconds.
+
+        Returns:
+        str: The signed URL.
+        """
+        return await self._sign_url(mode=FileMode.WRITE, expiry=expiry)
+
+    async def download_url(self, expiry: Optional[Union[timedelta, int]] = None):
+        """
+        Get a temporary readable URL to this file.
+
+        Parameters:
+
+        expiry (timedelta or int, optional): The expiry time for the signed URL.
+        If an integer is provided, it is treated as seconds. Default is 600 seconds.
 
+        Returns:
+        str: The signed URL.
+        """
+        return await self._sign_url(mode=FileMode.READ, expiry=expiry)
+
+    async def _sign_url(self, mode: FileMode = FileMode.READ, expiry: Optional[Union[timedelta, int]] = None):
+        """Generate a signed URL for reading or writing to a file."""
         if expiry is None:
             expiry = timedelta(seconds=600)
+        if not isinstance(expiry, timedelta):
+            expiry = timedelta(seconds=expiry)
 
         try:
             response = await self._bucket._storage_stub.pre_sign_url(  # type: ignore pylint: disable=protected-access
                 storage_pre_sign_url_request=StoragePreSignUrlRequest(
                     bucket_name=self._bucket.name, key=self.key, operation=mode.to_request_operation(), expiry=expiry
                 )
             )
             return response.url
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
 
-BucketPermission = Literal["reading", "writing", "deleting"]
+LegacyBucketPermission = Literal["reading", "writing", "deleting"]
+BucketPermission = Literal["read", "write", "delete"]
+
+legacy_perms: List[LegacyBucketPermission] = ["reading", "writing", "deleting"]
+new_perms: List[BucketPermission] = ["read", "write", "delete"]
+
+
+def check_permission(permission: Union[LegacyBucketPermission, BucketPermission]) -> BucketPermission:
+    """Check if the permission is valid and return the new permission if it is a legacy permission."""
+    if permission in legacy_perms:
+        new_perm = new_perms[legacy_perms.index(cast(LegacyBucketPermission, permission))]
+        warn(
+            f"The permission '{permission}' is deprecated. Use '{new_perm}' instead.", DeprecationWarning, stacklevel=2
+        )
+        return new_perm
+    elif permission in new_perms:
+        return cast(BucketPermission, permission)
+    else:
+        raise ValueError("Invalid permission value, must be one of 'read', 'write', or 'delete'.")
 
 
 class BucketNotificationWorkerOptions:
     """Options for bucket notification workers."""
 
     def __init__(self, bucket_name: str, notification_type: str, notification_prefix_filter: str):
         """Construct a new options object."""
@@ -207,27 +245,33 @@
                 resource_declare_request=ResourceDeclareRequest(id=self._to_resource_id())
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     def _perms_to_actions(self, *args: BucketPermission) -> List[Action]:
         permission_actions_map: dict[BucketPermission, List[Action]] = {
-            "reading": [Action.BucketFileGet, Action.BucketFileList],
-            "writing": [Action.BucketFilePut],
-            "deleting": [Action.BucketFileDelete],
+            "read": [Action.BucketFileGet, Action.BucketFileList],
+            "write": [Action.BucketFilePut],
+            "delete": [Action.BucketFileDelete],
         }
 
         return [action for perm in args for action in permission_actions_map[perm]]
 
     def _to_resource_id(self) -> ResourceIdentifier:
         return ResourceIdentifier(name=self.name, type=ResourceType.Bucket)  # type:ignore
 
-    def allow(self, perm: BucketPermission, *args: BucketPermission) -> BucketRef:
+    def allow(
+        self,
+        perm: Union[LegacyBucketPermission, BucketPermission],
+        *args: Union[LegacyBucketPermission, BucketPermission],
+    ) -> BucketRef:
         """Request the required permissions for this resource."""
-        str_args = [str(perm)] + [str(permission) for permission in args]
+        all_perms: List[BucketPermission] = [check_permission(perm)] + [check_permission(p) for p in args]
+
+        str_args = [str(permission) for permission in all_perms]
         self._register_policy(*str_args)
 
         return BucketRef(self.name)
 
     def on(
         self, notification_type: str, notification_prefix_filter: str
     ) -> Callable[[BucketNotificationHandler], None]:
```

### Comparing `nitric-1.0.2/nitric/resources/kv.py` & `nitric-1.0.3/nitric/resources/kv.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/queues.py` & `nitric-1.0.3/nitric/resources/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/resource.py` & `nitric-1.0.3/nitric/resources/resource.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/schedules.py` & `nitric-1.0.3/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/secrets.py` & `nitric-1.0.3/nitric/resources/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/topics.py` & `nitric-1.0.3/nitric/resources/topics.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/resources/websockets.py` & `nitric-1.0.3/nitric/resources/websockets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric/utils.py` & `nitric-1.0.3/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/nitric.egg-info/PKG-INFO` & `nitric-1.0.3/nitric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -22,21 +22,21 @@
 </h2>
 
 <p align="center">
   <a href="https://actions-badge.atrox.dev/nitrictech/python-sdk/goto?ref=main"><img alt="Build Status" src="https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fnitrictech%2Fpython-sdk%2Fbadge%3Fref%3Dmain&style=for-the-badge" /></a>
   <a href="https://codecov.io/gh/nitrictech/python-sdk">
     <img alt="Codecov" src="https://img.shields.io/codecov/c/gh/nitrictech/python-sdk?style=for-the-badge&token=SBFRNSZ4ZF">
   </a>
-  <a href="https://npmjs.org/package/@nitric/sdk">
+  <a href="https://pypi.org/project/nitric">
     <img alt="Version" src="https://img.shields.io/pypi/v/nitric?style=for-the-badge">
   </a>
   <a href="https://pypi.org/project/nitric">
     <img alt="Downloads/week" src="https://img.shields.io/pypi/dw/nitric?style=for-the-badge">
   </a>
-  <a href="https://discord.gg/Webemece5C"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
+  <a href="https://nitric.io/chat"><img alt="Discord" src="https://img.shields.io/discord/955259353043173427?label=discord&style=for-the-badge"></a>
 </p>
 
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework with Python 3.10+. For more information check out the main [Nitric repo](https://github.com/nitrictech/nitric).
 
 Python SDKs provide an infrastructure-from-code style that lets you define resources in code. You can also write the functions that support the logic behind APIs, subscribers and schedules.
 
 You can request the type of access you need to resources such as publishing for topics, without dealing directly with IAM or policy documents.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.2 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.3 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.2/nitric.egg-info/SOURCES.txt` & `nitric-1.0.3/nitric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitric-1.0.2/setup.py` & `nitric-1.0.3/setup.py`

 * *Files identical despite different names*

