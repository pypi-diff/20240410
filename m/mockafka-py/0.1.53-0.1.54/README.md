# Comparing `tmp/mockafka_py-0.1.53.tar.gz` & `tmp/mockafka_py-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockafka_py-0.1.53.tar", max compression
+gzip compressed data, was "mockafka_py-0.1.54.tar", max compression
```

## Comparing `mockafka_py-0.1.53.tar` & `mockafka_py-0.1.54.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/LICENSE
--rw-r--r--   0        0        0     6491 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/README.md
--rw-r--r--   0        0        0      465 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/mockafka/__init__.py
--rw-r--r--   0        0        0     7147 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/mockafka/admin_client.py
--rw-r--r--   0        0        0      252 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/mockafka/aiokafka/__init__.py
--rw-r--r--   0        0        0     2425 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_admin_client.py
--rw-r--r--   0        0        0     3434 2024-03-23 13:34:22.766797 mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_consumer.py
--rw-r--r--   0        0        0     2050 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_producer.py
--rw-r--r--   0        0        0      522 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/broker_metadata.py
--rw-r--r--   0        0        0     1300 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/cluster_metadata.py
--rw-r--r--   0        0        0    11750 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/conumser.py
--rw-r--r--   0        0        0      376 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/__init__.py
--rw-r--r--   0        0        0     1825 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/aconsumer.py
--rw-r--r--   0        0        0     1769 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/aproducer.py
--rw-r--r--   0        0        0     1620 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/asetup_kafka.py
--rw-r--r--   0        0        0     1956 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/bulk_producer.py
--rw-r--r--   0        0        0     1366 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/consumer.py
--rw-r--r--   0        0        0     1524 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/producer.py
--rw-r--r--   0        0        0     1373 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/decorators/setup_kafka.py
--rw-r--r--   0        0        0     6283 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/kafka_store.py
--rw-r--r--   0        0        0     1643 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/message.py
--rw-r--r--   0        0        0     1579 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/producer.py
--rw-r--r--   0        0        0      798 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/mockafka/topic_metadata.py
--rw-r--r--   0        0        0      850 2024-03-23 13:34:22.770797 mockafka_py-0.1.53/pyproject.toml
--rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 mockafka_py-0.1.53/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-10 08:04:55.410152 mockafka_py-0.1.54/LICENSE
+-rw-r--r--   0        0        0     6491 2024-04-10 08:04:55.410152 mockafka_py-0.1.54/README.md
+-rw-r--r--   0        0        0      465 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/__init__.py
+-rw-r--r--   0        0        0     7147 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/admin_client.py
+-rw-r--r--   0        0        0      252 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/__init__.py
+-rw-r--r--   0        0        0     2425 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_admin_client.py
+-rw-r--r--   0        0        0     3434 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_consumer.py
+-rw-r--r--   0        0        0     2050 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_producer.py
+-rw-r--r--   0        0        0      522 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/broker_metadata.py
+-rw-r--r--   0        0        0     1282 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/cluster_metadata.py
+-rw-r--r--   0        0        0    11791 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/conumser.py
+-rw-r--r--   0        0        0      376 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/aconsumer.py
+-rw-r--r--   0        0        0     1769 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/aproducer.py
+-rw-r--r--   0        0        0     1620 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/asetup_kafka.py
+-rw-r--r--   0        0        0     1956 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/bulk_producer.py
+-rw-r--r--   0        0        0     1366 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/consumer.py
+-rw-r--r--   0        0        0     1524 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/producer.py
+-rw-r--r--   0        0        0     1373 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/decorators/setup_kafka.py
+-rw-r--r--   0        0        0     6283 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/kafka_store.py
+-rw-r--r--   0        0        0     1643 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/message.py
+-rw-r--r--   0        0        0     1579 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/producer.py
+-rw-r--r--   0        0        0      798 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/mockafka/topic_metadata.py
+-rw-r--r--   0        0        0      879 2024-04-10 08:04:55.414152 mockafka_py-0.1.54/pyproject.toml
+-rw-r--r--   0        0        0     7414 1970-01-01 00:00:00.000000 mockafka_py-0.1.54/PKG-INFO
```

### Comparing `mockafka_py-0.1.53/LICENSE` & `mockafka_py-0.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/README.md` & `mockafka_py-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/admin_client.py` & `mockafka_py-0.1.54/mockafka/admin_client.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_admin_client.py` & `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_admin_client.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_consumer.py` & `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_consumer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/aiokafka/aiokafka_producer.py` & `mockafka_py-0.1.54/mockafka/aiokafka/aiokafka_producer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/broker_metadata.py` & `mockafka_py-0.1.54/mockafka/broker_metadata.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/cluster_metadata.py` & `mockafka_py-0.1.54/mockafka/cluster_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Returned by list_topics().
 
     This class is typically not user instantiated.
     """
 
     def __init__(self, topic: str = None):
         self.kafka = KafkaStore()
-        self.cluster_id = 'eAvlnr_4QISNbc5bIwBRVA'
+        self.cluster_id = 'test'
         self.controller_id = 1
         self.brokers = {1: BrokerMetadata()}
         self.topics = CustomDict()
         if topic:
             if self.kafka.is_topic_exist(topic=topic):
                 self.topics[topic] = TopicMetadata(topic, self.kafka.partition_list(topic=topic))
```

### Comparing `mockafka_py-0.1.53/mockafka/conumser.py` & `mockafka_py-0.1.54/mockafka/conumser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from time import sleep
+import warnings
 
 from mockafka.cluster_metadata import ClusterMetadata
 from mockafka.message import Message
 from mockafka.kafka_store import KafkaStore, KafkaException
 
 __all__ = ["FakeConsumer"]
 
@@ -80,22 +80,23 @@
 
         Parameters:
         - message (Message): Consumed message (unused).
         - args: Additional arguments (unused).
         - kwargs: Additional keyword arguments (unused).
         """
         if message:
