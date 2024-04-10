# Comparing `tmp/kafka-python-ng-2.2.1.tar.gz` & `tmp/kafka-python-ng-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka-python-ng-2.2.1.tar", last modified: Thu Apr  4 15:56:52 2024, max compression
+gzip compressed data, was "kafka-python-ng-2.2.2.tar", last modified: Wed Apr 10 16:58:52 2024, max compression
```

## Comparing `kafka-python-ng-2.2.1.tar` & `kafka-python-ng-2.2.2.tar`

### file list

```diff
@@ -1,394 +1,395 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    57213 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.051602 kafka-python-ng-2.2.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/consumer_performance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1618 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/load_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/producer_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/record_batch_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/record_batch_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/benchmarks/varint_speed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2694 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/build_integration.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.055602 kafka-python-ng-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.055602 kafka-python-ng-2.2.1/docs/apidoc/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/BrokerConnection.rst
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/ClusterMetadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaAdminClient.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaClient.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaConsumer.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/KafkaProducer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/apidoc/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59846 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/docs/usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1983 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/acl_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    64300 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/config_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/new_partitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/admin/new_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    45437 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/client_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    56893 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/conn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.059602 kafka-python-ng-2.2.1/kafka/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47504 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    59428 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/consumer/subscription_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/assignors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/roundrobin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/partition_movements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sorted_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    34038 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sticky_assignor.py
--rw-r--r--   0 runner    (1001) docker     (127)    49041 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    39291 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/coordinator/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/future.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.063603 kafka-python-ng-2.2.1/kafka/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/compound_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/dict_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/kafka_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/measurable.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/measurable_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metric_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metric_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/metrics_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/metrics/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/avg.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/max_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/min_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/percentile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/sampled_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/metrics/stats/total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/oauth/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/partitioner/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/partitioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/partitioner/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.067602 kafka-python-ng-2.2.1/kafka/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/future.py
--rw-r--r--   0 runner    (1001) docker     (127)    37865 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    24926 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/record_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/producer/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.071602 kafka-python-ng-2.2.1/kafka/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    29905 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/produce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/protocol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/record/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/README
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/_crc32c.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/default_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/legacy_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/memory_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/record/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/sasl/
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/gssapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/msk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/oauthbearer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/plain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/sasl/scram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/scram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/kafka/serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/serializer/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-04-04 15:56:52.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:56:51.000000 kafka-python-ng-2.2.1/kafka_python_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/pylint.rc
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.075603 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.10.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.10.2.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.079603 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.11.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.11.0.3/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.043602 kafka-python-ng-2.2.1/servers/0.8.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.083603 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.8.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.8.2.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.9.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/0.9.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/0.9.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.0.2/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.087603 kafka-python-ng-2.2.1/servers/1.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/1.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/1.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.0.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.0.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.1.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.1.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.1.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.091603 kafka-python-ng-2.2.1/servers/2.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.2.1/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.3.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.4.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.5.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.5.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/2.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/2.6.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/2.6.0/resources/zookeeper.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.047602 kafka-python-ng-2.2.1/servers/trunk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.095603 kafka-python-ng-2.2.1/servers/trunk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/kafka.properties
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/kafka_server_jaas.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/log4j.properties
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/servers/trunk/resources/zookeeper.properties
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.099603 kafka-python-ng-2.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26996 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:56:52.103603 kafka-python-ng-2.2.1/test/record/
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_default_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_legacy_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/record/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_acl_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_admin_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_api_object_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_assignors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_client_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_consumer_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    26676 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_msk.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_object_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_partition_movements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_sasl_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/test_subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/test/testutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/tox.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-04 15:56:46.000000 kafka-python-ng-2.2.1/travis_java_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.257385 kafka-python-ng-2.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.257385 kafka-python-ng-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    57213 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.257385 kafka-python-ng-2.2.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/consumer_performance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1618 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/load_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/producer_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/record_batch_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/record_batch_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/benchmarks/varint_speed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2694 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/build_integration.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.257385 kafka-python-ng-2.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.261385 kafka-python-ng-2.2.2/docs/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/BrokerConnection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/ClusterMetadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/KafkaAdminClient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/KafkaClient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/KafkaConsumer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/KafkaProducer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/apidoc/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59846 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/docs/usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1983 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.261385 kafka-python-ng-2.2.2/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.261385 kafka-python-ng-2.2.2/kafka/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/acl_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64300 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/new_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/admin/new_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45889 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/client_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56893 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/conn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.265385 kafka-python-ng-2.2.2/kafka/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47504 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/consumer/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59428 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/consumer/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/consumer/subscription_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.265385 kafka-python-ng-2.2.2/kafka/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.265385 kafka-python-ng-2.2.2/kafka/coordinator/assignors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/roundrobin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.265385 kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/partition_movements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/sorted_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34038 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/sticky_assignor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49041 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39291 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/coordinator/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/future.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.269385 kafka-python-ng-2.2.2/kafka/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/compound_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/dict_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/kafka_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/measurable_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/metric_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/metric_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/metrics_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.269385 kafka-python-ng-2.2.2/kafka/metrics/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/max_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/min_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/sampled_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/metrics/stats/total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.269385 kafka-python-ng-2.2.2/kafka/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/oauth/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.269385 kafka-python-ng-2.2.2/kafka/partitioner/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/partitioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/partitioner/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.269385 kafka-python-ng-2.2.2/kafka/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37865 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24926 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/record_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22820 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/producer/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.273385 kafka-python-ng-2.2.2/kafka/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29905 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/produce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/protocol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.273385 kafka-python-ng-2.2.2/kafka/record/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/README
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/_crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/default_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/legacy_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/memory_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/record/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/kafka/sasl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/gssapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/msk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/oauthbearer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/sasl/scram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/scram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/kafka/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/serializer/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-10 16:58:52.000000 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-04-10 16:58:52.000000 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:58:52.000000 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 16:58:52.000000 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 16:58:52.000000 kafka-python-ng-2.2.2/kafka_python_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/pylint.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.245385 kafka-python-ng-2.2.2/servers/0.10.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/servers/0.10.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.245385 kafka-python-ng-2.2.2/servers/0.10.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/servers/0.10.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.245385 kafka-python-ng-2.2.2/servers/0.10.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/servers/0.10.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.245385 kafka-python-ng-2.2.2/servers/0.10.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.277385 kafka-python-ng-2.2.2/servers/0.10.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.10.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.10.2.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.10.2.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.11.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.11.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.11.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.11.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.11.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.11.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.11.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.11.0.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.3/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.3/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.3/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.11.0.3/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.281385 kafka-python-ng-2.2.2/servers/0.8.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.8.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.8.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.8.2.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.8.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.8.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.8.2.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.8.2.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.9.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.9.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/0.9.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/0.9.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/0.9.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.285385 kafka-python-ng-2.2.2/servers/1.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/1.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/1.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.2/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.2/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.2/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.0.2/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/1.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/1.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/1.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/2.0.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.249385 kafka-python-ng-2.2.2/servers/2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.289384 kafka-python-ng-2.2.2/servers/2.0.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.0.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.1.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.1.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.2.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.2.1/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.2.1/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.2.1/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.2.1/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.3.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.3.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.3.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.3.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.3.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.4.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.4.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.4.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.4.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.5.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.5.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.5.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.5.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.293385 kafka-python-ng-2.2.2/servers/2.6.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.6.0/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.6.0/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.6.0/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/2.6.0/resources/zookeeper.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.253385 kafka-python-ng-2.2.2/servers/trunk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.297385 kafka-python-ng-2.2.2/servers/trunk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/trunk/resources/kafka.properties
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/trunk/resources/kafka_server_jaas.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/trunk/resources/log4j.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/servers/trunk/resources/zookeeper.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27271 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:58:52.301385 kafka-python-ng-2.2.2/test/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/record/test_default_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/record/test_legacy_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/record/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/record/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_acl_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_admin_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_api_object_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36014 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_assignors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_client_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_consumer_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26676 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_msk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_object_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_partition_movements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_sasl_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_ssl_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/test_subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/test/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/tox.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-10 16:58:46.000000 kafka-python-ng-2.2.2/travis_java_install.sh
```

### Comparing `kafka-python-ng-2.2.1/.github/workflows/codeql-analysis.yml` & `kafka-python-ng-2.2.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/.github/workflows/python-package.yml` & `kafka-python-ng-2.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/.travis.yml` & `kafka-python-ng-2.2.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/AUTHORS.md` & `kafka-python-ng-2.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/CHANGES.md` & `kafka-python-ng-2.2.2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/LICENSE` & `kafka-python-ng-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/Makefile` & `kafka-python-ng-2.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/PKG-INFO` & `kafka-python-ng-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-python-ng
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pure Python client for Apache Kafka
 Home-page: https://github.com/wbarnha/kafka-python-ng
 Author: Dana Powers
 Author-email: dana.powers@gmail.com
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 License: Apache License 2.0
```

### Comparing `kafka-python-ng-2.2.1/README.rst` & `kafka-python-ng-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/consumer_performance.py` & `kafka-python-ng-2.2.2/benchmarks/consumer_performance.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/load_example.py` & `kafka-python-ng-2.2.2/benchmarks/load_example.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/producer_performance.py` & `kafka-python-ng-2.2.2/benchmarks/producer_performance.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/record_batch_compose.py` & `kafka-python-ng-2.2.2/benchmarks/record_batch_compose.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/record_batch_read.py` & `kafka-python-ng-2.2.2/benchmarks/record_batch_read.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/benchmarks/varint_speed.py` & `kafka-python-ng-2.2.2/benchmarks/varint_speed.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/build_integration.sh` & `kafka-python-ng-2.2.2/build_integration.sh`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/Makefile` & `kafka-python-ng-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/changelog.rst` & `kafka-python-ng-2.2.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/compatibility.rst` & `kafka-python-ng-2.2.2/docs/compatibility.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/conf.py` & `kafka-python-ng-2.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/index.rst` & `kafka-python-ng-2.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/install.rst` & `kafka-python-ng-2.2.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/make.bat` & `kafka-python-ng-2.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/tests.rst` & `kafka-python-ng-2.2.2/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/docs/usage.rst` & `kafka-python-ng-2.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/example.py` & `kafka-python-ng-2.2.2/example.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/__init__.py` & `kafka-python-ng-2.2.2/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/__init__.py` & `kafka-python-ng-2.2.2/kafka/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/acl_resource.py` & `kafka-python-ng-2.2.2/kafka/admin/acl_resource.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/client.py` & `kafka-python-ng-2.2.2/kafka/admin/client.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/config_resource.py` & `kafka-python-ng-2.2.2/kafka/admin/config_resource.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/new_partitions.py` & `kafka-python-ng-2.2.2/kafka/admin/new_partitions.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/admin/new_topic.py` & `kafka-python-ng-2.2.2/kafka/admin/new_topic.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/client_async.py` & `kafka-python-ng-2.2.2/kafka/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,15 +262,22 @@
             if conn.connecting():
                 # SSL connections can enter this state 2x (second during Handshake)
                 if node_id not in self._connecting:
                     self._connecting.add(node_id)
                 try:
                     self._selector.register(sock, selectors.EVENT_WRITE, conn)
                 except KeyError:
-                    self._selector.modify(sock, selectors.EVENT_WRITE, conn)
+                    # SSL detaches the original socket, and transfers the
+                    # underlying file descriptor to a new SSLSocket. We should
+                    # explicitly unregister the original socket.
+                    if conn.state == ConnectionStates.HANDSHAKE:
+                        self._selector.unregister(sock)
+                        self._selector.register(sock, selectors.EVENT_WRITE, conn)
+                    else:
+                        self._selector.modify(sock, selectors.EVENT_WRITE, conn)
 
                 if self.cluster.is_bootstrap(node_id):
                     self._last_bootstrap = time.time()
 
             elif conn.connected():
                 log.debug("Node %s connected", node_id)
                 if node_id in self._connecting:
```

