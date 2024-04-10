# Comparing `tmp/robotframework-confluentkafkalibrary-2.0.2.post4.tar.gz` & `tmp/robotframework-confluentkafkalibrary-2.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post4.tar", last modified: Thu Apr  4 22:05:32 2024, max compression
+gzip compressed data, was "robotframework-confluentkafkalibrary-2.1.1.post1.tar", last modified: Wed Apr 10 19:32:30 2024, max compression
```

## Comparing `robotframework-confluentkafkalibrary-2.0.2.post4.tar` & `robotframework-confluentkafkalibrary-2.1.1.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.013607 robotframework-confluentkafkalibrary-2.0.2.post4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 22:05:28.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:05:32.017607 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 22:05:32.000000 robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:30.342513 robotframework-confluentkafkalibrary-2.1.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-10 19:32:30.342513 robotframework-confluentkafkalibrary-2.1.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:32:30.342513 robotframework-confluentkafkalibrary-2.1.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:30.338513 robotframework-confluentkafkalibrary-2.1.1.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:30.338513 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 19:32:26.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:30.338513 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-10 19:32:30.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 19:32:30.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:32:30.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-10 19:32:30.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 19:32:30.000000 robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/LICENSE` & `robotframework-confluentkafkalibrary-2.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/PKG-INFO` & `robotframework-confluentkafkalibrary-2.1.1.post1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post4
+Version: 2.1.1.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 Requires-Dist: robotframework>=3.2.1
-Requires-Dist: confluent-kafka==2.0.2
+Requires-Dist: confluent-kafka==2.1.1
 Requires-Dist: requests>=2.25.1
-Requires-Dist: avro-python3>=1.10.1
-Requires-Dist: fastavro>=1.3.2
-Requires-Dist: jsonschema>=3.2.0
-Requires-Dist: protobuf>=4.22.0
+Provides-Extra: all
+Requires-Dist: fastavro>=1.3.2; extra == "all"
+Requires-Dist: avro-python3>=1.10.1; extra == "all"
+Requires-Dist: jsonschema>=3.2.0; extra == "all"
+Requires-Dist: protobuf>=4.22.0; extra == "all"
+Provides-Extra: avro
+Requires-Dist: fastavro>=1.3.2; extra == "avro"
+Requires-Dist: avro-python3>=1.10.1; extra == "avro"
+Provides-Extra: json
+Requires-Dist: jsonschema>=3.2.0; extra == "json"
+Provides-Extra: protobuf
+Requires-Dist: protobuf>=4.22.0; extra == "protobuf"
 
 Confluent Kafka wrapped in Robot Framework.
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/README.md` & `robotframework-confluentkafkalibrary-2.1.1.post1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -18,14 +18,25 @@
 
 To install the library, run the following command:
 
 ```
 pip install robotframework-confluentkafkalibrary
 ```
 
+Extra packages:
+* [avro] = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
+* [json] = ['jsonschema >= 3.2.0']
+* [protobuf] = ['protobuf >= 4.22.0']
+
+To install all dependencies use `[all]` extension like:
+
+```
+pip install robotframework-confluentkafkalibrary[all]
+```
+
 ## Usage
 
 In most cases, you can refer to the [confluent-kafka-python documentation](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html) for guidance. Every keyword in ConfluentKafkaLibrary is designed to match the corresponding Python functions. If you are unsure about the pre-configured keywords, please visit the  [robotframework-ConfluentKafkaLibrary documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/). The Kafka team maintains the up-to-date documentation for configuration properties and their values [here](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md).
 
 * You can find basic usage examples in the [./examples/test.robot](./examples/test.robot)
 * For more complex examples, such as handling byte data from a topic, using multiple consumers, or running threaded avro consumers, please refer to the [documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/#Examples).
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/setup.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 filename=join(dirname(__file__), 'src', 'ConfluentKafkaLibrary', 'version.py')
 exec(compile(open(filename).read(),filename, 'exec'))
 
 DESCRIPTION = """
 Confluent Kafka wrapped in Robot Framework.
 """[1:-1]
 
+AVRO_REQUIRES = ['fastavro >= 1.3.2', 'avro-python3 >= 1.10.1']
+JSON_REQUIRES = ['jsonschema >= 3.2.0']
+PROTO_REQUIRES = ['protobuf >= 4.22.0']
+ALL = AVRO_REQUIRES + JSON_REQUIRES + PROTO_REQUIRES
 setup(name         = 'robotframework-confluentkafkalibrary',
       version      = VERSION,
       description  = 'Confluent Kafka library for Robot Framework',
       long_description = DESCRIPTION,
       author       = 'Robert Karasek',
       author_email = '<robo.karasek@gmail.com>',
       url          = 'https://github.com/robooo/robotframework-ConfluentKafkaLibrary',
@@ -24,17 +28,19 @@
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
           "Programming Language :: Python",
           "Topic :: Software Development :: Testing"
       ],
       install_requires = [
           'robotframework >= 3.2.1',
-          'confluent-kafka == 2.0.2',
+          'confluent-kafka == 2.1.1',
           'requests >= 2.25.1',
-          'avro-python3 >= 1.10.1',
-          'fastavro >= 1.3.2',
-          'jsonschema >= 3.2.0',
-          'protobuf >= 4.22.0'
       ],
+      extras_require={
+          'all': ALL,
+          'avro': AVRO_REQUIRES,
+          'json': JSON_REQUIRES,
+          'protobuf': PROTO_REQUIRES,
+      },
       package_dir  = {'' : 'src'},
-      packages    = ['ConfluentKafkaLibrary'],
+      packages     = ['ConfluentKafkaLibrary'],
       )
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/__init__.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import confluent_kafka
 from confluent_kafka import ConsumerGroupState
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.admin import AdminClient, NewTopic, NewPartitions, ConfigResource
 from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