-            pass  # Commit offsets by changing offset of the topic (not implemented yet)
-        else:
-            for item in self.consumer_store:
-                topic, partition = item.split('*')
-                if self.kafka.get_partition_first_offset(topic, partition) <= self.consumer_store[item]:
-                    self.kafka.set_first_offset(topic=topic, partition=partition, value=self.consumer_store[item])
+            warnings.warn("commit a specific message is not yet implemented in mockafka and it act like commit a "
+                          "consumer entire messages ")
 
-            self.consumer_store = {}
+        for item in self.consumer_store:
+            topic, partition = item.split('*')
+            if self.kafka.get_partition_first_offset(topic, partition) <= self.consumer_store[item]:
+                self.kafka.set_first_offset(topic=topic, partition=partition, value=self.consumer_store[item])
+
+        self.consumer_store = {}
 
     def list_topics(self, topic=None, *args, **kwargs):
         """
         List topics (returns ClusterMetadata).
 
         Parameters:
         - topic: Topic name (unused).
```

### Comparing `mockafka_py-0.1.53/mockafka/decorators/aconsumer.py` & `mockafka_py-0.1.54/mockafka/decorators/aconsumer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/aproducer.py` & `mockafka_py-0.1.54/mockafka/decorators/aproducer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/asetup_kafka.py` & `mockafka_py-0.1.54/mockafka/decorators/asetup_kafka.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/bulk_producer.py` & `mockafka_py-0.1.54/mockafka/decorators/bulk_producer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/consumer.py` & `mockafka_py-0.1.54/mockafka/decorators/consumer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/producer.py` & `mockafka_py-0.1.54/mockafka/decorators/producer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/decorators/setup_kafka.py` & `mockafka_py-0.1.54/mockafka/decorators/setup_kafka.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/kafka_store.py` & `mockafka_py-0.1.54/mockafka/kafka_store.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/message.py` & `mockafka_py-0.1.54/mockafka/message.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/producer.py` & `mockafka_py-0.1.54/mockafka/producer.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/mockafka/topic_metadata.py` & `mockafka_py-0.1.54/mockafka/topic_metadata.py`

 * *Files identical despite different names*

### Comparing `mockafka_py-0.1.53/pyproject.toml` & `mockafka_py-0.1.54/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "mockafka-py"
-version = "0.1.53"
+version = "0.1.54"
 authors = ["alm0ra <ali.mrd318@gmail.com>"]
 repository = "https://github.com/alm0ra/mockafka-py"
 documentation = "https://github.com/alm0ra/mockafka-py/docs"
 
 
 description = "A mock library for confluent kafka"
 readme = "README.md"
 packages = [{ include = "mockafka" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 confluent-kafka = ">= 1.9.2"
 aiokafka = "^0.10.0"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-asyncio = "^0.23.5"
+parameterized = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2,<9.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 mypy = "^1.5.1"
 pre-commit = "^3.4.0"
 tox = "^4.11.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.2.7"
```

### Comparing `mockafka_py-0.1.53/PKG-INFO` & `mockafka_py-0.1.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mockafka-py
-Version: 0.1.53
+Version: 0.1.54
 Summary: A mock library for confluent kafka
 Home-page: https://github.com/alm0ra/mockafka-py
 Author: alm0ra
 Author-email: ali.mrd318@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiokafka (>=0.10.0,<0.11.0)
 Requires-Dist: confluent-kafka (>=1.9.2)
+Requires-Dist: parameterized (>=0.9.0,<0.10.0)
 Requires-Dist: pytest-asyncio (>=0.23.5,<0.24.0)
-Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
+Requires-Dist: pytest-cov (>=4.1,<6.0)
 Project-URL: Documentation, https://github.com/alm0ra/mockafka-py/docs
 Project-URL: Repository, https://github.com/alm0ra/mockafka-py
 Description-Content-Type: text/markdown
 
 ![Alt text](banner.png)
 <p align="center">
     <em>Mockafka-py is a Python library designed for in-memory mocking of Kafka.</em>
```

