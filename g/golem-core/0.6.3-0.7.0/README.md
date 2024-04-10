# Comparing `tmp/golem_core-0.6.3.tar.gz` & `tmp/golem_core-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_core-0.6.3.tar", max compression
+gzip compressed data, was "golem_core-0.7.0.tar", max compression
```

## Comparing `golem_core-0.6.3.tar` & `golem_core-0.7.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0    35149 2023-09-13 08:05:36.792448 golem_core-0.6.3/LICENSE
--rw-r--r--   0        0        0        0 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/__init__.py
--rw-r--r--   0        0        0       64 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/__main__.py
--rw-r--r--   0        0        0       50 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/cli/__init__.py
--rw-r--r--   0        0        0     2641 2023-11-25 08:20:36.562759 golem_core-0.6.3/golem/cli/cli.py
--rw-r--r--   0        0        0     4463 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/cli/utils.py
--rw-r--r--   0        0        0      151 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/__init__.py
--rw-r--r--   0        0        0     1280 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/base.py
--rw-r--r--   0        0        0       98 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/in_memory/__init__.py
--rw-r--r--   0        0        0     6737 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/event_bus/in_memory/event_bus.py
--rw-r--r--   0        0        0      332 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/exceptions.py
--rw-r--r--   0        0        0     2554 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/__init__.py
--rw-r--r--   0        0        0      475 2023-10-10 09:27:48.015544 golem_core-0.6.3/golem/managers/activity/__init__.py
--rw-r--r--   0        0        0      476 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/activity/defaults.py
--rw-r--r--   0        0        0     2111 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/mixins.py
--rw-r--r--   0        0        0     3872 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/pool.py
--rw-r--r--   0        0        0     1734 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/single_use.py
--rw-r--r--   0        0        0      109 2023-10-03 11:48:04.547546 golem_core-0.6.3/golem/managers/agreement/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/agreement/default.py
--rw-r--r--   0        0        0     5925 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/managers/base.py
--rw-r--r--   0        0        0      218 2024-02-28 10:31:22.882324 golem_core-0.6.3/golem/managers/demand/__init__.py
--rw-r--r--   0        0        0     2286 2024-02-28 10:31:22.882324 golem_core-0.6.3/golem/managers/demand/aggregating.py
--rw-r--r--   0        0        0     5488 2024-02-15 12:52:48.457251 golem_core-0.6.3/golem/managers/demand/refreshing.py
--rw-r--r--   0        0        0     1658 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/mixins.py
--rw-r--r--   0        0        0      100 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/network/__init__.py
--rw-r--r--   0        0        0     2197 2023-12-13 09:08:00.946133 golem_core-0.6.3/golem/managers/network/single.py
--rw-r--r--   0        0        0      103 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/payment/__init__.py
--rw-r--r--   0        0        0     5682 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/payment/default.py
--rw-r--r--   0        0        0      980 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/__init__.py
--rw-r--r--   0        0        0     1586 2023-11-02 09:14:12.499044 golem_core-0.6.3/golem/managers/proposal/default.py
--rw-r--r--   0        0        0     1155 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/__init__.py
--rw-r--r--   0        0        0     1005 2023-10-13 09:42:33.129828 golem_core-0.6.3/golem/managers/proposal/plugins/blacklist.py
--rw-r--r--   0        0        0     5011 2024-03-20 09:04:31.378487 golem_core-0.6.3/golem/managers/proposal/plugins/buffer.py
--rw-r--r--   0        0        0     1054 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/proposal/plugins/linear_coeffs.py
--rw-r--r--   0        0        0      422 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/__init__.py
--rw-r--r--   0        0        0     4671 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
--rw-r--r--   0        0        0     4879 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
--rw-r--r--   0        0        0     1567 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/payment_platform.py
--rw-r--r--   0        0        0     2441 2024-01-05 09:59:46.197955 golem_core-0.6.3/golem/managers/proposal/plugins/reject_costs_exceeds.py
--rw-r--r--   0        0        0      738 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/__init__.py
--rw-r--r--   0        0        0     1738 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/map.py
--rw-r--r--   0        0        0     4008 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/mixins.py
--rw-r--r--   0        0        0     1938 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/pricings.py
--rw-r--r--   0        0        0     3457 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py
--rw-r--r--   0        0        0      505 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/random.py
--rw-r--r--   0        0        0     4217 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py
--rw-r--r--   0        0        0      996 2023-10-13 09:42:33.129828 golem_core-0.6.3/golem/managers/proposal/plugins/whitelist.py
--rw-r--r--   0        0        0      474 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/work/__init__.py
--rw-r--r--   0        0        0     2087 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/concurrent.py
--rw-r--r--   0        0        0     2024 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/mixins.py
--rw-r--r--   0        0        0     2038 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/work/plugins.py
--rw-r--r--   0        0        0     1201 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/sequential.py
--rw-r--r--   0        0        0      257 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/node/__init__.py
--rw-r--r--   0        0        0      856 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/node/events.py
--rw-r--r--   0        0        0    16730 2024-01-26 10:08:12.206583 golem_core-0.6.3/golem/node/node.py
--rw-r--r--   0        0        0     1153 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/payload/__init__.py
--rw-r--r--   0        0        0     6649 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/base.py
--rw-r--r--   0        0        0     1939 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/payload/constraints.py
--rw-r--r--   0        0        0     5156 2024-03-28 09:34:15.049644 golem_core-0.6.3/golem/payload/defaults.py
--rw-r--r--   0        0        0      284 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/exceptions.py
--rw-r--r--   0        0        0      973 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/generic.py
--rw-r--r--   0        0        0     1405 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/mixins.py
--rw-r--r--   0        0        0     1186 2024-01-08 09:28:36.246646 golem_core-0.6.3/golem/payload/parser.py
--rw-r--r--   0        0        0      621 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/parser.tx
--rw-r--r--   0        0        0      868 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/properties.py
--rw-r--r--   0        0        0     5677 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/payload/vm.py
--rw-r--r--   0        0        0      504 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/__init__.py
--rw-r--r--   0        0        0     4535 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/buffer.py
--rw-r--r--   0        0        0     1847 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/chain.py
--rw-r--r--   0        0        0     3704 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/default_payment_handler.py
--rw-r--r--   0        0        0     1363 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/exceptions.py
--rw-r--r--   0        0        0      842 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/limit.py
--rw-r--r--   0        0        0     3990 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/map.py
--rw-r--r--   0        0        0     4152 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/sort.py
--rw-r--r--   0        0        0     2453 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/pipeline/zip.py
--rw-r--r--   0        0        0     3462 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/__init__.py
--rw-r--r--   0        0        0      592 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/__init__.py
--rw-r--r--   0        0        0     6327 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/resources/activity/activity.py
--rw-r--r--   0        0        0     6903 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/commands.py
--rw-r--r--   0        0        0      391 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/events.py
--rw-r--r--   0        0        0      735 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/pipeline.py
--rw-r--r--   0        0        0      360 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/__init__.py
--rw-r--r--   0        0        0     6475 2024-03-25 15:48:24.993493 golem_core-0.6.3/golem/resources/agreement/agreement.py
--rw-r--r--   0        0        0      375 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/agreement/data.py
--rw-r--r--   0        0        0      400 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/events.py
--rw-r--r--   0        0        0      289 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/pipeline.py
--rw-r--r--   0        0        0      410 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/__init__.py
--rw-r--r--   0        0        0     3220 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/allocation/allocation.py
--rw-r--r--   0        0        0      409 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/events.py
--rw-r--r--   0        0        0      835 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/exceptions.py
--rw-r--r--   0        0        0    11150 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/resources/base.py
--rw-r--r--   0        0        0      372 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/__init__.py
--rw-r--r--   0        0        0     9201 2024-04-03 13:30:08.983271 golem_core-0.6.3/golem/resources/debit_note/debit_note.py
--rw-r--r--   0        0        0      784 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/event_collectors.py
--rw-r--r--   0        0        0      402 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/events.py
--rw-r--r--   0        0        0      379 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/demand/__init__.py
--rw-r--r--   0        0        0      315 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/demand/data.py
--rw-r--r--   0        0        0     5532 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/demand/demand.py
--rw-r--r--   0        0        0     2959 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/resources/demand/demand_builder.py
--rw-r--r--   0        0        0      373 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/demand/events.py
--rw-r--r--   0        0        0     1559 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/event_collectors.py
--rw-r--r--   0        0        0     4215 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/events.py
--rw-r--r--   0        0        0     1016 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/exceptions.py
--rw-r--r--   0        0        0      340 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/__init__.py
--rw-r--r--   0        0        0      760 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/event_collectors.py
--rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/events.py
--rw-r--r--   0        0        0     5320 2024-04-03 13:30:08.983271 golem_core-0.6.3/golem/resources/invoice/invoice.py
--rw-r--r--   0        0        0      394 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/__init__.py
--rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/events.py
--rw-r--r--   0        0        0      590 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/exceptions.py
--rw-r--r--   0        0        0     5803 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/network/network.py
--rw-r--r--   0        0        0      509 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/__init__.py
--rw-r--r--   0        0        0      456 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/events.py
--rw-r--r--   0        0        0     2122 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/exceptions.py
--rw-r--r--   0        0        0     5510 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/pooling_batch.py
--rw-r--r--   0        0        0      499 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/proposal/__init__.py
--rw-r--r--   0        0        0      508 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/proposal/data.py
--rw-r--r--   0        0        0      391 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/proposal/events.py
--rw-r--r--   0        0        0      664 2023-11-02 09:14:12.503044 golem_core-0.6.3/golem/resources/proposal/exceptions.py
--rw-r--r--   0        0        0      860 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/proposal/pipeline.py
--rw-r--r--   0        0        0     9303 2024-02-20 09:06:29.551136 golem_core-0.6.3/golem/resources/proposal/proposal.py
--rw-r--r--   0        0        0        0 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/utils/__init__.py
--rw-r--r--   0        0        0      626 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/utils/infrastructure.py
--rw-r--r--   0        0        0     6493 2024-03-28 09:34:26.741806 golem_core-0.6.3/golem/resources/utils/payment.py
--rw-r--r--   0        0        0        0 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/__init__.py
--rw-r--r--   0        0        0      704 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/__init__.py
--rw-r--r--   0        0        0    13576 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/buffer.py
--rw-r--r--   0        0        0     2044 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/queue.py
--rw-r--r--   0        0        0     2056 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/semaphore.py
--rw-r--r--   0        0        0     1943 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/tasks.py
--rw-r--r--   0        0        0     1726 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/waiter.py
--rw-r--r--   0        0        0      741 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/http.py
--rw-r--r--   0        0        0     7521 2024-02-08 13:35:10.795401 golem_core-0.6.3/golem/utils/logging.py
--rw-r--r--   0        0        0      307 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/__init__.py
--rw-r--r--   0        0        0     6571 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/api.py
--rw-r--r--   0        0        0     3323 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/event_collector.py
--rw-r--r--   0        0        0      105 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/__init__.py
--rw-r--r--   0        0        0     4024 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/base.py
--rw-r--r--   0        0        0       88 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/gftp/__init__.py
--rw-r--r--   0        0        0    16077 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/gftp/provider.py
--rw-r--r--   0        0        0      673 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/utils.py
--rw-r--r--   0        0        0      767 2024-02-08 13:35:10.795401 golem_core-0.6.3/golem/utils/typing.py
--rw-r--r--   0        0        0     4722 2024-04-03 13:30:53.986345 golem_core-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 golem_core-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 08:29:54.314856 golem_core-0.7.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/__main__.py
+-rw-r--r--   0        0        0       50 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/cli.py
+-rw-r--r--   0        0        0     4463 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/cli/utils.py
+-rw-r--r--   0        0        0      151 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/base.py
+-rw-r--r--   0        0        0       98 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/in_memory/__init__.py
+-rw-r--r--   0        0        0     6737 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/event_bus/in_memory/event_bus.py
+-rw-r--r--   0        0        0      332 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/exceptions.py
+-rw-r--r--   0        0        0     2554 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/__init__.py
+-rw-r--r--   0        0        0      476 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/defaults.py
+-rw-r--r--   0        0        0     2111 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/mixins.py
+-rw-r--r--   0        0        0     3872 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/pool.py
+-rw-r--r--   0        0        0     1734 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/activity/single_use.py
+-rw-r--r--   0        0        0      109 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/agreement/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/agreement/default.py
+-rw-r--r--   0        0        0     5925 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/base.py
+-rw-r--r--   0        0        0      218 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/aggregating.py
+-rw-r--r--   0        0        0     5488 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/demand/refreshing.py
+-rw-r--r--   0        0        0     1658 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/mixins.py
+-rw-r--r--   0        0        0      100 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/network/__init__.py
+-rw-r--r--   0        0        0     2197 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/network/single.py
+-rw-r--r--   0        0        0      103 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/payment/__init__.py
+-rw-r--r--   0        0        0     5937 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/payment/default.py
+-rw-r--r--   0        0        0      980 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/__init__.py
+-rw-r--r--   0        0        0     1586 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/default.py
+-rw-r--r--   0        0        0     1155 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/blacklist.py
+-rw-r--r--   0        0        0     5125 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/buffer.py
+-rw-r--r--   0        0        0     1054 2024-04-10 08:29:54.322856 golem_core-0.7.0/golem/managers/proposal/plugins/linear_coeffs.py
+-rw-r--r--   0        0        0      422 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/__init__.py
+-rw-r--r--   0        0        0     4671 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
+-rw-r--r--   0        0        0     5467 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
+-rw-r--r--   0        0        0     1567 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/payment_platform.py
+-rw-r--r--   0        0        0     2441 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/reject_costs_exceeds.py
+-rw-r--r--   0        0        0      738 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/__init__.py
+-rw-r--r--   0        0        0     1738 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/map.py
+-rw-r--r--   0        0        0     4008 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/mixins.py
+-rw-r--r--   0        0        0     1938 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/pricings.py
+-rw-r--r--   0        0        0     3457 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/property_value_lerp.py
+-rw-r--r--   0        0        0      505 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/random.py
+-rw-r--r--   0        0        0     4217 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/scoring/scoring_buffer.py
+-rw-r--r--   0        0        0      996 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/proposal/plugins/whitelist.py
+-rw-r--r--   0        0        0      474 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/__init__.py
+-rw-r--r--   0        0        0     2087 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/concurrent.py
+-rw-r--r--   0        0        0     2024 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/mixins.py
+-rw-r--r--   0        0        0     2038 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/plugins.py
+-rw-r--r--   0        0        0     1201 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/managers/work/sequential.py
+-rw-r--r--   0        0        0      257 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/events.py
+-rw-r--r--   0        0        0    16730 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/node/node.py
+-rw-r--r--   0        0        0     1153 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/__init__.py
+-rw-r--r--   0        0        0     6649 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/base.py
+-rw-r--r--   0        0        0     1939 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/constraints.py
+-rw-r--r--   0        0        0     5156 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/defaults.py
+-rw-r--r--   0        0        0      284 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/exceptions.py
+-rw-r--r--   0        0        0      973 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/generic.py
+-rw-r--r--   0        0        0     1405 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/mixins.py
+-rw-r--r--   0        0        0     1186 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/parser.py
+-rw-r--r--   0        0        0      621 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/parser.tx
+-rw-r--r--   0        0        0      868 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/properties.py
+-rw-r--r--   0        0        0     5677 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/payload/vm.py
+-rw-r--r--   0        0        0      504 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/__init__.py
+-rw-r--r--   0        0        0     4535 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/buffer.py
+-rw-r--r--   0        0        0     1847 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/chain.py
+-rw-r--r--   0        0        0     3704 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/default_payment_handler.py
+-rw-r--r--   0        0        0     1363 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/exceptions.py
+-rw-r--r--   0        0        0      842 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/limit.py
+-rw-r--r--   0        0        0     3990 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/map.py
+-rw-r--r--   0        0        0     4152 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/sort.py
+-rw-r--r--   0        0        0     2453 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/pipeline/zip.py
+-rw-r--r--   0        0        0     3462 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/__init__.py
+-rw-r--r--   0        0        0      592 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/__init__.py
+-rw-r--r--   0        0        0     6327 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/activity.py
+-rw-r--r--   0        0        0     6903 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/commands.py
+-rw-r--r--   0        0        0      391 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/events.py
+-rw-r--r--   0        0        0      735 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/activity/pipeline.py
+-rw-r--r--   0        0        0      360 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/__init__.py
+-rw-r--r--   0        0        0     6718 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/agreement.py
+-rw-r--r--   0        0        0      375 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/data.py
+-rw-r--r--   0        0        0      400 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/events.py
+-rw-r--r--   0        0        0      289 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/agreement/pipeline.py
+-rw-r--r--   0        0        0      410 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/__init__.py
+-rw-r--r--   0        0        0     3220 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/allocation.py
+-rw-r--r--   0        0        0      409 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/events.py
+-rw-r--r--   0        0        0      835 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/allocation/exceptions.py
+-rw-r--r--   0        0        0    11150 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/base.py
+-rw-r--r--   0        0        0      372 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/__init__.py
+-rw-r--r--   0        0        0     9169 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/debit_note.py
+-rw-r--r--   0        0        0      784 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/event_collectors.py
+-rw-r--r--   0        0        0      402 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/debit_note/events.py
+-rw-r--r--   0        0        0      379 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/data.py
+-rw-r--r--   0        0        0     5532 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/demand.py
+-rw-r--r--   0        0        0     2959 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/demand_builder.py
+-rw-r--r--   0        0        0      373 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/demand/events.py
+-rw-r--r--   0        0        0     1559 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/event_collectors.py
+-rw-r--r--   0        0        0     4215 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/events.py
+-rw-r--r--   0        0        0     1016 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/exceptions.py
+-rw-r--r--   0        0        0      340 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/event_collectors.py
+-rw-r--r--   0        0        0      382 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/events.py
+-rw-r--r--   0        0        0     5307 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/invoice/invoice.py
+-rw-r--r--   0        0        0      394 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/events.py
+-rw-r--r--   0        0        0      590 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/exceptions.py
+-rw-r--r--   0        0        0     5803 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/network/network.py
+-rw-r--r--   0        0        0      509 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/events.py
+-rw-r--r--   0        0        0     2122 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/exceptions.py
+-rw-r--r--   0        0        0     5510 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/pooling_batch/pooling_batch.py
+-rw-r--r--   0        0        0      499 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/__init__.py
+-rw-r--r--   0        0        0      508 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/data.py
+-rw-r--r--   0        0        0      391 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/events.py
+-rw-r--r--   0        0        0      664 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/exceptions.py
+-rw-r--r--   0        0        0      860 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/pipeline.py
+-rw-r--r--   0        0        0     9303 2024-04-10 08:29:54.326856 golem_core-0.7.0/golem/resources/proposal/proposal.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/infrastructure.py
+-rw-r--r--   0        0        0     6602 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/resources/utils/payment.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/__init__.py
+-rw-r--r--   0        0        0      704 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/__init__.py
+-rw-r--r--   0        0        0    13751 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/buffer.py
+-rw-r--r--   0        0        0     2044 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/queue.py
+-rw-r--r--   0        0        0     2056 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/semaphore.py
+-rw-r--r--   0        0        0     2820 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/tasks.py
+-rw-r--r--   0        0        0     1726 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/asyncio/waiter.py
+-rw-r--r--   0        0        0      741 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/http.py
+-rw-r--r--   0        0        0     7521 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/logging.py
+-rw-r--r--   0        0        0      307 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/__init__.py
+-rw-r--r--   0        0        0     6571 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/api.py
+-rw-r--r--   0        0        0     3323 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/low/event_collector.py
+-rw-r--r--   0        0        0      105 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/base.py
+-rw-r--r--   0        0        0       88 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/gftp/__init__.py
+-rw-r--r--   0        0        0    16077 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/gftp/provider.py
+-rw-r--r--   0        0        0      673 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/storage/utils.py
+-rw-r--r--   0        0        0      767 2024-04-10 08:29:54.330856 golem_core-0.7.0/golem/utils/typing.py
+-rw-r--r--   0        0        0     4722 2024-04-10 08:29:54.330856 golem_core-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 golem_core-0.7.0/PKG-INFO
```

### Comparing `golem_core-0.6.3/LICENSE` & `golem_core-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/cli/cli.py` & `golem_core-0.7.0/golem/cli/cli.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/cli/utils.py` & `golem_core-0.7.0/golem/cli/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/event_bus/base.py` & `golem_core-0.7.0/golem/event_bus/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/event_bus/in_memory/event_bus.py` & `golem_core-0.7.0/golem/event_bus/in_memory/event_bus.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/__init__.py` & `golem_core-0.7.0/golem/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/activity/mixins.py` & `golem_core-0.7.0/golem/managers/activity/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/activity/pool.py` & `golem_core-0.7.0/golem/managers/activity/pool.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/activity/single_use.py` & `golem_core-0.7.0/golem/managers/activity/single_use.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/agreement/default.py` & `golem_core-0.7.0/golem/managers/agreement/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/base.py` & `golem_core-0.7.0/golem/managers/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/demand/aggregating.py` & `golem_core-0.7.0/golem/managers/demand/aggregating.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import asyncio
 import logging
 from typing import Awaitable, Callable, MutableMapping, Sequence
 
 from golem.managers import DemandManager
 from golem.node import GolemNode
 from golem.resources import Proposal
