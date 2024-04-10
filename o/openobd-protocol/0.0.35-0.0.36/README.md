# Comparing `tmp/openobd-protocol-0.0.35.tar.gz` & `tmp/openobd-protocol-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-protocol-0.0.35.tar", last modified: Tue Apr  9 11:44:29 2024, max compression
+gzip compressed data, was "openobd-protocol-0.0.36.tar", last modified: Wed Apr 10 14:28:04 2024, max compression
```

## Comparing `openobd-protocol-0.0.35.tar` & `openobd-protocol-0.0.36.tar`

### file list

```diff
@@ -1,46 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 11:44:29.963477 openobd-protocol-0.0.35/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.943476 openobd-protocol-0.0.35/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.953476 openobd-protocol-0.0.35/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.957476 openobd-protocol-0.0.35/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2376 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2994 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3706 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ModuleConfiguration_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/ObdMessage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3032 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    14057 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.959476 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     1961 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     9440 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.961476 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     2008 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6578 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-09 11:44:24.000000 openobd-protocol-0.0.35/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:44:29.962477 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1698 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-09 11:44:29.000000 openobd-protocol-0.0.35/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.034864 openobd-protocol-0.0.36/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.041864 openobd-protocol-0.0.36/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.046864 openobd-protocol-0.0.36/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.048864 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     1940 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     9440 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.051864 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.052864 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd-protocol-0.0.35/LICENSE` & `openobd-protocol-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/PKG-INFO` & `openobd-protocol-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.35
+Version: 0.0.36
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.35/pyproject.toml` & `openobd-protocol-0.0.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/Authentication_pb2.pyi` & `openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/BasicResponse_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,25 +10,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
-from openobd_protocol import ModuleConfiguration_pb2 as openobd__protocol_dot_ModuleConfiguration__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
-from openobd_protocol import ObdMessage_pb2 as openobd__protocol_dot_ObdMessage__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.CAN import Isotp_pb2 as openobd__protocol_dot_CAN_dot_Isotp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&openobd_protocol/CAN/CanServices.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a*openobd_protocol/ModuleConfiguration.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a!openobd_protocol/ObdMessage.proto\x1a\x1dopenobd_protocol/Status.proto\x1a openobd_protocol/CAN/Isotp.proto2\xf0\x01\n\x0b\x43\x61nServices\x12j\n\x04send\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00\x12u\n\x0bopenChannel\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&openobd_protocol/CAN/CanServices.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto\x1a openobd_protocol/CAN/Isotp.proto2\xf0\x01\n\x0b\x43\x61nServices\x12j\n\x04send\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00\x12u\n\x0bopenChannel\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.CAN.CanServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_CANSERVICES']._serialized_start=340
-  _globals['_CANSERVICES']._serialized_end=580
+  _globals['_CANSERVICES']._serialized_start=261
+  _globals['_CANSERVICES']._serialized_end=501
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
-from openobd_protocol import ModuleConfiguration_pb2 as openobd__protocol_dot_ModuleConfiguration__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
-from openobd_protocol import ObdMessage_pb2 as openobd__protocol_dot_ObdMessage__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a*openobd_protocol/ModuleConfiguration.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a!openobd_protocol/ObdMessage.proto\x1a\x1dopenobd_protocol/Status.proto2\xd4\x06\n\x18RemoteDiagnosticServices\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12}\n\x0c\x41uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12\x86\x01\n\x15RefreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12y\n\x1arequestModuleConfiguration\x12\x32.com.jifeline.OpenOBD.Protocol.ModuleConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Result\"\x00\x12h\n\x0esendObdMessage\x12).com.jifeline.OpenOBD.Protocol.ObdMessage\x1a).com.jifeline.OpenOBD.Protocol.ObdMessage\"\x00\x12s\n\x15openObdMessageChannel\x12).com.jifeline.OpenOBD.Protocol.ObdMessage\x1a).com.jifeline.OpenOBD.Protocol.ObdMessage\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto2\xfa\x03\n\x18RemoteDiagnosticServices\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12}\n\x0c\x41uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12\x86\x01\n\x15RefreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.RemoteDiagnosticServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_REMOTEDIAGNOSTICSERVICES']._serialized_start=311
-  _globals['_REMOTEDIAGNOSTICSERVICES']._serialized_end=1163
+  _globals['_REMOTEDIAGNOSTICSERVICES']._serialized_start=232
+  _globals['_REMOTEDIAGNOSTICSERVICES']._serialized_end=738
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
-from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
-from openobd_protocol import ModuleConfiguration_pb2 as openobd__protocol_dot_ModuleConfiguration__pb2
-from openobd_protocol import ObdMessage_pb2 as openobd__protocol_dot_ObdMessage__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
 class RemoteDiagnosticServicesStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
