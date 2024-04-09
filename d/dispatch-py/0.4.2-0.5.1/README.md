# Comparing `tmp/dispatch-py-0.4.2.tar.gz` & `tmp/dispatch-py-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispatch-py-0.4.2.tar", last modified: Thu Mar 28 01:41:39 2024, max compression
+gzip compressed data, was "dispatch-py-0.5.1.tar", last modified: Tue Apr  9 23:37:50 2024, max compression
```

## Comparing `dispatch-py-0.4.2.tar` & `dispatch-py-0.5.1.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.336716 dispatch-py-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-03-28 01:41:39.336716 dispatch-py-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 01:41:39.336716 dispatch-py-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.316716 dispatch-py-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.320716 dispatch-py-0.4.2/src/buf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.320716 dispatch-py-0.4.2/src/buf/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/expression_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/expression_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.320716 dispatch-py-0.4.2/src/buf/validate/priv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/priv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/priv/private_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/priv/private_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/validate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.324716 dispatch-py-0.4.2/src/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.324716 dispatch-py-0.4.2/src/dispatch/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.324716 dispatch-py-0.4.2/src/dispatch/experimental/durable/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame308.h
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame309.h
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame310.h
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame311.h
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame312.h
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/frame313.h
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/function.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/experimental/durable/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.324716 dispatch-py-0.4.2/src/dispatch/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/integrations/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    13466 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19942 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.324716 dispatch-py-0.4.2/src/dispatch/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.328716 dispatch-py-0.4.2/src/dispatch/sdk/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/call_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/call_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/call_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/exit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/exit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/exit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/poll_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/poll_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/poll_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/sdk/v1/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.332716 dispatch-py-0.4.2/src/dispatch/signature/
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/signature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/signature/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/signature/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/signature/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.332716 dispatch-py-0.4.2/src/dispatch/test/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/src/dispatch/test/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.332716 dispatch-py-0.4.2/src/dispatch_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-03-28 01:41:39.000000 dispatch-py-0.4.2/src/dispatch_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-28 01:41:39.000000 dispatch-py-0.4.2/src/dispatch_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 01:41:39.000000 dispatch-py-0.4.2/src/dispatch_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-28 01:41:39.000000 dispatch-py-0.4.2/src/dispatch_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 01:41:39.000000 dispatch-py-0.4.2/src/dispatch_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 01:41:39.332716 dispatch-py-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21307 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-28 01:41:29.000000 dispatch-py-0.4.2/tests/test_full.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.543831 dispatch-py-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/validate/priv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/dispatch/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/experimental/durable/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame308.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame309.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame310.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame311.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame312.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame313.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.555831 dispatch-py-0.5.1/src/dispatch/sdk/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.555831 dispatch-py-0.5.1/src/dispatch/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/src/dispatch/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/src/dispatch_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21510 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_full.py
```

### Comparing `dispatch-py-0.4.2/CONTRIBUTING.md` & `dispatch-py-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/LICENSE` & `dispatch-py-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/Makefile` & `dispatch-py-0.5.1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 .PHONY: install test typecheck unittest dev fmt fmt-check generate clean update-proto coverage build check push push-test
 
 PYTHON := python
 
+ifdef PROTO_VERSION
+PROTO_TARGET := buf.build/stealthrocket/dispatch-proto:$(PROTO_VERSION)
+else
+PROTO_TARGET := buf.build/stealthrocket/dispatch-proto
+endif
+
+
 all: test
 
 install:
 	$(PYTHON) -m pip install -e .
 
 dev:
 	$(PYTHON) -m pip install -e .[dev]
 
+lambda:
+	$(PYTHON) -m pip install -e .[lambda]
+
 fmt:
 	$(PYTHON) -m isort .
 	$(PYTHON) -m black .
 
 fmt-check:
 	@$(PYTHON) -m isort . --check --diff; isort_status=$$?; \
 	$(PYTHON) -m black . --check --diff; black_status=$$?; \
@@ -35,15 +45,15 @@
 
 test: typecheck unittest
 
 .proto:
 	mkdir -p $@
 
 .proto/dispatch-proto: .proto
-	buf export buf.build/stealthrocket/dispatch-proto --output=.proto/dispatch-proto
+	buf export $(PROTO_TARGET) --output=.proto/dispatch-proto
 
 update-proto:
 	$(MAKE) clean
 	find . -type f -name '*_pb2*.py*' -exec rm  {} \;
 	$(MAKE) generate
 
 generate: .proto/dispatch-proto
```

### Comparing `dispatch-py-0.4.2/PKG-INFO` & `dispatch-py-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.4.2
+Version: 0.5.1
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
@@ -14,24 +14,27 @@
 Requires-Dist: docopt>=0.6.2
 Requires-Dist: types-docopt>=0.6.11.4
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: typing_extensions>=4.10
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
 Requires-Dist: httpx; extra == "fastapi"