-from golem.utils.asyncio import create_task_with_logging, ensure_cancelled_many
-from golem.utils.logging import trace_span
+from golem.utils.asyncio import (
+    Buffer,
+    SimpleBuffer,
+    create_task_with_logging,
+    ensure_cancelled_many,
+)
+from golem.utils.logging import get_trace_id_name, trace_span
 
 
 class AggregatingDemandManager(DemandManager):
     """DemandManager that combines multiple get_initial_proposal functions into one."""
 
     def __init__(
         self,
@@ -20,15 +25,15 @@
         self._golem = golem
         self._get_initial_proposal_funcs = get_initial_proposal_funcs
 
         self._lock = asyncio.Lock()
 
         self._task_map: MutableMapping[Callable[[], Awaitable[Proposal]], asyncio.Task] = {}
 
-        self._queue: asyncio.Queue[Proposal] = asyncio.Queue()
+        self._buffer: Buffer[Proposal] = SimpleBuffer()
 
     @trace_span("Stopping AggregatingDemandManager", log_level=logging.INFO)
     async def stop(self) -> None:
         await ensure_cancelled_many(self._task_map.values())
         self._task_map.clear()
 
     @trace_span("Getting initial proposal", show_results=True)
@@ -37,25 +42,34 @@
 
         `get_initial_proposal_funcs` will be called concurrently, where not returned results will
         be saved and returned with the next call. If no proposals are saved, and some other
         functions are pending, completed functions will be run again. In case of multiple proposals
         are saved, they will be returned in completion  order.
         """
 
-        try:
-            return self._queue.get_nowait()
-        except asyncio.QueueEmpty:
-            pass
+        if self._buffer.size():
+            return await self._buffer.get()
 
         async with self._lock:
-            for func in self._get_initial_proposal_funcs:
+            for idx, func in enumerate(self._get_initial_proposal_funcs):
                 if func not in self._task_map:
-                    self._task_map[func] = create_task_with_logging(self._feed_queue(func))
+                    self._task_map[func] = create_task_with_logging(
+                        self._feed_queue(func),
+                        trace_id=get_trace_id_name(self, f"feed-func-{idx}"),
+                    )
 
-        return await self._queue.get()
+        return await self._buffer.get()
 
     async def _feed_queue(self, func: Callable[[], Awaitable[Proposal]]):
-        proposal = await func()
-        self._queue.put_nowait(proposal)
+        try:
+            proposal = await func()
+        except asyncio.CancelledError:
+            # we don't want to store cancellation error
+            raise
+        except Exception as e:
+            await self._buffer.set_exception(e)
+        else:
+            self._buffer.reset_exception()
+            await self._buffer.put(proposal)
 
         async with self._lock:
             del self._task_map[func]
```

### Comparing `golem_core-0.6.3/golem/managers/demand/refreshing.py` & `golem_core-0.7.0/golem/managers/demand/refreshing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/mixins.py` & `golem_core-0.7.0/golem/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/network/single.py` & `golem_core-0.7.0/golem/managers/network/single.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/payment/default.py` & `golem_core-0.7.0/golem/managers/payment/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         shutdown_timeout: timedelta = DEFAULT_SHUTDOWN_TIMEOUT,
     ):
         self._golem = golem
         self._budget = budget
         self._network = network
         self._driver = driver
         self._shutdown_timeout = shutdown_timeout.total_seconds()
+        self._lock = asyncio.Lock()
 
         self._allocation: Optional[Allocation] = None
 
         self._event_handlers: List = []
 
         self._agreements: Dict[str, Agreement] = {}
         self._no_agreements_event: asyncio.Event = asyncio.Event()
@@ -58,32 +59,35 @@
                 await self._golem.event_bus.on(NewDebitNote, self._handle_pay_debit_note_payment),
                 await self._golem.event_bus.on(NewAgreement, self._handle_new_agreement),
             ]
         )
 
     @trace_span("Getting allocation", show_results=True, log_level=logging.INFO)
     async def get_allocation(self) -> Allocation:
-        if self._allocation is None:
-            self._allocation = await self._create_allocation()
+        async with self._lock:
+            if not self._allocation:
+                self._allocation = await self._create_allocation(
+                    Decimal(self._budget),
+                    self._network,
+                    self._driver,
+                )
 
-        return self._allocation
+        return self._allocation  # type: ignore[return-value]
 
     async def _release_allocation(self) -> None:
         if self._allocation is None:
             return
 
         await self._allocation.release()
         self._allocation = None
 
-    @trace_span()
-    async def _create_allocation(self) -> Allocation:
+    @trace_span(show_arguments=True, show_results=True)
+    async def _create_allocation(self, budget: Decimal, network: str, driver: str) -> Allocation:
         try:
-            return await Allocation.create_any_account(
-                self._golem, Decimal(self._budget), self._network, self._driver
-            )
+            return await Allocation.create_any_account(self._golem, budget, network, driver)
         except ApiException as e:
             raise ManagerException(json.loads(e.body)["message"]) from e
 
     @trace_span("Stopping DefaultPaymentManager", log_level=logging.INFO)
     async def stop(self):
         """Terminate all related agreements."""
         try:
```

### Comparing `golem_core-0.6.3/golem/managers/proposal/__init__.py` & `golem_core-0.7.0/golem/managers/proposal/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/default.py` & `golem_core-0.7.0/golem/managers/proposal/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/__init__.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/blacklist.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/blacklist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/buffer.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,22 +67,25 @@
             self._max_size,
         )
 
     async def _on_expired(self, proposal: Proposal):
         logger.debug("Rejecting expired `%r` and requesting fill", proposal)
 
         try:
-            await proposal.reject("Proposal no longer needed due to its near expiration.")
+            if proposal.draft:
+                await proposal.reject("Proposal no longer needed due to its near expiration.")
         except ApiException as e:
             message = json.loads(e.body)["message"]
             if e.status == 400 and re.match(
-                r"^Subscription \[([^]]+)\] (wasn't found|expired).$", message
+                r"^Subscription \[([^]]+)\] (wasn't found|expired|was already unsubscribed).$",
+                message,
             ):
                 logger.warning(
-                    "Proposal assumed already expired. Consider shortening the expiry duration."
+                    f"Proposal assumed already expired. Consider shortening the expiry duration:"
+                    f" `{message}`"
                 )
             else:
                 raise
 
         await self._request_proposals()
 
         if self._on_expiration_func:
```

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/linear_coeffs.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/linear_coeffs.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/payment_platform.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/negotiating/payment_platform.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/reject_costs_exceeds.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/reject_costs_exceeds.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/__init__.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/map.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/mixins.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/pricings.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/pricings.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/property_value_lerp.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/scoring/scoring_buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/proposal/plugins/whitelist.py` & `golem_core-0.7.0/golem/managers/proposal/plugins/whitelist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/work/concurrent.py` & `golem_core-0.7.0/golem/managers/work/concurrent.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/work/mixins.py` & `golem_core-0.7.0/golem/managers/work/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/work/plugins.py` & `golem_core-0.7.0/golem/managers/work/plugins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/managers/work/sequential.py` & `golem_core-0.7.0/golem/managers/work/sequential.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/node/events.py` & `golem_core-0.7.0/golem/node/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/node/node.py` & `golem_core-0.7.0/golem/node/node.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/__init__.py` & `golem_core-0.7.0/golem/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/base.py` & `golem_core-0.7.0/golem/payload/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/constraints.py` & `golem_core-0.7.0/golem/payload/constraints.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/defaults.py` & `golem_core-0.7.0/golem/payload/defaults.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/generic.py` & `golem_core-0.7.0/golem/payload/generic.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/mixins.py` & `golem_core-0.7.0/golem/payload/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/parser.py` & `golem_core-0.7.0/golem/payload/parser.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/parser.tx` & `golem_core-0.7.0/golem/payload/parser.tx`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/properties.py` & `golem_core-0.7.0/golem/payload/properties.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/payload/vm.py` & `golem_core-0.7.0/golem/payload/vm.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/buffer.py` & `golem_core-0.7.0/golem/pipeline/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/chain.py` & `golem_core-0.7.0/golem/pipeline/chain.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/default_payment_handler.py` & `golem_core-0.7.0/golem/pipeline/default_payment_handler.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/exceptions.py` & `golem_core-0.7.0/golem/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/limit.py` & `golem_core-0.7.0/golem/pipeline/limit.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/map.py` & `golem_core-0.7.0/golem/pipeline/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/sort.py` & `golem_core-0.7.0/golem/pipeline/sort.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/pipeline/zip.py` & `golem_core-0.7.0/golem/pipeline/zip.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/__init__.py` & `golem_core-0.7.0/golem/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/activity/__init__.py` & `golem_core-0.7.0/golem/resources/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/activity/activity.py` & `golem_core-0.7.0/golem/resources/activity/activity.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/activity/commands.py` & `golem_core-0.7.0/golem/resources/activity/commands.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/activity/pipeline.py` & `golem_core-0.7.0/golem/resources/activity/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/agreement/agreement.py` & `golem_core-0.7.0/golem/resources/agreement/agreement.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         activity = await agreement.create_activity()
         # Use the activity
         await agreement.terminate()
     """
 
     def __init__(self, node: "GolemNode", id_: str, data: Optional[models.Agreement] = None):
         super().__init__(node, id_, data)
+        self._approved_at: Optional[datetime] = None
         asyncio.create_task(node.event_bus.emit(NewAgreement(self)))
 
     @api_call_wrapper()
     async def confirm(self) -> None:
         """Confirm the agreement.
 
         First step that leads to an active agreement.
@@ -47,15 +48,17 @@
         """Wait for provider's approval of the agreement.
 
         Second (and last) step leading to an active agreement.
 
         :returns: True if agreement was approved.
         """
         try:
+            approved_at = datetime.now(timezone.utc)
             await self.api.wait_for_approval(self.id, timeout=15, _request_timeout=16)
+            self._approved_at = approved_at
             return True
         except ApiException as e:
             if e.status == 410:
                 return False
             elif e.status == 408:
                 #   TODO: maybe this should be in api_call_wrapper?
                 return await self.wait_for_approval()
@@ -92,14 +95,18 @@
         except ApiException as e:
             if self._is_permanent_410(e):
                 pass
             else:
                 raise
 
     @property
+    def approved_at(self) -> Optional[datetime]:
+        return self._approved_at
+
+    @property
     def invoice(self) -> Optional[Invoice]:
         """:any:`Invoice` for this :any:`Agreement`, or None if we didn't yet receive an invoice."""
         try:
             return [child for child in self.children if isinstance(child, Invoice)][0]
         except IndexError:
             return None
 
@@ -157,15 +164,15 @@
     @property
     def proposal(self) -> "Proposal":
         return self.parent
 
     async def get_agreement_data(self, force=False) -> AgreementData:
         data = await self.get_data(force=force)
         agreement_duration = (
-            datetime.now(timezone.utc) - data.approved_date if data.approved_date else None
+            datetime.now(timezone.utc) - self.approved_at if self.approved_at else None
         )
         return AgreementData(
             agreement_id=data.agreement_id,
             provider_id=data.offer.provider_id,
             approved_date=data.approved_date,
             properties=data.offer.properties,  # type: ignore
             agreement_duration=agreement_duration,
```

### Comparing `golem_core-0.6.3/golem/resources/allocation/allocation.py` & `golem_core-0.7.0/golem/resources/allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/allocation/exceptions.py` & `golem_core-0.7.0/golem/resources/allocation/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/base.py` & `golem_core-0.7.0/golem/resources/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/debit_note/debit_note.py` & `golem_core-0.7.0/golem/resources/debit_note/debit_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,17 +182,15 @@
     async def validate_and_accept(self, allocation: Allocation) -> None:
         """Validate debit note and accept using a given :any:`Allocation`."""
         debit_note_data = await self.get_data(force=True)
         if debit_note_data.status != PayDocumentStatus.RECEIVED:
             logger.warning(f"Wrong status of debit_note {debit_note_data.status} != RECEIVED")
             return
 
-        agreement_data: "AgreementData" = await self.activity.agreement.get_agreement_data(
-            force=True
-        )
+        agreement_data: "AgreementData" = await self.activity.agreement.get_agreement_data()
 
         previous_debit_note = await self.get_previous_debit_note()
         previous_debit_notes_count = await self.get_previous_debit_notes_count()
         previous_payable_debit_notes_count = await self.get_previous_payable_debit_notes_count()
 
         try:
             total_amount_due = self.validate_payment_data(
```

### Comparing `golem_core-0.6.3/golem/resources/debit_note/event_collectors.py` & `golem_core-0.7.0/golem/resources/debit_note/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/demand/demand.py` & `golem_core-0.7.0/golem/resources/demand/demand.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/demand/demand_builder.py` & `golem_core-0.7.0/golem/resources/demand/demand_builder.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/event_collectors.py` & `golem_core-0.7.0/golem/resources/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/events.py` & `golem_core-0.7.0/golem/resources/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/exceptions.py` & `golem_core-0.7.0/golem/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/invoice/event_collectors.py` & `golem_core-0.7.0/golem/resources/invoice/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/invoice/invoice.py` & `golem_core-0.7.0/golem/resources/invoice/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,20 @@
     async def validate_and_accept(self, allocation: Allocation) -> None:
         """Validate invoice and accept using a given :any:`Allocation`."""
         invoice_data = await self.get_data(force=True)
         if invoice_data.status != PayDocumentStatus.RECEIVED:
             logger.warning(f"Wrong status of invoice {invoice_data.status} != RECEIVED")
             return
 
-        agreement_data: "AgreementData" = await self.agreement.get_agreement_data(force=True)
-        if agreement_data.agreement_duration is None:
+        if self.agreement.approved_at is None:
             logger.warning("Agreement was not approved")
             return
 
         try:
+            agreement_data: "AgreementData" = await self.agreement.get_agreement_data()
             amount_due = eth_decimal(invoice_data.amount)
             (
                 cumulative_time_since_last_dn,
                 cumulative_amount_since_last_dn,
             ) = await self.get_time_and_amount_since_latest_debit_notes(amount_due)
             coeffs = LinearCoeffs.from_properties(agreement_data.properties)
             infrastructure = InfrastructureProps.from_properties(agreement_data.properties)
```

### Comparing `golem_core-0.6.3/golem/resources/network/exceptions.py` & `golem_core-0.7.0/golem/resources/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/network/network.py` & `golem_core-0.7.0/golem/resources/network/network.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/pooling_batch/exceptions.py` & `golem_core-0.7.0/golem/resources/pooling_batch/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/pooling_batch/pooling_batch.py` & `golem_core-0.7.0/golem/resources/pooling_batch/pooling_batch.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/proposal/exceptions.py` & `golem_core-0.7.0/golem/resources/proposal/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/proposal/pipeline.py` & `golem_core-0.7.0/golem/resources/proposal/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/proposal/proposal.py` & `golem_core-0.7.0/golem/resources/proposal/proposal.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/utils/infrastructure.py` & `golem_core-0.7.0/golem/resources/utils/infrastructure.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/resources/utils/payment.py` & `golem_core-0.7.0/golem/resources/utils/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,29 +113,31 @@
 def validate_payment_max_cost(
     coeffs: LinearCoeffs,
     inf: InfrastructureProps,
     duration: timedelta,
     amount: Decimal,
     time_since_last_debit_note: Optional[timedelta] = None,
     amount_since_last_debit_note: Optional[Decimal] = None,
+    grace_period: timedelta = timedelta(minutes=1),
 ) -> Tuple[Decimal, Optional[Decimal]]:
     """Validate payment data max cost.
 
     Returns:
         maximum cost given `coeffs` and `infrastructure` could generate in
         - given `duration`
         - given `time_since_last_debit_note` if provided
 
     Raises: PaymentValidationException
     """
+    duration_grace = duration + grace_period
     max_cost = eth_decimal(
         coeffs.price_storage_gib * Decimal(inf.storage_gib)
         + coeffs.price_mem_gib * Decimal(inf.memory_gib)
-        + coeffs.price_cpu_sec * Decimal(inf.cpu_threads) * Decimal(duration.total_seconds())
-        + coeffs.price_duration_sec * Decimal(duration.total_seconds())
+        + coeffs.price_cpu_sec * Decimal(inf.cpu_threads) * Decimal(duration_grace.total_seconds())
+        + coeffs.price_duration_sec * Decimal(duration_grace.total_seconds())
         + coeffs.price_initial
     )
 
     if amount > max_cost:
         raise PaymentValidationException(
             "Total amount due exceeds expected max possible cost " f"{amount} > {max_cost}"
         )
```

### Comparing `golem_core-0.6.3/golem/utils/asyncio/__init__.py` & `golem_core-0.7.0/golem/utils/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/asyncio/buffer.py` & `golem_core-0.7.0/golem/utils/asyncio/buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import itertools
 import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from datetime import timedelta
 from typing import (
     Awaitable,
@@ -14,15 +15,17 @@
     Optional,
     Sequence,
     TypeVar,
 )
 
 from golem.utils.asyncio.semaphore import SingleUseSemaphore
 from golem.utils.asyncio.tasks import (
+    create_delayed_task_with_logging,
     create_task_with_logging,
+    ensure_cancelled,
     ensure_cancelled_many,
     resolve_maybe_awaitable,
 )
 from golem.utils.logging import get_trace_id_name
 from golem.utils.typing import MaybeAwaitable
 
 TItem = TypeVar("TItem")
@@ -225,97 +228,98 @@
         on_expired_func: Optional[Callable[[TItem], MaybeAwaitable[None]]] = None,
     ):
         super().__init__(buffer)
 
         self._get_expiration_func = get_expiration_func
         self._on_expired_func = on_expired_func
 
-        # TODO: Could this collection be liable to race conditions?
-        self._expiration_handlers: Dict[int, List[asyncio.TimerHandle]] = defaultdict(list)
+        self._expiration_tasks: Dict[int, List[asyncio.Task]] = defaultdict(list)
 
     async def _add_expiration_task_for_item(self, item: TItem) -> None:
         expiration = await resolve_maybe_awaitable(self._get_expiration_func(item))
 
         if expiration is None:
             return
 
-        loop = asyncio.get_event_loop()
-
-        self._expiration_handlers[id(item)].append(
-            loop.call_later(
-                expiration.total_seconds(),
-                lambda: create_task_with_logging(
-                    self._expire_item(item), trace_id=get_trace_id_name(self, f"item-expire-{item}")
-                ),
+        self._expiration_tasks[id(item)].append(
+            create_delayed_task_with_logging(
+                expiration,
+                self._expire_item_shielded(item),
+                trace_id=get_trace_id_name(self, f"item-expire-{item}"),
             )
         )
 
-    def _remove_expiration_handler_for_item(self, item: TItem) -> None:
+    async def _remove_expiration_task_for_item(self, item: TItem) -> None:
         item_id = id(item)
 
-        if item_id not in self._expiration_handlers or not len(self._expiration_handlers[item_id]):
+        if item_id not in self._expiration_tasks or not len(self._expiration_tasks[item_id]):
             return
 
-        expiration_handle = self._expiration_handlers[item_id].pop(0)
-        expiration_handle.cancel()
+        await ensure_cancelled(self._expiration_tasks[item_id].pop(0))
+
+        if not self._expiration_tasks[item_id]:
+            del self._expiration_tasks[item_id]
 
-        if not self._expiration_handlers[item_id]:
-            del self._expiration_handlers[item_id]
+    async def _remove_all_expiration_handlers(self) -> None:
+        await ensure_cancelled_many(itertools.chain.from_iterable(self._expiration_tasks.values()))
 
-    def _remove_all_expiration_handlers(self) -> None:
-        for handlers in self._expiration_handlers.values():
-            for handler in handlers:
-                handler.cancel()
+        self._expiration_tasks.clear()
 
-        self._expiration_handlers.clear()
+    async def _expire_item_shielded(self, item: TItem) -> None:
+        # We need to shield this function as by self.remove it will try to cancel itself
+        await asyncio.shield(self._expire_item(item))
+
+    async def _expire_item(self, item: TItem) -> None:
+        try:
+            await self.remove(item)
+        except ValueError:
+            # Item was removed in the meantime
+            return
+
+        if self._on_expired_func:
+            await resolve_maybe_awaitable(self._on_expired_func(item))
 
     async def get(self, *, lock=True) -> TItem:
         async with self._handle_lock(lock):
             item = await super().get(lock=False)
 
-            self._remove_expiration_handler_for_item(item)
+            await self._remove_expiration_task_for_item(item)
 
             return item
 
     async def get_all(self, *, lock=True) -> MutableSequence[TItem]:
         async with self._handle_lock(lock):
             items = await super().get_all(lock=False)
 
-            self._remove_all_expiration_handlers()
+            await self._remove_all_expiration_handlers()
 
             return items
 
     async def put(self, item: TItem, *, lock=True) -> None:
         async with self._handle_lock(lock):
             await super().put(item, lock=False)
 
             await self._add_expiration_task_for_item(item)
 
     async def put_all(self, items: Sequence[TItem], *, lock=True) -> None:
         async with self._handle_lock(lock):
             await super().put_all(items, lock=False)
 
-            self._remove_all_expiration_handlers()
+            await self._remove_all_expiration_handlers()
 
             await asyncio.gather(
                 *[self._add_expiration_task_for_item(item) for item in items],
                 return_exceptions=True,
             )
 
     async def remove(self, item: TItem, *, lock=True) -> None:
         async with self._handle_lock(lock):
             await super().remove(item, lock=False)
 
-            self._remove_expiration_handler_for_item(item)
-
-    async def _expire_item(self, item: TItem) -> None:
-        await self.remove(item)
-
-        if self._on_expired_func:
-            await resolve_maybe_awaitable(self._on_expired_func(item))
+            await self._remove_expiration_task_for_item(item)
 
 
 class BackgroundFillBuffer(ComposableBuffer[TItem]):
     """Composable `Buffer` that adds option to fill buffer in background tasks.
 
     Background fill will happen only if background tasks are started by calling `.start()`
     and items were requested by `.request()`.
```

### Comparing `golem_core-0.6.3/golem/utils/asyncio/queue.py` & `golem_core-0.7.0/golem/utils/asyncio/queue.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/asyncio/semaphore.py` & `golem_core-0.7.0/golem/utils/asyncio/semaphore.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/asyncio/tasks.py` & `golem_core-0.7.0/golem/utils/asyncio/tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,67 @@
 import asyncio
 import contextvars
 import inspect
 import logging
-from typing import Iterable, Optional, TypeVar, cast
+from datetime import timedelta
+from typing import Coroutine, Iterable, Optional, Tuple, TypeVar, cast
 
 from golem.utils.logging import trace_id_var
 from golem.utils.typing import MaybeAwaitable
 
 T = TypeVar("T")
 
 logger = logging.getLogger(__name__)
 
 
-def create_task_with_logging(coro, *, trace_id: Optional[str] = None) -> asyncio.Task:
+def create_task_with_logging(coro: Coroutine, *, trace_id: Optional[str] = None) -> asyncio.Task:
+    task, task_name = _create_task_with_context(coro, trace_id=trace_id)
+
+    logger.debug("Task `%s` created", task_name)
+
+    return task
+
+
+def create_delayed_task_with_logging(
+    delay: timedelta, coro: Coroutine, *, trace_id: Optional[str] = None
+) -> asyncio.Task:
+    task, task_name = _create_task_with_context(
+        _create_delayed_task_with_logging(delay, coro), trace_id=trace_id
+    )
+
+    logger.debug("Task `%s` created with delay `%s`", task_name, delay)
+
+    return task
+
+
+async def _create_delayed_task_with_logging(delay: timedelta, coro: Coroutine):
+    try:
+        await asyncio.sleep(delay.total_seconds())
+    except asyncio.CancelledError:
+        coro.close()
+        raise
+
+    return await coro
+
+
+def _create_task_with_context(
+    coro: Coroutine, *, trace_id: Optional[str] = None
+) -> Tuple[asyncio.Task, str]:
     context = contextvars.copy_context()
     task = context.run(_create_task_with_logging, coro, trace_id=trace_id)
 
     if trace_id is not None:
         task_name = trace_id
     else:
         task_name = task.get_name()
 
-    logger.debug("Task `%s` created", task_name)
-
-    return task
+    return task, task_name
 
 
-def _create_task_with_logging(coro, *, trace_id: Optional[str] = None) -> asyncio.Task:
+def _create_task_with_logging(coro: Coroutine, *, trace_id: Optional[str] = None) -> asyncio.Task:
     if trace_id is not None:
         trace_id_var.set(trace_id)
 
     task = asyncio.create_task(coro)
     task.add_done_callback(_handle_task_logging)
     return task
```

### Comparing `golem_core-0.6.3/golem/utils/asyncio/waiter.py` & `golem_core-0.7.0/golem/utils/asyncio/waiter.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/http.py` & `golem_core-0.7.0/golem/utils/http.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/logging.py` & `golem_core-0.7.0/golem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/low/api.py` & `golem_core-0.7.0/golem/utils/low/api.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/low/event_collector.py` & `golem_core-0.7.0/golem/utils/low/event_collector.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/storage/base.py` & `golem_core-0.7.0/golem/utils/storage/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/storage/gftp/provider.py` & `golem_core-0.7.0/golem/utils/storage/gftp/provider.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/storage/utils.py` & `golem_core-0.7.0/golem/utils/storage/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/golem/utils/typing.py` & `golem_core-0.7.0/golem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.3/pyproject.toml` & `golem_core-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "golem-core"
-version = "0.6.3"
+version = "0.7.0"
 description = "Golem Network (https://golem.network/) API for Python"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `golem_core-0.6.3/PKG-INFO` & `golem_core-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: golem-core
-Version: 0.6.3
+Version: 0.7.0
 Summary: Golem Network (https://golem.network/) API for Python
 Home-page: https://github.com/golemfactory/golem-core-python
 License: LGPL-3.0-or-later
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: async-exit-stack (==1.0.1)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jsonrpc-base (>=1.0.3,<2.0.0)
 Requires-Dist: prettytable (>=3.4.1,<4.0.0)
 Requires-Dist: semantic-version (>=2.8,<3.0)
```