### Comparing `kafka-python-ng-2.2.1/kafka/cluster.py` & `kafka-python-ng-2.2.2/kafka/cluster.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/codec.py` & `kafka-python-ng-2.2.2/kafka/codec.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/conn.py` & `kafka-python-ng-2.2.2/kafka/conn.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -374,18 +374,18 @@
 
             # Connection succeeded
             if not ret or ret == errno.EISCONN:
                 log.debug('%s: established TCP connection', self)
 
                 if self.config['security_protocol'] in ('SSL', 'SASL_SSL'):
                     log.debug('%s: initiating SSL handshake', self)
-                    self.state = ConnectionStates.HANDSHAKE
-                    self.config['state_change_callback'](self.node_id, self._sock, self)
                     # _wrap_ssl can alter the connection state -- disconnects on failure
                     self._wrap_ssl()
+                    self.state = ConnectionStates.HANDSHAKE
+                    self.config['state_change_callback'](self.node_id, self._sock, self)
 
                 elif self.config['security_protocol'] == 'SASL_PLAINTEXT':
                     log.debug('%s: initiating SASL authentication', self)
                     self.state = ConnectionStates.AUTHENTICATING
                     self.config['state_change_callback'](self.node_id, self._sock, self)
 
                 else:
```

### Comparing `kafka-python-ng-2.2.1/kafka/consumer/fetcher.py` & `kafka-python-ng-2.2.2/kafka/consumer/fetcher.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/consumer/group.py` & `kafka-python-ng-2.2.2/kafka/consumer/group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/consumer/subscription_state.py` & `kafka-python-ng-2.2.2/kafka/consumer/subscription_state.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/abstract.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/abstract.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/range.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/range.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/roundrobin.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/roundrobin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/partition_movements.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/partition_movements.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sorted_set.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/sorted_set.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/assignors/sticky/sticky_assignor.py` & `kafka-python-ng-2.2.2/kafka/coordinator/assignors/sticky/sticky_assignor.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/base.py` & `kafka-python-ng-2.2.2/kafka/coordinator/base.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/consumer.py` & `kafka-python-ng-2.2.2/kafka/coordinator/consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/heartbeat.py` & `kafka-python-ng-2.2.2/kafka/coordinator/heartbeat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/coordinator/protocol.py` & `kafka-python-ng-2.2.2/kafka/coordinator/protocol.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/errors.py` & `kafka-python-ng-2.2.2/kafka/errors.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/future.py` & `kafka-python-ng-2.2.2/kafka/future.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/__init__.py` & `kafka-python-ng-2.2.2/kafka/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/compound_stat.py` & `kafka-python-ng-2.2.2/kafka/metrics/compound_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/dict_reporter.py` & `kafka-python-ng-2.2.2/kafka/metrics/dict_reporter.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/kafka_metric.py` & `kafka-python-ng-2.2.2/kafka/metrics/kafka_metric.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/measurable.py` & `kafka-python-ng-2.2.2/kafka/metrics/measurable.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/metric_config.py` & `kafka-python-ng-2.2.2/kafka/metrics/metric_config.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/metric_name.py` & `kafka-python-ng-2.2.2/kafka/metrics/metric_name.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/metrics.py` & `kafka-python-ng-2.2.2/kafka/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/metrics_reporter.py` & `kafka-python-ng-2.2.2/kafka/metrics/metrics_reporter.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/quota.py` & `kafka-python-ng-2.2.2/kafka/metrics/quota.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stat.py` & `kafka-python-ng-2.2.2/kafka/metrics/stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/__init__.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/avg.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/avg.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/histogram.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/histogram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/max_stat.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/max_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/min_stat.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/min_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/percentiles.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/percentiles.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/rate.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/rate.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/sampled_stat.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/sampled_stat.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/metrics/stats/sensor.py` & `kafka-python-ng-2.2.2/kafka/metrics/stats/sensor.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/oauth/abstract.py` & `kafka-python-ng-2.2.2/kafka/oauth/abstract.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/partitioner/default.py` & `kafka-python-ng-2.2.2/kafka/partitioner/default.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/producer/buffer.py` & `kafka-python-ng-2.2.2/kafka/producer/buffer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/producer/future.py` & `kafka-python-ng-2.2.2/kafka/producer/future.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/producer/kafka.py` & `kafka-python-ng-2.2.2/kafka/producer/kafka.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/producer/record_accumulator.py` & `kafka-python-ng-2.2.2/kafka/producer/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/producer/sender.py` & `kafka-python-ng-2.2.2/kafka/producer/sender.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/__init__.py` & `kafka-python-ng-2.2.2/kafka/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/admin.py` & `kafka-python-ng-2.2.2/kafka/protocol/admin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/api.py` & `kafka-python-ng-2.2.2/kafka/protocol/api.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/commit.py` & `kafka-python-ng-2.2.2/kafka/protocol/commit.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/fetch.py` & `kafka-python-ng-2.2.2/kafka/protocol/fetch.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/frame.py` & `kafka-python-ng-2.2.2/kafka/protocol/frame.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/group.py` & `kafka-python-ng-2.2.2/kafka/protocol/group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/message.py` & `kafka-python-ng-2.2.2/kafka/protocol/message.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/metadata.py` & `kafka-python-ng-2.2.2/kafka/protocol/metadata.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/offset.py` & `kafka-python-ng-2.2.2/kafka/protocol/offset.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/parser.py` & `kafka-python-ng-2.2.2/kafka/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/pickle.py` & `kafka-python-ng-2.2.2/kafka/protocol/pickle.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/produce.py` & `kafka-python-ng-2.2.2/kafka/protocol/produce.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/struct.py` & `kafka-python-ng-2.2.2/kafka/protocol/struct.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/protocol/types.py` & `kafka-python-ng-2.2.2/kafka/protocol/types.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/_crc32c.py` & `kafka-python-ng-2.2.2/kafka/record/_crc32c.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/abc.py` & `kafka-python-ng-2.2.2/kafka/record/abc.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/default_records.py` & `kafka-python-ng-2.2.2/kafka/record/default_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/legacy_records.py` & `kafka-python-ng-2.2.2/kafka/record/legacy_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/memory_records.py` & `kafka-python-ng-2.2.2/kafka/record/memory_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/record/util.py` & `kafka-python-ng-2.2.2/kafka/record/util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/__init__.py` & `kafka-python-ng-2.2.2/kafka/sasl/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/gssapi.py` & `kafka-python-ng-2.2.2/kafka/sasl/gssapi.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/msk.py` & `kafka-python-ng-2.2.2/kafka/sasl/msk.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/oauthbearer.py` & `kafka-python-ng-2.2.2/kafka/sasl/oauthbearer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/plain.py` & `kafka-python-ng-2.2.2/kafka/sasl/plain.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/sasl/scram.py` & `kafka-python-ng-2.2.2/kafka/sasl/scram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/scram.py` & `kafka-python-ng-2.2.2/kafka/scram.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/structs.py` & `kafka-python-ng-2.2.2/kafka/structs.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka/util.py` & `kafka-python-ng-2.2.2/kafka/util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/kafka_python_ng.egg-info/PKG-INFO` & `kafka-python-ng-2.2.2/kafka_python_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-python-ng
-Version: 2.2.1
+Version: 2.2.2
 Summary: Pure Python client for Apache Kafka
 Home-page: https://github.com/wbarnha/kafka-python-ng
 Author: Dana Powers
 Author-email: dana.powers@gmail.com
 Maintainer: William Barnhart
 Maintainer-email: williambbarnhart@gmail.com
 License: Apache License 2.0
