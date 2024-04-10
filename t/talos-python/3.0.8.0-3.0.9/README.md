# Comparing `tmp/talos-python-3.0.8.0.tar.gz` & `tmp/talos-python-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talos-python-3.0.8.0.tar", last modified: Mon Jun 27 13:17:02 2022, max compression
+gzip compressed data, was "dist/talos-python-3.0.9.tar", last modified: Mon Nov 20 06:18:18 2023, max compression
```

## Comparing `talos-python-3.0.8.0.tar` & `talos-python-3.0.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/
--rw-r--r--   0 mac        (501) staff       (20)      276 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/PKG-INFO
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/producer/
--rw-r--r--   0 mac        (501) staff       (20)     5031 2022-06-27 12:56:14.000000 talos-python-3.0.8.0/talos/producer/TalosProducerConfigKey.py
--rw-r--r--   0 mac        (501) staff       (20)      693 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/UserMessage.py
--rw-r--r--   0 mac        (501) staff       (20)      643 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/UserMessageCallback.py
--rw-r--r--   0 mac        (501) staff       (20)      234 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/Partitioner.py
--rw-r--r--   0 mac        (501) staff       (20)    18544 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/producer/PartitionSender.py
--rw-r--r--   0 mac        (501) staff       (20)    17269 2022-06-27 12:58:29.000000 talos-python-3.0.8.0/talos/producer/TalosProducer.py
--rw-r--r--   0 mac        (501) staff       (20)      338 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/ProducerNotActiveException.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1301 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/BufferedMessageCount.py
--rw-r--r--   0 mac        (501) staff       (20)     5828 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/producer/PartitionMessageQueue.py
--rw-r--r--   0 mac        (501) staff       (20)     5960 2022-06-27 12:55:58.000000 talos-python-3.0.8.0/talos/producer/TalosProducerConfig.py
--rw-r--r--   0 mac        (501) staff       (20)      430 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/SimplePartitioner.py
--rw-r--r--   0 mac        (501) staff       (20)     6351 2022-06-27 12:55:09.000000 talos-python-3.0.8.0/talos/producer/SimpleProducer.py
--rw-r--r--   0 mac        (501) staff       (20)      920 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/producer/UserMessageResult.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/test/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/test/producer/
--rw-r--r--   0 mac        (501) staff       (20)      942 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/producer/test_UserMessage.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/producer/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7639 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/producer/test_TalosProducer.py
--rw-r--r--   0 mac        (501) staff       (20)     3380 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/producer/test_PartitionMessageQueue.py
--rw-r--r--   0 mac        (501) staff       (20)     6215 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/producer/test_PartitionSender.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/test/admin/
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/admin/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/test/consumer/
--rw-r--r--   0 mac        (501) staff       (20)     5855 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/consumer/test_PartitionFetcher.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/consumer/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24040 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/consumer/test_TalosConsumer.py
--rw-r--r--   0 mac        (501) staff       (20)     1957 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/consumer/test_SimpleConsumer.py
--rw-r--r--   0 mac        (501) staff       (20)     6830 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/consumer/test_TalosMessageReader.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/test/client/
--rw-r--r--   0 mac        (501) staff       (20)      244 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/client/test_socket.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/test/client/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/example/
--rw-r--r--   0 mac        (501) staff       (20)     3405 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/example/TalosConsumerDemo.py
--rw-r--r--   0 mac        (501) staff       (20)     3514 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/example/TalosAdminDemo.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/example/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     2313 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/example/SimpleConsumerDemo.py
--rw-r--r--   0 mac        (501) staff       (20)     2334 2022-06-27 13:04:34.000000 talos-python-3.0.8.0/talos/example/SimpleProducerDemo.py
--rw-r--r--   0 mac        (501) staff       (20)     2774 2022-06-27 13:04:26.000000 talos-python-3.0.8.0/talos/example/TalosProducerDemo.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/admin/
--rw-r--r--   0 mac        (501) staff       (20)     2262 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/admin/TalosAdmin.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/admin/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/utils/
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      693 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/utils/FalconWriter.py
--rw-r--r--   0 mac        (501) staff       (20)     8431 2022-06-27 13:10:01.000000 talos-python-3.0.8.0/talos/utils/Utils.py
--rw-r--r--   0 mac        (501) staff       (20)      590 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/utils/Const.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/transport/
--rw-r--r--   0 mac        (501) staff       (20)    13211 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/TTransport.py
--rw-r--r--   0 mac        (501) staff       (20)    10904 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/TTwisted.py
--rw-r--r--   0 mac        (501) staff       (20)    16389 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/TSSLSocket.py
--rw-r--r--   0 mac        (501) staff       (20)      855 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    12979 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/THeaderTransport.py
--rw-r--r--   0 mac        (501) staff       (20)     8053 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/TSocket.py
--rw-r--r--   0 mac        (501) staff       (20)     3662 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/sslcompat.py
--rw-r--r--   0 mac        (501) staff       (20)     7114 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/THttpClient.py
--rw-r--r--   0 mac        (501) staff       (20)     8778 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/transport/TZlibTransport.py
--rw-r--r--   0 mac        (501) staff       (20)     1315 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/compat.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/auth/
--rw-r--r--   0 mac        (501) staff       (20)      758 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/auth/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       34 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/auth/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    11218 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/auth/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)      817 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3333 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/TRecursive.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/message/
--rw-r--r--   0 mac        (501) staff       (20)      142 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/message/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       52 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/message/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)   107912 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/message/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)    72642 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/message/MessageService.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/server/
--rw-r--r--   0 mac        (501) staff       (20)      830 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/server/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    11784 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/server/TServer.py
--rw-r--r--   0 mac        (501) staff       (20)     4054 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/server/TProcessPoolServer.py
--rw-r--r--   0 mac        (501) staff       (20)     5551 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/server/THttpServer.py
--rw-r--r--   0 mac        (501) staff       (20)    12495 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/server/TNonblockingServer.py
--rw-r--r--   0 mac        (501) staff       (20)     6407 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/TTornado.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/topic/
--rw-r--r--   0 mac        (501) staff       (20)      244 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/topic/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       50 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/topic/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)   101305 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/topic/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)   114771 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/topic/TopicService.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/protocol/
--rw-r--r--   0 mac        (501) staff       (20)     1101 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TProtocolDecorator.py
--rw-r--r--   0 mac        (501) staff       (20)     7401 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/THeaderProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)    19403 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TJSONProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)     1457 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TMultiplexedProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)      922 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9140 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TBinaryProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)     2827 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TBase.py
--rw-r--r--   0 mac        (501) staff       (20)    15465 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TCompactProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)    13480 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/protocol/TProtocol.py
--rw-r--r--   0 mac        (501) staff       (20)     3337 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/TMultiplexedProcessor.py
--rw-r--r--   0 mac        (501) staff       (20)     5843 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/Thrift.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/common/
--rw-r--r--   0 mac        (501) staff       (20)      555 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/common/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       54 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/common/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    13159 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/common/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)    13012 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/common/TalosBaseService.py
--rw-r--r--   0 mac        (501) staff       (20)     1309 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/TSCons.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/quota/
--rw-r--r--   0 mac        (501) staff       (20)      142 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/quota/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       50 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/quota/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    44115 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/quota/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)    60949 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/quota/QuotaService.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/consumer/
--rw-r--r--   0 mac        (501) staff       (20)      143 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/consumer/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       53 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/consumer/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    56579 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/consumer/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)    59460 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/consumer/ConsumerService.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/authorization/
--rw-r--r--   0 mac        (501) staff       (20)      141 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/authorization/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       34 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/authorization/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3125 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/authorization/ttypes.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/thrift/metric/
--rw-r--r--   0 mac        (501) staff       (20)      141 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/metric/constants.py
--rw-r--r--   0 mac        (501) staff       (20)       51 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/metric/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    27643 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/metric/MetricService.py
--rw-r--r--   0 mac        (501) staff       (20)    23130 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/metric/ttypes.py
--rw-r--r--   0 mac        (501) staff       (20)     1389 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/thrift/TSerialization.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/consumer/
--rw-r--r--   0 mac        (501) staff       (20)     1341 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/MessageProcessor.py
--rw-r--r--   0 mac        (501) staff       (20)    10986 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/consumer/TalosMessageReader.py
--rw-r--r--   0 mac        (501) staff       (20)      296 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/MessageReaderFactory.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    10773 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/consumer/MessageReader.py
--rw-r--r--   0 mac        (501) staff       (20)     7165 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/consumer/SimpleConsumer.py
--rw-r--r--   0 mac        (501) staff       (20)    13260 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/consumer/PartitionFetcher.py
--rw-r--r--   0 mac        (501) staff       (20)    29359 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/consumer/TalosConsumer.py
--rw-r--r--   0 mac        (501) staff       (20)     1354 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/MessageCheckpointer.py
--rw-r--r--   0 mac        (501) staff       (20)      163 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/MessageProcessorFactory.py
--rw-r--r--   0 mac        (501) staff       (20)     6030 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/consumer/TalosConsumerConfigKeys.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/client/
--rw-r--r--   0 mac        (501) staff       (20)     7494 2021-11-02 06:42:41.000000 talos-python-3.0.8.0/talos/client/ScheduleInfoCache.py
--rw-r--r--   0 mac        (501) staff       (20)    15710 2022-06-27 02:19:14.000000 talos-python-3.0.8.0/talos/client/TalosClientFactory.py
--rw-r--r--   0 mac        (501) staff       (20)    18902 2022-06-27 12:52:46.000000 talos-python-3.0.8.0/talos/client/TalosClientConfig.py
--rw-r--r--   0 mac        (501) staff       (20)    19008 2022-06-27 02:19:14.000000 talos-python-3.0.8.0/talos/client/TalosHttpClient.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/client/serialization/
--rw-r--r--   0 mac        (501) staff       (20)     3268 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV1.py
--rw-r--r--   0 mac        (501) staff       (20)      567 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerializationFactory.py
--rw-r--r--   0 mac        (501) staff       (20)     1250 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerializer.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     2235 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerialization.py
--rw-r--r--   0 mac        (501) staff       (20)     2531 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV3.py
--rw-r--r--   0 mac        (501) staff       (20)      496 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageVersion.py
--rw-r--r--   0 mac        (501) staff       (20)     6741 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV2.py
--rw-r--r--   0 mac        (501) staff       (20)     1924 2022-06-27 12:05:47.000000 talos-python-3.0.8.0/talos/client/Constants.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      321 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/TopicAbnormalCallback.py
--rw-r--r--   0 mac        (501) staff       (20)      504 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/SimpleAbnormalCallback.py
--rw-r--r--   0 mac        (501) staff       (20)     1546 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/TalosErrors.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos/client/compression/
--rw-r--r--   0 mac        (501) staff       (20)      911 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/compression/Gzip.py
--rw-r--r--   0 mac        (501) staff       (20)     4888 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/compression/Snappy.py
--rw-r--r--   0 mac        (501) staff       (20)     5562 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/compression/Compression.py
--rw-r--r--   0 mac        (501) staff       (20)       85 2021-04-26 12:19:20.000000 talos-python-3.0.8.0/talos/client/compression/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9342 2022-06-27 02:19:14.000000 talos-python-3.0.8.0/talos/client/TalosClientConfigkeys.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      276 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        1 2022-06-27 13:05:49.000000 talos-python-3.0.8.0/talos_python.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)     4963 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)       57 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/talos_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      524 2022-06-27 13:16:49.000000 talos-python-3.0.8.0/setup.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2022-06-27 13:17:02.000000 talos-python-3.0.8.0/setup.cfg
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/
+-rw-r--r--   0 humkum     (501) staff       (20)      274 2023-11-20 06:18:18.000000 talos-python-3.0.9/PKG-INFO
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/producer/
+-rw-r--r--   0 humkum     (501) staff       (20)     5031 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/producer/TalosProducerConfigKey.py
+-rw-r--r--   0 humkum     (501) staff       (20)      693 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/UserMessage.py
+-rw-r--r--   0 humkum     (501) staff       (20)      643 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/UserMessageCallback.py
+-rw-r--r--   0 humkum     (501) staff       (20)      234 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/Partitioner.py
+-rw-r--r--   0 humkum     (501) staff       (20)    18544 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/producer/PartitionSender.py
+-rw-r--r--   0 humkum     (501) staff       (20)    17269 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/producer/TalosProducer.py
+-rw-r--r--   0 humkum     (501) staff       (20)      338 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/ProducerNotActiveException.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1301 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/BufferedMessageCount.py
+-rw-r--r--   0 humkum     (501) staff       (20)     5862 2023-11-16 11:39:15.000000 talos-python-3.0.9/talos/producer/PartitionMessageQueue.py
+-rw-r--r--   0 humkum     (501) staff       (20)     5960 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/producer/TalosProducerConfig.py
+-rw-r--r--   0 humkum     (501) staff       (20)      430 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/SimplePartitioner.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6453 2023-10-20 07:15:03.000000 talos-python-3.0.9/talos/producer/SimpleProducer.py
+-rw-r--r--   0 humkum     (501) staff       (20)      920 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/producer/UserMessageResult.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/test/
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/test/producer/
+-rw-r--r--   0 humkum     (501) staff       (20)      942 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/producer/test_UserMessage.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/producer/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     7639 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/producer/test_TalosProducer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3380 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/producer/test_PartitionMessageQueue.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6215 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/producer/test_PartitionSender.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/test/admin/
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/admin/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)        0 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/__init__.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/test/consumer/
+-rw-r--r--   0 humkum     (501) staff       (20)     5855 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/consumer/test_PartitionFetcher.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/consumer/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    24040 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/consumer/test_TalosConsumer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1957 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/consumer/test_SimpleConsumer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6830 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/consumer/test_TalosMessageReader.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/test/client/
+-rw-r--r--   0 humkum     (501) staff       (20)      244 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/client/test_socket.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/test/client/__init__.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/example/
+-rw-r--r--   0 humkum     (501) staff       (20)     3405 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/example/TalosConsumerDemo.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3514 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/example/TalosAdminDemo.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/example/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2313 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/example/SimpleConsumerDemo.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2334 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/example/SimpleProducerDemo.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2774 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/example/TalosProducerDemo.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/admin/
+-rw-r--r--   0 humkum     (501) staff       (20)     2262 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/admin/TalosAdmin.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/admin/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)        0 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/__init__.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/utils/
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/utils/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)      693 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/utils/FalconWriter.py
+-rw-r--r--   0 humkum     (501) staff       (20)     8431 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/utils/Utils.py
+-rw-r--r--   0 humkum     (501) staff       (20)      590 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/utils/Const.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/transport/
+-rw-r--r--   0 humkum     (501) staff       (20)    13211 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/TTransport.py
+-rw-r--r--   0 humkum     (501) staff       (20)    10904 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/TTwisted.py
+-rw-r--r--   0 humkum     (501) staff       (20)    16389 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/TSSLSocket.py
+-rw-r--r--   0 humkum     (501) staff       (20)      855 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    12979 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/THeaderTransport.py
+-rw-r--r--   0 humkum     (501) staff       (20)     8053 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/TSocket.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3662 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/sslcompat.py
+-rw-r--r--   0 humkum     (501) staff       (20)     7114 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/THttpClient.py
+-rw-r--r--   0 humkum     (501) staff       (20)     8778 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/transport/TZlibTransport.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1315 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/compat.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/auth/
+-rw-r--r--   0 humkum     (501) staff       (20)      758 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/auth/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       34 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/auth/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    11218 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/auth/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)      817 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3333 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/TRecursive.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/message/
+-rw-r--r--   0 humkum     (501) staff       (20)      142 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/message/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       52 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/message/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)   107912 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/message/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)    72642 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/message/MessageService.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/server/
+-rw-r--r--   0 humkum     (501) staff       (20)      830 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/server/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    11784 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/server/TServer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     4054 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/server/TProcessPoolServer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     5551 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/server/THttpServer.py
+-rw-r--r--   0 humkum     (501) staff       (20)    12495 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/server/TNonblockingServer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6407 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/TTornado.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/topic/
+-rw-r--r--   0 humkum     (501) staff       (20)      244 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/topic/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       50 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/topic/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)   101305 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/topic/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)   114771 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/topic/TopicService.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/protocol/
+-rw-r--r--   0 humkum     (501) staff       (20)     1101 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TProtocolDecorator.py
+-rw-r--r--   0 humkum     (501) staff       (20)     7401 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/THeaderProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)    19403 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TJSONProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1457 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TMultiplexedProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)      922 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     9140 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TBinaryProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2827 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TBase.py
+-rw-r--r--   0 humkum     (501) staff       (20)    15465 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TCompactProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)    13480 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/protocol/TProtocol.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3337 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/TMultiplexedProcessor.py
+-rw-r--r--   0 humkum     (501) staff       (20)     5843 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/Thrift.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/common/
+-rw-r--r--   0 humkum     (501) staff       (20)      555 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/common/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       54 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/common/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    13159 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/common/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)    13012 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/common/TalosBaseService.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1309 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/TSCons.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/quota/
+-rw-r--r--   0 humkum     (501) staff       (20)      142 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/quota/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       50 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/quota/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    44115 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/quota/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)    60949 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/quota/QuotaService.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/consumer/
+-rw-r--r--   0 humkum     (501) staff       (20)      143 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/consumer/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       53 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/consumer/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    56579 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/consumer/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)    59460 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/consumer/ConsumerService.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/authorization/
+-rw-r--r--   0 humkum     (501) staff       (20)      141 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/authorization/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       34 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/authorization/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3125 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/authorization/ttypes.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/thrift/metric/
+-rw-r--r--   0 humkum     (501) staff       (20)      141 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/metric/constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       51 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/metric/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    27643 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/metric/MetricService.py
+-rw-r--r--   0 humkum     (501) staff       (20)    23130 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/metric/ttypes.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1389 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/thrift/TSerialization.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/consumer/
+-rw-r--r--   0 humkum     (501) staff       (20)     1341 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/MessageProcessor.py
+-rw-r--r--   0 humkum     (501) staff       (20)    10986 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/consumer/TalosMessageReader.py
+-rw-r--r--   0 humkum     (501) staff       (20)      296 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/MessageReaderFactory.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    10773 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/consumer/MessageReader.py
+-rw-r--r--   0 humkum     (501) staff       (20)     7165 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/consumer/SimpleConsumer.py
+-rw-r--r--   0 humkum     (501) staff       (20)    13260 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/consumer/PartitionFetcher.py
+-rw-r--r--   0 humkum     (501) staff       (20)    29359 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/consumer/TalosConsumer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1354 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/MessageCheckpointer.py
+-rw-r--r--   0 humkum     (501) staff       (20)      163 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/MessageProcessorFactory.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6030 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/consumer/TalosConsumerConfigKeys.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/client/
+-rw-r--r--   0 humkum     (501) staff       (20)     7494 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/ScheduleInfoCache.py
+-rw-r--r--   0 humkum     (501) staff       (20)    15710 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/TalosClientFactory.py
+-rw-r--r--   0 humkum     (501) staff       (20)    18902 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/TalosClientConfig.py
+-rw-r--r--   0 humkum     (501) staff       (20)    19008 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/TalosHttpClient.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/client/serialization/
+-rw-r--r--   0 humkum     (501) staff       (20)     3268 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerializerV1.py
+-rw-r--r--   0 humkum     (501) staff       (20)      567 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerializationFactory.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1250 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerializer.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2235 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerialization.py
+-rw-r--r--   0 humkum     (501) staff       (20)     2531 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerializerV3.py
+-rw-r--r--   0 humkum     (501) staff       (20)      496 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageVersion.py
+-rw-r--r--   0 humkum     (501) staff       (20)     6741 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/serialization/MessageSerializerV2.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1924 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/Constants.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)      321 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/TopicAbnormalCallback.py
+-rw-r--r--   0 humkum     (501) staff       (20)      504 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/SimpleAbnormalCallback.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1546 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/TalosErrors.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos/client/compression/
+-rw-r--r--   0 humkum     (501) staff       (20)      911 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/compression/Gzip.py
+-rw-r--r--   0 humkum     (501) staff       (20)     4888 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/compression/Snappy.py
+-rw-r--r--   0 humkum     (501) staff       (20)     5562 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/compression/Compression.py
+-rw-r--r--   0 humkum     (501) staff       (20)       85 2022-10-18 05:05:03.000000 talos-python-3.0.9/talos/client/compression/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     9342 2022-10-24 06:49:22.000000 talos-python-3.0.9/talos/client/TalosClientConfigkeys.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/
+-rw-r--r--   0 humkum     (501) staff       (20)      274 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/PKG-INFO
+-rw-r--r--   0 humkum     (501) staff       (20)        1 2023-11-16 11:38:00.000000 talos-python-3.0.9/talos_python.egg-info/not-zip-safe
+-rw-r--r--   0 humkum     (501) staff       (20)     4963 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/SOURCES.txt
+-rw-r--r--   0 humkum     (501) staff       (20)       57 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/requires.txt
+-rw-r--r--   0 humkum     (501) staff       (20)        6 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/top_level.txt
+-rw-r--r--   0 humkum     (501) staff       (20)        1 2023-11-20 06:18:18.000000 talos-python-3.0.9/talos_python.egg-info/dependency_links.txt
+-rw-r--r--   0 humkum     (501) staff       (20)      522 2023-11-20 03:31:46.000000 talos-python-3.0.9/setup.py
+-rw-r--r--   0 humkum     (501) staff       (20)       38 2023-11-20 06:18:18.000000 talos-python-3.0.9/setup.cfg
```

### Comparing `talos-python-3.0.8.0/talos/producer/TalosProducerConfigKey.py` & `talos-python-3.0.9/talos/producer/TalosProducerConfigKey.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/UserMessage.py` & `talos-python-3.0.9/talos/producer/UserMessage.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/UserMessageCallback.py` & `talos-python-3.0.9/talos/producer/UserMessageCallback.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/PartitionSender.py` & `talos-python-3.0.9/talos/producer/PartitionSender.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/TalosProducer.py` & `talos-python-3.0.9/talos/producer/TalosProducer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/BufferedMessageCount.py` & `talos-python-3.0.9/talos/producer/BufferedMessageCount.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/PartitionMessageQueue.py` & `talos-python-3.0.9/talos/producer/PartitionMessageQueue.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         # update total buffered count when poll messageList
         self.producer.decrease_buffered_count(returnMsgNumber, returnMsgBytes)
         if self.logger.isEnabledFor(level=logging.DEBUG):
             self.logger.debug("Ready to put message batch: " + str(len(returnList)) +
                               " queue size: " + str(len(self.userMessageList))
                               + " and curBytes: " + str(self.curMessageBytes) +
                               " for partition: " + str(self.partitionId))