+Provides-Extra: lambda
+Requires-Dist: awslambdaric; extra == "lambda"
 Provides-Extra: dev
 Requires-Dist: black>=24.1.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: mypy>=1.8.0; extra == "dev"
 Requires-Dist: pytest==8.0.0; extra == "dev"
 Requires-Dist: fastapi>=0.109.0; extra == "dev"
 Requires-Dist: coverage>=7.4.1; extra == "dev"
 Requires-Dist: requests>=2.31.0; extra == "dev"
 Requires-Dist: types-requests>=2.31.0.20240125; extra == "dev"
 Requires-Dist: uvicorn>=0.28.0; extra == "dev"
+Requires-Dist: awslambdaric-stubs; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.24.0; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.9; extra == "docs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "docs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "docs"
 Requires-Dist: mike==2.0.0; extra == "docs"
```

### Comparing `dispatch-py-0.4.2/README.md` & `dispatch-py-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/mkdocs.yml` & `dispatch-py-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/pyproject.toml` & `dispatch-py-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,25 +19,27 @@
     "types-docopt >= 0.6.11.4",
     "httpx >= 0.27.0",
     "typing_extensions >= 4.10"
 ]
 
 [project.optional-dependencies]
 fastapi = ["fastapi", "httpx"]
+lambda = ["awslambdaric"]
 
 dev = [
     "black >= 24.1.0",
     "isort >= 5.13.2",
     "mypy >= 1.8.0",
     "pytest==8.0.0",
     "fastapi >= 0.109.0",
     "coverage >= 7.4.1",
     "requests >= 2.31.0",
     "types-requests >= 2.31.0.20240125",
-    "uvicorn >= 0.28.0"
+    "uvicorn >= 0.28.0",
+    "awslambdaric-stubs"
 ]
 
 docs = [
     "mkdocs==1.5.3",
     "mkdocstrings[python]==0.24.0",
     "mkdocs-material==9.5.9",
     "mkdocs-gen-files==0.5.0",
```

### Comparing `dispatch-py-0.4.2/src/buf/validate/expression_pb2.py` & `dispatch-py-0.5.1/src/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/buf/validate/expression_pb2.pyi` & `dispatch-py-0.5.1/src/buf/validate/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/buf/validate/priv/private_pb2.py` & `dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/buf/validate/priv/private_pb2.pyi` & `dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/buf/validate/validate_pb2.py` & `dispatch-py-0.5.1/src/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/buf/validate/validate_pb2.pyi` & `dispatch-py-0.5.1/src/buf/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/__init__.py` & `dispatch-py-0.5.1/src/dispatch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """The Dispatch SDK for Python."""
 
 from __future__ import annotations
 
 import dispatch.integrations
 from dispatch.coroutine import all, any, call, gather, race
-from dispatch.function import DEFAULT_API_URL, Client, Registry
+from dispatch.function import DEFAULT_API_URL, Client, Registry, Reset
 from dispatch.id import DispatchID
 from dispatch.proto import Call, Error, Input, Output
 from dispatch.status import Status
 
 __all__ = [
     "Client",
     "DispatchID",
     "DEFAULT_API_URL",
     "Input",
     "Output",
     "Call",
     "Error",
+    "Reset",
     "Status",
     "call",
     "gather",
     "all",
     "any",
     "race",
     "Registry",
```

### Comparing `dispatch-py-0.4.2/src/dispatch/coroutine.py` & `dispatch-py-0.5.1/src/dispatch/coroutine.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/__init__.py` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame.c` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.c`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame.pyi` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame308.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame308.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame309.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame309.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame310.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame310.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame311.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame311.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame312.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame312.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/frame313.h` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame313.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/function.py` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/function.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/experimental/durable/registry.py` & `dispatch-py-0.5.1/src/dispatch/experimental/durable/registry.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/fastapi.py` & `dispatch-py-0.5.1/src/dispatch/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 
     import fastapi
     from dispatch.fastapi import Dispatch
 
     app = fastapi.FastAPI()
     dispatch = Dispatch(app, api_key="test-key")
 
-    @dispatch.function()
+    @dispatch.function
     def my_function():
         return "Hello World!"
 
     @app.get("/")
     def read_root():
         my_function.dispatch()
     """
 
+import asyncio
 import base64
 import logging
 import os
 from datetime import timedelta
 from typing import Optional, Union
 from urllib.parse import urlparse
 
 import fastapi
 import fastapi.responses
 from http_message_signatures import InvalidSignature
 
-from dispatch.function import Batch, Client, Registry
+from dispatch.function import Batch, Registry
 from dispatch.proto import Input
 from dispatch.sdk.v1 import function_pb2 as function_pb
 from dispatch.signature import (
     CaseInsensitiveDict,
     Ed25519PublicKey,
     Request,
     public_key_from_bytes,
@@ -225,16 +226,19 @@
             logger.debug("function '%s' not found", req.function)
             raise _ConnectError(
                 404, "not_found", f"function '{req.function}' does not exist"
             )
 
         input = Input(req)
         logger.info("running function '%s'", req.function)
+
+        loop = asyncio.get_running_loop()
+
         try:
-            output = func._primitive_call(input)
+            output = await loop.run_in_executor(None, func._primitive_call, input)
         except Exception:
             # This indicates that an exception was raised in a primitive
             # function. Primitive functions must catch exceptions, categorize
             # them in order to derive a Status, and then return a RunResponse
             # that carries the Status and the error details. A failure to do
             # so indicates a problem, and we return a 500 rather than attempt
             # to catch and categorize the error here.
```

### Comparing `dispatch-py-0.4.2/src/dispatch/function.py` & `dispatch-py-0.5.1/src/dispatch/function.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import ParamSpec, TypeAlias
 
 import dispatch.coroutine
 import dispatch.sdk.v1.dispatch_pb2 as dispatch_pb
 import dispatch.sdk.v1.dispatch_pb2_grpc as dispatch_grpc
 from dispatch.experimental.durable import durable
 from dispatch.id import DispatchID
-from dispatch.proto import Arguments, Call, Error, Input, Output
+from dispatch.proto import Arguments, Call, Error, Input, Output, TailCall
 from dispatch.scheduler import OneShotScheduler
 
 logger = logging.getLogger(__name__)
 
 
 PrimitiveFunctionType: TypeAlias = Callable[[Input], Output]
 """A primitive function is a function that accepts a dispatch.proto.Input
@@ -58,14 +58,18 @@
         self._name = name
         self._primitive_func = primitive_func
 
     @property
     def endpoint(self) -> str:
         return self._endpoint
 
+    @endpoint.setter
+    def endpoint(self, value: str):
+        self._endpoint = value
+
     @property
     def name(self) -> str:
         return self._name
 
     def _primitive_call(self, input: Input) -> Output:
         return self._primitive_func(input)
 
@@ -153,14 +157,22 @@
             Call: can be passed to Client.dispatch.
         """
         return self._build_primitive_call(
             Arguments(args, kwargs), correlation_id=correlation_id
         )
 
 
+class Reset(TailCall):
+    """The current coroutine is aborted and scheduling reset to be replaced with
+    the call embedded in this exception."""
+
+    def __init__(self, func: Function[P, T], *args: P.args, **kwargs: P.kwargs):
+        super().__init__(call=func.build_call(*args, correlation_id=None, **kwargs))
+
+
 class Registry:
     """Registry of functions."""
 
     __slots__ = ("functions", "endpoint", "client")
 
     def __init__(
         self,
@@ -255,14 +267,18 @@
             fn._client = client
 
     def batch(self) -> Batch:
         """Returns a Batch instance that can be used to build
         a set of calls to dispatch."""
         return self.client.batch()
 
+    def override_endpoint(self, endpoint: str):
+        for fn in self.functions.values():
+            fn.endpoint = endpoint
+
 
 class Client:
     """Client for the Dispatch API."""
 
     __slots__ = ("api_url", "api_key", "_stub", "api_key_from")
 
     def __init__(self, api_key: Optional[str] = None, api_url: Optional[str] = None):
```

### Comparing `dispatch-py-0.4.2/src/dispatch/integrations/http.py` & `dispatch-py-0.5.1/src/dispatch/integrations/http.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/integrations/httpx.py` & `dispatch-py-0.5.1/src/dispatch/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/integrations/openai.py` & `dispatch-py-0.5.1/src/dispatch/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/integrations/requests.py` & `dispatch-py-0.5.1/src/dispatch/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/integrations/slack.py` & `dispatch-py-0.5.1/src/dispatch/integrations/slack.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/proto.py` & `dispatch-py-0.5.1/src/dispatch/proto.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,38 @@
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Tuple
 
 import google.protobuf.any_pb2
 import google.protobuf.message
 import google.protobuf.wrappers_pb2
 import tblib  # type: ignore[import-untyped]
-from google.protobuf import duration_pb2
+from google.protobuf import descriptor_pool, duration_pb2, message_factory
 
 from dispatch.sdk.v1 import call_pb2 as call_pb
 from dispatch.sdk.v1 import error_pb2 as error_pb
 from dispatch.sdk.v1 import exit_pb2 as exit_pb
 from dispatch.sdk.v1 import function_pb2 as function_pb
 from dispatch.sdk.v1 import poll_pb2 as poll_pb
 from dispatch.sdk.v1 import status_pb2 as status_pb
 from dispatch.status import Status, status_for_error, status_for_output
 
+
+class TailCall(Exception):
+    """The current coroutine is aborted and scheduling reset to be replaced with
+    the call embedded in this exception."""
+
+    call: Call
+    status: Status
+
+    def __init__(self, call: Call, status: Status = Status.TEMPORARY_ERROR):
+        super().__init__(f"reset coroutine to ${call.function}")
+        self.call = call
+        self.status = status
+
+
 # Most types in this package are thin wrappers around the various protobuf
 # messages of dispatch.sdk.v1. They provide some safeguards and ergonomics.
 
 
 class Input:
     """The input to a primitive function.
 
@@ -43,24 +57,26 @@
         "_call_results",
         "_poll_error",
     )
 
     def __init__(self, req: function_pb.RunRequest):
         self._has_input = req.HasField("input")
         if self._has_input:
-            input_pb = google.protobuf.wrappers_pb2.BytesValue()
-            req.input.Unpack(input_pb)
-            input_bytes = input_pb.value
-            self._input = pickle.loads(input_bytes)
-        else:
-            state_bytes = req.poll_result.coroutine_state
-            if len(state_bytes) > 0:
-                self._coroutine_state = pickle.loads(state_bytes)
+            if req.input.Is(google.protobuf.wrappers_pb2.BytesValue.DESCRIPTOR):
+                input_pb = google.protobuf.wrappers_pb2.BytesValue()
+                req.input.Unpack(input_pb)
+                input_bytes = input_pb.value
+                try:
+                    self._input = pickle.loads(input_bytes)
+                except Exception as e:
+                    self._input = input_bytes
             else:
-                self._coroutine_state = None
+                self._input = _pb_any_unpack(req.input)
+        else:
+            self._coroutine_state = req.poll_result.coroutine_state
             self._call_results = [
                 CallResult._from_proto(r) for r in req.poll_result.results
             ]
             self._poll_error = (
                 Error._from_proto(req.poll_result.error)
                 if req.poll_result.HasField("error")
                 else None
@@ -119,15 +135,15 @@
             )
         )
 
     @classmethod
     def from_poll_results(
         cls,
         function: str,
-        coroutine_state: Any,
+        coroutine_state: Optional[bytes],
         call_results: List[CallResult],
         error: Optional[Error] = None,
     ):
         return Input(
             req=function_pb.RunRequest(
                 function=function,
                 poll_result=poll_pb.PollResult(
@@ -171,18 +187,18 @@
 
     @classmethod
     def error(cls, error: Error) -> Output:
         """Terminally exit the function with the provided error."""
         return cls.exit(result=CallResult.from_error(error), status=error.status)
 
     @classmethod
-    def tail_call(cls, tail_call: Call) -> Output:
+    def tail_call(cls, tail_call: Call, status: Status = Status.OK) -> Output:
         """Terminally exit the function, and instruct the orchestrator to
         tail call the specified function."""
-        return cls.exit(tail_call=tail_call)
+        return cls.exit(tail_call=tail_call, status=status)
 
     @classmethod
     def exit(
         cls,
         result: Optional[CallResult] = None,
         tail_call: Optional[Call] = None,
         status: Status = Status.OK,
@@ -196,31 +212,30 @@
                 exit=exit_pb.Exit(result=result_proto, tail_call=tail_call_proto),
             )
         )
 
     @classmethod
     def poll(
         cls,
-        state: Any,
+        coroutine_state: Optional[bytes] = None,
         calls: Optional[List[Call]] = None,
         min_results: int = 1,
         max_results: int = 10,
         max_wait_seconds: Optional[int] = None,
     ) -> Output:
         """Suspend the function with a set of Calls, instructing the
         orchestrator to resume the function with the provided state when
         call results are ready."""
-        state_bytes = pickle.dumps(state)
         max_wait = (
             duration_pb2.Duration(seconds=max_wait_seconds)
             if max_wait_seconds is not None
             else None
         )
         poll = poll_pb.Poll(
-            coroutine_state=state_bytes,
+            coroutine_state=coroutine_state,
             min_results=min_results,
             max_results=max_results,
             max_wait=max_wait,
         )
 
         if calls is not None:
             for c in calls:
@@ -415,7 +430,15 @@
 
 def _pb_any_pickle(x: Any) -> google.protobuf.any_pb2.Any:
     value_bytes = pickle.dumps(x)
     pb_bytes = google.protobuf.wrappers_pb2.BytesValue(value=value_bytes)
     pb_any = google.protobuf.any_pb2.Any()
     pb_any.Pack(pb_bytes)
     return pb_any
+
+
+def _pb_any_unpack(x: google.protobuf.any_pb2.Any) -> Any:
+    pool = descriptor_pool.Default()
+    msg_descriptor = pool.FindMessageTypeByName(x.TypeName())
+    proto = message_factory.GetMessageClass(msg_descriptor)()
+    x.Unpack(proto)
+    return proto
```

### Comparing `dispatch-py-0.4.2/src/dispatch/scheduler.py` & `dispatch-py-0.5.1/src/dispatch/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 from typing_extensions import TypeAlias
 
 from dispatch.coroutine import AllDirective, AnyDirective, AnyException, RaceDirective
 from dispatch.error import IncompatibleStateError
 from dispatch.experimental.durable.function import DurableCoroutine, DurableGenerator
-from dispatch.proto import Call, Error, Input, Output
+from dispatch.proto import Call, Error, Input, Output, TailCall
 from dispatch.status import Status
 
 logger = logging.getLogger(__name__)
 
 CallID: TypeAlias = int
 CoroutineID: TypeAlias = int
 CorrelationID: TypeAlias = int
@@ -33,14 +33,16 @@
 @dataclass
 class CoroutineResult:
     """The result from running a coroutine to completion."""
 
     coroutine_id: CoroutineID
     value: Optional[Any] = None
     error: Optional[Exception] = None
+    call: Optional[Call] = None
+    status: Status = Status.OK
 
 
 @dataclass
 class CallResult:
     """The result of an asynchronous function call."""
 
     call_id: CallID
@@ -368,15 +370,14 @@
                 )
             return state
         except (pickle.PickleError, ValueError) as e:
             logger.warning("state is incompatible", exc_info=True)
             raise IncompatibleStateError from e
 
     def _run(self, input: Input) -> Output:
-
         if input.is_first_call:
             state = self._init_state(input)
         else:
             state = self._rebuild_state(input)
 
             poll_error = input.poll_error
             if poll_error is not None:
@@ -434,39 +435,52 @@
 
             assert coroutine.id not in state.suspended
 
             coroutine_yield = None
             coroutine_result: Optional[CoroutineResult] = None
             try:
                 coroutine_yield = coroutine.run()
+            except TailCall as tc:
+                coroutine_result = CoroutineResult(
+                    coroutine_id=coroutine.id, call=tc.call, status=tc.status
+                )
             except StopIteration as e:
                 coroutine_result = CoroutineResult(
                     coroutine_id=coroutine.id, value=e.value
                 )
             except Exception as e:
                 logger.debug(
                     f"@dispatch.function: '{coroutine}' raised an exception", exc_info=e
                 )
                 coroutine_result = CoroutineResult(coroutine_id=coroutine.id, error=e)
 
             # Handle coroutines that return or raise.
             if coroutine_result is not None:
-                if coroutine_result.error is not None:
+                if coroutine_result.call is not None:
+                    logger.debug(
+                        "%s reset to %s", coroutine, coroutine_result.call.function
+                    )
+                elif coroutine_result.error is not None:
                     logger.debug("%s raised %s", coroutine, coroutine_result.error)
                 else:
                     logger.debug("%s returned %s", coroutine, coroutine_result.value)
 
                 # If this is the main coroutine, we're done.
                 if coroutine.parent_id is None:
                     for suspended in state.suspended.values():
                         suspended.coroutine.close()
                     if coroutine_result.error is not None:
                         return Output.error(
                             Error.from_exception(coroutine_result.error)
                         )
+                    if coroutine_result.call is not None:
+                        return Output.tail_call(
+                            tail_call=coroutine_result.call,
+                            status=coroutine_result.status,
+                        )
                     return Output.value(coroutine_result.value)
 
                 # Otherwise, notify the parent of the result.
                 try:
                     parent = state.suspended[coroutine.parent_id]
                     future = parent.result
                     assert future is not None
@@ -540,15 +554,15 @@
         # Yield to Dispatch.
         logger.debug(
             "yielding to Dispatch with %d call(s) and %d bytes of state",
             len(pending_calls),
             len(serialized_state),
         )
         return Output.poll(
-            state=serialized_state,
+            coroutine_state=serialized_state,
             calls=pending_calls,
             min_results=max(1, min(state.outstanding_calls, self.poll_min_results)),
             max_results=max(1, min(state.outstanding_calls, self.poll_max_results)),
             max_wait_seconds=self.poll_max_wait_seconds,
         )
```

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/call_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from dispatch.sdk.v1 import error_pb2 as dispatch_dot_sdk_dot_v1_dot_error__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1a\x64ispatch/sdk/v1/call.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1b\x64ispatch/sdk/v1/error.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto"\x84\x02\n\x04\x43\x61ll\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12$\n\x08\x65ndpoint\x18\x02 \x01(\tB\x08\xbaH\x05r\x03\x88\x01\x01R\x08\x65ndpoint\x12>\n\x08\x66unction\x18\x03 \x01(\tB"\xbaH\x1fr\x1a\x32\x18^[a-zA-Z_][a-zA-Z0-9_]*$\xc8\x01\x01R\x08\x66unction\x12*\n\x05input\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05input\x12\x43\n\nexpiration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xbaH\x05\xaa\x01\x02\x32\x00R\nexpiration"\x8f\x01\n\nCallResult\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12,\n\x06output\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x06output\x12,\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x16.dispatch.sdk.v1.ErrorR\x05\x65rrorB~\n\x13\x63om.dispatch.sdk.v1B\tCallProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
+    b'\n\x1a\x64ispatch/sdk/v1/call.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1b\x64ispatch/sdk/v1/error.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto"\x87\x02\n\x04\x43\x61ll\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12$\n\x08\x65ndpoint\x18\x02 \x01(\tB\x08\xbaH\x05r\x03\x88\x01\x01R\x08\x65ndpoint\x12\x41\n\x08\x66unction\x18\x03 \x01(\tB%\xbaH"r\x1d\x32\x1b^[a-zA-Z_][a-zA-Z0-9_<>.]*$\xc8\x01\x01R\x08\x66unction\x12*\n\x05input\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05input\x12\x43\n\nexpiration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xbaH\x05\xaa\x01\x02\x32\x00R\nexpiration"\x8f\x01\n\nCallResult\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12,\n\x06output\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x06output\x12,\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x16.dispatch.sdk.v1.ErrorR\x05\x65rrorB~\n\x13\x63om.dispatch.sdk.v1B\tCallProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "dispatch.sdk.v1.call_pb2", _globals
 )
@@ -36,17 +36,17 @@
     _globals["_CALL"].fields_by_name["endpoint"]._options = None
     _globals["_CALL"].fields_by_name[
         "endpoint"
     ]._serialized_options = b"\272H\005r\003\210\001\001"
     _globals["_CALL"].fields_by_name["function"]._options = None
     _globals["_CALL"].fields_by_name[
         "function"
-    ]._serialized_options = b"\272H\037r\0322\030^[a-zA-Z_][a-zA-Z0-9_]*$\310\001\001"
+    ]._serialized_options = b'\272H"r\0352\033^[a-zA-Z_][a-zA-Z0-9_<>.]*$\310\001\001'
     _globals["_CALL"].fields_by_name["expiration"]._options = None
     _globals["_CALL"].fields_by_name[
         "expiration"
     ]._serialized_options = b"\272H\005\252\001\0022\000"
     _globals["_CALL"]._serialized_start = 165
-    _globals["_CALL"]._serialized_end = 425
-    _globals["_CALLRESULT"]._serialized_start = 428
-    _globals["_CALLRESULT"]._serialized_end = 571
+    _globals["_CALL"]._serialized_end = 428
+    _globals["_CALLRESULT"]._serialized_start = 431
+    _globals["_CALLRESULT"]._serialized_end = 574
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/call_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 _sym_db = _symbol_database.Default()
 
 
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from dispatch.sdk.v1 import call_pb2 as dispatch_dot_sdk_dot_v1_dot_call__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b"\n\x1e\x64ispatch/sdk/v1/dispatch.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1a\x64ispatch/sdk/v1/call.proto\"\xf3\x02\n\x0f\x44ispatchRequest\x12+\n\x05\x63\x61lls\x18\x01 \x03(\x0b\x32\x15.dispatch.sdk.v1.CallR\x05\x63\x61lls:\xb2\x02\xbaH\xae\x02\x1as\n(dispatch.request.calls.endpoint.nonempty\x12\x1d\x43\x61ll endpoint cannot be empty\x1a(this.calls.all(call, has(call.endpoint))\x1a\xb6\x01\n&dispatch.request.calls.endpoint.scheme\x12)Call endpoint must be a http or https URL\x1a\x61this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://'))\"5\n\x10\x44ispatchResponse\x12!\n\x0c\x64ispatch_ids\x18\x01 \x03(\tR\x0b\x64ispatchIds2d\n\x0f\x44ispatchService\x12Q\n\x08\x44ispatch\x12 .dispatch.sdk.v1.DispatchRequest\x1a!.dispatch.sdk.v1.DispatchResponse\"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rDispatchProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3"
+    b"\n\x1e\x64ispatch/sdk/v1/dispatch.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1a\x64ispatch/sdk/v1/call.proto\"\xb7\x03\n\x0f\x44ispatchRequest\x12+\n\x05\x63\x61lls\x18\x01 \x03(\x0b\x32\x15.dispatch.sdk.v1.CallR\x05\x63\x61lls:\xf6\x02\xbaH\xf2\x02\x1as\n(dispatch.request.calls.endpoint.nonempty\x12\x1d\x43\x61ll endpoint cannot be empty\x1a(this.calls.all(call, has(call.endpoint))\x1a\xfa\x01\n&dispatch.request.calls.endpoint.scheme\x12>Call endpoint must be a http or https URL or an AWS Lambda ARN\x1a\x8f\x01this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('arn:aws:lambda'))\"5\n\x10\x44ispatchResponse\x12!\n\x0c\x64ispatch_ids\x18\x01 \x03(\tR\x0b\x64ispatchIds2d\n\x0f\x44ispatchService\x12Q\n\x08\x44ispatch\x12 .dispatch.sdk.v1.DispatchRequest\x1a!.dispatch.sdk.v1.DispatchResponse\"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rDispatchProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3"
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "dispatch.sdk.v1.dispatch_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals["DESCRIPTOR"]._serialized_options = (
         b"\n\023com.dispatch.sdk.v1B\rDispatchProtoP\001\242\002\003DSX\252\002\017Dispatch.Sdk.V1\312\002\017Dispatch\\Sdk\\V1\342\002\033Dispatch\\Sdk\\V1\\GPBMetadata\352\002\021Dispatch::Sdk::V1"
     )
     _globals["_DISPATCHREQUEST"]._options = None
     _globals["_DISPATCHREQUEST"]._serialized_options = (
-        b"\272H\256\002\032s\n(dispatch.request.calls.endpoint.nonempty\022\035Call endpoint cannot be empty\032(this.calls.all(call, has(call.endpoint))\032\266\001\n&dispatch.request.calls.endpoint.scheme\022)Call endpoint must be a http or https URL\032athis.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://'))"
+        b"\272H\362\002\032s\n(dispatch.request.calls.endpoint.nonempty\022\035Call endpoint cannot be empty\032(this.calls.all(call, has(call.endpoint))\032\372\001\n&dispatch.request.calls.endpoint.scheme\022>Call endpoint must be a http or https URL or an AWS Lambda ARN\032\217\001this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('arn:aws:lambda'))"
     )
     _globals["_DISPATCHREQUEST"]._serialized_start = 109
-    _globals["_DISPATCHREQUEST"]._serialized_end = 480
-    _globals["_DISPATCHRESPONSE"]._serialized_start = 482
-    _globals["_DISPATCHRESPONSE"]._serialized_end = 535
-    _globals["_DISPATCHSERVICE"]._serialized_start = 537
-    _globals["_DISPATCHSERVICE"]._serialized_end = 637
+    _globals["_DISPATCHREQUEST"]._serialized_end = 548
+    _globals["_DISPATCHRESPONSE"]._serialized_start = 550
+    _globals["_DISPATCHRESPONSE"]._serialized_end = 603
+    _globals["_DISPATCHSERVICE"]._serialized_start = 605
+    _globals["_DISPATCHSERVICE"]._serialized_end = 705
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/dispatch_pb2_grpc.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/error_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/error_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/exit_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/exit_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/function_pb2_grpc.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/poll_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/poll_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/status_pb2.py` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/sdk/v1/status_pb2.pyi` & `dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/signature/__init__.py` & `dispatch-py-0.5.1/src/dispatch/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/signature/digest.py` & `dispatch-py-0.5.1/src/dispatch/signature/digest.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/signature/key.py` & `dispatch-py-0.5.1/src/dispatch/signature/key.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/status.py` & `dispatch-py-0.5.1/src/dispatch/status.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/test/__main__.py` & `dispatch-py-0.5.1/src/dispatch/test/__main__.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/test/client.py` & `dispatch-py-0.5.1/src/dispatch/test/client.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/test/server.py` & `dispatch-py-0.5.1/src/dispatch/test/server.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch/test/service.py` & `dispatch-py-0.5.1/src/dispatch/test/service.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/src/dispatch_py.egg-info/PKG-INFO` & `dispatch-py-0.5.1/src/dispatch_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.4.2
+Version: 0.5.1
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
@@ -14,24 +14,27 @@
 Requires-Dist: docopt>=0.6.2
 Requires-Dist: types-docopt>=0.6.11.4
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: typing_extensions>=4.10
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
 Requires-Dist: httpx; extra == "fastapi"
+Provides-Extra: lambda
+Requires-Dist: awslambdaric; extra == "lambda"
 Provides-Extra: dev
 Requires-Dist: black>=24.1.0; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: mypy>=1.8.0; extra == "dev"
 Requires-Dist: pytest==8.0.0; extra == "dev"
 Requires-Dist: fastapi>=0.109.0; extra == "dev"
 Requires-Dist: coverage>=7.4.1; extra == "dev"
 Requires-Dist: requests>=2.31.0; extra == "dev"
 Requires-Dist: types-requests>=2.31.0.20240125; extra == "dev"
 Requires-Dist: uvicorn>=0.28.0; extra == "dev"
+Requires-Dist: awslambdaric-stubs; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.24.0; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.9; extra == "docs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "docs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "docs"
 Requires-Dist: mike==2.0.0; extra == "docs"
```

### Comparing `dispatch-py-0.4.2/src/dispatch_py.egg-info/SOURCES.txt` & `dispatch-py-0.5.1/src/dispatch_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/dispatch/function.py
 src/dispatch/id.py
 src/dispatch/proto.py
 src/dispatch/py.typed
 src/dispatch/scheduler.py
 src/dispatch/status.py
 src/dispatch/experimental/__init__.py
+src/dispatch/experimental/lambda_handler.py
 src/dispatch/experimental/durable/README.md
 src/dispatch/experimental/durable/__init__.py
 src/dispatch/experimental/durable/frame.c
 src/dispatch/experimental/durable/frame.pyi
 src/dispatch/experimental/durable/frame308.h
 src/dispatch/experimental/durable/frame309.h
 src/dispatch/experimental/durable/frame310.h
```

### Comparing `dispatch-py-0.4.2/src/dispatch_py.egg-info/requires.txt` & `dispatch-py-0.5.1/src/dispatch_py.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,19 +15,23 @@
 mypy>=1.8.0
 pytest==8.0.0
 fastapi>=0.109.0
 coverage>=7.4.1
 requests>=2.31.0
 types-requests>=2.31.0.20240125
 uvicorn>=0.28.0
+awslambdaric-stubs
 
 [docs]
 mkdocs==1.5.3
 mkdocstrings[python]==0.24.0
 mkdocs-material==9.5.9
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mike==2.0.0
 
 [fastapi]
 fastapi
 httpx
+
+[lambda]
+awslambdaric
```

### Comparing `dispatch-py-0.4.2/tests/test_client.py` & `dispatch-py-0.5.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.4.2/tests/test_fastapi.py` & `dispatch-py-0.5.1/tests/test_fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import os
 import pickle
+import struct
 import unittest
 from typing import Any
 from unittest import mock
 
 import fastapi
 import google.protobuf.any_pb2
 import google.protobuf.wrappers_pb2
@@ -35,15 +36,14 @@
         endpoint=endpoint,
         api_key="0000000000000000",
         api_url="http://127.0.0.1:10000",
     )
 
 
 class TestFastAPI(unittest.TestCase):