```

### Comparing `kafka-python-ng-2.2.1/kafka_python_ng.egg-info/SOURCES.txt` & `kafka-python-ng-2.2.2/kafka_python_ng.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -292,13 +292,14 @@
 test/test_package.py
 test/test_partition_movements.py
 test/test_partitioner.py
 test/test_producer.py
 test/test_protocol.py
 test/test_sasl_integration.py
 test/test_sender.py
+test/test_ssl_integration.py
 test/test_subscription_state.py
 test/testutil.py
 test/record/test_default_records.py
 test/record/test_legacy_records.py
 test/record/test_records.py
 test/record/test_util.py
```

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.10.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.10.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.10.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.10.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.10.2.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.10.2.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.3/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.3/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.11.0.3/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.11.0.3/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.8.2.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.8.2.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/0.9.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/0.9.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/1.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/1.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/1.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/1.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/1.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/1.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.2/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/1.0.2/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.2/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/1.0.2/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.0.2/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/1.0.2/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/1.1.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/1.1.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/1.1.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/1.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/1.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/1.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/1.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.0.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.0.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.0.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.0.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.0.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.0.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.0.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.1.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.1.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.1.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.1.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.1.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.1.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.1.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.2.1/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.2.1/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.2.1/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.2.1/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.2.1/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.2.1/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.3.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.3.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.3.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.3.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.3.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.3.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.4.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.4.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.4.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.4.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.4.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.4.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.5.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.5.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.5.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.5.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.5.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.5.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.6.0/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/2.6.0/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.6.0/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/2.6.0/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/2.6.0/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/2.6.0/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/trunk/resources/kafka.properties` & `kafka-python-ng-2.2.2/servers/trunk/resources/kafka.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/trunk/resources/log4j.properties` & `kafka-python-ng-2.2.2/servers/trunk/resources/log4j.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/servers/trunk/resources/zookeeper.properties` & `kafka-python-ng-2.2.2/servers/trunk/resources/zookeeper.properties`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/setup.py` & `kafka-python-ng-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/conftest.py` & `kafka-python-ng-2.2.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/fixtures.py` & `kafka-python-ng-2.2.2/test/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def gen_ssl_resources(directory):
     os.system("""
     cd {0}
     echo Generating SSL resources in {0}
 
     # Step 1
     keytool -keystore kafka.server.keystore.jks -alias localhost -validity 1 \
-      -genkey -storepass foobar -keypass foobar \
+      -genkey -keyalg RSA -storepass foobar -keypass foobar \
       -dname "CN=localhost, OU=kafka-python, O=kafka-python, L=SF, ST=CA, C=US" \
       -ext SAN=dns:localhost
 
     # Step 2
     openssl genrsa -out ca-key 2048
     openssl req -new -x509 -key ca-key -out ca-cert -days 1 \
       -subj "/C=US/ST=CA/O=MyOrg, Inc./CN=mydomain.com"
@@ -285,15 +285,15 @@
         self.broker_id = broker_id
         self.auto_create_topic = auto_create_topic
         self.transport = transport.upper()
         if sasl_mechanism is not None:
             self.sasl_mechanism = sasl_mechanism.upper()
         else:
             self.sasl_mechanism = None
-        self.ssl_dir = self.test_resource('ssl')
+        self.ssl_dir = None
 
         # TODO: checking for port connection would be better than scanning logs
         # until then, we need the pattern to work across all supported broker versions
         # The logging format changed slightly in 1.0.0
         self.start_pattern = r"\[Kafka ?Server (id=)?%d\],? started" % (broker_id,)
         # Need to wait until the broker has fetched user configs from zookeeper in case we use scram as sasl mechanism
         self.scram_pattern = r"Removing Produce quota for user %s" % (self.broker_user)
@@ -406,14 +406,16 @@
 
     def start(self):
         # Configure Kafka child process
         properties = self.tmp_dir.join("kafka.properties")
         jaas_conf = self.tmp_dir.join("kafka_server_jaas.conf")
         properties_template = self.test_resource("kafka.properties")
         jaas_conf_template = self.test_resource("kafka_server_jaas.conf")
+        self.ssl_dir = self.tmp_dir
+        gen_ssl_resources(self.ssl_dir.strpath) 
 
         args = self.kafka_run_class_args("kafka.Kafka", properties.strpath)
         env = self.kafka_run_class_env()
         if self.sasl_enabled:
             opts = env.get('KAFKA_OPTS', '').strip()
             opts += ' -Djava.security.auth.login.config={}'.format(jaas_conf.strpath)
             env['KAFKA_OPTS'] = opts
@@ -637,14 +639,17 @@
         params.setdefault('bootstrap_servers', self.bootstrap_server())
         if self.sasl_enabled:
             params.setdefault('sasl_mechanism', self.sasl_mechanism)
             params.setdefault('security_protocol', self.transport)
             if self.sasl_mechanism in ('PLAIN', 'SCRAM-SHA-256', 'SCRAM-SHA-512'):
                 params.setdefault('sasl_plain_username', self.broker_user)
                 params.setdefault('sasl_plain_password', self.broker_password)
+        if self.transport in ["SASL_SSL", "SSL"]:
+            params.setdefault("ssl_cafile", self.ssl_dir.join('ca-cert').strpath)
+            params.setdefault("security_protocol", self.transport)
         return params
 
     @staticmethod
     def _create_many_clients(cnt, cls, *args, **params):
         client_id = params['client_id']
         for _ in range(cnt):
             params['client_id'] = '%s_%s' % (client_id, random_string(4))
```

### Comparing `kafka-python-ng-2.2.1/test/record/test_default_records.py` & `kafka-python-ng-2.2.2/test/record/test_default_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/record/test_legacy_records.py` & `kafka-python-ng-2.2.2/test/record/test_legacy_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/record/test_records.py` & `kafka-python-ng-2.2.2/test/record/test_records.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/record/test_util.py` & `kafka-python-ng-2.2.2/test/record/test_util.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/service.py` & `kafka-python-ng-2.2.2/test/service.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_acl_comparisons.py` & `kafka-python-ng-2.2.2/test/test_acl_comparisons.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_admin.py` & `kafka-python-ng-2.2.2/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_admin_integration.py` & `kafka-python-ng-2.2.2/test/test_admin_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_api_object_implementation.py` & `kafka-python-ng-2.2.2/test/test_api_object_implementation.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_assignors.py` & `kafka-python-ng-2.2.2/test/test_assignors.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_client_async.py` & `kafka-python-ng-2.2.2/test/test_client_async.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_cluster.py` & `kafka-python-ng-2.2.2/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_codec.py` & `kafka-python-ng-2.2.2/test/test_codec.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_conn.py` & `kafka-python-ng-2.2.2/test/test_conn.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_consumer.py` & `kafka-python-ng-2.2.2/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_consumer_group.py` & `kafka-python-ng-2.2.2/test/test_consumer_group.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_consumer_integration.py` & `kafka-python-ng-2.2.2/test/test_consumer_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_coordinator.py` & `kafka-python-ng-2.2.2/test/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_fetcher.py` & `kafka-python-ng-2.2.2/test/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_metrics.py` & `kafka-python-ng-2.2.2/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_msk.py` & `kafka-python-ng-2.2.2/test/test_msk.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_object_conversion.py` & `kafka-python-ng-2.2.2/test/test_object_conversion.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_package.py` & `kafka-python-ng-2.2.2/test/test_package.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_partition_movements.py` & `kafka-python-ng-2.2.2/test/test_partition_movements.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_partitioner.py` & `kafka-python-ng-2.2.2/test/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_producer.py` & `kafka-python-ng-2.2.2/test/test_producer.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_protocol.py` & `kafka-python-ng-2.2.2/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_sasl_integration.py` & `kafka-python-ng-2.2.2/test/test_sasl_integration.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_sender.py` & `kafka-python-ng-2.2.2/test/test_sender.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/test_subscription_state.py` & `kafka-python-ng-2.2.2/test/test_subscription_state.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/test/testutil.py` & `kafka-python-ng-2.2.2/test/testutil.py`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/tox.ini` & `kafka-python-ng-2.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `kafka-python-ng-2.2.1/travis_java_install.sh` & `kafka-python-ng-2.2.2/travis_java_install.sh`

 * *Files identical despite different names*