-
 from .consumer import KafkaConsumer
 from .producer import KafkaProducer
 from .admin_client import KafkaAdminClient
-from .serialization import Serializer, Deserializer
 from .version import VERSION
 
+IMPORTS = KafkaConsumer, KafkaProducer, KafkaAdminClient
+try:
+    from .serialization import Serializer, Deserializer
+    IMPORTS += Serializer, Deserializer
+except ImportError:
+    pass
 
 #class ConfluentKafkaLibrary(KafkaConsumer, KafkaProducer, Serializer, Deserializer):
-class ConfluentKafkaLibrary(KafkaConsumer, KafkaProducer, KafkaAdminClient, Serializer, Deserializer):
+class ConfluentKafkaLibrary(*IMPORTS):
     """ConfluentKafkaLibrary is a Robot Framework library which wraps up
     [https://github.com/confluentinc/confluent-kafka-python | confluent-kafka-python].
     Library supports more functionality like running more clients based on `group_id`
     or running them in threaded mode during the tests, decoding of gathered data etc. (`See` `Examples`).
 
     This document explains how to use keywords provided by ConfluentKafkaLibrary.
     For information about installation, support, and more, please visit the
@@ -85,15 +89,15 @@
             BuiltIn().set_global_variable('${OFFSET_END}', confluent_kafka.OFFSET_END)
             BuiltIn().set_global_variable('${OFFSET_STORED}', confluent_kafka.OFFSET_STORED)
             BuiltIn().set_global_variable('${OFFSET_INVALID}', confluent_kafka.OFFSET_INVALID)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_BROKER}', confluent_kafka.admin.RESOURCE_BROKER)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_GROUP}', confluent_kafka.admin.RESOURCE_GROUP)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_TOPIC}', confluent_kafka.admin.RESOURCE_TOPIC)
 
-            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_UNKNOWN}', confluent_kafka.ConsumerGroupState.UNKOWN)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_UNKNOWN}', confluent_kafka.ConsumerGroupState.UNKNOWN)
             BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_PREPARING_REBALANCING}', confluent_kafka.ConsumerGroupState.PREPARING_REBALANCING)
             BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_COMPLETING_REBALANCING}', confluent_kafka.ConsumerGroupState.COMPLETING_REBALANCING)
             BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_STABLE}', confluent_kafka.ConsumerGroupState.STABLE)
             BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_DEAD}', confluent_kafka.ConsumerGroupState.DEAD)
             BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_EMPTY}', confluent_kafka.ConsumerGroupState.EMPTY)
 
         except RobotNotRunningError as e:
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/admin_client.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/admin_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/consumer.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import uuid
 from threading import Thread
 from confluent_kafka import Consumer, KafkaException, KafkaError, TopicPartition
 from confluent_kafka import DeserializingConsumer
-from confluent_kafka.avro.serializer import SerializerError
-from confluent_kafka.avro import AvroConsumer
 from confluent_kafka.admin import AdminClient
 
+try:
+    from confluent_kafka.avro.serializer import SerializerError
+    from confluent_kafka.avro import AvroConsumer
+except ImportError:
+    pass
+
 
 class GetMessagesThread(Thread):
 
     def __init__(
         self,
         server='127.0.0.1',
         port='9092',
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/producer.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import uuid
 import os
-from avro import schema
 from confluent_kafka import SerializingProducer
 from confluent_kafka import Producer
-from confluent_kafka import avro
-from confluent_kafka.avro import AvroProducer
 
+try:
+    from avro import schema
+    from confluent_kafka import avro
+    from confluent_kafka.avro import AvroProducer
+except ImportError:
+    pass
 
 class KafkaProducer():
 
     def __init__(self):
         self.producers = {}
 
     def load_schema(self, data):
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/ConfluentKafkaLibrary/serialization.py` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/ConfluentKafkaLibrary/serialization.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post4
+Version: 2.1.1.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 Requires-Dist: robotframework>=3.2.1
-Requires-Dist: confluent-kafka==2.0.2
+Requires-Dist: confluent-kafka==2.1.1
 Requires-Dist: requests>=2.25.1
-Requires-Dist: avro-python3>=1.10.1
-Requires-Dist: fastavro>=1.3.2
-Requires-Dist: jsonschema>=3.2.0
-Requires-Dist: protobuf>=4.22.0
+Provides-Extra: all
+Requires-Dist: fastavro>=1.3.2; extra == "all"
+Requires-Dist: avro-python3>=1.10.1; extra == "all"
+Requires-Dist: jsonschema>=3.2.0; extra == "all"
+Requires-Dist: protobuf>=4.22.0; extra == "all"
+Provides-Extra: avro
+Requires-Dist: fastavro>=1.3.2; extra == "avro"
+Requires-Dist: avro-python3>=1.10.1; extra == "avro"
+Provides-Extra: json
+Requires-Dist: jsonschema>=3.2.0; extra == "json"
+Provides-Extra: protobuf
+Requires-Dist: protobuf>=4.22.0; extra == "protobuf"
 
 Confluent Kafka wrapped in Robot Framework.
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post4/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework-confluentkafkalibrary-2.1.1.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