-
     def test_Dispatch(self):
         app = fastapi.FastAPI()
         create_dispatch_instance(app, "https://127.0.0.1:9999")
 
         @app.get("/")
         def read_root():
             return {"Hello": "World"}
@@ -279,27 +279,27 @@
             "This input is for a first function call", resp.exit.result.error.message
         )
 
     def test_error_on_access_input_in_second_call(self):
         @self.dispatch.primitive_function
         def my_function(input: Input) -> Output:
             if input.is_first_call:
-                return Output.poll(state=42)
+                return Output.poll(coroutine_state=b"42")
             try:
                 print(input.input)
             except ValueError:
                 return Output.error(
                     Error.from_exception(
                         ValueError("This input is for a resumed coroutine")
                     )
                 )
             return Output.value("not reached")
 
         resp = self.execute(my_function, input="cool stuff")
-        self.assertEqual(42, pickle.loads(resp.poll.coroutine_state))
+        self.assertEqual(b"42", resp.poll.coroutine_state)
 
         resp = self.execute(my_function, state=resp.poll.coroutine_state)
         self.assertEqual("ValueError", resp.exit.result.error.type)
         self.assertEqual(
             "This input is for a resumed coroutine", resp.exit.result.error.message
         )
 
@@ -334,19 +334,20 @@
 
     def test_coroutine_with_state(self):
         @self.dispatch.primitive_function
         def coroutine3(input: Input) -> Output:
             if input.is_first_call:
                 counter = input.input
             else:
