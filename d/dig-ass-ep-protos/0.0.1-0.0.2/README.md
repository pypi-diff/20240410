# Comparing `tmp/dig_ass_ep_protos-0.0.1.tar.gz` & `tmp/dig_ass_ep_protos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-0.0.1.tar", last modified: Wed Apr 10 11:15:40 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-0.0.2.tar", last modified: Wed Apr 10 14:20:14 2024, max compression
```

## Comparing `dig_ass_ep_protos-0.0.1.tar` & `dig_ass_ep_protos-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 11:15:40.360397 dig_ass_ep_protos-0.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 11:15:40.360397 dig_ass_ep_protos-0.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 11:15:40.360397 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2173 2024-04-10 11:15:39.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-10 11:15:39.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-10 11:15:39.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      973 2024-04-10 11:09:18.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 11:15:40.360397 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 11:15:40.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      471 2024-04-10 11:15:40.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-10 11:15:40.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-10 11:15:40.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-10 11:15:40.000000 dig_ass_ep_protos-0.0.1/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-10 11:15:40.360397 dig_ass_ep_protos-0.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      793 2024-04-10 09:02:25.000000 dig_ass_ep_protos-0.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:20:14.815061 dig_ass_ep_protos-0.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 14:20:14.815061 dig_ass_ep_protos-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:20:14.811062 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2171 2024-04-10 14:20:13.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-10 14:20:13.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-10 14:20:13.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-10 14:18:41.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      973 2024-04-10 11:09:18.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:20:14.815061 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 14:20:14.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      471 2024-04-10 14:20:14.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-10 14:20:14.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-10 14:20:14.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-10 14:20:14.000000 dig_ass_ep_protos-0.0.2/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-10 14:20:14.815061 dig_ass_ep_protos-0.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      793 2024-04-10 09:02:25.000000 dig_ass_ep_protos-0.0.2/setup.py
```

### Comparing `dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\x05\x12\x0e\n\x06UserId\x18\x03 \x01(\x05\x12\x11\n\tSessionId\x18\x04 \x01(\x05\x32\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\x05\x32\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTENTRYPOINTRESPONSE']._serialized_start=69
```

### Comparing `dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.1/dig_ass_ep_protos/client.py` & `dig_ass_ep_protos-0.0.2/dig_ass_ep_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.1/setup.py` & `dig_ass_ep_protos-0.0.2/setup.py`

 * *Files identical despite different names*