+        self.globalLock.release()
         return returnList
 
     @synchronized
     def should_put(self):
         # when TalosProducer is not active;
         if not self.producer.is_active():
             return True
```

### Comparing `talos-python-3.0.8.0/talos/producer/TalosProducerConfig.py` & `talos-python-3.0.9/talos/producer/TalosProducerConfig.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/producer/SimpleProducer.py` & `talos-python-3.0.9/talos/producer/SimpleProducer.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if (not msgList) or len(msgList) == 0:
             return True
 
         try:
             self.put_message_list(msgList)
             return True
         except Exception as e:
-            self.logger.error("putMessage error， please try to put again", e)
+            self.logger.error("putMessage to " + self.topicAndPartition + " error， please try to put again", e)
 
         return False
 
     def put_message_list(self, msgList=None):
         if (not msgList) or len(msgList) == 0:
             return
 
@@ -114,19 +114,19 @@
                         "can't connect to the host directly, refresh scheduleInfo and retry using url. "
                         + "The exception message is :" + e.message +
                         ". Ignore this if not frequently.")
                     self.scheduleInfoCache.update_schedule_info_cache()
                     putMessageResponse = self.messageClient.put_message(putMessageRequest)
                 else:
                     self.logger.error(
-                        "put message request failed." + str(traceback.format_exc()))
+                        "put message request to " + self.topicAndPartition + " failed." + str(traceback.format_exc()))
                     raise e
             else:
                 self.logger.error(
-                    "put message request failed." + str(traceback.format_exc()))
+                    "put message request to " + self.topicAndPartition + " failed." + str(traceback.format_exc()))
                 raise e
 
         # update scheduleInfocache when request have been transfered and talos auto location was set up
         if putMessageResponse.isTransfer and putMessageResponse.isTransfer and self.scheduleInfoCache \
                 and self.scheduleInfoCache.get_is_auto_location():
             self.logger.info(
                 "request has been transfered when talos auto location set up, refresh scheduleInfo")