@@ -35,29 +32,14 @@
                 response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
                 )
         self.RefreshAuthentication = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/RefreshAuthentication',
                 request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
                 )
-        self.requestModuleConfiguration = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/requestModuleConfiguration',
-                request_serializer=openobd__protocol_dot_ModuleConfiguration__pb2.ModuleConfiguration.SerializeToString,
-                response_deserializer=openobd__protocol_dot_BasicResponse__pb2.Result.FromString,
-                )
-        self.sendObdMessage = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/sendObdMessage',
-                request_serializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-                response_deserializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-                )
-        self.openObdMessageChannel = channel.stream_stream(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/openObdMessageChannel',
-                request_serializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-                response_deserializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-                )
 
 
 class RemoteDiagnosticServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def configureBus(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -79,32 +61,14 @@
 
     def RefreshAuthentication(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def requestModuleConfiguration(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def sendObdMessage(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def openObdMessageChannel(self, request_iterator, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_RemoteDiagnosticServicesServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'configureBus': grpc.unary_unary_rpc_method_handler(
                     servicer.configureBus,
                     request_deserializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
@@ -120,29 +84,14 @@
                     response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
             ),
             'RefreshAuthentication': grpc.unary_unary_rpc_method_handler(
                     servicer.RefreshAuthentication,
                     request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
                     response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
             ),
-            'requestModuleConfiguration': grpc.unary_unary_rpc_method_handler(
-                    servicer.requestModuleConfiguration,
-                    request_deserializer=openobd__protocol_dot_ModuleConfiguration__pb2.ModuleConfiguration.FromString,
-                    response_serializer=openobd__protocol_dot_BasicResponse__pb2.Result.SerializeToString,
-            ),
-            'sendObdMessage': grpc.unary_unary_rpc_method_handler(
-                    servicer.sendObdMessage,
-                    request_deserializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-                    response_serializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-            ),
-            'openObdMessageChannel': grpc.stream_stream_rpc_method_handler(
-                    servicer.openObdMessageChannel,
-                    request_deserializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-                    response_serializer=openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -212,58 +161,7 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/RefreshAuthentication',
             openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
             openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def requestModuleConfiguration(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/requestModuleConfiguration',
-            openobd__protocol_dot_ModuleConfiguration__pb2.ModuleConfiguration.SerializeToString,
-            openobd__protocol_dot_BasicResponse__pb2.Result.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def sendObdMessage(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/sendObdMessage',
-            openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-            openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def openObdMessageChannel(request_iterator,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/openObdMessageChannel',
-            openobd__protocol_dot_ObdMessage__pb2.ObdMessage.SerializeToString,
-            openobd__protocol_dot_ObdMessage__pb2.ObdMessage.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: openobd_protocol/SessionController/AuthenticationServices.proto
+# source: openobd_protocol/SessionController/SessionServices.proto
 # Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?openobd_protocol/SessionController/AuthenticationServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto2\xf4\x03\n\x0fSessionServices\x12\x61\n\x0fgetSessionToken\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rcreateSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\\\n\ngetSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rdeleteSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12^\n\x0clistSessions\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto2\xf4\x03\n\x0fSessionServices\x12\x61\n\x0fgetSessionToken\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rcreateSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\\\n\ngetSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rdeleteSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12^\n\x0clistSessions\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.AuthenticationServices_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_SESSIONSERVICES']._serialized_start=148
-  _globals['_SESSIONSERVICES']._serialized_end=648
+  _globals['_SESSIONSERVICES']._serialized_start=141
+  _globals['_SESSIONSERVICES']._serialized_end=641
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/SessionController/AuthenticationServices_pb2_grpc.py` & `openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/Status_pb2.pyi` & `openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol.UserInterface import UserInterface_pb2 as openobd__protocol_dot_UserInterface_dot_UserInterface__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:openobd_protocol/UserInterface/UserInterfaceServices.proto\x12+com.jifeline.OpenOBD.Protocol.UserInterface\x1a\x32openobd_protocol/UserInterface/UserInterface.proto\x1a\x1dopenobd_protocol/Status.proto2\x87\x03\n\x15UserInterfaceServices\x12q\n\nattachForm\x12:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x87\x01\n\x07\x63ontrol\x12:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\x1a:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\"\x00(\x01\x30\x01\x12q\n\ndetachForm\x12:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:openobd_protocol/UserInterface/UserInterfaceServices.proto\x12+com.jifeline.OpenOBD.Protocol.UserInterface\x1a\x32openobd_protocol/UserInterface/UserInterface.proto\x1a\x1dopenobd_protocol/Status.proto2\xa1\x01\n\x15UserInterfaceServices\x12\x87\x01\n\x07\x63ontrol\x12:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\x1a:.com.jifeline.OpenOBD.Protocol.UserInterface.UserInterface\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.UserInterface.UserInterfaceServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_USERINTERFACESERVICES']._serialized_start=191
-  _globals['_USERINTERFACESERVICES']._serialized_end=582
+  _globals['_USERINTERFACESERVICES']._serialized_end=352
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol.egg-info/PKG-INFO` & `openobd-protocol-0.0.36/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.35
+Version: 0.0.36
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.35/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd-protocol-0.0.36/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 pyproject.toml
 src/openobd_protocol/Authentication_pb2.py
 src/openobd_protocol/Authentication_pb2.pyi
 src/openobd_protocol/BasicResponse_pb2.py
 src/openobd_protocol/BasicResponse_pb2.pyi
 src/openobd_protocol/BusConfiguration_pb2.py
 src/openobd_protocol/BusConfiguration_pb2.pyi
-src/openobd_protocol/ModuleConfiguration_pb2.py
-src/openobd_protocol/ModuleConfiguration_pb2.pyi
-src/openobd_protocol/ObdMessage_pb2.py
-src/openobd_protocol/ObdMessage_pb2.pyi
 src/openobd_protocol/RemoteDiagnosticServices_pb2.py
 src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
 src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
 src/openobd_protocol/Status_pb2.py
 src/openobd_protocol/Status_pb2.pyi
 src/openobd_protocol/__init__.py
 src/openobd_protocol.egg-info/PKG-INFO
@@ -23,15 +19,15 @@
 src/openobd_protocol.egg-info/requires.txt
 src/openobd_protocol.egg-info/top_level.txt
 src/openobd_protocol/CAN/CanServices_pb2.py
 src/openobd_protocol/CAN/CanServices_pb2.pyi
 src/openobd_protocol/CAN/CanServices_pb2_grpc.py
 src/openobd_protocol/CAN/Isotp_pb2.py
 src/openobd_protocol/CAN/Isotp_pb2.pyi
-src/openobd_protocol/SessionController/AuthenticationServices_pb2.py
-src/openobd_protocol/SessionController/AuthenticationServices_pb2.pyi
-src/openobd_protocol/SessionController/AuthenticationServices_pb2_grpc.py
+src/openobd_protocol/SessionController/SessionServices_pb2.py
+src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
```