-                counter = input.coroutine_state
+                (counter,) = struct.unpack("@i", input.coroutine_state)
             counter -= 1
             if counter <= 0:
                 return Output.value("done")
-            return Output.poll(state=counter)
+            coroutine_state = struct.pack("@i", counter)
+            return Output.poll(coroutine_state=coroutine_state)
 
         # first call
         resp = self.execute(coroutine3, input=4)
         state = resp.poll.coroutine_state
         self.assertTrue(len(state) > 0)
 
         # resume, state = 3
@@ -372,17 +373,18 @@
             return Output.value(len(input.input))
 
         @self.dispatch.primitive_function
         def coroutine_main(input: Input) -> Output:
             if input.is_first_call:
                 text: str = input.input
                 return Output.poll(
-                    state=text, calls=[coro_compute_len._build_primitive_call(text)]
+                    coroutine_state=text.encode(),
+                    calls=[coro_compute_len._build_primitive_call(text)],
                 )
-            text = input.coroutine_state
+            text = input.coroutine_state.decode()
             length = input.call_results[0].output
             return Output.value(f"length={length} text='{text}'")
 
         resp = self.execute(coroutine_main, input="cool stuff")
 
         # main saved some state
         state = resp.poll.coroutine_state
@@ -412,15 +414,16 @@
             return Output.error(Error(Status.PERMANENT_ERROR, "type", "Dead"))
 
         @self.dispatch.primitive_function
         def coroutine_main(input: Input) -> Output:
             if input.is_first_call:
                 text: str = input.input
                 return Output.poll(
-                    state=text, calls=[coro_compute_len._build_primitive_call(text)]
+                    coroutine_state=text.encode(),
+                    calls=[coro_compute_len._build_primitive_call(text)],
                 )
             error = input.call_results[0].error
             if error is not None:
                 return Output.value(f"msg={error.message} type='{error.type}'")
             else:
                 raise RuntimeError(f"unexpected call results: {input.call_results}")
```

### Comparing `dispatch-py-0.4.2/tests/test_full.py` & `dispatch-py-0.5.1/tests/test_full.py`

 * *Files identical despite different names*