```

### Comparing `talos-python-3.0.8.0/talos/producer/UserMessageResult.py` & `talos-python-3.0.9/talos/producer/UserMessageResult.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/producer/test_UserMessage.py` & `talos-python-3.0.9/talos/test/producer/test_UserMessage.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/producer/test_TalosProducer.py` & `talos-python-3.0.9/talos/test/producer/test_TalosProducer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/producer/test_PartitionMessageQueue.py` & `talos-python-3.0.9/talos/test/producer/test_PartitionMessageQueue.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/producer/test_PartitionSender.py` & `talos-python-3.0.9/talos/test/producer/test_PartitionSender.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/consumer/test_PartitionFetcher.py` & `talos-python-3.0.9/talos/test/consumer/test_PartitionFetcher.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/consumer/test_TalosConsumer.py` & `talos-python-3.0.9/talos/test/consumer/test_TalosConsumer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/consumer/test_SimpleConsumer.py` & `talos-python-3.0.9/talos/test/consumer/test_SimpleConsumer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/test/consumer/test_TalosMessageReader.py` & `talos-python-3.0.9/talos/test/consumer/test_TalosMessageReader.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/example/TalosConsumerDemo.py` & `talos-python-3.0.9/talos/example/TalosConsumerDemo.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/example/TalosAdminDemo.py` & `talos-python-3.0.9/talos/example/TalosAdminDemo.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/example/SimpleConsumerDemo.py` & `talos-python-3.0.9/talos/example/SimpleConsumerDemo.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/example/SimpleProducerDemo.py` & `talos-python-3.0.9/talos/example/SimpleProducerDemo.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/example/TalosProducerDemo.py` & `talos-python-3.0.9/talos/example/TalosProducerDemo.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/admin/TalosAdmin.py` & `talos-python-3.0.9/talos/admin/TalosAdmin.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/utils/FalconWriter.py` & `talos-python-3.0.9/talos/utils/FalconWriter.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/utils/Utils.py` & `talos-python-3.0.9/talos/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/utils/Const.py` & `talos-python-3.0.9/talos/utils/Const.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/TTransport.py` & `talos-python-3.0.9/talos/thrift/transport/TTransport.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/TTwisted.py` & `talos-python-3.0.9/talos/thrift/transport/TTwisted.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/TSSLSocket.py` & `talos-python-3.0.9/talos/thrift/transport/TSSLSocket.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/__init__.py` & `talos-python-3.0.9/talos/thrift/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/THeaderTransport.py` & `talos-python-3.0.9/talos/thrift/transport/THeaderTransport.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/TSocket.py` & `talos-python-3.0.9/talos/thrift/transport/TSocket.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/sslcompat.py` & `talos-python-3.0.9/talos/thrift/transport/sslcompat.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/THttpClient.py` & `talos-python-3.0.9/talos/thrift/transport/THttpClient.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/transport/TZlibTransport.py` & `talos-python-3.0.9/talos/thrift/transport/TZlibTransport.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/compat.py` & `talos-python-3.0.9/talos/thrift/compat.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/auth/constants.py` & `talos-python-3.0.9/talos/thrift/auth/constants.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/auth/ttypes.py` & `talos-python-3.0.9/talos/thrift/auth/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/__init__.py` & `talos-python-3.0.9/talos/thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/TRecursive.py` & `talos-python-3.0.9/talos/thrift/TRecursive.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/message/ttypes.py` & `talos-python-3.0.9/talos/thrift/message/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/message/MessageService.py` & `talos-python-3.0.9/talos/thrift/message/MessageService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/server/__init__.py` & `talos-python-3.0.9/talos/thrift/server/__init__.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/server/TServer.py` & `talos-python-3.0.9/talos/thrift/server/TServer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/server/TProcessPoolServer.py` & `talos-python-3.0.9/talos/thrift/server/TProcessPoolServer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/server/THttpServer.py` & `talos-python-3.0.9/talos/thrift/server/THttpServer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/server/TNonblockingServer.py` & `talos-python-3.0.9/talos/thrift/server/TNonblockingServer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/TTornado.py` & `talos-python-3.0.9/talos/thrift/TTornado.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/topic/ttypes.py` & `talos-python-3.0.9/talos/thrift/topic/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/topic/TopicService.py` & `talos-python-3.0.9/talos/thrift/topic/TopicService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TProtocolDecorator.py` & `talos-python-3.0.9/talos/thrift/protocol/TProtocolDecorator.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/THeaderProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/THeaderProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TJSONProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/TJSONProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TMultiplexedProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/TMultiplexedProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/__init__.py` & `talos-python-3.0.9/talos/thrift/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TBinaryProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/TBinaryProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TBase.py` & `talos-python-3.0.9/talos/thrift/protocol/TBase.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TCompactProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/TCompactProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/protocol/TProtocol.py` & `talos-python-3.0.9/talos/thrift/protocol/TProtocol.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/TMultiplexedProcessor.py` & `talos-python-3.0.9/talos/thrift/TMultiplexedProcessor.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/Thrift.py` & `talos-python-3.0.9/talos/thrift/Thrift.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/common/constants.py` & `talos-python-3.0.9/talos/thrift/common/constants.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/common/ttypes.py` & `talos-python-3.0.9/talos/thrift/common/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/common/TalosBaseService.py` & `talos-python-3.0.9/talos/thrift/common/TalosBaseService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/TSCons.py` & `talos-python-3.0.9/talos/thrift/TSCons.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/quota/ttypes.py` & `talos-python-3.0.9/talos/thrift/quota/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/quota/QuotaService.py` & `talos-python-3.0.9/talos/thrift/quota/QuotaService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/consumer/ttypes.py` & `talos-python-3.0.9/talos/thrift/consumer/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/consumer/ConsumerService.py` & `talos-python-3.0.9/talos/thrift/consumer/ConsumerService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/authorization/ttypes.py` & `talos-python-3.0.9/talos/thrift/authorization/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/metric/MetricService.py` & `talos-python-3.0.9/talos/thrift/metric/MetricService.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/metric/ttypes.py` & `talos-python-3.0.9/talos/thrift/metric/ttypes.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/thrift/TSerialization.py` & `talos-python-3.0.9/talos/thrift/TSerialization.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/MessageProcessor.py` & `talos-python-3.0.9/talos/consumer/MessageProcessor.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/TalosMessageReader.py` & `talos-python-3.0.9/talos/consumer/TalosMessageReader.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/MessageReader.py` & `talos-python-3.0.9/talos/consumer/MessageReader.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/SimpleConsumer.py` & `talos-python-3.0.9/talos/consumer/SimpleConsumer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/PartitionFetcher.py` & `talos-python-3.0.9/talos/consumer/PartitionFetcher.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/TalosConsumer.py` & `talos-python-3.0.9/talos/consumer/TalosConsumer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/MessageCheckpointer.py` & `talos-python-3.0.9/talos/consumer/MessageCheckpointer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/consumer/TalosConsumerConfigKeys.py` & `talos-python-3.0.9/talos/consumer/TalosConsumerConfigKeys.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/ScheduleInfoCache.py` & `talos-python-3.0.9/talos/client/ScheduleInfoCache.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/TalosClientFactory.py` & `talos-python-3.0.9/talos/client/TalosClientFactory.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/TalosClientConfig.py` & `talos-python-3.0.9/talos/client/TalosClientConfig.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/TalosHttpClient.py` & `talos-python-3.0.9/talos/client/TalosHttpClient.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV1.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerializerV1.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerializationFactory.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerializationFactory.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerializer.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerializer.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerialization.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerialization.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV3.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerializerV3.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/serialization/MessageSerializerV2.py` & `talos-python-3.0.9/talos/client/serialization/MessageSerializerV2.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/Constants.py` & `talos-python-3.0.9/talos/client/Constants.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/TalosErrors.py` & `talos-python-3.0.9/talos/client/TalosErrors.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/compression/Gzip.py` & `talos-python-3.0.9/talos/client/compression/Gzip.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/compression/Snappy.py` & `talos-python-3.0.9/talos/client/compression/Snappy.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/compression/Compression.py` & `talos-python-3.0.9/talos/client/compression/Compression.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos/client/TalosClientConfigkeys.py` & `talos-python-3.0.9/talos/client/TalosClientConfigkeys.py`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/talos_python.egg-info/SOURCES.txt` & `talos-python-3.0.9/talos_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talos-python-3.0.8.0/setup.py` & `talos-python-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='talos-python',
-    version='3.0.8.0',
+    version='3.0.9',
     author='huyumei',
     author_email='huyumei@xiaomi.com',
     maintainer='fangchengjin',
     maintainer_email='fangchengjin@xiaomi.com',
     description='talos python2 sdk',
     packages=find_packages(),
     include_package_data=True,
```

