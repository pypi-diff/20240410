# Comparing `tmp/neptune-1.9.1.tar.gz` & `tmp/neptune-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-1.9.1.tar", max compression
+gzip compressed data, was "neptune-2.0.0a0.tar", max compression
```

## Comparing `neptune-1.9.1.tar` & `neptune-2.0.0a0.tar`

### file list

```diff
@@ -1,347 +1,280 @@
--rw-r--r--   0        0        0    40153 2024-02-15 11:39:11.949261 neptune-1.9.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-02-15 11:39:11.949261 neptune-1.9.1/LICENSE
--rw-r--r--   0        0        0    12786 2024-02-15 11:39:11.953261 neptune-1.9.1/README.md
--rw-r--r--   0        0        0    13431 2024-02-15 11:39:21.981269 neptune-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3606 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/__init__.py
--rw-r--r--   0        0        0      982 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/dtos.py
--rw-r--r--   0        0        0      990 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     7780 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1923 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2444 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2685 2024-02-15 11:39:11.953261 neptune-1.9.1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3021 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4609 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2594 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4432 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3525 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5403 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     4994 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10847 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5177 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     5211 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14767 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2481 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2024-02-15 11:39:11.957261 neptune-1.9.1/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7359 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7555 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/utils.py
--rw-r--r--   0        0        0     3284 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     1087 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1853 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2472 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/envs.py
--rw-r--r--   0        0        0    43813 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    32771 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3095 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1006 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0     1042 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0     1038 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5143 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7609 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9559 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6434 2024-02-15 11:39:11.961261 neptune-1.9.1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18149 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    43349 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9068 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    32457 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     2056 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4778 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5656 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    10284 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1537 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1154 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      689 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1723 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5124 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17296 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13125 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3070 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1430 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1144 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2423 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2919 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1695 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4947 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1787 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     2023 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3041 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5579 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2417 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2114 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5776 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2374 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10246 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2638 2024-02-15 11:39:11.965261 neptune-1.9.1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2211 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2021 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5232 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     4331 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.969261 neptune-1.9.1/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     4554 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    42137 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2013 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2367 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    26758 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9834 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0    15430 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0    13755 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    18238 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    26859 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     1576 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/structure_version.py
--rw-r--r--   0        0        0     5051 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/metadata_containers/utils.py
--rw-r--r--   0        0        0     2606 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-02-15 11:39:11.973261 neptune-1.9.1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11856 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3852 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3199 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/typing.py
--rw-r--r--   0        0        0     4621 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2240 2024-02-15 11:39:11.977261 neptune-1.9.1/src/neptune/version.py
--rw-r--r--   0        0        0    16499 1970-01-01 00:00:00.000000 neptune-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0    43968 2024-04-10 07:14:20.632583 neptune-2.0.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-10 07:14:20.632583 neptune-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0    12786 2024-04-10 07:14:20.632583 neptune-2.0.0a0/README.md
+-rw-r--r--   0        0        0    10949 2024-04-10 07:14:30.776590 neptune-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     2768 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/field_visitor.py
+-rw-r--r--   0        0        0    19028 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/models.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
+-rw-r--r--   0        0        0     1642 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
+-rw-r--r--   0        0        0     6126 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
+-rw-r--r--   0        0        0    17492 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
+-rw-r--r--   0        0        0      990 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     8193 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2105 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1923 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2446 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2665 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2139 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3023 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4585 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4432 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3505 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2057 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5391 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     5220 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10813 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5167 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0     1087 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2573 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/envs.py
+-rw-r--r--   0        0        0    42022 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    32661 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      775 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      795 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/mosaicml/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0     3633 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pandas/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3026 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5141 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2377 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     6311 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9567 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6338 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18056 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    45673 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     9535 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    32992 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2894 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     5864 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3948 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5005 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13843 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5658 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    15904 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1517 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1134 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2349 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      859 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/envs.py
+-rw-r--r--   0        0        0    15028 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1725 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3216 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2031 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1772 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1756 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5122 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3496 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1681 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      949 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2323 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2512 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0      933 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0     4784 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/oauth.py
+-rw-r--r--   0        0        0    17298 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13129 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3936 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
+-rw-r--r--   0        0        0     3070 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1422 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1146 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2443 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      886 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/patches/bravado.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2883 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1663 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4899 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1789 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/state.py
+-rw-r--r--   0        0        0     1130 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/__init__.py
+-rw-r--r--   0        0        0     3227 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/datastream.py
+-rw-r--r--   0        0        0     7330 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/storage_utils.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3066 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5581 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2409 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2116 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5746 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2300 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0     2490 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/git_info.py
+-rw-r--r--   0        0        0      849 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10577 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1152 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/iso_dates.py
+-rw-r--r--   0        0        0     1288 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2972 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0      726 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/patterns.py
+-rw-r--r--   0        0        0     2187 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1168 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/requirement_check.py
+-rw-r--r--   0        0        0     1566 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2266 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2001 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     7575 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/utils.py
+-rw-r--r--   0        0        0     4442 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0     3284 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/warnings.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3591 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2638 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     5210 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1231 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0     4795 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    44742 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2021 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      923 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/__init__.py
+-rw-r--r--   0        0        0     2351 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/abstract.py
+-rw-r--r--   0        0        0    15938 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/model.py
+-rw-r--r--   0        0        0    13843 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/model_version.py
+-rw-r--r--   0        0        0    26824 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/neptune_object.py
+-rw-r--r--   0        0        0    19268 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/project.py
+-rw-r--r--   0        0        0    26572 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/run.py
+-rw-r--r--   0        0        0     1576 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/structure_version.py
+-rw-r--r--   0        0        0     4043 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/utils.py
+-rw-r--r--   0        0        0     5783 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/table.py
+-rw-r--r--   0        0        0     1071 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    12157 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3854 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3210 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/typing.py
+-rw-r--r--   0        0        0     4252 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     1431 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/version.py
+-rw-r--r--   0        0        0    16631 1970-01-01 00:00:00.000000 neptune-2.0.0a0/PKG-INFO
```

### Comparing `neptune-1.9.1/CHANGELOG.md` & `neptune-2.0.0a0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,67 @@
+## [UNRELEASED] neptune 2.0.0
+
+### Breaking changes
+- Deleted `neptune.new` package ([#1684](https://github.com/neptune-ai/neptune-client/pull/1684))
+- Deleted `neptune.legacy` package ([#1685](https://github.com/neptune-ai/neptune-client/pull/1685))
+- Deleted `neptune.common` package ([#1693](https://github.com/neptune-ai/neptune-client/pull/1693))
+([#1690](https://github.com/neptune-ai/neptune-client/pull/1690))
+- Renamed `metadata_containers` to `objects` ([#1696](https://github.com/neptune-ai/neptune-client/pull/1696))
+- Removed `neptune-client` ([#1699](https://github.com/neptune-ai/neptune-client/pull/1699))
+- Deleted `neptune.logging` package ([#1698](https://github.com/neptune-ai/neptune-client/pull/1698))
+- Disabled `Model` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1701))
+- Disabled `ModelVersion` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1708))
+- Disabled `Project` ([#1709](https://github.com/neptune-ai/neptune-client/pull/1709))
+- Disabled `neptune command-line tool` ([#1718](https://github.com/neptune-ai/neptune-client/pull/1718))
+
+### Changes
+- Stop sending `X-Neptune-LegacyClient` header ([#1715](https://github.com/neptune-ai/neptune-client/pull/1715))
+- Use `tqdm.auto` ([#1717](https://github.com/neptune-ai/neptune-client/pull/1717))
+- Fields DTO conversion reworked ([#1722](https://github.com/neptune-ai/neptune-client/pull/1722))
+- Added support for Protocol Buffers ([#1728](https://github.com/neptune-ai/neptune-client/pull/1728))
+
+### Features
+- ?
+
+### Fixes
+- Fixed `tqdm.notebook` import only in Notebook environment ([#1716](https://github.com/neptune-ai/neptune-client/pull/1716))
+- Added `setuptools` to dependencies for `python >= 3.12` ([#1721](https://github.com/neptune-ai/neptune-client/pull/1721))
+
+
+## neptune 1.10.0
+
+### Features
+- Added `get_workspace_status()` method to management API ([#1662](https://github.com/neptune-ai/neptune-client/pull/1662))
+- Added auto-scaling pixel values for image logging ([#1664](https://github.com/neptune-ai/neptune-client/pull/1664))
+- Introduce querying capabilities to `fetch_runs_table()` ([#1660](https://github.com/neptune-ai/neptune-client/pull/1660))
+- Introduce querying capabilities to `fetch_models_table()` ([#1677](https://github.com/neptune-ai/neptune-client/pull/1677))
+- Introduce querying capabilities to `fetch_model_versions_table()` ([#1688](https://github.com/neptune-ai/neptune-client/pull/1688))
+
+### Fixes
+- Restored support for SSL verification exception ([#1661](https://github.com/neptune-ai/neptune-client/pull/1661))
+- Allow user to control logging level ([#1679](https://github.com/neptune-ai/neptune-client/pull/1679))
+- Fix sending data with forked container ([#1692](https://github.com/neptune-ai/neptune-client/pull/1692))
+
+### Changes
+- Improve dependency installation checking ([#1670](https://github.com/neptune-ai/neptune-client/pull/1670))
+- Cache dependencies check ([#1675](https://github.com/neptune-ai/neptune-client/pull/1675))
+- Improve datetime parsing in `fetch_*_table()` ([#1680](https://github.com/neptune-ai/neptune-client/pull/1680))
+- Remove deprecation warning in `fetch_runs_table()` ([#1686](https://github.com/neptune-ai/neptune-client/pull/1686))
+- Make sleep dur in some e2e tests consistent (#[1700](https://github.com/neptune-ai/neptune-client/pull/1700))
+- Minor updates to made package compatible with Python 3.11 and 3.12 ([#1678](https://github.com/neptune-ai/neptune-client/pull/1678))
+
+
 ## neptune 1.9.1
 
 ### Fixes
 - Fixed conda package ([#1652](https://github.com/neptune-ai/neptune-client/pull/1652))
+- Resource cleaning in PyTorch Dataloaders with multiple workers ([issue](https://github.com/neptune-ai/neptune-client/issues/1622)) ([#1649](https://github.com/neptune-ai/neptune-client/pull/1649))
+
+### Changes
+- Lazy initialization of operation processor when forking ([#1649](https://github.com/neptune-ai/neptune-client/pull/1649))
 
 
 ## neptune 1.9.0
 
 ### Features
 - Add support for seaborn figures ([#1613](https://github.com/neptune-ai/neptune-client/pull/1613))
 - Added fetching with iterators in `fetch_*_table()` methods ([#1585](https://github.com/neptune-ai/neptune-client/pull/1585))
```

### Comparing `neptune-1.9.1/LICENSE` & `neptune-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/README.md` & `neptune-2.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/__init__.py` & `neptune-2.0.0a0/src/neptune/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     "Model",
     "ModelVersion",
     "Project",
     "__version__",
 ]
 
 
-from neptune.common.patches import apply_patches
 from neptune.constants import ANONYMOUS_API_TOKEN
 from neptune.internal.extensions import load_extensions
-from neptune.metadata_containers import (
+from neptune.internal.patches import apply_patches
+from neptune.objects import (
     Model,
     ModelVersion,
     Project,
     Run,
 )
 from neptune.version import __version__
```

### Comparing `neptune-1.9.1/src/neptune/api/__init__.py` & `neptune-2.0.0a0/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/api/dtos.py` & `neptune-2.0.0a0/src/neptune/internal/types/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 #
-# Copyright (c) 2024, Neptune Labs Sp. z o.o.
+# Copyright (c) 2023, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__all__ = ["FileEntry"]
+__all__ = ["is_unsupported_float"]
 
-import datetime
-from dataclasses import dataclass
-from typing import Any
+import math
 
 
-@dataclass
-class FileEntry:
-    name: str
-    size: int
-    mtime: datetime.datetime
-    file_type: str
-
-    @classmethod
-    def from_dto(cls, file_dto: Any) -> "FileEntry":
-        return cls(name=file_dto.name, size=file_dto.size, mtime=file_dto.mtime, file_type=file_dto.fileType)
+def is_unsupported_float(value: float) -> bool:
+    if isinstance(value, float):
+        return math.isinf(value) or math.isnan(value)
+    return False
```

### Comparing `neptune-1.9.1/src/neptune/api/requests_utils.py` & `neptune-2.0.0a0/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/api/searching_entries.py` & `neptune-2.0.0a0/src/neptune/api/searching_entries.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,30 +17,34 @@
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Generator,
     Iterable,
-    List,
     Optional,
 )
 
 from bravado.client import construct_request  # type: ignore
 from bravado.config import RequestConfig  # type: ignore
+from bravado.exception import HTTPBadRequest  # type: ignore
 from typing_extensions import (
     Literal,
     TypeAlias,
 )
 
-from neptune.internal.backends.api_model import (
-    AttributeType,
-    AttributeWithProperties,
+from neptune.api.field_visitor import FieldToValueVisitor
+from neptune.api.models import (
+    Field,
+    FieldType,
+    LeaderboardEntriesSearchResult,
     LeaderboardEntry,
 )
+from neptune.api.proto.neptune_pb.api.model.leaderboard_entries_pb2 import ProtoLeaderboardEntriesSearchResultDTO
+from neptune.exceptions import NeptuneInvalidQueryException
 from neptune.internal.backends.hosted_client import DEFAULT_REQUEST_KWARGS
 from neptune.internal.backends.nql import (
     NQLAggregator,
     NQLAttributeOperator,
     NQLAttributeType,
     NQLEmptyQuery,
     NQLQuery,
@@ -52,15 +56,15 @@
 from neptune.typing import ProgressBarType
 
 if TYPE_CHECKING:
     from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
     from neptune.internal.id_formats import UniqueId
 
 
-SUPPORTED_ATTRIBUTE_TYPES = {item.value for item in AttributeType}
+SUPPORTED_ATTRIBUTE_TYPES = {item.value for item in FieldType}
 
 SORT_BY_COLUMN_TYPE: TypeAlias = Literal["string", "datetime", "integer", "boolean", "float"]
 
 
 class NoLimit(int):
     def __gt__(self, other: Any) -> bool:
         return True
@@ -84,23 +88,24 @@
 def get_single_page(
     *,
     client: "SwaggerClientWrapper",
     project_id: "UniqueId",
     attributes_filter: Dict[str, Any],
     limit: int,
     offset: int,
-    sort_by: Optional[str] = None,
-    sort_by_column_type: Optional[SORT_BY_COLUMN_TYPE] = None,
-    ascending: bool = False,
-    types: Optional[Iterable[str]] = None,
-    query: Optional["NQLQuery"] = None,
-    searching_after: Optional[str] = None,
-) -> Any:
+    sort_by: str,
+    sort_by_column_type: SORT_BY_COLUMN_TYPE,
+    ascending: bool,
+    types: Optional[Iterable[str]],
+    query: Optional["NQLQuery"],
+    searching_after: Optional[str],
+    use_proto: Optional[bool] = None,
+) -> LeaderboardEntriesSearchResult:
     normalized_query = query or NQLEmptyQuery()
-    sort_by_column_type = sort_by_column_type if sort_by_column_type else AttributeType.STRING.value
+    sort_by_column_type = sort_by_column_type if sort_by_column_type else FieldType.STRING.value
     if sort_by and searching_after:
         sort_by_as_nql = NQLQueryAttribute(
             name=sort_by,
             type=NQLAttributeType(sort_by_column_type),
             operator=NQLAttributeOperator.GREATER_THAN,
             value=searching_after,
         )
@@ -113,15 +118,15 @@
     sorting = (
         {
             "sorting": {
                 "dir": "ascending" if ascending else "descending",
                 "aggregationMode": "none",
                 "sortBy": {
                     "name": sort_by,
-                    "type": sort_by_column_type if sort_by_column_type else AttributeType.STRING.value,
+                    "type": sort_by_column_type if sort_by_column_type else FieldType.STRING.value,
                 },
             }
         }
         if sort_by
         else {}
     )
 
@@ -132,120 +137,120 @@
             **sorting,
             **attributes_filter,
             "query": {"query": str(normalized_query)},
             "pagination": {"limit": limit, "offset": offset},
         },
     }
 
-    request_options = DEFAULT_REQUEST_KWARGS.get("_request_options", {})
-    request_config = RequestConfig(request_options, True)
-    request_params = construct_request(client.api.searchLeaderboardEntries, request_options, **params)
-
-    http_client = client.swagger_spec.http_client
-
-    return (
-        http_client.request(request_params, operation=None, request_config=request_config)
-        .response()
-        .incoming_response.json()
-    )
-
-
-def to_leaderboard_entry(entry: Dict[str, Any]) -> LeaderboardEntry:
-    return LeaderboardEntry(
-        id=entry["experimentId"],
-        attributes=[
-            AttributeWithProperties(
-                path=attr["name"],
-                type=AttributeType(attr["type"]),
-                properties=attr.__getitem__(f"{attr['type']}Properties"),
+    try:
+        if use_proto:
+            result = client.api.searchLeaderboardEntriesProto(**params).response().result
+            proto_data = ProtoLeaderboardEntriesSearchResultDTO.FromString(result)
+            return LeaderboardEntriesSearchResult.from_proto(proto_data)
+        else:
+            request_options = DEFAULT_REQUEST_KWARGS.get("_request_options", {})
+            request_config = RequestConfig(request_options, True)
+            request_params = construct_request(client.api.searchLeaderboardEntries, request_options, **params)
+
+            http_client = client.swagger_spec.http_client
+
+            json_data = (
+                http_client.request(request_params, operation=None, request_config=request_config)
+                .response()
+                .incoming_response.json()
             )
-            for attr in entry["attributes"]
-            if attr["type"] in SUPPORTED_ATTRIBUTE_TYPES
-        ],
-    )
+
+            return LeaderboardEntriesSearchResult.from_dict(json_data)
+    except HTTPBadRequest as e:
+        title = e.response.json().get("title")
+        if title == "Syntax error":
+            raise NeptuneInvalidQueryException(nql_query=str(normalized_query))
+        raise e
 
 
-def find_attribute(*, entry: LeaderboardEntry, path: str) -> Optional[AttributeWithProperties]:
-    return next((attr for attr in entry.attributes if attr.path == path), None)
+def find_attribute(*, entry: LeaderboardEntry, path: str) -> Optional[Field]:
+    return next((attr for attr in entry.fields if attr.path == path), None)
 
 
 def iter_over_pages(
     *,
     step_size: int,
-    limit: Optional[int] = None,
-    sort_by: str = "sys/id",
+    limit: Optional[int],
+    sort_by: str,
+    sort_by_column_type: SORT_BY_COLUMN_TYPE,
+    ascending: bool,
+    progress_bar: Optional[ProgressBarType],
     max_offset: int = MAX_SERVER_OFFSET,
-    sort_by_column_type: Optional[SORT_BY_COLUMN_TYPE] = None,
-    ascending: bool = False,
-    progress_bar: Optional[ProgressBarType] = None,
     **kwargs: Any,
 ) -> Generator[Any, None, None]:
     searching_after = None
     last_page = None
 
-    total = get_single_page(
+    data = get_single_page(
         limit=0,
         offset=0,
+        sort_by=sort_by,
+        ascending=ascending,
+        sort_by_column_type=sort_by_column_type,
+        searching_after=None,
         **kwargs,
-    ).get("matchingItemCount", 0)
+    )
+    total = data.matching_item_count
 
     limit = limit if limit is not None else NoLimit()
 
     total = total if total < limit else limit
 
     progress_bar = False if total <= step_size else progress_bar  # disable progress bar if only one page is fetched
 
     extracted_records = 0
 
+    field_to_value_visitor = FieldToValueVisitor()
+
     with construct_progress_bar(progress_bar, "Fetching table...") as bar:
         # beginning of the first page
         bar.update(
             by=0,
             total=total,
         )
 
         while True:
             if last_page:
-                page_attribute = find_attribute(entry=last_page[-1], path=sort_by)
-
-                if not page_attribute:
+                searching_after_field = find_attribute(entry=last_page[-1], path=sort_by)
+                if not searching_after_field:
                     raise ValueError(f"Cannot find attribute {sort_by} in last page")
-
-                searching_after = page_attribute.properties["value"]
+                searching_after = field_to_value_visitor.visit(searching_after_field)
 
             for offset in range(0, max_offset, step_size):
                 local_limit = min(step_size, max_offset - offset)
                 if extracted_records + local_limit > limit:
                     local_limit = limit - extracted_records
+
                 result = get_single_page(
                     limit=local_limit,
                     offset=offset,
                     sort_by=sort_by,
                     sort_by_column_type=sort_by_column_type,
                     searching_after=searching_after,
                     ascending=ascending,
                     **kwargs,
                 )
 
                 # fetch the item count everytime a new page is started (except for the very fist page)
                 if offset == 0 and last_page is not None:
-                    total += result.get("matchingItemCount", 0)
+                    total += result.matching_item_count
 
                 total = min(total, limit)
 
-                page = _entries_from_page(result)
+                page = result.entries
                 extracted_records += len(page)
                 bar.update(by=len(page), total=total)
 
                 if not page:
                     return
 
                 yield from page
 
                 if extracted_records == limit:
                     return
 
                 last_page = page
-
-
-def _entries_from_page(single_page: Dict[str, Any]) -> List[LeaderboardEntry]:
-    return list(map(to_leaderboard_entry, single_page.get("entries", [])))
```

### Comparing `neptune-1.9.1/src/neptune/attributes/__init__.py` & `neptune-2.0.0a0/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/__init__.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/artifact.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/atom.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/boolean.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,22 +44,20 @@
                     source_attr_cls=source_attr.__class__,
                 ),
                 wait=wait,
             )
 
     @staticmethod
     @abc.abstractmethod
-    def create_assignment_operation(path, value: int):
-        ...
+    def create_assignment_operation(path, value: int): ...
 
     @staticmethod
     @abc.abstractmethod
     def getter(
         backend: "NeptuneBackend",
         container_id: str,
         container_type: ContainerType,
         path: typing.List[str],
-    ) -> int:
-        ...
+    ) -> int: ...
 
     def fetch(self):
         return self.getter(self._backend, self._container_id, self._container_type, self._path)
```

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/datetime.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/file.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/float.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/float.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # limitations under the License.
 #
 __all__ = ["Float"]
 
 import typing
 
 from neptune.attributes.atoms.copiable_atom import CopiableAtom
-from neptune.common.warnings import (
-    NeptuneUnsupportedValue,
-    warn_once,
-)
 from neptune.internal.container_type import ContainerType
 from neptune.internal.operation import AssignFloat
 from neptune.internal.types.utils import is_unsupported_float
+from neptune.internal.warnings import (
+    NeptuneUnsupportedValue,
+    warn_once,
+)
 from neptune.types.atoms.float import Float as FloatVal
 
 if typing.TYPE_CHECKING:
     from neptune.internal.backends.neptune_backend import NeptuneBackend
 
 
 class Float(CopiableAtom):
```

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/git_ref.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/integer.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/run_state.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/atoms/string.py` & `neptune-2.0.0a0/src/neptune/attributes/atoms/string.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 from neptune.internal.operation import AssignString
 from neptune.internal.utils.logger import get_logger
 from neptune.internal.utils.paths import path_to_str
 from neptune.types.atoms.string import String as StringVal
 
 if typing.TYPE_CHECKING:
     from neptune.internal.backends.neptune_backend import NeptuneBackend
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 logger = get_logger()
 
 
 class String(CopiableAtom):
 
     MAX_VALUE_LENGTH = 16384
 
-    def __init__(self, container: "MetadataContainer", path: typing.List[str]):
+    def __init__(self, container: "NeptuneObject", path: typing.List[str]):
         super().__init__(container, path)
         self._value_truncation_occurred = False
 
     @staticmethod
     def create_assignment_operation(path, value: str):
         return AssignString(path, value)
```

### Comparing `neptune-1.9.1/src/neptune/attributes/attribute.py` & `neptune-2.0.0a0/src/neptune/attributes/attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 from neptune.exceptions import TypeDoesNotSupportAttributeException
 from neptune.internal.backends.neptune_backend import NeptuneBackend
 from neptune.internal.operation import Operation
 from neptune.types.value_copy import ValueCopy
 
 if TYPE_CHECKING:
     from neptune.internal.container_type import ContainerType
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class Attribute:
     supports_copy = False
 
-    def __init__(self, container: "MetadataContainer", path: List[str]):
+    def __init__(self, container: "NeptuneObject", path: List[str]):
         super().__init__()
         self._container = container
         self._path = path
 
     def __getattr__(self, attr):
         raise TypeDoesNotSupportAttributeException(type_=type(self), attribute=attr)
```

### Comparing `neptune-1.9.1/src/neptune/attributes/constants.py` & `neptune-2.0.0a0/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/file_set.py` & `neptune-2.0.0a0/src/neptune/attributes/file_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import (
     Iterable,
     List,
     Optional,
     Union,
 )
 
-from neptune.api.dtos import FileEntry
+from neptune.api.models import FileEntry
 from neptune.attributes.attribute import Attribute
 from neptune.internal.operation import (
     DeleteFiles,
     UploadFileSet,
 )
 from neptune.internal.utils import (
     verify_collection_type,
```

### Comparing `neptune-1.9.1/src/neptune/attributes/namespace.py` & `neptune-2.0.0a0/src/neptune/attributes/namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 from neptune.internal.utils.paths import (
     parse_path,
     path_to_str,
 )
 from neptune.types.namespace import Namespace as NamespaceVal
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 logger = get_logger()
 RunStructure = ContainerStructure  # backwards compatibility
 
 
 class Namespace(Attribute, MutableMapping):
-    def __init__(self, container: "MetadataContainer", path: List[str]):
+    def __init__(self, container: "NeptuneObject", path: List[str]):
         Attribute.__init__(self, container, path)
         self._attributes = {}
         self._str_path = path_to_str(path)
 
     def __setitem__(self, k: str, v: Attribute) -> None:
         if not parse_path(k):
             logger.warning(
@@ -126,12 +126,12 @@
         prefix_len = len(self._path)
         for attr_name, attr_type, attr_value in attributes:
             run_struct.set(parse_path(attr_name)[prefix_len:], (attr_type, attr_value))
         return self._collect_atom_values(run_struct.get_structure())
 
 
 class NamespaceBuilder:
-    def __init__(self, container: "MetadataContainer"):
+    def __init__(self, container: "NeptuneObject"):
         self._run = container
 
     def __call__(self, path: List[str]) -> Namespace:
         return Namespace(self._run, path)
```

### Comparing `neptune-1.9.1/src/neptune/attributes/series/__init__.py` & `neptune-2.0.0a0/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/series/fetchable_series.py` & `neptune-2.0.0a0/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/series/file_series.py` & `neptune-2.0.0a0/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/series/float_series.py` & `neptune-2.0.0a0/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/series/series.py` & `neptune-2.0.0a0/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/series/string_series.py` & `neptune-2.0.0a0/src/neptune/attributes/series/string_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 from neptune.internal.utils import is_collection
 from neptune.internal.utils.logger import get_logger
 from neptune.internal.utils.paths import path_to_str
 from neptune.types.series.string_series import MAX_STRING_SERIES_VALUE_LENGTH
 from neptune.types.series.string_series import StringSeries as StringSeriesVal
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 Val = StringSeriesVal
 Data = str
 LogOperation = LogStrings
 
 logger = get_logger()
 
 
 class StringSeries(
     Series[Val, Data, LogOperation], FetchableSeries[StringSeriesValues], max_batch_size=10, operation_cls=LogOperation
 ):
-    def __init__(self, container: "MetadataContainer", path: List[str]):
+    def __init__(self, container: "NeptuneObject", path: List[str]):
         super().__init__(container, path)
         self._value_truncation_occurred = False
 
     def _get_log_operations_from_value(
         self,
         value: Val,
     ) -> List[LogOperation]:
```

### Comparing `neptune-1.9.1/src/neptune/attributes/sets/__init__.py` & `neptune-2.0.0a0/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/sets/set.py` & `neptune-2.0.0a0/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/sets/string_set.py` & `neptune-2.0.0a0/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/attributes/utils.py` & `neptune-2.0.0a0/src/neptune/attributes/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 __all__ = ["create_attribute_from_type"]
 
 from typing import (
     TYPE_CHECKING,
     List,
 )
 
+from neptune.api.models import FieldType
 from neptune.attributes import (
     Artifact,
     Boolean,
     Datetime,
     File,
     FileSeries,
     FileSet,
@@ -33,43 +34,42 @@
     Integer,
     NotebookRef,
     RunState,
     String,
     StringSeries,
     StringSet,
 )
-from neptune.common.exceptions import InternalClientError
-from neptune.internal.backends.api_model import AttributeType
+from neptune.internal.exceptions import InternalClientError
 
 if TYPE_CHECKING:
     from neptune.attributes.attribute import Attribute
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 _attribute_type_to_attr_class_map = {
-    AttributeType.FLOAT: Float,
-    AttributeType.INT: Integer,
-    AttributeType.BOOL: Boolean,
-    AttributeType.STRING: String,
-    AttributeType.DATETIME: Datetime,
-    AttributeType.FILE: File,
-    AttributeType.FILE_SET: FileSet,
-    AttributeType.FLOAT_SERIES: FloatSeries,
-    AttributeType.STRING_SERIES: StringSeries,
-    AttributeType.IMAGE_SERIES: FileSeries,
-    AttributeType.STRING_SET: StringSet,
-    AttributeType.GIT_REF: GitRef,
-    AttributeType.RUN_STATE: RunState,
-    AttributeType.NOTEBOOK_REF: NotebookRef,
-    AttributeType.ARTIFACT: Artifact,
+    FieldType.FLOAT: Float,
+    FieldType.INT: Integer,
+    FieldType.BOOL: Boolean,
+    FieldType.STRING: String,
+    FieldType.DATETIME: Datetime,
+    FieldType.FILE: File,
+    FieldType.FILE_SET: FileSet,
+    FieldType.FLOAT_SERIES: FloatSeries,
+    FieldType.STRING_SERIES: StringSeries,
+    FieldType.IMAGE_SERIES: FileSeries,
+    FieldType.STRING_SET: StringSet,
+    FieldType.GIT_REF: GitRef,
+    FieldType.OBJECT_STATE: RunState,
+    FieldType.NOTEBOOK_REF: NotebookRef,
+    FieldType.ARTIFACT: Artifact,
 }
 
 
 def create_attribute_from_type(
-    attribute_type: AttributeType,
-    container: "MetadataContainer",
+    attribute_type: FieldType,
+    container: "NeptuneObject",
     path: List[str],
 ) -> "Attribute":
     try:
         return _attribute_type_to_attr_class_map[attribute_type](container, path)
     except KeyError:
         raise InternalClientError(f"Unexpected type: {attribute_type}")
```

### Comparing `neptune-1.9.1/src/neptune/cli/__init__.py` & `neptune-2.0.0a0/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/__main__.py` & `neptune-2.0.0a0/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/clear.py` & `neptune-2.0.0a0/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/collect.py` & `neptune-2.0.0a0/src/neptune/cli/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 )
 from neptune.constants import (
     ASYNC_DIRECTORY,
     OFFLINE_DIRECTORY,
 )
 from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import UniqueId
-from neptune.metadata_containers.structure_version import StructureVersion
+from neptune.objects.structure_version import StructureVersion
 
 if TYPE_CHECKING:
     from neptune.internal.backends.neptune_backend import NeptuneBackend
 
 
 class CollectedContainers(NamedTuple):
     async_containers: List[AsyncContainer]
```

### Comparing `neptune-1.9.1/src/neptune/cli/commands.py` & `neptune-2.0.0a0/src/neptune/cli/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 import click
 
 from neptune.cli.clear import ClearRunner
 from neptune.cli.path_option import path_option
 from neptune.cli.status import StatusRunner
 from neptune.cli.sync import SyncRunner
+from neptune.exceptions import NeptuneUnsupportedFunctionalityException
 from neptune.internal.backends.hosted_neptune_backend import HostedNeptuneBackend
 from neptune.internal.credentials import Credentials
 
 
 @click.command()
 @path_option
 def status(path: Path) -> None:
@@ -48,14 +49,15 @@
     neptune status
 
     \b
     # List synchronized and unsynchronized objects in directory "foo/bar" without actually syncing
     neptune status --path foo/bar
     """
 
+    raise NeptuneUnsupportedFunctionalityException
     backend = HostedNeptuneBackend(Credentials.from_token())
 
     StatusRunner.status(backend=backend, path=path)
 
 
 @click.command()
 @path_option
@@ -123,14 +125,15 @@
     neptune sync --offline-only
 
     \b
     # Synchronize only the offline runs to project "workspace/project"
     neptune sync --project workspace/project --offline-only
     """
 
+    raise NeptuneUnsupportedFunctionalityException
     backend = HostedNeptuneBackend(Credentials.from_token())
 
     if offline_only:
         if object_names:
             raise click.BadParameter("--object and --offline-only are mutually exclusive")
 
         SyncRunner.sync_all_offline(backend=backend, base_path=path, project_name=project_name)
@@ -155,10 +158,12 @@
     # Clear junk metadata from local storage
     neptune clear
 
     \b
     # Clear junk metadata from directory "foo/bar"
     neptune clear --path foo/bar
     """
+
+    raise NeptuneUnsupportedFunctionalityException
     backend = HostedNeptuneBackend(Credentials.from_token())
 
     ClearRunner.clear(backend=backend, path=path)
```

### Comparing `neptune-1.9.1/src/neptune/cli/containers.py` & `neptune-2.0.0a0/src/neptune/cli/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     Callable,
     Dict,
     List,
     Optional,
 )
 
 from neptune.cli.utils import get_qualified_name
-from neptune.common.exceptions import NeptuneConnectionLostException
 from neptune.constants import ASYNC_DIRECTORY
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.core.components.queue.disk_queue import DiskQueue
 from neptune.envs import NEPTUNE_SYNC_BATCH_TIMEOUT_ENV
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneConnectionLostException
 from neptune.internal.id_formats import UniqueId
 from neptune.internal.operation import Operation
 from neptune.internal.operation_processors.utils import get_container_dir
 from neptune.internal.utils.logger import get_logger
-from neptune.metadata_containers.structure_version import StructureVersion
+from neptune.objects.structure_version import StructureVersion
 
 if TYPE_CHECKING:
     from neptune.internal.backends.api_model import (
         ApiExperiment,
         Project,
     )
     from neptune.internal.backends.neptune_backend import NeptuneBackend
@@ -145,29 +145,26 @@
         self._path = base_path / ASYNC_DIRECTORY / new_online_dir
         self._structure_version = StructureVersion.DIRECT_DIRECTORY
 
 
 class Container(ABC):
     @property
     @abstractmethod
-    def container_id(self) -> UniqueId:
-        ...
+    def container_id(self) -> UniqueId: ...
 
     @property
     @abstractmethod
-    def execution_dirs(self) -> List[ExecutionDirectory]:
-        ...
+    def execution_dirs(self) -> List[ExecutionDirectory]: ...
 
     @property
     def synced(self) -> bool:
         return all(map(lambda execution_dir: execution_dir.synced, self.execution_dirs))
 
     @abstractmethod
-    def sync(self, *, base_path: Path, backend: "NeptuneBackend", project: Optional["Project"] = None) -> None:
-        ...
+    def sync(self, *, base_path: Path, backend: "NeptuneBackend", project: Optional["Project"] = None) -> None: ...
 
     def clear(self) -> None:
         for execution_dir in self.execution_dirs:
             execution_dir.clear()
 
         for execution_dir in self.execution_dirs:
             if execution_dir.parent is not None:
```

### Comparing `neptune-1.9.1/src/neptune/cli/path_option.py` & `neptune-2.0.0a0/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/status.py` & `neptune-2.0.0a0/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/sync.py` & `neptune-2.0.0a0/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/cli/utils.py` & `neptune-2.0.0a0/src/neptune/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,34 +32,34 @@
     Callable,
     Dict,
     Optional,
     Tuple,
     Union,
 )
 
-from neptune.common.exceptions import NeptuneException
 from neptune.core.components.queue.disk_queue import DiskQueue
 from neptune.envs import PROJECT_ENV_NAME
 from neptune.exceptions import (
     MetadataContainerNotFound,
     ProjectNotFound,
 )
 from neptune.internal.backends.api_model import (
     ApiExperiment,
     Project,
 )
 from neptune.internal.backends.neptune_backend import NeptuneBackend
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.id_formats import (
     QualifiedName,
     UniqueId,
 )
 from neptune.internal.operation import Operation
 from neptune.internal.utils.logger import get_logger
-from neptune.metadata_containers.structure_version import StructureVersion
+from neptune.objects.structure_version import StructureVersion
 
 logger = get_logger(with_prefix=False)
 
 
 def get_metadata_container(
     backend: NeptuneBackend,
     container_id: Union[UniqueId, QualifiedName],
```

### Comparing `neptune-1.9.1/src/neptune/common/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/backends/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/envs.py` & `neptune-2.0.0a0/src/neptune/internal/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/exceptions.py` & `neptune-2.0.0a0/src/neptune/internal/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import platform
+from typing import (
+    Any,
+    Optional,
+)
 
-from neptune.common.envs import (
+from neptune.internal.envs import (
     API_TOKEN_ENV_NAME,
     PROJECT_ENV_NAME,
 )
 
 UNIX_STYLES = {
     "h1": "\033[95m",
     "h2": "\033[94m",
@@ -65,26 +69,26 @@
 elif platform.system() == "Windows":
     STYLES = WINDOWS_STYLES
 else:
     STYLES = EMPTY_STYLES
 
 
 class NeptuneException(Exception):
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if type(other) is type(self):
             return super().__eq__(other) and str(self).__eq__(str(other))
         else:
             return False
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((super().__hash__(), str(self)))
 
 
 class NeptuneInvalidApiTokenException(NeptuneException):
-    def __init__(self):
+    def __init__(self) -> None:
         message = """
 {h1}
 ----NeptuneInvalidApiTokenException------------------------------------------------
 {end}
 The provided API token is invalid.
 Make sure you copied and provided your API token correctly.
 
@@ -118,20 +122,20 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         super().__init__(message.format(env_api_token=API_TOKEN_ENV_NAME, **STYLES))
 
 
 class UploadedFileChanged(NeptuneException):
-    def __init__(self, filename: str):
+    def __init__(self, filename: str) -> None:
         super().__init__("File {} changed during upload, restarting upload.".format(filename))
 
 
 class InternalClientError(NeptuneException):
-    def __init__(self, msg: str):
+    def __init__(self, msg: str) -> None:
         message = """
 {h1}
 ----InternalClientError-----------------------------------------------------------------------
 {end}
 The Neptune client library encountered an unexpected internal error:
 {msg}
 
@@ -139,15 +143,15 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         super().__init__(message.format(msg=msg, **STYLES))
 
 
 class ClientHttpError(NeptuneException):
-    def __init__(self, status, response):
+    def __init__(self, status: str, response: str) -> None:
         self.status = status
         self.response = response
         message = """
 {h1}
 ----ClientHttpError-----------------------------------------------------------------------
 {end}
 The Neptune server returned the status {fail}{status}{end}.
@@ -163,15 +167,15 @@
 
 
 class NeptuneApiException(NeptuneException):
     pass
 
 
 class Forbidden(NeptuneApiException):
-    def __init__(self):
+    def __init__(self) -> None:
         message = """
 {h1}
 ----Forbidden-----------------------------------------------------------------------
 {end}
 You don't have permission to access the given resource.
 
     - Verify that your API token is correct.
@@ -187,15 +191,15 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         super().__init__(message.format(**STYLES))
 
 
 class Unauthorized(NeptuneApiException):
-    def __init__(self, msg=None):
+    def __init__(self, msg: Optional[str] = None) -> None:
         default_message = """
 {h1}
 ----Unauthorized-----------------------------------------------------------------------
 {end}
 You don't have permission to access the given resource.
 
     - Verify that your API token is correct.
@@ -212,20 +216,20 @@
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         message = msg if msg is not None else default_message
         super().__init__(message.format(**STYLES))
 
 
 class NeptuneAuthTokenExpired(Unauthorized):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("Authorization token expired")
 
 
 class InternalServerError(NeptuneApiException):
-    def __init__(self, response):
+    def __init__(self, response: str) -> None:
         message = """
 {h1}
 ----InternalServerError-----------------------------------------------------------------------
 {end}
 The Neptune client library encountered an unexpected internal server error.
 
 The server response was:
@@ -235,15 +239,15 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         super().__init__(message.format(response=response, **STYLES))
 
 
 class NeptuneConnectionLostException(NeptuneException):
-    def __init__(self, cause: Exception):
+    def __init__(self, cause: Exception) -> None:
         self.cause = cause
         message = """
 {h1}
 ----NeptuneConnectionLostException---------------------------------------------------------
 {end}
 The connection to the Neptune server was lost.
 If you are using the asynchronous (default) connection mode, Neptune continues to locally track your metadata and continuously tries to re-establish a connection to the Neptune servers.
@@ -264,15 +268,15 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """  # noqa: E501
         super().__init__(message.format(**STYLES))
 
 
 class NeptuneSSLVerificationError(NeptuneException):
-    def __init__(self):
+    def __init__(self) -> None:
         message = """
 {h1}
 ----NeptuneSSLVerificationError-----------------------------------------------------------------------
 {end}
 
 The Neptune client was unable to verify your SSL Certificate.
 
@@ -315,27 +319,27 @@
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """  # noqa: E501
         super().__init__(message.format(**STYLES))
 
 
 class FileNotFound(NeptuneException):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super(FileNotFound, self).__init__("File {} doesn't exist.".format(path))
 
 
 class InvalidNotebookPath(NeptuneException):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super(InvalidNotebookPath, self).__init__(
             "File {} is not a valid notebook. Should end with .ipynb.".format(path)
         )
 
 
 class NeptuneIncorrectProjectQualifiedNameException(NeptuneException):
-    def __init__(self, project_qualified_name):
+    def __init__(self, project_qualified_name: str) -> None:
         message = """
 {h1}
 ----NeptuneIncorrectProjectQualifiedNameException-----------------------------------------------------------------------
 {end}
 Project qualified name {fail}"{project_qualified_name}"{end} you specified was incorrect.
 
 The correct project qualified name should look like this {correct}WORKSPACE/PROJECT_NAME{end}.
@@ -357,15 +361,15 @@
 """
         super(NeptuneIncorrectProjectQualifiedNameException, self).__init__(
             message.format(project_qualified_name=project_qualified_name, **STYLES)
         )
 
 
 class NeptuneMissingProjectQualifiedNameException(NeptuneException):
-    def __init__(self):
+    def __init__(self) -> None:
         message = """
 {h1}
 ----NeptuneMissingProjectQualifiedNameException-------------------------------------------------------------------------
 {end}
 Neptune client couldn't find your project name.
 
 There are two options two add it:
@@ -398,25 +402,25 @@
 """
         super(NeptuneMissingProjectQualifiedNameException, self).__init__(
             message.format(env_project=PROJECT_ENV_NAME, **STYLES)
         )
 
 
 class NotAFile(NeptuneException):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super(NotAFile, self).__init__("Path {} is not a file.".format(path))
 
 
 class NotADirectory(NeptuneException):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super(NotADirectory, self).__init__("Path {} is not a directory.".format(path))
 
 
 class WritingToArchivedProjectException(NeptuneException):
-    def __init__(self):
+    def __init__(self) -> None:
         message = """
 {h1}
 ----WritingToArchivedProjectException-----------------------------------------------------------------------
 {end}
 You're trying to write to a project that was archived.
 
 Set the project as active again or use mode="read-only" at initialization to fetch metadata from it.
```

### Comparing `neptune-1.9.1/src/neptune/common/experiments.py` & `neptune-2.0.0a0/src/neptune/api/proto/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-class LegacyExperiment:
-    pass
```

### Comparing `neptune-1.9.1/src/neptune/common/git_info.py` & `neptune-2.0.0a0/src/neptune/internal/utils/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/cgroup/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import time
 
-from neptune.common.hardware.cgroup.cgroup_filesystem_reader import CGroupFilesystemReader
-from neptune.common.hardware.system.system_monitor import SystemMonitor
+from neptune.internal.hardware.cgroup.cgroup_filesystem_reader import CGroupFilesystemReader
+from neptune.internal.hardware.system.system_monitor import SystemMonitor
 
 
 class CGroupMonitor(object):
     def __init__(self, cgroup_filesystem_reader, system_monitor):
         self.__cgroup_filesystem_reader = cgroup_filesystem_reader
         self.__system_monitor = system_monitor
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/constants.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/cpu.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/cpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from neptune.common.hardware.cgroup.cgroup_monitor import CGroupMonitor
-from neptune.common.hardware.gauges.gauge import Gauge
-from neptune.common.hardware.system.system_monitor import SystemMonitor
+from neptune.internal.hardware.cgroup.cgroup_monitor import CGroupMonitor
+from neptune.internal.hardware.gauges.gauge import Gauge
+from neptune.internal.hardware.system.system_monitor import SystemMonitor
 
 
 class SystemCpuUsageGauge(Gauge):
     def __init__(self):
         self.__system_monitor = SystemMonitor()
 
     def name(self):
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.gauges.cpu import (
+from neptune.internal.hardware.gauges.cpu import (
     CGroupCpuUsageGauge,
     SystemCpuUsageGauge,
 )
-from neptune.common.hardware.gauges.gauge_mode import GaugeMode
-from neptune.common.hardware.gauges.gpu import (
+from neptune.internal.hardware.gauges.gauge_mode import GaugeMode
+from neptune.internal.hardware.gauges.gpu import (
     GpuMemoryGauge,
     GpuUsageGauge,
 )
-from neptune.common.hardware.gauges.memory import (
+from neptune.internal.hardware.gauges.memory import (
     CGroupMemoryUsageGauge,
     SystemMemoryUsageGauge,
 )
 
 
 class GaugeFactory(object):
     def __init__(self, gauge_mode):
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/gpu.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.constants import BYTES_IN_ONE_GB
-from neptune.common.hardware.gauges.gauge import Gauge
-from neptune.common.hardware.gpu.gpu_monitor import GPUMonitor
+from neptune.internal.hardware.constants import BYTES_IN_ONE_GB
+from neptune.internal.hardware.gauges.gauge import Gauge
+from neptune.internal.hardware.gpu.gpu_monitor import GPUMonitor
 
 
 class GpuUsageGauge(Gauge):
     def __init__(self, card_index):
         self.card_index = card_index
         self.__gpu_monitor = GPUMonitor()
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gauges/memory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from neptune.common.hardware.cgroup.cgroup_monitor import CGroupMonitor
-from neptune.common.hardware.constants import BYTES_IN_ONE_GB
-from neptune.common.hardware.gauges.gauge import Gauge
-from neptune.common.hardware.system.system_monitor import SystemMonitor
+from neptune.internal.hardware.cgroup.cgroup_monitor import CGroupMonitor
+from neptune.internal.hardware.constants import BYTES_IN_ONE_GB
+from neptune.internal.hardware.gauges.gauge import Gauge
+from neptune.internal.hardware.system.system_monitor import SystemMonitor
 
 
 class SystemMemoryUsageGauge(Gauge):
     def __init__(self):
         self.__system_monitor = SystemMonitor()
 
     def name(self):
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gpu/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["GPUMonitor"]
 
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
+from neptune.internal.utils.logger import get_logger
 from neptune.vendor.pynvml import (
     NVMLError,
     nvmlDeviceGetCount,
     nvmlDeviceGetHandleByIndex,
     nvmlDeviceGetMemoryInfo,
     nvmlDeviceGetUtilizationRates,
     nvmlInit,
 )
 
+_logger = get_logger()
+
 
 class GPUMonitor(object):
 
     nvml_error_printed = False
 
     def get_card_count(self):
         return self.__nvml_get_or_else(nvmlDeviceGetCount, default=0)
@@ -58,16 +58,16 @@
             return 0
         return max(memory_per_card)
 
     def __nvml_get_or_else(self, getter, default=None):
         try:
             nvmlInit()
             return getter()
-        except NVMLError:
+        except NVMLError as e:
             if not GPUMonitor.nvml_error_printed:
                 warning = (
                     "Info (NVML): %s. GPU usage metrics may not be reported. For more information, "
                     "see https://docs.neptune.ai/help/nvml_error/"
                 )
-                warn_once(message=warning, exception=NeptuneWarning)
+                _logger.warning(warning, e)
                 GPUMonitor.nvml_error_printed = True
             return default
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/metric.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.constants import BYTES_IN_ONE_GB
-from neptune.common.hardware.metrics.metric import (
+from neptune.internal.hardware.constants import BYTES_IN_ONE_GB
+from neptune.internal.hardware.metrics.metric import (
     Metric,
     MetricResourceType,
 )
-from neptune.common.hardware.metrics.metrics_container import MetricsContainer
+from neptune.internal.hardware.metrics.metrics_container import MetricsContainer
 
 
 class MetricsFactory(object):
     def __init__(self, gauge_factory, system_resource_info):
         self.__gauge_factory = gauge_factory
         self.__system_resource_info = system_resource_info
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.metrics.reports.metric_report import (
+from neptune.internal.hardware.metrics.reports.metric_report import (
     MetricReport,
     MetricValue,
 )
 
 
 class MetricReporter(object):
     def __init__(self, metrics, reference_timestamp):
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.metrics.reports.metric_reporter import MetricReporter
+from neptune.internal.hardware.metrics.reports.metric_reporter import MetricReporter
 
 
 class MetricReporterFactory(object):
     def __init__(self, reference_timestamp):
         self.__reference_timestamp = reference_timestamp
 
     def create(self, metrics):
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from neptune.common.hardware.gauges.gauge_factory import GaugeFactory
-from neptune.common.hardware.gpu.gpu_monitor import GPUMonitor
-from neptune.common.hardware.metrics.metrics_factory import MetricsFactory
-from neptune.common.hardware.metrics.reports.metric_reporter_factory import MetricReporterFactory
-from neptune.common.hardware.metrics.service.metric_service import MetricService
-from neptune.common.hardware.resources.system_resource_info_factory import SystemResourceInfoFactory
-from neptune.common.hardware.system.system_monitor import SystemMonitor
+from neptune.internal.hardware.gauges.gauge_factory import GaugeFactory
+from neptune.internal.hardware.gpu.gpu_monitor import GPUMonitor
+from neptune.internal.hardware.metrics.metrics_factory import MetricsFactory
+from neptune.internal.hardware.metrics.reports.metric_reporter_factory import MetricReporterFactory
+from neptune.internal.hardware.metrics.service.metric_service import MetricService
+from neptune.internal.hardware.resources.system_resource_info_factory import SystemResourceInfoFactory
+from neptune.internal.hardware.system.system_monitor import SystemMonitor
 
 
 class MetricServiceFactory(object):
     def __init__(self, backend, os_environ):
         self.__backend = backend
         self.__os_environ = os_environ
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/resources/__init__.py` & `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from neptune.common.hardware.cgroup.cgroup_monitor import CGroupMonitor
-from neptune.common.hardware.gauges.gauge_mode import GaugeMode
-from neptune.common.hardware.resources.gpu_card_indices_provider import GPUCardIndicesProvider
-from neptune.common.hardware.resources.system_resource_info import SystemResourceInfo
+from neptune.internal.hardware.cgroup.cgroup_monitor import CGroupMonitor
+from neptune.internal.hardware.gauges.gauge_mode import GaugeMode
+from neptune.internal.hardware.resources.gpu_card_indices_provider import GPUCardIndicesProvider
+from neptune.internal.hardware.resources.system_resource_info import SystemResourceInfo
 
 
 class SystemResourceInfoFactory(object):
     def __init__(self, system_monitor, gpu_monitor, os_environ):
         self.__system_monitor = system_monitor
         self.__gpu_monitor = gpu_monitor
         self.__gpu_card_indices_provider = GPUCardIndicesProvider(
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/system/__init__.py` & `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `neptune-1.9.1/src/neptune/common/hardware/system/system_monitor.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/oauth.py` & `neptune-2.0.0a0/src/neptune/internal/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from oauthlib.oauth2 import (
     OAuth2Error,
     TokenExpiredError,
 )
 from requests.auth import AuthBase
 from requests_oauthlib import OAuth2Session
 
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.exceptions import NeptuneInvalidApiTokenException
-from neptune.common.utils import update_session_proxies
+from neptune.internal.backends.utils import with_api_exceptions_handler
+from neptune.internal.exceptions import NeptuneInvalidApiTokenException
+from neptune.internal.utils.utils import update_session_proxies
 
 _decoding_options = {
     "verify_signature": False,
     "verify_exp": False,
     "verify_nbf": False,
     "verify_iat": False,
     "verify_aud": False,
```

### Comparing `neptune-1.9.1/src/neptune/common/patches/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/patches/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["apply_patches"]
 
-from neptune.common.patches.bravado import patch as bravado_patch
+from neptune.internal.patches.bravado import patch as bravado_patch
 
 patches = [bravado_patch]
 
 
 # Apply patches when importing a patching module
 # Should be called before usages of patched objects
 def apply_patches():
```

### Comparing `neptune-1.9.1/src/neptune/common/patches/bravado.py` & `neptune-2.0.0a0/src/neptune/internal/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/patterns.py` & `neptune-2.0.0a0/src/neptune/internal/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/storage/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/storage/datastream.py` & `neptune-2.0.0a0/src/neptune/internal/storage/datastream.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import tarfile
 from typing import (
     Any,
     Generator,
     Optional,
 )
 
-from neptune.common.backends.api_model import MultipartConfig
-from neptune.common.exceptions import (
+from neptune.internal.backends.api_model import MultipartConfig
+from neptune.internal.exceptions import (
     InternalClientError,
     UploadedFileChanged,
 )
 
 
 @dataclasses.dataclass
 class FileChunk:
```

### Comparing `neptune-1.9.1/src/neptune/common/storage/storage_utils.py` & `neptune-2.0.0a0/src/neptune/internal/storage/storage_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     BinaryIO,
     Generator,
     List,
     Set,
     Union,
 )
 
-import six
-
 from neptune.internal.utils.logger import get_logger
 
 _logger = get_logger()
 
 
 @dataclass
 class AttributeUploadConfiguration:
@@ -160,16 +158,15 @@
     def __repr__(self):
         """
         For `print` and `pprint`
         """
         return self.to_str()
 
 
-@six.add_metaclass(ABCMeta)
-class ProgressIndicator(object):
+class ProgressIndicator(metaclass=ABCMeta):
     @abstractmethod
     def progress(self, steps):
         pass
 
     @abstractmethod
     def complete(self):
         pass
```

### Comparing `neptune-1.9.1/src/neptune/common/utils.py` & `neptune-2.0.0a0/src/neptune/internal/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 import re
 import ssl
 import sys
 
 import numpy as np
 import pandas as pd
 
-from neptune.common import envs
-from neptune.common.exceptions import (
+from neptune.internal import envs
+from neptune.internal.exceptions import (
     FileNotFound,
     InvalidNotebookPath,
     NeptuneIncorrectProjectQualifiedNameException,
     NeptuneMissingProjectQualifiedNameException,
     NotADirectory,
     NotAFile,
 )
-from neptune.common.git_info import GitInfo
-from neptune.common.patterns import PROJECT_QUALIFIED_NAME_PATTERN
+from neptune.internal.utils.git_info import GitInfo
 from neptune.internal.utils.logger import get_logger
+from neptune.internal.utils.patterns import PROJECT_QUALIFIED_NAME_PATTERN
 
 _logger = get_logger()
 
 IS_WINDOWS = sys.platform == "win32"
 IS_MACOS = sys.platform == "darwin"
```

### Comparing `neptune-1.9.1/src/neptune/common/warnings.py` & `neptune-2.0.0a0/src/neptune/internal/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/websockets/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune-2.0.0a0/src/neptune/internal/websockets/reconnecting_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import random
 
 from websocket import (
     WebSocketConnectionClosedException,
     WebSocketTimeoutException,
 )
 
-from neptune.common.websockets.websocket_client_adapter import (
+from neptune.internal.websockets.websocket_client_adapter import (
     WebsocketClientAdapter,
     WebsocketNotConnectedException,
 )
 
 
 class ReconnectingWebsocket(object):
     def __init__(self, url, oauth2_session, shutdown_event, proxies=None):
```

### Comparing `neptune-1.9.1/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune-2.0.0a0/src/neptune/internal/websockets/websocket_client_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import ssl
+import urllib.parse
 
-from future.utils import PY3
-from six.moves import urllib
 from websocket import (
     ABNF,
     create_connection,
 )
 
 
 class WebsocketClientAdapter(object):
@@ -58,15 +57,15 @@
             raise WebsocketNotConnectedException()
 
         opcode, data = None, None
 
         while opcode != ABNF.OPCODE_TEXT:
             opcode, data = self._ws_client.recv_data()
 
-        return data.decode("utf-8") if PY3 else data
+        return data.decode("utf-8")
 
     @property
     def connected(self):
         return self._ws_client and self._ws_client.connected
 
     def close(self):
         if self._ws_client:
```

### Comparing `neptune-1.9.1/src/neptune/constants.py` & `neptune-2.0.0a0/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/__init__.py` & `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/__init__.py` & `neptune-2.0.0a0/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/abstract.py` & `neptune-2.0.0a0/src/neptune/core/components/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,48 +29,44 @@
 
 
 class AutoCloseable(ABC):
     def __enter__(self) -> AutoCloseable:
         return self
 
     @abstractmethod
-    def close(self) -> None:
-        ...
+    def close(self) -> None: ...
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         self.close()
 
 
 class Resource(AutoCloseable):
     @abstractmethod
-    def cleanup(self) -> None:
-        ...
+    def cleanup(self) -> None: ...
 
     def flush(self) -> None:
         pass
 
     def close(self) -> None:
         self.flush()
 
     @property
     @abstractmethod
-    def data_path(self) -> Path:
-        ...
+    def data_path(self) -> Path: ...
 
 
 class WithResources(Resource):
     @property
     @abstractmethod
-    def resources(self) -> Tuple[Resource, ...]:
-        ...
+    def resources(self) -> Tuple[Resource, ...]: ...
 
     def flush(self) -> None:
         for resource in self.resources:
             resource.flush()
 
     def close(self) -> None:
         for resource in self.resources:
```

### Comparing `neptune-1.9.1/src/neptune/core/components/metadata_file.py` & `neptune-2.0.0a0/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/operation_storage.py` & `neptune-2.0.0a0/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/queue/__init__.py` & `neptune-2.0.0a0/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/queue/disk_queue.py` & `neptune-2.0.0a0/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/queue/json_file_splitter.py` & `neptune-2.0.0a0/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/queue/log_file.py` & `neptune-2.0.0a0/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/core/components/queue/sync_offset_file.py` & `neptune-2.0.0a0/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/envs.py` & `neptune-2.0.0a0/src/neptune/envs.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,19 @@
     "NEPTUNE_FETCH_TABLE_STEP_SIZE",
     "NEPTUNE_SYNC_AFTER_STOP_TIMEOUT",
     "NEPTUNE_REQUEST_TIMEOUT",
     "NEPTUNE_MAX_DISK_USAGE",
     "NEPTUNE_RAISE_ERROR_ON_DISK_USAGE_EXCEEDED",
     "NEPTUNE_ENABLE_DEFAULT_ASYNC_LAG_CALLBACK",
     "NEPTUNE_ENABLE_DEFAULT_ASYNC_NO_PROGRESS_CALLBACK",
+    "NEPTUNE_USE_PROTOCOL_BUFFERS",
     "NEPTUNE_ASYNC_BATCH_SIZE",
 ]
 
-from neptune.common.envs import (
+from neptune.internal.envs import (
     API_TOKEN_ENV_NAME,
     NEPTUNE_RETRIES_TIMEOUT_ENV,
 )
 
 CONNECTION_MODE = "NEPTUNE_MODE"
 
 PROJECT_ENV_NAME = "NEPTUNE_PROJECT"
@@ -70,8 +71,10 @@
 
 NEPTUNE_MAX_DISK_USAGE = "NEPTUNE_MAX_DISK_USAGE"
 
 NEPTUNE_RAISE_ERROR_ON_DISK_USAGE_EXCEEDED = "NEPTUNE_RAISE_ERROR_ON_DISK_USAGE_EXCEEDED"
 
 NEPTUNE_ASYNC_BATCH_SIZE = "NEPTUNE_ASYNC_BATCH_SIZE"
 
+NEPTUNE_USE_PROTOCOL_BUFFERS = "NEPTUNE_USE_PROTOCOL_BUFFERS"
+
 S3_ENDPOINT_URL = "S3_ENDPOINT_URL"
```

### Comparing `neptune-1.9.1/src/neptune/exceptions.py` & `neptune-2.0.0a0/src/neptune/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,24 +62,21 @@
     "Forbidden",
     "NeptuneOfflineModeException",
     "NeptuneOfflineModeFetchException",
     "NeptuneOfflineModeChangeStageException",
     "NeptuneProtectedPathException",
     "NeptuneCannotChangeStageManually",
     "OperationNotSupported",
-    "NeptuneLegacyProjectException",
-    "NeptuneIntegrationNotInstalledException",
+    "NeptuneMissingRequirementException",
     "NeptuneLimitExceedException",
     "NeptuneFieldCountLimitExceedException",
     "NeptuneStorageLimitException",
     "FetchAttributeNotFoundException",
     "ArtifactNotFoundException",
     "PlotlyIncompatibilityException",
-    "NeptunePossibleLegacyUsageException",
-    "NeptuneLegacyIncompatibilityException",
     "NeptuneUnhandledArtifactSchemeException",
     "NeptuneUnhandledArtifactTypeException",
     "NeptuneLocalStorageAccessException",
     "NeptuneRemoteStorageCredentialsException",
     "NeptuneRemoteStorageAccessException",
     "ArtifactUploadingError",
     "NeptuneUnsupportedArtifactFunctionalityException",
@@ -87,50 +84,50 @@
     "NeptuneFeatureNotAvailableException",
     "NeptuneObjectCreationConflict",
     "NeptuneModelKeyAlreadyExistsError",
     "NeptuneSynchronizationAlreadyStoppedException",
     "StreamAlreadyUsedException",
     "NeptuneUserApiInputException",
     "NeptuneMaxDiskUtilizationExceeded",
+    "NeptuneInvalidQueryException",
+    "NeptuneUnsupportedFunctionalityException",
 ]
 
 from typing import (
     List,
     Optional,
     Union,
 )
 from urllib.parse import urlparse
 
 from packaging.version import Version
 
-from neptune.common.envs import API_TOKEN_ENV_NAME
-
-# Backward compatibility import
-from neptune.common.exceptions import (
+from neptune.envs import (
+    CUSTOM_RUN_ID_ENV_NAME,
+    PROJECT_ENV_NAME,
+)
+from neptune.internal.backends.api_model import (
+    Project,
+    Workspace,
+)
+from neptune.internal.container_type import ContainerType
+from neptune.internal.envs import API_TOKEN_ENV_NAME
+from neptune.internal.exceptions import (
     STYLES,
     ClientHttpError,
     Forbidden,
     InternalClientError,
     InternalServerError,
     NeptuneApiException,
     NeptuneConnectionLostException,
     NeptuneException,
     NeptuneInvalidApiTokenException,
     NeptuneSSLVerificationError,
     Unauthorized,
 )
-from neptune.envs import (
-    CUSTOM_RUN_ID_ENV_NAME,
-    PROJECT_ENV_NAME,
-)
-from neptune.internal.backends.api_model import (
-    Project,
-    Workspace,
-)
-from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import QualifiedName
 from neptune.internal.utils import replace_patch_version
 from neptune.internal.utils.paths import path_to_str
 
 
 class MetadataInconsistency(NeptuneException):
     pass
@@ -275,22 +272,22 @@
                 lambda workspace: f"    - https://app.neptune.ai/{workspace.name}/-/projects",
                 available_workspaces,
             )
         )
 
         super().__init__(
             message.format(
-                available_projects_message=available_projects_message.format(projects=projects_formated_list)
-                if available_projects
-                else "",
-                available_workspaces_message=available_workspaces_message.format(
-                    workspaces_urls=workspaces_formated_list
-                )
-                if available_workspaces
-                else "",
+                available_projects_message=(
+                    available_projects_message.format(projects=projects_formated_list) if available_projects else ""
+                ),
+                available_workspaces_message=(
+                    available_workspaces_message.format(workspaces_urls=workspaces_formated_list)
+                    if available_workspaces
+                    else ""
+                ),
                 **STYLES,
                 **kwargs,
             )
         )
 
 
 class ContainerUUIDNotFound(NeptuneException):
@@ -638,15 +635,15 @@
 {end}
 Your version of the Neptune client library ({current_version}) is no longer supported by the Neptune
  server. The minimum required version is {required_version}.
 
 In order to update the Neptune client library, run the following command in your terminal:
     {bash}pip install -U neptune{end}
 Or if you are using Conda, run the following instead:
-    {bash}conda update -c conda-forge neptune-client{end}
+    {bash}conda update -c conda-forge neptune{end}
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
 """
         super().__init__(
             message.format(
                 current_version=current_version,
                 required_version=required_version,
@@ -767,53 +764,35 @@
 
 
 class OperationNotSupported(NeptuneException):
     def __init__(self, message: str):
         super().__init__(f"Operation not supported: {message}")
 
 
-class NeptuneLegacyProjectException(NeptuneException):
-    def __init__(self, project: QualifiedName):
+class NeptuneMissingRequirementException(NeptuneException):
+    def __init__(self, package_name: str, framework_name: Optional[str]):
         message = """
-{h1}
-----NeptuneLegacyProjectException---------------------------------------------------------
-{end}
-Your project "{project}" has not been migrated to the new structure yet.
-Unfortunately the neptune.new Python API is incompatible with projects using the old structure,
-so please use legacy neptune Python API.
-Don't worry - we are working hard on migrating all the projects and you will be able to use the neptune.new API soon.
-
-You can find documentation for the legacy neptune Python API here:
-    - https://docs-legacy.neptune.ai/index.html
-
-{correct}Need help?{end}-> https://docs.neptune.ai/getting_help
-"""
-        super().__init__(message.format(project=project, **STYLES))
-
-
-class NeptuneIntegrationNotInstalledException(NeptuneException):
-    def __init__(self, integration_package_name, framework_name):
-        message = """
-{h1}
-----NeptuneIntegrationNotInstalledException-----------------------------------------
-{end}
-Looks like integration {integration_package_name} wasn't installed.
-To install, run:
-    {bash}pip install {integration_package_name}{end}
-Or:
-    {bash}pip install "neptune[{framework_name}]"{end}
+    {h1}
+    ----NeptuneMissingRequirementException-----------------------------------------
+    {end}
+    Looks like the {package_name} package isn't installed.
+    To install it, run:
+        {bash}pip install {package_name}{end}
+    Or install both Neptune and the integration:
+        {bash}pip install "neptune[{framework_name}]"{end}
 
-You may also want to check the following docs page:
-    - https://docs.neptune.ai/integrations
+    For detailed instructions, check the integration guides:
+        - https://docs.neptune.ai/integrations
 
-{correct}Need help?{end}-> https://docs.neptune.ai/getting_help
-"""
+    {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
+    """
+        framework_name = framework_name if framework_name else package_name
         super().__init__(
             message.format(
-                integration_package_name=integration_package_name,
+                package_name=package_name,
                 framework_name=framework_name,
                 **STYLES,
             )
         )
 
 
 class NeptuneLimitExceedException(NeptuneException):
@@ -949,61 +928,14 @@
         super().__init__(
             "Unable to convert plotly figure to matplotlib format. "
             "Your matplotlib ({}) and plotlib ({}) versions are not compatible. "
             "{}".format(matplotlib_version, plotly_version, details)
         )
 
 
-class NeptunePossibleLegacyUsageException(NeptuneWrongInitParametersException):
-    def __init__(self):
-        message = """
-{h1}
-----NeptunePossibleLegacyUsageException----------------------------------------------------------------
-{end}
-It seems you are trying to use the legacy API, but you imported the new one.
-
-Simply update your import statement to:
-    {python}import neptune{end}
-
-You may want to check the legacy API docs:
-    - https://docs-legacy.neptune.ai
-
-If you want to update your code with the new API, we prepared a handy migration guide:
-    - https://docs.neptune.ai/about/legacy/#migrating-to-neptunenew
-
-You can read more about neptune.new in the release blog post:
-    - https://neptune.ai/blog/neptune-new
-
-You may also want to check the following docs page:
-    - https://docs-legacy.neptune.ai/getting-started/integrate-neptune-into-your-codebase.html
-
-{correct}Need help?{end}-> https://docs.neptune.ai/getting_help
-"""
-        super().__init__(message.format(**STYLES))
-
-
-class NeptuneLegacyIncompatibilityException(NeptuneException):
-    def __init__(self):
-        message = """
-{h1}
-----NeptuneLegacyIncompatibilityException----------------------------------------
-{end}
-It seems you are passing the legacy Experiment object, when a Run object is expected.
-
-What can I do?
-    - Updating your code to the new Python API requires few changes, but to help you with this process we prepared a handy migration guide:
-    https://docs.neptune.ai/about/legacy/#migrating-to-neptunenew
-    - You can read more about neptune.new in the release blog post:
-    https://neptune.ai/blog/neptune-new
-
-{correct}Need help?{end}-> https://docs.neptune.ai/getting_help
-"""  # noqa: E501
-        super().__init__(message.format(**STYLES))
-
-
 class NeptuneUnhandledArtifactSchemeException(NeptuneException):
     def __init__(self, path: str):
         scheme = urlparse(path).scheme
         message = """
 {h1}
 ----NeptuneUnhandledArtifactProtocolException------------------------------------
 {end}
@@ -1219,7 +1151,29 @@
 Current disk utilization ({disk_utilization}%) exceeds the limit ({utilization_limit}%).
 
 {correct}Need help?{end}-> https://docs.neptune.ai/getting_help
     """
         super().__init__(
             message.format(disk_utilization=disk_utilization, utilization_limit=utilization_limit, **STYLES)
         )
+
+
+class NeptuneInvalidQueryException(NeptuneException):
+    def __init__(self, nql_query: str):
+        message = f"""
+The provided NQL query is invalid: {nql_query}.
+For syntax help, see https://docs.neptune.ai/usage/nql/
+"""
+        super().__init__(message)
+
+
+class NeptuneUnsupportedFunctionalityException(NeptuneException):
+    def __init__(self):
+        message = """
+{h1}
+----NeptuneUnsupportedFunctionalityException----------------------------
+{end}
+You're using neptune 2.0, which is in Beta.
+Some functionality that you tried to use is not supported in the installed version.
+We will gradually add missing features to the Beta. Check that you're on the latest version.
+"""
+        super().__init__(message)
```

### Comparing `neptune-1.9.1/src/neptune/handler.py` & `neptune-2.0.0a0/src/neptune/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,28 @@
     TYPE_CHECKING,
     Any,
     Collection,
     Dict,
     Iterable,
     Iterator,
     List,
-    NewType,
     Optional,
     Union,
 )
 
-from neptune.api.dtos import FileEntry
+from neptune.api.models import FileEntry
 from neptune.attributes import File
 from neptune.attributes.atoms.artifact import Artifact
 from neptune.attributes.constants import SYSTEM_STAGE_ATTRIBUTE_PATH
 from neptune.attributes.file_set import FileSet
 from neptune.attributes.namespace import Namespace
 from neptune.attributes.series import FileSeries
 from neptune.attributes.series.float_series import FloatSeries
 from neptune.attributes.series.string_series import StringSeries
 from neptune.attributes.sets.string_set import StringSet
-from neptune.common.warnings import warn_about_unsupported_type
 from neptune.exceptions import (
     MissingFieldException,
     NeptuneCannotChangeStageManually,
     NeptuneUserApiInputException,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.types.stringify_value import StringifyValue
@@ -58,25 +56,24 @@
     verify_type,
 )
 from neptune.internal.utils.paths import (
     join_paths,
     parse_path,
 )
 from neptune.internal.value_to_attribute_visitor import ValueToAttributeVisitor
-from neptune.metadata_containers.abstract import SupportsNamespaces
+from neptune.internal.warnings import warn_about_unsupported_type
+from neptune.objects.abstract import SupportsNamespaces
 from neptune.types.atoms.file import File as FileVal
 from neptune.types.type_casting import cast_value_for_extend
 from neptune.types.value_copy import ValueCopy
 from neptune.typing import ProgressBarType
 from neptune.utils import stringify_unsupported
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
-
-    NeptuneObject = NewType("NeptuneObject", MetadataContainer)
+    from neptune.objects import NeptuneObject
 
 
 def validate_path_not_protected(target_path: str, handler: "Handler"):
     path_protection_exception = handler._PROTECTED_PATHS.get(target_path)
     if path_protection_exception:
         raise path_protection_exception(target_path)
 
@@ -95,15 +92,15 @@
 
 class Handler(SupportsNamespaces):
     # paths which can't be modified by client directly
     _PROTECTED_PATHS = {
         SYSTEM_STAGE_ATTRIBUTE_PATH: NeptuneCannotChangeStageManually,
     }
 
-    def __init__(self, container: "MetadataContainer", path: str):
+    def __init__(self, container: "NeptuneObject", path: str):
         super().__init__()
         self._container = container
         self._path = str(path)
 
     def __repr__(self):
         attr = self._container.get_attribute(self._path)
         formal_type = type(attr).__name__ if attr else "Unassigned"
@@ -140,15 +137,15 @@
         """Returns an attribute defined in `self._path` or throws MissingFieldException."""
         attr = self._container.get_attribute(self._path)
         if attr is None:
             raise MissingFieldException(self._path)
         return attr
 
     @property
-    def container(self) -> "MetadataContainer":
+    def container(self) -> "NeptuneObject":
         """Returns the container that the attribute is attached to."""
         return self._container
 
     def get_root_object(self) -> "NeptuneObject":
         """Returns the root-level object of a namespace handler.
 
         Example:
```

### Comparing `neptune-1.9.1/src/neptune/integrations/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/integrations/aws/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/aws/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_aws.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_aws":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-aws", suggestion="aws")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-aws", framework_name="aws"
-        ) from None
-    else:
-        raise
+from neptune_aws.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/detectron2/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/prophet/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_detectron2.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_detectron2":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune_prophet", suggestion="prophet")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-detectron2",
-            framework_name="detectron2",
-        ) from None
-    else:
-        raise
+from neptune_prophet.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/fastai/__init__.py` & `neptune-2.0.0a0/src/neptune/types/model_version_stage.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["ModelVersionStage"]
 
-try:
-    from neptune_fastai.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_fastai":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+import enum
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-fastai", framework_name="fastai"
-        ) from None
-    else:
-        raise
+
+class ModelVersionStage(enum.Enum):
+    NONE = "none"
+    STAGING = "staging"
+    PRODUCTION = "production"
+    ARCHIVED = "archived"
```

### Comparing `neptune-1.9.1/src/neptune/integrations/kedro/__init__.py` & `neptune-2.0.0a0/src/neptune/types/sets/string_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,19 +9,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["StringSet"]
 
-try:
-    from kedro_neptune import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "kedro_neptune":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
-
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="kedro-neptune", framework_name="kedro"
-        ) from None
-    else:
-        raise
+from typing import (
+    TYPE_CHECKING,
+    Iterable,
+    TypeVar,
+)
+
+from neptune.types.sets.set import Set
+
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
+
+Ret = TypeVar("Ret")
+
+
+class StringSet(Set):
+    def __init__(self, values: Iterable[str]):
+        self.values = set(values)
+
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        return visitor.visit_string_set(self)
+
+    def __str__(self):
+        return "StringSet({})".format(str(self.values))
```

### Comparing `neptune-1.9.1/src/neptune/integrations/lightgbm/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["NeptuneLogger"]
 
-try:
-    from neptune_lightgbm.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_lightgbm":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+from neptune.internal.utils.requirement_check import require_installed
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-lightgbm", framework_name="lightgbm"
-        ) from None
-    else:
-        raise
+require_installed("pytorch-lightning")
+
+
+from pytorch_lightning.loggers import NeptuneLogger  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/optuna/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/optuna/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_optuna.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_optuna":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-optuna", suggestion="optuna")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-optuna", framework_name="optuna"
-        ) from None
-    else:
-        raise
+from neptune_optuna.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/prophet/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_prophet.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_prophet":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-tensorflow-keras", suggestion="tensorflow-keras")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-prophet", framework_name="prophet"
-        ) from None
-    else:
-        raise
+from neptune_tensorflow_keras.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/python_logger.py` & `neptune-2.0.0a0/src/neptune/integrations/python_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 import logging
 import threading
 
 from neptune import Run
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import verify_type
-from neptune.logging import Logger
-from neptune.version import version as neptune_client_version
+from neptune.version import version as neptune_version
 
 INTEGRATION_VERSION_KEY = "source_code/integrations/neptune-python-logger"
 
 
 class NeptuneHandler(logging.Handler):
     """Handler that sends the log records created by the logger to Neptune
 
@@ -54,29 +53,27 @@
         ...
         >>> logger.debug("Data preparation done")
     """
 
     def __init__(self, *, run: Run, level=logging.NOTSET, path: str = None):
         verify_type("run", run, Run)
         verify_type("level", level, int)
-        if path is None:
-            path = f"{run.monitoring_namespace}/python_logger"
-        verify_type("path", path, str)
+        verify_type("path", path, (str, type(None)))
 
         super().__init__(level=level)
+        self._path = path if path else f"{run.monitoring_namespace}/python_logger"
         self._run = run
-        self._logger = Logger(run, path)
         self._thread_local = threading.local()
 
-        self._run[INTEGRATION_VERSION_KEY] = str(neptune_client_version)
+        self._run[INTEGRATION_VERSION_KEY] = str(neptune_version)
 
     def emit(self, record: logging.LogRecord) -> None:
         if not hasattr(self._thread_local, "inside_write"):
             self._thread_local.inside_write = False
 
         if self._run.get_state() == ContainerState.STARTED.value and not self._thread_local.inside_write:
             try:
                 self._thread_local.inside_write = True
                 message = self.format(record)
-                self._logger.log(message)
+                self._run[self._path].append(message)
             finally:
                 self._thread_local.inside_write = False
```

### Comparing `neptune-1.9.1/src/neptune/integrations/pytorch/__init__.py` & `neptune-2.0.0a0/src/neptune/types/atoms/atom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 #
-# Copyright (c) 2023, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["Atom"]
 
-try:
-    from neptune_pytorch.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_pytorch":
-        from neptune.new.exceptions import NeptuneIntegrationNotInstalledException
-
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-pytorch",
-            framework_name="pytorch",
-        ) from None
-    else:
-        raise
+import abc
+from typing import (
+    TYPE_CHECKING,
+    TypeVar,
+)
+
+from neptune.types.value import Value
+
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
+
+Ret = TypeVar("Ret")
+
+
+class Atom(Value):
+    @abc.abstractmethod
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        pass
```

### Comparing `neptune-1.9.1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/kedro/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,21 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["NeptuneLogger"]
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from pytorch_lightning.loggers import NeptuneLogger
-except ModuleNotFoundError as e:
-    if e.name == "pytorch_lightning":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("kedro-neptune", suggestion="kedro")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="pytorch-lightning",
-            framework_name="pytorch-lightning",
-        ) from None
-    else:
-        raise
+from kedro_neptune.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/sacred/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/tensorboard/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2023, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_sacred.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_sacred":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-tensorboard", suggestion="tensorboard")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-sacred", framework_name="sacred"
-        ) from None
-    else:
-        raise
+from neptune_tensorboard.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/sklearn/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/lightgbm/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,19 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_sklearn.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_sklearn":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-lightgbm", suggestion="lightgbm")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-sklearn", framework_name="sklearn"
-        ) from None
-    else:
-        raise
+from neptune_lightgbm.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/tensorboard/__init__.py` & `neptune-2.0.0a0/src/neptune/integrations/detectron2/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 #
-# Copyright (c) 2023, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-try:
-    from neptune_tensorboard.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_tensorboard":
-        from neptune.new.exceptions import NeptuneIntegrationNotInstalledException
+require_installed("neptune-detectron2", suggestion="detectron2")
 
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-tensorboard",
-            framework_name="tensorboard",
-        ) from None
-    else:
-        raise
+from neptune_detectron2.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-2.0.0a0/src/neptune/objects/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = [
+    "NeptuneObject",
+    "Model",
+    "ModelVersion",
+    "Project",
+    "Run",
+]
 
-try:
-    from neptune_tensorflow_keras.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_tensorflow_keras":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
-
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-tensorflow-keras",
-            framework_name="tensorflow-keras",
-        ) from None
-    else:
-        raise
+from neptune.objects.model import Model
+from neptune.objects.model_version import ModelVersion
+from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.project import Project
+from neptune.objects.run import Run
```

### Comparing `neptune-1.9.1/src/neptune/integrations/utils.py` & `neptune-2.0.0a0/src/neptune/types/sets/set.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["expect_not_an_experiment", "join_paths", "verify_type", "RunType"]
+__all__ = ["Set"]
 
-from typing import Union
+import abc
+from typing import (
+    TYPE_CHECKING,
+    TypeVar,
+)
 
-from neptune import Run
-from neptune.common.experiments import LegacyExperiment as Experiment
-from neptune.exceptions import NeptuneLegacyIncompatibilityException
-from neptune.handler import Handler
-from neptune.internal.utils import verify_type
-from neptune.internal.utils.paths import join_paths
+from neptune.types.value import Value
 
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
 
-def expect_not_an_experiment(run: Run):
-    if isinstance(run, Experiment):
-        raise NeptuneLegacyIncompatibilityException()
+Ret = TypeVar("Ret")
 
 
-RunType = Union[Run, Handler]
+class Set(Value):
+    @abc.abstractmethod
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        pass
```

### Comparing `neptune-1.9.1/src/neptune/integrations/xgboost/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/utils/requirement_check.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = [
+    "require_installed",
+    "is_installed",
+]
 
-try:
-    from neptune_xgboost.impl import *  # noqa: F401,F403
-except ModuleNotFoundError as e:
-    if e.name == "neptune_xgboost":
-        from neptune.exceptions import NeptuneIntegrationNotInstalledException
-
-        raise NeptuneIntegrationNotInstalledException(
-            integration_package_name="neptune-xgboost", framework_name="xgboost"
-        ) from None
-    else:
-        raise
+from functools import lru_cache
+from importlib.util import find_spec
+from typing import Optional
+
+from neptune.exceptions import NeptuneMissingRequirementException
+
+
+@lru_cache(maxsize=32)
+def is_installed(requirement_name: str) -> bool:
+    return find_spec(requirement_name) is not None
+
+
+def require_installed(requirement_name: str, *, suggestion: Optional[str] = None) -> None:
+    if is_installed(requirement_name):
+        return
+
+    raise NeptuneMissingRequirementException(requirement_name, suggestion)
```

### Comparing `neptune-1.9.1/src/neptune/internal/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/drivers/local.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/file_hasher.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/file_hasher.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,25 +44,25 @@
         absolute = Path(file_path).resolve()
         modification_date = datetime.datetime.fromtimestamp(absolute.stat().st_mtime).strftime("%Y%m%d_%H%M%S%f")
 
         stored_file_hash = local_storage.fetch_one(absolute)
 
         if stored_file_hash:
             if stored_file_hash.modification_date >= modification_date:
-                return stored_file_hash.file_hash
+                computed_hash = stored_file_hash.file_hash
             else:
                 computed_hash = sha1(absolute)
                 local_storage.update(absolute, computed_hash, modification_date)
-
-                return computed_hash
         else:
             computed_hash = sha1(absolute)
             local_storage.insert(absolute, computed_hash, modification_date)
 
-            return computed_hash
+        local_storage.close()
+
+        return computed_hash
 
     @classmethod
     def _number_to_bytes(cls, int_value: int, bytes_cnt):
         return int_value.to_bytes(bytes_cnt, cls.SERVER_BYTE_ORDER)
 
     @classmethod
     def get_artifact_hash(cls, artifact_files: typing.Iterable[ArtifactFileData]) -> str:
```

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,7 +59,10 @@
 
     def update(self, path: Path, computed_hash: str, modification_date: str):
         self.cursor.execute(
             "UPDATE local_file_hashes SET file_hash=?, modification_date=? WHERE file_path = ?",
             (computed_hash, modification_date, str(path)),
         )
         self.session.commit()
+
+    def close(self) -> None:
+        self.session.close()
```

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/types.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/artifacts/utils.py` & `neptune-2.0.0a0/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/backends/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/backends/api_model.py` & `neptune-2.0.0a0/src/neptune/internal/backends/api_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,57 +16,56 @@
 __all__ = [
     "Project",
     "Workspace",
     "ApiExperiment",
     "OptionalFeatures",
     "VersionInfo",
     "ClientConfig",
-    "AttributeType",
-    "Attribute",
-    "AttributeWithProperties",
-    "LeaderboardEntry",
     "StringPointValue",
     "ImageSeriesValues",
     "StringSeriesValues",
     "FloatPointValue",
     "FloatSeriesValues",
-    "FloatAttribute",
-    "IntAttribute",
-    "BoolAttribute",
-    "FileAttribute",
-    "StringAttribute",
-    "DatetimeAttribute",
-    "ArtifactAttribute",
     "ArtifactModel",
-    "FloatSeriesAttribute",
-    "StringSeriesAttribute",
-    "StringSetAttribute",
+    "MultipartConfig",
 ]
 
 from dataclasses import dataclass
-from datetime import datetime
-from enum import Enum
 from typing import (
-    Any,
     FrozenSet,
     List,
     Optional,
-    Set,
 )
 
 from packaging import version
 
-from neptune.common.backends.api_model import MultipartConfig
 from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import (
     SysId,
     UniqueId,
 )
 
 
+@dataclass(frozen=True)
+class MultipartConfig:
+    min_chunk_size: int
+    max_chunk_size: int
+    max_chunk_count: int
+    max_single_part_size: int
+
+    @staticmethod
+    def get_default() -> "MultipartConfig":
+        return MultipartConfig(
+            min_chunk_size=5242880,
+            max_chunk_size=1073741824,
+            max_chunk_count=1000,
+            max_single_part_size=5242880,
+        )
+
+
 @dataclass
 class Project:
     id: UniqueId
     name: str
     workspace: str
     sys_id: SysId
 
@@ -178,51 +177,14 @@
             display_url=config.applicationUrl,
             _missing_features=frozenset(missing_features),
             version_info=VersionInfo.build(min_recommended, min_compatible, max_compatible),
             multipart_config=multipart_upload_config,
         )
 
 
-class AttributeType(Enum):
-    FLOAT = "float"
-    INT = "int"
-    BOOL = "bool"
-    STRING = "string"
-    DATETIME = "datetime"
-    FILE = "file"
-    FILE_SET = "fileSet"
-    FLOAT_SERIES = "floatSeries"
-    STRING_SERIES = "stringSeries"
-    IMAGE_SERIES = "imageSeries"
-    STRING_SET = "stringSet"
-    GIT_REF = "gitRef"
-    RUN_STATE = "experimentState"
-    NOTEBOOK_REF = "notebookRef"
-    ARTIFACT = "artifact"
-
-
-@dataclass
-class Attribute:
-    path: str
-    type: AttributeType
-
-
-@dataclass
-class AttributeWithProperties:
-    path: str
-    type: AttributeType
-    properties: Any
-
-
-@dataclass
-class LeaderboardEntry:
-    id: str
-    attributes: List[AttributeWithProperties]
-
-
 @dataclass
 class StringPointValue:
     timestampMillis: int
     step: float
     value: str
 
 
@@ -247,63 +209,11 @@
 @dataclass
 class FloatSeriesValues:
     totalItemCount: int
     values: List[FloatPointValue]
 
 
 @dataclass
-class FloatAttribute:
-    value: float
-
-
-@dataclass
-class IntAttribute:
-    value: int
-
-
-@dataclass
-class BoolAttribute:
-    value: bool
-
-
-@dataclass
-class FileAttribute:
-    name: str
-    ext: str
-    size: int
-
-
-@dataclass
-class StringAttribute:
-    value: str
-
-
-@dataclass
-class DatetimeAttribute:
-    value: datetime
-
-
-@dataclass
-class ArtifactAttribute:
-    hash: str
-
-
-@dataclass
 class ArtifactModel:
     received_metadata: bool
     hash: str
     size: int
-
-
-@dataclass
-class FloatSeriesAttribute:
-    last: Optional[float]
-
-
-@dataclass
-class StringSeriesAttribute:
-    last: Optional[str]
-
-
-@dataclass
-class StringSetAttribute:
-    values: Set[str]
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/factory.py` & `neptune-2.0.0a0/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-2.0.0a0/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,32 +26,30 @@
     Optional,
     Tuple,
     Type,
 )
 
 from bravado.exception import HTTPNotFound
 
-from neptune.common.backends.utils import with_api_exceptions_handler
+from neptune.api.models import ArtifactField
 from neptune.exceptions import (
     ArtifactNotFoundException,
     ArtifactUploadingError,
     FetchAttributeNotFoundException,
     NeptuneEmptyLocationException,
 )
 from neptune.internal.artifacts.file_hasher import FileHasher
 from neptune.internal.artifacts.types import (
     ArtifactDriver,
     ArtifactDriversMap,
     ArtifactFileData,
 )
-from neptune.internal.backends.api_model import (
-    ArtifactAttribute,
-    ArtifactModel,
-)
+from neptune.internal.backends.api_model import ArtifactModel
 from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
+from neptune.internal.backends.utils import with_api_exceptions_handler
 from neptune.internal.operation import (
     AssignArtifact,
     Operation,
 )
 from neptune.internal.utils.paths import path_to_str
 
 
@@ -250,24 +248,24 @@
 
 @with_api_exceptions_handler
 def get_artifact_attribute(
     swagger_client: SwaggerClientWrapper,
     parent_identifier: str,
     path: List[str],
     default_request_params: Dict,
-) -> ArtifactAttribute:
+) -> ArtifactField:
     requests_params = add_artifact_version_to_request_params(default_request_params)
     params = {
         "experimentId": parent_identifier,
         "attribute": path_to_str(path),
         **requests_params,
     }
     try:
         result = swagger_client.api.getArtifactAttribute(**params).response().result
-        return ArtifactAttribute(hash=result.hash)
+        return ArtifactField.from_model(result)
     except HTTPNotFound:
         raise FetchAttributeNotFoundException(path_to_str(path))
 
 
 @with_api_exceptions_handler
 def list_artifact_files(
     swagger_client: SwaggerClientWrapper,
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/hosted_client.py` & `neptune-2.0.0a0/src/neptune/internal/backends/hosted_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,44 +28,44 @@
     Tuple,
 )
 
 import requests
 from bravado.http_client import HttpClient
 from bravado.requests_client import RequestsClient
 
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.oauth import NeptuneAuthenticator
 from neptune.envs import NEPTUNE_REQUEST_TIMEOUT
 from neptune.exceptions import NeptuneClientUpgradeRequiredError
 from neptune.internal.backends.api_model import ClientConfig
 from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
 from neptune.internal.backends.utils import (
     NeptuneResponseAdapter,
     build_operation_url,
     cache,
     create_swagger_client,
     update_session_proxies,
     verify_client_version,
     verify_host_resolution,
+    with_api_exceptions_handler,
 )
 from neptune.internal.credentials import Credentials
-from neptune.version import version as neptune_client_version
+from neptune.internal.oauth import NeptuneAuthenticator
+from neptune.version import version as neptune_version
 
 BACKEND_SWAGGER_PATH = "/api/backend/swagger.json"
 LEADERBOARD_SWAGGER_PATH = "/api/leaderboard/swagger.json"
 ARTIFACTS_SWAGGER_PATH = "/api/artifacts/swagger.json"
 
 CONNECT_TIMEOUT = 30  # helps detecting internet connection lost
 REQUEST_TIMEOUT = int(os.getenv(NEPTUNE_REQUEST_TIMEOUT, "600"))
 
 DEFAULT_REQUEST_KWARGS = {
     "_request_options": {
         "connect_timeout": CONNECT_TIMEOUT,
         "timeout": REQUEST_TIMEOUT,
-        "headers": {"X-Neptune-LegacyClient": "false"},
+        "headers": {},
     }
 }
 
 
 def _close_connections_on_fork(session: requests.Session):
     try:
         os.register_at_fork(before=session.close, after_in_child=session.close, after_in_parent=session.close)
@@ -85,15 +85,15 @@
     _set_pool_size(http_client)
 
     _close_connections_on_fork(http_client.session)
 
     update_session_proxies(http_client.session, proxies)
 
     user_agent = "neptune-client/{lib_version} ({system}, python {python_version})".format(
-        lib_version=neptune_client_version,
+        lib_version=neptune_version,
         system=platform.platform(),
         python_version=platform.python_version(),
     )
     http_client.session.headers.update({"User-Agent": user_agent})
 
     return http_client
 
@@ -132,27 +132,27 @@
         )
         .response()
         .result
     )
 
     client_config = ClientConfig.from_api_response(config)
     if not client_config.version_info:
-        raise NeptuneClientUpgradeRequiredError(neptune_client_version, max_version="0.4.111")
+        raise NeptuneClientUpgradeRequiredError(neptune_version, max_version="0.4.111")
     return client_config
 
 
 @cache
 def create_http_client_with_auth(
     credentials: Credentials, ssl_verify: bool, proxies: Dict[str, str]
 ) -> Tuple[RequestsClient, ClientConfig]:
     client_config = get_client_config(credentials=credentials, ssl_verify=ssl_verify, proxies=proxies)
 
     config_api_url = credentials.api_url_opt or credentials.token_origin_address
 
-    verify_client_version(client_config, neptune_client_version)
+    verify_client_version(client_config, neptune_version)
 
     endpoint_url = None
     if config_api_url != client_config.api_url:
         endpoint_url = build_operation_url(client_config.api_url, BACKEND_SWAGGER_PATH)
 
     http_client = create_http_client(ssl_verify=ssl_verify, proxies=proxies)
     http_client.authenticator = NeptuneAuthenticator(
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-2.0.0a0/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,47 +44,45 @@
 )
 from bravado.requests_client import RequestsClient
 from requests import (
     Request,
     Response,
 )
 
-from neptune.common.backends.api_model import MultipartConfig
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.exceptions import (
-    InternalClientError,
-    NeptuneException,
-    UploadedFileChanged,
-)
-from neptune.common.hardware.constants import BYTES_IN_ONE_MB
-from neptune.common.storage.datastream import (
-    FileChunk,
-    FileChunker,
-    compress_to_tar_gz_in_memory,
-)
-from neptune.common.storage.storage_utils import (
-    AttributeUploadConfiguration,
-    UploadEntry,
-    normalize_file_name,
-    scan_unique_upload_entries,
-    split_upload_files,
-)
 from neptune.exceptions import (
     FileUploadError,
     MetadataInconsistency,
     NeptuneLimitExceedException,
 )
+from neptune.internal.backends.api_model import MultipartConfig
 from neptune.internal.backends.swagger_client_wrapper import (
     ApiMethodWrapper,
     SwaggerClientWrapper,
 )
 from neptune.internal.backends.utils import (
     build_operation_url,
     construct_progress_bar,
     handle_server_raw_response_messages,
+    with_api_exceptions_handler,
+)
+from neptune.internal.exceptions import (
+    InternalClientError,
+    NeptuneException,
+    UploadedFileChanged,
+)
+from neptune.internal.hardware.constants import BYTES_IN_ONE_MB
+from neptune.internal.storage import (
+    AttributeUploadConfiguration,
+    FileChunk,
+    FileChunker,
+    UploadEntry,
+    compress_to_tar_gz_in_memory,
+    normalize_file_name,
+    scan_unique_upload_entries,
+    split_upload_files,
 )
 from neptune.internal.utils import (
     get_absolute_paths,
     get_common_root,
 )
 from neptune.internal.utils.logger import get_logger
 from neptune.typing import ProgressBarType
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-2.0.0a0/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,66 +34,62 @@
 from bravado.exception import (
     HTTPConflict,
     HTTPNotFound,
     HTTPPaymentRequired,
     HTTPUnprocessableEntity,
 )
 
-from neptune.api.dtos import FileEntry
-from neptune.api.searching_entries import iter_over_pages
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.exceptions import (
-    ClientHttpError,
-    InternalClientError,
-    NeptuneException,
-)
-from neptune.common.patterns import PROJECT_QUALIFIED_NAME_PATTERN
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
+from neptune.api.models import (
+    ArtifactField,
+    BoolField,
+    DateTimeField,
+    Field,
+    FieldDefinition,
+    FieldType,
+    FileEntry,
+    FileField,
+    FloatField,
+    FloatSeriesField,
+    IntField,
+    LeaderboardEntry,
+    StringField,
+    StringSeriesField,
+    StringSetField,
 )
+from neptune.api.proto.neptune_pb.api.model.attributes_pb2 import ProtoAttributesSearchResultDTO
+from neptune.api.proto.neptune_pb.api.model.leaderboard_entries_pb2 import ProtoAttributesDTO
+from neptune.api.searching_entries import iter_over_pages
 from neptune.core.components.operation_storage import OperationStorage
-from neptune.envs import NEPTUNE_FETCH_TABLE_STEP_SIZE
+from neptune.envs import (
+    NEPTUNE_FETCH_TABLE_STEP_SIZE,
+    NEPTUNE_USE_PROTOCOL_BUFFERS,
+)
 from neptune.exceptions import (
     AmbiguousProjectName,
     ContainerUUIDNotFound,
     FetchAttributeNotFoundException,
     FileSetNotFound,
     MetadataContainerNotFound,
     MetadataInconsistency,
     NeptuneFeatureNotAvailableException,
-    NeptuneLegacyProjectException,
     NeptuneLimitExceedException,
     NeptuneObjectCreationConflict,
     ProjectNotFound,
     ProjectNotFoundWithSuggestions,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    ArtifactAttribute,
-    Attribute,
-    AttributeType,
-    BoolAttribute,
-    DatetimeAttribute,
-    FileAttribute,
-    FloatAttribute,
     FloatPointValue,
-    FloatSeriesAttribute,
     FloatSeriesValues,
     ImageSeriesValues,
-    IntAttribute,
-    LeaderboardEntry,
     OptionalFeatures,
     Project,
-    StringAttribute,
     StringPointValue,
-    StringSeriesAttribute,
     StringSeriesValues,
-    StringSetAttribute,
     Workspace,
 )
 from neptune.internal.backends.hosted_artifact_operations import (
     get_artifact_attribute,
     list_artifact_files,
     track_to_existing_artifact,
     track_to_new_artifact,
@@ -118,17 +114,23 @@
 from neptune.internal.backends.operation_api_object_converter import OperationApiObjectConverter
 from neptune.internal.backends.operations_preprocessor import OperationsPreprocessor
 from neptune.internal.backends.utils import (
     ExecuteOperationsBatchingManager,
     MissingApiClient,
     build_operation_url,
     ssl_verify,
+    with_api_exceptions_handler,
 )
 from neptune.internal.container_type import ContainerType
 from neptune.internal.credentials import Credentials
+from neptune.internal.exceptions import (
+    ClientHttpError,
+    InternalClientError,
+    NeptuneException,
+)
 from neptune.internal.id_formats import (
     QualifiedName,
     UniqueId,
 )
 from neptune.internal.operation import (
     DeleteAttribute,
     Operation,
@@ -138,55 +140,54 @@
     UploadFileSet,
 )
 from neptune.internal.utils import base64_decode
 from neptune.internal.utils.generic_attribute_mapper import map_attribute_result_to_value
 from neptune.internal.utils.git import GitInfo
 from neptune.internal.utils.logger import get_logger
 from neptune.internal.utils.paths import path_to_str
+from neptune.internal.utils.patterns import PROJECT_QUALIFIED_NAME_PATTERN
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
 from neptune.internal.websockets.websockets_factory import WebsocketsFactory
 from neptune.management.exceptions import ObjectNotFound
 from neptune.typing import ProgressBarType
-from neptune.version import version as neptune_client_version
+from neptune.version import version as neptune_version
 
 if TYPE_CHECKING:
     from bravado.requests_client import RequestsClient
 
     from neptune.internal.backends.api_model import ClientConfig
 
 
 _logger = get_logger()
 
 ATOMIC_ATTRIBUTE_TYPES = {
-    AttributeType.INT.value,
-    AttributeType.FLOAT.value,
-    AttributeType.STRING.value,
-    AttributeType.BOOL.value,
-    AttributeType.DATETIME.value,
-    AttributeType.RUN_STATE.value,
-}
-
-ATOMIC_ATTRIBUTE_TYPES = {
-    AttributeType.INT.value,
-    AttributeType.FLOAT.value,
-    AttributeType.STRING.value,
-    AttributeType.BOOL.value,
-    AttributeType.DATETIME.value,
-    AttributeType.RUN_STATE.value,
+    FieldType.INT.value,
+    FieldType.FLOAT.value,
+    FieldType.STRING.value,
+    FieldType.BOOL.value,
+    FieldType.DATETIME.value,
+    FieldType.OBJECT_STATE.value,
 }
 
 
 class HostedNeptuneBackend(NeptuneBackend):
     def __init__(self, credentials: Credentials, proxies: Optional[Dict[str, str]] = None):
         self.credentials = credentials
         self.proxies = proxies
         self.missing_features = []
+        self.use_proto = os.getenv(NEPTUNE_USE_PROTOCOL_BUFFERS, "False").lower() in {"true", "1", "y"}
 
-        self._http_client, self._client_config = create_http_client_with_auth(
+        http_client, client_config = create_http_client_with_auth(
             credentials=credentials, ssl_verify=ssl_verify(), proxies=proxies
-        )  # type: (RequestsClient, ClientConfig)
+        )
+        self._http_client: "RequestsClient" = http_client
+        self._client_config: "ClientConfig" = client_config
 
         self.backend_client = create_backend_client(self._client_config, self._http_client)
         self.leaderboard_client = create_leaderboard_client(self._client_config, self._http_client)
 
         if self._client_config.has_feature(OptionalFeatures.ARTIFACTS):
             self.artifacts_client = create_artifacts_client(self._client_config, self._http_client)
         else:
@@ -235,17 +236,15 @@
                     )
 
             response = self.backend_client.api.getProject(
                 projectIdentifier=project_id,
                 **DEFAULT_REQUEST_KWARGS,
             ).response()
             project = response.result
-            project_version = project.version if hasattr(project, "version") else 1
-            if project_version < 2:
-                raise NeptuneLegacyProjectException(project_id)
+
             return Project(
                 id=project.id,
                 name=project.name,
                 workspace=project.organizationName,
                 sys_id=project.projectKey,
             )
         except HTTPNotFound:
@@ -413,21 +412,21 @@
         if additional_params is None:
             additional_params = dict()
 
         params = {
             "projectIdentifier": project_id,
             "parentId": parent_id,
             "type": container_type.to_api(),
-            "cliVersion": str(neptune_client_version),
+            "cliVersion": str(neptune_version),
             **additional_params,
         }
 
         kwargs = {
             "experimentCreationParams": params,
-            "X-Neptune-CliVersion": str(neptune_client_version),
+            "X-Neptune-CliVersion": str(neptune_version),
             **DEFAULT_REQUEST_KWARGS,
         }
 
         try:
             experiment = self.leaderboard_client.api.createExperiment(**kwargs).response().result
             return ApiExperiment.from_experiment(experiment)
         except HTTPNotFound:
@@ -495,15 +494,18 @@
                 container_id=container_id,
                 container_type=container_type,
                 upload_operations=preprocessed_operations.upload_operations,
                 operation_storage=operation_storage,
             )
         )
 
-        (artifact_operations_errors, assign_artifact_operations,) = self._execute_artifact_operations(
+        (
+            artifact_operations_errors,
+            assign_artifact_operations,
+        ) = self._execute_artifact_operations(
             container_id=container_id,
             container_type=container_type,
             artifact_operations=preprocessed_operations.artifact_operations,
         )
 
         errors.extend(artifact_operations_errors)
 
@@ -676,39 +678,38 @@
             return [MetadataInconsistency(err.errorDescription) for err in result]
         except HTTPNotFound as e:
             raise ContainerUUIDNotFound(container_id, container_type) from e
         except (HTTPPaymentRequired, HTTPUnprocessableEntity) as e:
             raise NeptuneLimitExceedException(reason=e.response.json().get("title", "Unknown reason")) from e
 
     @with_api_exceptions_handler
-    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[Attribute]:
-        def to_attribute(attr) -> Attribute:
-            return Attribute(attr.name, AttributeType(attr.type))
-
+    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[FieldDefinition]:
         params = {
             "experimentId": container_id,
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             experiment = self.leaderboard_client.api.getExperimentAttributes(**params).response().result
 
-            attribute_type_names = [at.value for at in AttributeType]
+            attribute_type_names = [at.value for at in FieldType]
             accepted_attributes = [attr for attr in experiment.attributes if attr.type in attribute_type_names]
 
             # Notify about ignored attrs
             ignored_attributes = set(attr.type for attr in experiment.attributes) - set(
                 attr.type for attr in accepted_attributes
             )
             if ignored_attributes:
                 _logger.warning(
                     "Ignored following attributes (unknown type): %s.\n" "Try to upgrade `neptune`.",
                     ignored_attributes,
                 )
 
-            return [to_attribute(attr) for attr in accepted_attributes if attr.type in attribute_type_names]
+            return [
+                FieldDefinition.from_model(field) for field in accepted_attributes if field.type in attribute_type_names
+            ]
         except HTTPNotFound as e:
             raise ContainerUUIDNotFound(
                 container_id=container_id,
                 container_type=container_type,
             ) from e
 
     def download_file_series_by_index(
@@ -776,98 +777,96 @@
         except ClientHttpError as e:
             if e.status == HTTPNotFound.status_code:
                 raise FetchAttributeNotFoundException(path_to_str(path))
             else:
                 raise
 
     @with_api_exceptions_handler
-    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatAttribute:
+    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getFloatAttribute(**params).response().result
-            return FloatAttribute(result.value)
+            return FloatField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
-    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntAttribute:
+    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getIntAttribute(**params).response().result
-            return IntAttribute(result.value)
+            return IntField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
-    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolAttribute:
+    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getBoolAttribute(**params).response().result
-            return BoolAttribute(result.value)
+            return BoolField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
-    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileAttribute:
+    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getFileAttribute(**params).response().result
-            return FileAttribute(name=result.name, ext=result.ext, size=result.size)
+            return FileField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
-    def get_string_attribute(
-        self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringAttribute:
+    def get_string_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> StringField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getStringAttribute(**params).response().result
-            return StringAttribute(result.value)
+            return StringField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_datetime_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> DatetimeAttribute:
+    ) -> DateTimeField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getDatetimeAttribute(**params).response().result
-            return DatetimeAttribute(result.value)
+            return DateTimeField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     def get_artifact_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> ArtifactAttribute:
+    ) -> ArtifactField:
         return get_artifact_attribute(
             swagger_client=self.leaderboard_client,
             parent_identifier=container_id,
             path=path,
             default_request_params=DEFAULT_REQUEST_KWARGS,
         )
 
@@ -893,53 +892,53 @@
             return [FileEntry.from_dto(entry) for entry in entries]
         except HTTPNotFound:
             raise FileSetNotFound(attribute, path)
 
     @with_api_exceptions_handler
     def get_float_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> FloatSeriesAttribute:
+    ) -> FloatSeriesField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getFloatSeriesAttribute(**params).response().result
-            return FloatSeriesAttribute(result.last)
+            return FloatSeriesField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_string_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSeriesAttribute:
+    ) -> StringSeriesField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getStringSeriesAttribute(**params).response().result
-            return StringSeriesAttribute(result.last)
+            return StringSeriesField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_string_set_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSetAttribute:
+    ) -> StringSetField:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getStringSetAttribute(**params).response().result
-            return StringSetAttribute(set(result.values))
+            return StringSetField.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_image_series_values(
         self,
         container_id: str,
@@ -1010,15 +1009,15 @@
             )
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def fetch_atom_attribute_values(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> List[Tuple[str, AttributeType, Any]]:
+    ) -> List[Tuple[str, FieldType, Any]]:
         params = {
             "experimentId": container_id,
         }
         try:
             namespace_prefix = path_to_str(path)
             if namespace_prefix:
                 # don't want to catch "ns/attribute/other" while looking for "ns/attr"
@@ -1065,24 +1064,29 @@
         types: Optional[Iterable[ContainerType]] = None,
         query: Optional[NQLQuery] = None,
         columns: Optional[Iterable[str]] = None,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
+        step_size: Optional[int] = None,
+        use_proto: Optional[bool] = None,
     ) -> Generator[LeaderboardEntry, None, None]:
-        default_step_size = int(os.getenv(NEPTUNE_FETCH_TABLE_STEP_SIZE, "100"))
+        use_proto = use_proto if use_proto is not None else self.use_proto
+        default_step_size = step_size or int(os.getenv(NEPTUNE_FETCH_TABLE_STEP_SIZE, "100"))
 
         step_size = min(default_step_size, limit) if limit else default_step_size
 
         types_filter = list(map(lambda container_type: container_type.to_api(), types)) if types else None
         attributes_filter = {"attributeFilters": [{"path": column} for column in columns]} if columns else {}
 
         if sort_by == "sys/creation_time":
-            sort_by_column_type = AttributeType.DATETIME.value
+            sort_by_column_type = FieldType.DATETIME.value
+        elif sort_by == "sys/id":
+            sort_by_column_type = FieldType.STRING.value
         else:
             sort_by_column_type_candidates = self._get_column_types(project_id, sort_by, types_filter)
             sort_by_column_type = _get_column_type_from_entries(sort_by_column_type_candidates, sort_by)
 
         try:
             return iter_over_pages(
                 client=self.leaderboard_client,
@@ -1092,14 +1096,15 @@
                 attributes_filter=attributes_filter,
                 step_size=step_size,
                 limit=limit,
                 sort_by=sort_by,
                 ascending=ascending,
                 sort_by_column_type=sort_by_column_type,
                 progress_bar=progress_bar,
+                use_proto=use_proto,
             )
         except HTTPNotFound:
             raise ProjectNotFound(project_id)
 
     def get_run_url(self, run_id: str, workspace: str, project_name: str, sys_id: str) -> str:
         base_url = self.get_display_address()
         return f"{base_url}/{workspace}/{project_name}/e/{sys_id}"
@@ -1119,14 +1124,69 @@
         workspace: str,
         project_name: str,
         sys_id: str,
     ) -> str:
         base_url = self.get_display_address()
         return f"{base_url}/{workspace}/{project_name}/m/{model_id}/v/{sys_id}"
 
+    def get_fields_definitions(
+        self,
+        container_id: str,
+        container_type: ContainerType,
+        use_proto: Optional[bool] = None,
+    ) -> List[FieldDefinition]:
+        use_proto = use_proto if use_proto is not None else self.use_proto
+
+        params = {
+            "experimentIdentifier": container_id,
+            **DEFAULT_REQUEST_KWARGS,
+        }
+
+        try:
+            if use_proto:
+                result = self.leaderboard_client.api.queryAttributeDefinitionsProto(**params).response().result
+                data = ProtoAttributesSearchResultDTO.FromString(result)
+                return [FieldDefinition.from_proto(field_def) for field_def in data.entries]
+            else:
+                data = self.leaderboard_client.api.queryAttributeDefinitions(**params).response().result
+                return [FieldDefinition.from_model(field_def) for field_def in data.entries]
+        except HTTPNotFound as e:
+            raise ContainerUUIDNotFound(
+                container_id=container_id,
+                container_type=container_type,
+            ) from e
+
+    def get_fields_with_paths_filter(
+        self, container_id: str, container_type: ContainerType, paths: List[str], use_proto: Optional[bool] = None
+    ) -> List[Field]:
+        use_proto = use_proto if use_proto is not None else self.use_proto
+
+        params = {
+            "holderIdentifier": container_id,
+            "holderType": "experiment",
+            "attributeQuery": {
+                "attributePathsFilter": paths,
+            },
+            **DEFAULT_REQUEST_KWARGS,
+        }
+
+        try:
+            if use_proto:
+                result = self.leaderboard_client.api.getAttributesWithPathsFilterProto(**params).response().result
+                data = ProtoAttributesDTO.FromString(result)
+                return [Field.from_proto(field) for field in data.attributes]
+            else:
+                data = self.leaderboard_client.api.getAttributesWithPathsFilter(**params).response().result
+                return [Field.from_model(field) for field in data.attributes]
+        except HTTPNotFound as e:
+            raise ContainerUUIDNotFound(
+                container_id=container_id,
+                container_type=container_type,
+            ) from e
+
 
 def _get_column_type_from_entries(entries: List[Any], column: str) -> str:
     if not entries:  # column chosen is not present in the table
         raise ValueError(f"Column '{column}' chosen for sorting is not present in the table")
 
     if len(entries) == 1 and entries[0].name == column:
         return entries[0].type
@@ -1138,15 +1198,15 @@
         if entry.type not in ATOMIC_ATTRIBUTE_TYPES:  # non-atomic type - no need to look further
             raise ValueError(
                 f"Column {column} used for sorting is a complex type. For more, "
                 f"see https://docs.neptune.ai/api/field_types/#simple-types"
             )
         types.add(entry.type)
 
-    if types == {AttributeType.INT.value, AttributeType.FLOAT.value}:
-        return AttributeType.FLOAT.value
+    if types == {FieldType.INT.value, FieldType.FLOAT.value}:
+        return FieldType.FLOAT.value
 
     warn_once(
         f"Column {column} contains more than one simple data type. Sorting result might be inaccurate.",
         exception=NeptuneWarning,
     )
-    return AttributeType.STRING.value
+    return FieldType.STRING.value
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/neptune_backend.py` & `neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,41 +21,44 @@
     Generator,
     List,
     Optional,
     Tuple,
     Union,
 )
 
-from neptune.api.dtos import FileEntry
-from neptune.common.exceptions import NeptuneException
+from neptune.api.models import (
+    ArtifactField,
+    BoolField,
+    DateTimeField,
+    Field,
+    FieldDefinition,
+    FieldType,
+    FileEntry,
+    FileField,
+    FloatField,
+    FloatSeriesField,
+    IntField,
+    LeaderboardEntry,
+    StringField,
+    StringSeriesField,
+    StringSetField,
+)
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    ArtifactAttribute,
-    Attribute,
-    AttributeType,
-    BoolAttribute,
-    DatetimeAttribute,
-    FileAttribute,
-    FloatAttribute,
-    FloatSeriesAttribute,
     FloatSeriesValues,
     ImageSeriesValues,
-    IntAttribute,
-    LeaderboardEntry,
     Project,
-    StringAttribute,
-    StringSeriesAttribute,
     StringSeriesValues,
-    StringSetAttribute,
     Workspace,
 )
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.id_formats import (
     QualifiedName,
     UniqueId,
 )
 from neptune.internal.operation import Operation
 from neptune.internal.utils.git import GitInfo
 from neptune.internal.websockets.websockets_factory import WebsocketsFactory
@@ -142,15 +145,15 @@
         container_type: ContainerType,
         operations: List[Operation],
         operation_storage: OperationStorage,
     ) -> Tuple[int, List[NeptuneException]]:
         pass
 
     @abc.abstractmethod
-    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[Attribute]:
+    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[FieldDefinition]:
         pass
 
     @abc.abstractmethod
     def download_file(
         self,
         container_id: str,
         container_type: ContainerType,
@@ -168,67 +171,65 @@
         path: List[str],
         destination: Optional[str] = None,
         progress_bar: Optional[ProgressBarType] = None,
     ):
         pass
 
     @abc.abstractmethod
-    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatAttribute:
+    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatField:
         pass
 
     @abc.abstractmethod
-    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntAttribute:
+    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntField:
         pass
 
     @abc.abstractmethod
-    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolAttribute:
+    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolField:
         pass
 
     @abc.abstractmethod
-    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileAttribute:
+    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileField:
         pass
 
     @abc.abstractmethod
-    def get_string_attribute(
-        self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringAttribute:
+    def get_string_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> StringField:
         pass
 
     @abc.abstractmethod
     def get_datetime_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> DatetimeAttribute:
+    ) -> DateTimeField:
         pass
 
     @abc.abstractmethod
     def get_artifact_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> ArtifactAttribute:
+    ) -> ArtifactField:
         pass
 
     @abc.abstractmethod
     def list_artifact_files(self, project_id: str, artifact_hash: str) -> List[ArtifactFileData]:
         pass
 
     @abc.abstractmethod
     def get_float_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> FloatSeriesAttribute:
+    ) -> FloatSeriesField:
         pass
 
     @abc.abstractmethod
     def get_string_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSeriesAttribute:
+    ) -> StringSeriesField:
         pass
 
     @abc.abstractmethod
     def get_string_set_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSetAttribute:
+    ) -> StringSetField:
         pass
 
     @abc.abstractmethod
     def download_file_series_by_index(
         self,
         container_id: str,
         container_type: ContainerType,
@@ -291,30 +292,46 @@
         model_id: str,
         workspace: str,
         project_name: str,
         sys_id: str,
     ) -> str:
         pass
 
+    # WARN: Used in Neptune Fetcher
+    @abc.abstractmethod
+    def get_fields_definitions(
+        self,
+        container_id: str,
+        container_type: ContainerType,
+        use_proto: Optional[bool] = None,
+    ) -> List[FieldDefinition]: ...
+
+    # WARN: Used in Neptune Fetcher
+    @abc.abstractmethod
+    def get_fields_with_paths_filter(
+        self, container_id: str, container_type: ContainerType, paths: List[str], use_proto: Optional[bool] = None
+    ) -> List[Field]: ...
+
     @abc.abstractmethod
     def fetch_atom_attribute_values(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> List[Tuple[str, AttributeType, Any]]:
+    ) -> List[Tuple[str, FieldType, Any]]:
         pass
 
     @abc.abstractmethod
     def search_leaderboard_entries(
         self,
         project_id: UniqueId,
         types: Optional[List[ContainerType]] = None,
         query: Optional[NQLQuery] = None,
         columns: Optional[List[str]] = None,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
+        use_proto: Optional[bool] = None,
     ) -> Generator[LeaderboardEntry, None, None]:
         pass
 
     @abc.abstractmethod
     def list_fileset_files(self, attribute: List[str], container_id: str, path: str) -> List[FileEntry]:
         pass
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,56 +30,59 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from zipfile import ZipFile
 
-from neptune.api.dtos import FileEntry
-from neptune.common.exceptions import (
-    InternalClientError,
-    NeptuneException,
+from neptune.api.models import (
+    ArtifactField,
+    BoolField,
+    DateTimeField,
+    Field,
+    FieldDefinition,
+    FieldType,
+    FileEntry,
+    FileField,
+    FloatField,
+    FloatSeriesField,
+    IntField,
+    LeaderboardEntry,
+    StringField,
+    StringSeriesField,
+    StringSetField,
 )
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.exceptions import (
     ContainerUUIDNotFound,
     MetadataInconsistency,
     ModelVersionNotFound,
     ProjectNotFound,
     RunNotFound,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    ArtifactAttribute,
-    Attribute,
-    AttributeType,
-    BoolAttribute,
-    DatetimeAttribute,
-    FileAttribute,
-    FloatAttribute,
     FloatPointValue,
-    FloatSeriesAttribute,
     FloatSeriesValues,
     ImageSeriesValues,
-    IntAttribute,
-    LeaderboardEntry,
     Project,
-    StringAttribute,
     StringPointValue,
-    StringSeriesAttribute,
     StringSeriesValues,
-    StringSetAttribute,
     Workspace,
 )
 from neptune.internal.backends.hosted_file_operations import get_unique_upload_entries
 from neptune.internal.backends.neptune_backend import NeptuneBackend
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_structure import ContainerStructure
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import (
+    InternalClientError,
+    NeptuneException,
+)
 from neptune.internal.id_formats import (
     QualifiedName,
     SysId,
     UniqueId,
 )
 from neptune.internal.operation import (
     AddStrings,
@@ -307,25 +310,25 @@
         visitor = NeptuneBackendMock.NewValueOpVisitor(self, op.path, val, operation_storage)
         new_val = visitor.visit(op)
         if new_val is not None:
             run.set(op.path, new_val)
         else:
             run.pop(op.path)
 
-    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[Attribute]:
+    def get_attributes(self, container_id: str, container_type: ContainerType) -> List[FieldDefinition]:
         run = self._get_container(container_id, container_type)
         return list(self._generate_attributes(None, run.get_structure()))
 
     def _generate_attributes(self, base_path: Optional[str], values: dict):
         for key, value_or_dict in values.items():
             new_path = base_path + "/" + key if base_path is not None else key
             if isinstance(value_or_dict, dict):
                 yield from self._generate_attributes(new_path, value_or_dict)
             else:
-                yield Attribute(
+                yield FieldDefinition(
                     new_path,
                     value_or_dict.accept(self._attribute_type_converter_value_visitor),
                 )
 
     def download_file(
         self,
         container_id: str,
@@ -366,72 +369,71 @@
 
         upload_entries = get_unique_upload_entries(source_file_set_value.file_globs)
 
         with ZipFile(target_file, "w") as zipObj:
             for upload_entry in upload_entries:
                 zipObj.write(upload_entry.source, upload_entry.target_path)
 
-    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatAttribute:
+    def get_float_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FloatField:
         val = self._get_attribute(container_id, container_type, path, Float)
-        return FloatAttribute(val.value)
+        return FloatField(path=path_to_str(path), value=val.value)
 
-    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntAttribute:
+    def get_int_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> IntField:
         val = self._get_attribute(container_id, container_type, path, Integer)
-        return IntAttribute(val.value)
+        return IntField(path=path_to_str(path), value=val.value)
 
-    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolAttribute:
+    def get_bool_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> BoolField:
         val = self._get_attribute(container_id, container_type, path, Boolean)
-        return BoolAttribute(val.value)
+        return BoolField(path=path_to_str(path), value=val.value)
 
-    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileAttribute:
+    def get_file_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> FileField:
         val = self._get_attribute(container_id, container_type, path, File)
-        return FileAttribute(
+        return FileField(
+            path=path_to_str(path),
             name=os.path.basename(val.path) if val.file_type is FileType.LOCAL_FILE else "",
             ext=val.extension or "",
             size=0,
         )
 
-    def get_string_attribute(
-        self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringAttribute:
+    def get_string_attribute(self, container_id: str, container_type: ContainerType, path: List[str]) -> StringField:
         val = self._get_attribute(container_id, container_type, path, String)
-        return StringAttribute(val.value)
+        return StringField(path=path_to_str(path), value=val.value)
 
     def get_datetime_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> DatetimeAttribute:
+    ) -> DateTimeField:
         val = self._get_attribute(container_id, container_type, path, Datetime)
-        return DatetimeAttribute(val.value)
+        return DateTimeField(path=path_to_str(path), value=val.value)
 
     def get_artifact_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> ArtifactAttribute:
+    ) -> ArtifactField:
         val = self._get_attribute(container_id, container_type, path, Artifact)
-        return ArtifactAttribute(val.hash)
+        return ArtifactField(path=path_to_str(path), hash=val.hash)
 
     def list_artifact_files(self, project_id: str, artifact_hash: str) -> List[ArtifactFileData]:
         return self._artifacts[(project_id, artifact_hash)]
 
     def get_float_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> FloatSeriesAttribute:
+    ) -> FloatSeriesField:
         val = self._get_attribute(container_id, container_type, path, FloatSeries)
-        return FloatSeriesAttribute(val.values[-1] if val.values else None)
+        return FloatSeriesField(path=path_to_str(path), last=val.values[-1] if val.values else None)
 
     def get_string_series_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSeriesAttribute:
+    ) -> StringSeriesField:
         val = self._get_attribute(container_id, container_type, path, StringSeries)
-        return StringSeriesAttribute(val.values[-1] if val.values else None)
+        return StringSeriesField(path=path_to_str(path), last=val.values[-1] if val.values else None)
 
     def get_string_set_attribute(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> StringSetAttribute:
+    ) -> StringSetField:
         val = self._get_attribute(container_id, container_type, path, StringSet)
-        return StringSetAttribute(set(val.values))
+        return StringSetField(path=path_to_str(path), values=set(val.values))
 
     def _get_attribute(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
         expected_type: Type[Val],
@@ -509,14 +511,22 @@
         model_id: str,
         workspace: str,
         project_name: str,
         sys_id: str,
     ) -> str:
         return f"offline/{model_version_id}"
 
+    def get_fields_definitions(
+        self,
+        container_id: str,
+        container_type: ContainerType,
+        use_proto: Optional[bool] = None,
+    ) -> List[FieldDefinition]:
+        return []
+
     def _get_attribute_values(self, value_dict, path_prefix: List[str]):
         assert isinstance(value_dict, dict)
         for k, value in value_dict.items():
             if isinstance(value, dict):
                 yield from self._get_attribute_values(value, path_prefix + [k])
             else:
                 attr_type = value.accept(self._attribute_type_converter_value_visitor).value
@@ -524,15 +534,15 @@
                 if hasattr(value, "value"):
                     yield attr_path, attr_type, value.value
                 else:
                     return attr_path, attr_type, NoValue
 
     def fetch_atom_attribute_values(
         self, container_id: str, container_type: ContainerType, path: List[str]
-    ) -> List[Tuple[str, AttributeType, Any]]:
+    ) -> List[Tuple[str, FieldType, Any]]:
         run = self._get_container(container_id, container_type)
         values = self._get_attribute_values(run.get(path), path)
         namespace_prefix = path_to_str(path)
         if namespace_prefix:
             # don't want to catch "ns/attribute/other" while looking for "ns/attr"
             namespace_prefix += "/"
         return [
@@ -547,61 +557,62 @@
         types: Optional[Iterable[ContainerType]] = None,
         query: Optional[NQLQuery] = None,
         columns: Optional[Iterable[str]] = None,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
+        use_proto: Optional[bool] = None,
     ) -> Generator[LeaderboardEntry, None, None]:
         """Non relevant for mock"""
 
-    class AttributeTypeConverterValueVisitor(ValueVisitor[AttributeType]):
-        def visit_float(self, _: Float) -> AttributeType:
-            return AttributeType.FLOAT
+    class AttributeTypeConverterValueVisitor(ValueVisitor[FieldType]):
+        def visit_float(self, _: Float) -> FieldType:
+            return FieldType.FLOAT
 
-        def visit_integer(self, _: Integer) -> AttributeType:
-            return AttributeType.INT
+        def visit_integer(self, _: Integer) -> FieldType:
+            return FieldType.INT
 
-        def visit_boolean(self, _: Boolean) -> AttributeType:
-            return AttributeType.BOOL
+        def visit_boolean(self, _: Boolean) -> FieldType:
+            return FieldType.BOOL
 
-        def visit_string(self, _: String) -> AttributeType:
-            return AttributeType.STRING
+        def visit_string(self, _: String) -> FieldType:
+            return FieldType.STRING
 
-        def visit_datetime(self, _: Datetime) -> AttributeType:
-            return AttributeType.DATETIME
+        def visit_datetime(self, _: Datetime) -> FieldType:
+            return FieldType.DATETIME
 
-        def visit_file(self, _: File) -> AttributeType:
-            return AttributeType.FILE
+        def visit_file(self, _: File) -> FieldType:
+            return FieldType.FILE
 
-        def visit_file_set(self, _: FileSet) -> AttributeType:
-            return AttributeType.FILE_SET
+        def visit_file_set(self, _: FileSet) -> FieldType:
+            return FieldType.FILE_SET
 
-        def visit_float_series(self, _: FloatSeries) -> AttributeType:
-            return AttributeType.FLOAT_SERIES
+        def visit_float_series(self, _: FloatSeries) -> FieldType:
+            return FieldType.FLOAT_SERIES
 
-        def visit_string_series(self, _: StringSeries) -> AttributeType:
-            return AttributeType.STRING_SERIES
+        def visit_string_series(self, _: StringSeries) -> FieldType:
+            return FieldType.STRING_SERIES
 
-        def visit_image_series(self, _: FileSeries) -> AttributeType:
-            return AttributeType.IMAGE_SERIES
+        def visit_image_series(self, _: FileSeries) -> FieldType:
+            return FieldType.IMAGE_SERIES
 
-        def visit_string_set(self, _: StringSet) -> AttributeType:
-            return AttributeType.STRING_SET
+        def visit_string_set(self, _: StringSet) -> FieldType:
+            return FieldType.STRING_SET
 
-        def visit_git_ref(self, _: GitRef) -> AttributeType:
-            return AttributeType.GIT_REF
+        def visit_git_ref(self, _: GitRef) -> FieldType:
+            return FieldType.GIT_REF
 
-        def visit_artifact(self, _: Artifact) -> AttributeType:
-            return AttributeType.ARTIFACT
+        def visit_artifact(self, _: Artifact) -> FieldType:
+            return FieldType.ARTIFACT
 
-        def visit_namespace(self, _: Namespace) -> AttributeType:
+        def visit_namespace(self, _: Namespace) -> FieldType:
             raise NotImplementedError
 
-        def copy_value(self, source_type: Type[Attribute], source_path: List[str]) -> AttributeType:
+        def copy_value(self, source_type: Type[FieldDefinition], source_path: List[str]) -> FieldType:
             raise NotImplementedError
 
     class NewValueOpVisitor(OperationVisitor[Optional[Value]]):
         def __init__(
             self, backend, path: List[str], current_value: Optional[Value], operation_storage: OperationStorage
         ):
             self._backend = backend
@@ -782,7 +793,12 @@
             FileEntry(
                 name="mock_name",
                 size=100,
                 mtime=datetime.now(),
                 file_type="file",
             )
         ]
+
+    def get_fields_with_paths_filter(
+        self, container_id: str, container_type: ContainerType, paths: List[str], use_proto: Optional[bool] = None
+    ) -> List[Field]:
+        return []
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-2.0.0a0/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["OperationApiNameVisitor"]
 
-from neptune.common.exceptions import InternalClientError
+from neptune.internal.exceptions import InternalClientError
 from neptune.internal.operation import (
     AddStrings,
     AssignArtifact,
     AssignBool,
     AssignDatetime,
     AssignFloat,
     AssignInt,
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-2.0.0a0/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["OperationApiObjectConverter"]
 
-from neptune.common.exceptions import InternalClientError
+from neptune.internal.exceptions import InternalClientError
 from neptune.internal.operation import (
     AddStrings,
     AssignArtifact,
     AssignBool,
     AssignDatetime,
     AssignFloat,
     AssignInt,
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-2.0.0a0/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from enum import Enum
 from typing import (
     Callable,
     List,
     TypeVar,
 )
 
-from neptune.common.exceptions import InternalClientError
 from neptune.exceptions import MetadataInconsistency
+from neptune.internal.exceptions import InternalClientError
 from neptune.internal.operation import (
     AddStrings,
     AssignArtifact,
     AssignBool,
     AssignDatetime,
     AssignFloat,
     AssignInt,
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/project_name_lookup.py` & `neptune-2.0.0a0/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-2.0.0a0/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     Optional,
 )
 
 from bravado.client import SwaggerClient
 from bravado.exception import HTTPError
 
 from neptune.api.requests_utils import ensure_json_response
-from neptune.common.exceptions import (
-    NeptuneAuthTokenExpired,
-    WritingToArchivedProjectException,
-)
 from neptune.exceptions import (
     NeptuneFieldCountLimitExceedException,
     NeptuneLimitExceedException,
 )
+from neptune.internal.exceptions import (
+    NeptuneAuthTokenExpired,
+    WritingToArchivedProjectException,
+)
 
 
 class ApiMethodWrapper:
     def __init__(self, api_method):
         self._api_method = api_method
 
     @staticmethod
```

### Comparing `neptune-1.9.1/src/neptune/internal/backends/utils.py` & `neptune-2.0.0a0/src/neptune/internal/backends/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,19 +24,22 @@
     "MissingApiClient",
     "cache",
     "ssl_verify",
     "parse_validation_errors",
     "ExecuteOperationsBatchingManager",
     "which_progress_bar",
     "construct_progress_bar",
+    "with_api_exceptions_handler",
 ]
 
 import dataclasses
+import itertools
 import os
 import socket
+import time
 from functools import (
     lru_cache,
     wraps,
 )
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -49,46 +52,73 @@
     Type,
 )
 from urllib.parse import (
     urljoin,
     urlparse,
 )
 
+import requests
 import urllib3
 from bravado.client import SwaggerClient
-from bravado.exception import HTTPError
+from bravado.exception import (
+    BravadoConnectionError,
+    BravadoTimeoutError,
+    HTTPBadGateway,
+    HTTPClientError,
+    HTTPError,
+    HTTPForbidden,
+    HTTPGatewayTimeout,
+    HTTPInternalServerError,
+    HTTPRequestTimeout,
+    HTTPServiceUnavailable,
+    HTTPTooManyRequests,
+    HTTPUnauthorized,
+)
 from bravado.http_client import HttpClient
 from bravado.requests_client import RequestsResponseAdapter
 from bravado_core.formatter import SwaggerFormat
+from bravado_core.util import RecursiveCallException
 from packaging.version import Version
 from requests import (
     Response,
     Session,
 )
+from requests.exceptions import ChunkedEncodingError
+from urllib3.exceptions import NewConnectionError
 
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
 from neptune.envs import NEPTUNE_ALLOW_SELF_SIGNED_CERTIFICATE
 from neptune.exceptions import (
     CannotResolveHostname,
     MetadataInconsistency,
     NeptuneClientUpgradeRequiredError,
     NeptuneFeatureNotAvailableException,
 )
 from neptune.internal.backends.api_model import ClientConfig
 from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
+from neptune.internal.envs import NEPTUNE_RETRIES_TIMEOUT_ENV
+from neptune.internal.exceptions import (
+    ClientHttpError,
+    Forbidden,
+    NeptuneAuthTokenExpired,
+    NeptuneConnectionLostException,
+    NeptuneInvalidApiTokenException,
+    NeptuneSSLVerificationError,
+    Unauthorized,
+)
 from neptune.internal.operation import (
     CopyAttribute,
     Operation,
 )
 from neptune.internal.utils import replace_patch_version
 from neptune.internal.utils.logger import get_logger
+from neptune.internal.utils.utils import reset_internal_ssl_state
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
 from neptune.typing import (
     ProgressBarCallback,
     ProgressBarType,
 )
 from neptune.utils import (
     NullProgressBar,
     TqdmProgressBar,
@@ -96,14 +126,127 @@
 
 logger = get_logger()
 
 if TYPE_CHECKING:
     from neptune.internal.backends.neptune_backend import NeptuneBackend
 
 
+MAX_RETRY_TIME = 30
+MAX_RETRY_MULTIPLIER = 10
+retries_timeout = int(os.getenv(NEPTUNE_RETRIES_TIMEOUT_ENV, "60"))
+
+
+def get_retry_from_headers_or_default(headers, retry_count):
+    try:
+        return (
+            int(headers["retry-after"][0]) if "retry-after" in headers else 2 ** min(MAX_RETRY_MULTIPLIER, retry_count)
+        )
+    except Exception:
+        return min(2 ** min(MAX_RETRY_MULTIPLIER, retry_count), MAX_RETRY_TIME)
+
+
+def with_api_exceptions_handler(func):
+    def wrapper(*args, **kwargs):
+        ssl_error_occurred = False
+        last_exception = None
+        start_time = time.monotonic()
+        for retry in itertools.count(0):
+            if time.monotonic() - start_time > retries_timeout:
+                break
+
+            try:
+                return func(*args, **kwargs)
+            except requests.exceptions.InvalidHeader as e:
+                if "X-Neptune-Api-Token" in e.args[0]:
+                    raise NeptuneInvalidApiTokenException()
+                raise
+            except requests.exceptions.SSLError as e:
+                """
+                OpenSSL's internal random number generator does not properly handle forked processes.
+                Applications must change the PRNG state of the parent process
+                if they use any SSL feature with os.fork().
+                Any successful call of RAND_add(), RAND_bytes() or RAND_pseudo_bytes() is sufficient.
+                https://docs.python.org/3/library/ssl.html#multi-processing
+                On Linux it looks like it does not help much but does not break anything either.
+                But single retry seems to solve the issue.
+                """
+                if not ssl_error_occurred:
+                    ssl_error_occurred = True
+                    reset_internal_ssl_state()
+                    continue
+
+                if "CertificateError" in str(e.__context__):
+                    raise NeptuneSSLVerificationError() from e
+                else:
+                    time.sleep(min(2 ** min(MAX_RETRY_MULTIPLIER, retry), MAX_RETRY_TIME))
+                    last_exception = e
+                    continue
+            except (
+                BravadoConnectionError,
+                BravadoTimeoutError,
+                requests.exceptions.ConnectionError,
+                requests.exceptions.Timeout,
+                HTTPRequestTimeout,
+                HTTPServiceUnavailable,
+                HTTPGatewayTimeout,
+                HTTPBadGateway,
+                HTTPInternalServerError,
+                NewConnectionError,
+                ChunkedEncodingError,
+                RecursiveCallException,
+            ) as e:
+                time.sleep(min(2 ** min(MAX_RETRY_MULTIPLIER, retry), MAX_RETRY_TIME))
+                last_exception = e
+                continue
+            except HTTPTooManyRequests as e:
+                wait_time = get_retry_from_headers_or_default(e.response.headers, retry)
+                time.sleep(wait_time)
+                last_exception = e
+                continue
+            except NeptuneAuthTokenExpired as e:
+                last_exception = e
+                continue
+            except HTTPUnauthorized:
+                raise Unauthorized()
+            except HTTPForbidden:
+                raise Forbidden()
+            except HTTPClientError as e:
+                raise ClientHttpError(e.status_code, e.response.text) from e
+            except requests.exceptions.RequestException as e:
+                if e.response is None:
+                    raise
+                status_code = e.response.status_code
+                if status_code in (
+                    HTTPRequestTimeout.status_code,
+                    HTTPBadGateway.status_code,
+                    HTTPServiceUnavailable.status_code,
+                    HTTPGatewayTimeout.status_code,
+                    HTTPInternalServerError.status_code,
+                ):
+                    time.sleep(min(2 ** min(MAX_RETRY_MULTIPLIER, retry), MAX_RETRY_TIME))
+                    last_exception = e
+                    continue
+                elif status_code == HTTPTooManyRequests.status_code:
+                    wait_time = get_retry_from_headers_or_default(e.response.headers, retry)
+                    time.sleep(wait_time)
+                    last_exception = e
+                    continue
+                elif status_code == HTTPUnauthorized.status_code:
+                    raise Unauthorized()
+                elif status_code == HTTPForbidden.status_code:
+                    raise Forbidden()
+                elif 400 <= status_code < 500:
+                    raise ClientHttpError(status_code, e.response.text) from e
+                else:
+                    raise
+        raise NeptuneConnectionLostException(last_exception) from last_exception
+
+    return wrapper
+
+
 @lru_cache(maxsize=None, typed=True)
 def verify_host_resolution(url: str) -> None:
     host = urlparse(url).netloc.split(":")[0]
     try:
         socket.gethostbyname(host)
     except socket.gaierror:
         raise CannotResolveHostname(host)
```

### Comparing `neptune-1.9.1/src/neptune/internal/backgroud_job_list.py` & `neptune-2.0.0a0/src/neptune/internal/backgroud_job_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     List,
     Optional,
 )
 
 from neptune.internal.background_job import BackgroundJob
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class BackgroundJobList(BackgroundJob):
     def __init__(self, jobs: List[BackgroundJob]):
         self._jobs = jobs
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         for job in self._jobs:
             job.start(container)
 
     def stop(self):
         for job in self._jobs:
             job.stop()
```

### Comparing `neptune-1.9.1/src/neptune/internal/background_job.py` & `neptune-2.0.0a0/src/neptune/internal/background_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 import abc
 from typing import (
     TYPE_CHECKING,
     Optional,
 )
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class BackgroundJob:
     @abc.abstractmethod
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         pass
 
     @abc.abstractmethod
     def stop(self):
         pass
 
     @abc.abstractmethod
```

### Comparing `neptune-1.9.1/src/neptune/internal/constants.py` & `neptune-2.0.0a0/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/container_structure.py` & `neptune-2.0.0a0/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/container_type.py` & `neptune-2.0.0a0/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/credentials.py` & `neptune-2.0.0a0/src/neptune/internal/credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 import os
 from dataclasses import dataclass
 from typing import (
     Dict,
     Optional,
 )
 
-from neptune.common.envs import API_TOKEN_ENV_NAME
-from neptune.common.exceptions import NeptuneInvalidApiTokenException
 from neptune.constants import ANONYMOUS_API_TOKEN
 from neptune.exceptions import NeptuneMissingApiTokenException
 from neptune.internal.constants import ANONYMOUS_API_TOKEN_CONTENT
+from neptune.internal.envs import API_TOKEN_ENV_NAME
+from neptune.internal.exceptions import NeptuneInvalidApiTokenException
 
 
 @dataclass(frozen=True)
 class Credentials:
     api_token: str
     token_origin_address: str
     api_url_opt: str
```

### Comparing `neptune-1.9.1/src/neptune/internal/exceptions.py` & `neptune-2.0.0a0/src/neptune/types/sets/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["NeptuneInternalException"]
+__all__ = ["StringSet"]
 
-
-class NeptuneInternalException(Exception):
-    pass
+from .string_set import StringSet
```

### Comparing `neptune-1.9.1/src/neptune/internal/extensions.py` & `neptune-2.0.0a0/src/neptune/internal/extensions.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import entry_points
 else:
     from importlib_metadata import entry_points
 
-from neptune.common.warnings import (
+from neptune.internal.warnings import (
     NeptuneWarning,
     warn_once,
 )
 
 
 def get_entry_points(name: str) -> List[Tuple[str, Callable[[], None]]]:
     if (3, 8) <= sys.version_info < (3, 10):
```

### Comparing `neptune-1.9.1/src/neptune/internal/hardware/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-2.0.0a0/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,43 +20,43 @@
 from itertools import groupby
 from typing import (
     TYPE_CHECKING,
     Dict,
     Optional,
 )
 
-from neptune.common.hardware.gauges.gauge_factory import GaugeFactory
-from neptune.common.hardware.gauges.gauge_mode import GaugeMode
-from neptune.common.hardware.metrics.metrics_factory import MetricsFactory
-from neptune.common.hardware.metrics.reports.metric_reporter import MetricReporter
-from neptune.common.hardware.metrics.reports.metric_reporter_factory import MetricReporterFactory
-from neptune.common.hardware.resources.system_resource_info_factory import SystemResourceInfoFactory
-from neptune.common.hardware.system.system_monitor import SystemMonitor
-from neptune.common.utils import in_docker
 from neptune.internal.background_job import BackgroundJob
+from neptune.internal.hardware.gauges.gauge_factory import GaugeFactory
+from neptune.internal.hardware.gauges.gauge_mode import GaugeMode
 from neptune.internal.hardware.gpu.gpu_monitor import GPUMonitor
+from neptune.internal.hardware.metrics.metrics_factory import MetricsFactory
+from neptune.internal.hardware.metrics.reports.metric_reporter import MetricReporter
+from neptune.internal.hardware.metrics.reports.metric_reporter_factory import MetricReporterFactory
+from neptune.internal.hardware.resources.system_resource_info_factory import SystemResourceInfoFactory
+from neptune.internal.hardware.system.system_monitor import SystemMonitor
 from neptune.internal.threading.daemon import Daemon
 from neptune.internal.utils.logger import get_logger
+from neptune.internal.utils.utils import in_docker
 from neptune.types.series import FloatSeries
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 _logger = get_logger()
 
 
 class HardwareMetricReportingJob(BackgroundJob):
     def __init__(self, period: float = 10, attribute_namespace: str = "monitoring"):
         self._period = period
         self._thread = None
         self._started = False
         self._gauges_in_resource: Dict[str, int] = dict()
         self._attribute_namespace = attribute_namespace
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         gauge_mode = GaugeMode.CGROUP if in_docker() else GaugeMode.SYSTEM
         system_resource_info = SystemResourceInfoFactory(
             system_monitor=SystemMonitor(),
             gpu_monitor=GPUMonitor(),
             os_environ=os.environ,
         ).create(gauge_mode=gauge_mode)
         gauge_factory = GaugeFactory(gauge_mode=gauge_mode)
@@ -100,15 +100,15 @@
         return "{}/{}".format(self._attribute_namespace, resource_type).lower()
 
     class ReportingThread(Daemon):
         def __init__(
             self,
             outer: "HardwareMetricReportingJob",
             period: float,
-            container: "MetadataContainer",
+            container: "NeptuneObject",
             metric_reporter: MetricReporter,
         ):
             super().__init__(sleep_time=period, name="NeptuneReporting")
             self._outer = outer
             self._container = container
             self._metric_reporter = metric_reporter
```

### Comparing `neptune-1.9.1/src/neptune/internal/id_formats.py` & `neptune-2.0.0a0/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/init/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/init/parameters.py` & `neptune-2.0.0a0/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/notebooks/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/notebooks/comm.py` & `neptune-2.0.0a0/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/notebooks/notebooks.py` & `neptune-2.0.0a0/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation.py` & `neptune-2.0.0a0/src/neptune/internal/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
 )
 
-from neptune.common.exceptions import (
-    InternalClientError,
-    NeptuneException,
-)
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.exceptions import MalformedOperation
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import (
+    InternalClientError,
+    NeptuneException,
+)
 from neptune.internal.types.file_types import FileType
 from neptune.types.atoms.file import File
 
 if TYPE_CHECKING:
     from neptune.attributes.attribute import Attribute
     from neptune.internal.backends.neptune_backend import NeptuneBackend
     from neptune.internal.operation_visitor import OperationVisitor
```

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,22 @@
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
 )
 
-from neptune.common.exceptions import NeptuneException
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
 from neptune.constants import ASYNC_DIRECTORY
 from neptune.core.components.abstract import WithResources
 from neptune.core.components.metadata_file import MetadataFile
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.core.components.queue.disk_queue import DiskQueue
 from neptune.envs import NEPTUNE_SYNC_AFTER_STOP_TIMEOUT
 from neptune.exceptions import NeptuneSynchronizationAlreadyStoppedException
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.init.parameters import DEFAULT_STOP_TIMEOUT
 from neptune.internal.operation import Operation
 from neptune.internal.operation_processors.operation_logger import ProcessorStopLogger
 from neptune.internal.operation_processors.operation_processor import OperationProcessor
 from neptune.internal.operation_processors.utils import (
     common_metadata,
     get_container_full_path,
@@ -57,14 +53,18 @@
     signal_batch_lag,
     signal_batch_processed,
     signal_batch_started,
 )
 from neptune.internal.threading.daemon import Daemon
 from neptune.internal.utils.disk_utilization import ensure_disk_not_overutilize
 from neptune.internal.utils.logger import get_logger
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
 
 if TYPE_CHECKING:
     from neptune.core.components.abstract import Resource
     from neptune.internal.backends.neptune_backend import NeptuneBackend
     from neptune.internal.container_type import ContainerType
     from neptune.internal.id_formats import UniqueId
     from neptune.internal.operation_processors.operation_logger import ProcessorStopSignal
```

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/factory.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/operation_logger.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 if TYPE_CHECKING:
     from neptune.core.components.operation_storage import OperationStorage
     from neptune.internal.operation import Operation
 
 
 class OperationProcessor(abc.ABC):
     @abc.abstractmethod
-    def enqueue_operation(self, op: "Operation", *, wait: bool) -> None:
-        ...
+    def enqueue_operation(self, op: "Operation", *, wait: bool) -> None: ...
 
     @property
     def operation_storage(self) -> "OperationStorage":
         raise NotImplementedError()
 
     def start(self) -> None:
         pass
```

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ("ReadOnlyOperationProcessor",)
 
 from typing import TYPE_CHECKING
 
-from neptune.common.warnings import (
+from neptune.internal.operation_processors.operation_processor import OperationProcessor
+from neptune.internal.warnings import (
     NeptuneWarning,
     warn_once,
 )
-from neptune.internal.operation_processors.operation_processor import OperationProcessor
 
 if TYPE_CHECKING:
     from neptune.internal.operation import Operation
 
 
 class ReadOnlyOperationProcessor(OperationProcessor):
     def enqueue_operation(self, op: "Operation", *, wait: bool) -> None:
```

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/operation_processors/utils.py` & `neptune-2.0.0a0/src/neptune/internal/operation_processors/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,27 @@
 __all__ = ["common_metadata", "get_container_full_path", "get_container_dir"]
 
 import os
 import platform
 import random
 import string
 import sys
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
 )
 
 from neptune.constants import NEPTUNE_DATA_DIRECTORY
-from neptune.metadata_containers.structure_version import StructureVersion
+from neptune.objects.structure_version import StructureVersion
 
 if TYPE_CHECKING:
     from neptune.internal.container_type import ContainerType
     from neptune.internal.id_formats import UniqueId
 
 
 RANDOM_KEY_LENGTH = 8
@@ -50,15 +53,15 @@
         "mode": mode,
         "containerId": container_id,
         "containerType": container_type,
         "structureVersion": StructureVersion.DIRECT_DIRECTORY.value,
         "os": platform.platform(),
         "pythonVersion": sys.version,
         "neptuneClientVersion": get_neptune_version(),
-        "createdAt": datetime.utcnow().isoformat(),
+        "createdAt": datetime.now(timezone.utc).isoformat(),
     }
 
 
 def get_container_dir(container_id: "UniqueId", container_type: "ContainerType") -> str:
     return f"{container_type.value}__{container_id}__{os.getpid()}__{random_key(RANDOM_KEY_LENGTH)}"
```

### Comparing `neptune-1.9.1/src/neptune/internal/operation_visitor.py` & `neptune-2.0.0a0/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/signals_processing/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/signals_processing/background_job.py` & `neptune-2.0.0a0/src/neptune/internal/signals_processing/background_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,37 +23,37 @@
 )
 
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.signals_processing.signals_processor import SignalsProcessor
 
 if TYPE_CHECKING:
     from neptune.internal.signals_processing.signals import Signal
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class CallbacksMonitor(BackgroundJob):
     def __init__(
         self,
         queue: "Queue[Signal]",
         async_lag_threshold: float,
         async_no_progress_threshold: float,
-        async_lag_callback: Optional[Callable[["MetadataContainer"], None]] = None,
-        async_no_progress_callback: Optional[Callable[["MetadataContainer"], None]] = None,
+        async_lag_callback: Optional[Callable[["NeptuneObject"], None]] = None,
+        async_no_progress_callback: Optional[Callable[["NeptuneObject"], None]] = None,
         period: float = 10,
     ) -> None:
         self._period: float = period
         self._queue: "Queue[Signal]" = queue
         self._thread: Optional["SignalsProcessor"] = None
         self._started: bool = False
         self._async_lag_threshold: float = async_lag_threshold
         self._async_no_progress_threshold: float = async_no_progress_threshold
-        self._async_lag_callback: Optional[Callable[["MetadataContainer"], None]] = async_lag_callback
-        self._async_no_progress_callback: Optional[Callable[["MetadataContainer"], None]] = async_no_progress_callback
+        self._async_lag_callback: Optional[Callable[["NeptuneObject"], None]] = async_lag_callback
+        self._async_no_progress_callback: Optional[Callable[["NeptuneObject"], None]] = async_no_progress_callback
 
-    def start(self, container: "MetadataContainer") -> None:
+    def start(self, container: "NeptuneObject") -> None:
         self._thread = SignalsProcessor(
             period=self._period,
             container=container,
             queue=self._queue,
             async_lag_threshold=self._async_lag_threshold,
             async_no_progress_threshold=self._async_no_progress_threshold,
             async_lag_callback=self._async_lag_callback,
```

### Comparing `neptune-1.9.1/src/neptune/internal/signals_processing/signals.py` & `neptune-2.0.0a0/src/neptune/internal/signals_processing/signals.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 
 @dataclass
 class Signal:
     occured_at: float
 
     @abstractmethod
-    def accept(self, visitor: "SignalsVisitor") -> None:
-        ...
+    def accept(self, visitor: "SignalsVisitor") -> None: ...
 
 
 @dataclass
 class BatchStartedSignal(Signal):
     def accept(self, visitor: "SignalsVisitor") -> None:
         visitor.visit_batch_started(signal=self)
 
@@ -52,17 +51,14 @@
 
     def accept(self, visitor: "SignalsVisitor") -> None:
         visitor.visit_batch_lag(signal=self)
 
 
 class SignalsVisitor:
     @abstractmethod
-    def visit_batch_started(self, signal: Signal) -> None:
-        ...
+    def visit_batch_started(self, signal: Signal) -> None: ...
 
     @abstractmethod
-    def visit_batch_processed(self, signal: Signal) -> None:
-        ...
+    def visit_batch_processed(self, signal: Signal) -> None: ...
 
     @abstractmethod
-    def visit_batch_lag(self, signal: Signal) -> None:
-        ...
+    def visit_batch_lag(self, signal: Signal) -> None: ...
```

### Comparing `neptune-1.9.1/src/neptune/internal/signals_processing/signals_processor.py` & `neptune-2.0.0a0/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,39 +32,39 @@
     BatchLagSignal,
     SignalsVisitor,
 )
 from neptune.internal.threading.daemon import Daemon
 
 if TYPE_CHECKING:
     from neptune.internal.signals_processing.signals import Signal
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class SignalsProcessor(Daemon, SignalsVisitor):
     def __init__(
         self,
         *,
         period: float,
-        container: "MetadataContainer",
+        container: "NeptuneObject",
         queue: "Queue[Signal]",
         async_lag_threshold: float,
         async_no_progress_threshold: float,
-        async_lag_callback: Optional[Callable[["MetadataContainer"], None]] = None,
-        async_no_progress_callback: Optional[Callable[["MetadataContainer"], None]] = None,
+        async_lag_callback: Optional[Callable[["NeptuneObject"], None]] = None,
+        async_no_progress_callback: Optional[Callable[["NeptuneObject"], None]] = None,
         callbacks_interval: float = IN_BETWEEN_CALLBACKS_MINIMUM_INTERVAL,
         in_async: bool = True,
     ) -> None:
         super().__init__(sleep_time=period, name="CallbacksMonitor")
 
-        self._container: "MetadataContainer" = container
+        self._container: "NeptuneObject" = container
         self._queue: "Queue[Signal]" = queue
         self._async_lag_threshold: float = async_lag_threshold
         self._async_no_progress_threshold: float = async_no_progress_threshold
-        self._async_lag_callback: Optional[Callable[["MetadataContainer"], None]] = async_lag_callback
-        self._async_no_progress_callback: Optional[Callable[["MetadataContainer"], None]] = async_no_progress_callback
+        self._async_lag_callback: Optional[Callable[["NeptuneObject"], None]] = async_lag_callback
+        self._async_no_progress_callback: Optional[Callable[["NeptuneObject"], None]] = async_no_progress_callback
         self._callbacks_interval: float = callbacks_interval
         self._in_async: bool = in_async
 
         self._last_batch_started_at: Optional[float] = None
         self._last_no_progress_callback_at: Optional[float] = None
         self._last_lag_callback_at: Optional[float] = None
 
@@ -115,13 +115,13 @@
                 signal.accept(self)
             self._check_callbacks()
         except Empty:
             pass
 
 
 def execute_callback(
-    *, callback: Callable[["MetadataContainer"], None], container: "MetadataContainer", in_async: bool
+    *, callback: Callable[["NeptuneObject"], None], container: "NeptuneObject", in_async: bool
 ) -> None:
     if in_async:
         Thread(target=callback, name="CallbackExecution", args=(container,), daemon=True).start()
     else:
         callback(container)
```

### Comparing `neptune-1.9.1/src/neptune/internal/signals_processing/utils.py` & `neptune-2.0.0a0/src/neptune/internal/signals_processing/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 from queue import (
     Full,
     Queue,
 )
 from time import monotonic
 from typing import Optional
 
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
 from neptune.internal.signals_processing.signals import (
     BatchLagSignal,
     BatchProcessedSignal,
     BatchStartedSignal,
     Signal,
 )
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
 
 
 def signal(*, queue: "Queue[Signal]", obj: "Signal") -> None:
     try:
         queue.put_nowait(item=obj)
     except Full:
         warn_once("Signal queue is full. Some signals will be lost.", exception=NeptuneWarning)
```

### Comparing `neptune-1.9.1/src/neptune/internal/state.py` & `neptune-2.0.0a0/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/streams/__init__.py` & `neptune-2.0.0a0/src/neptune/core/components/queue/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `neptune-1.9.1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-2.0.0a0/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.streams.std_stream_capture_logger import (
     StderrCaptureLogger,
     StdoutCaptureLogger,
 )
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class StdoutCaptureBackgroundJob(BackgroundJob):
     def __init__(self, attribute_name: str):
         self._attribute_name = attribute_name
         self._logger = None
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         self._logger = StdoutCaptureLogger(container, self._attribute_name)
 
     def stop(self):
         self._logger.close()
 
     def pause(self):
         self._logger.pause()
@@ -52,15 +52,15 @@
 
 
 class StderrCaptureBackgroundJob(BackgroundJob):
     def __init__(self, attribute_name: str):
         self._attribute_name = attribute_name
         self._logger = None
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         self._logger = StderrCaptureLogger(container, self._attribute_name)
 
     def stop(self):
         self._logger.close()
 
     def pause(self):
         self._logger.pause()
```

### Comparing `neptune-1.9.1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-2.0.0a0/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 
 import sys
 import threading
 from queue import Queue
 from typing import TextIO
 
 from neptune.internal.threading.daemon import Daemon
-from neptune.logging import Logger as NeptuneLogger
-from neptune.metadata_containers import MetadataContainer
+from neptune.objects import NeptuneObject
 
 
 class StdStreamCaptureLogger:
-    def __init__(self, container: MetadataContainer, attribute_name: str, stream: TextIO):
-        self._logger = NeptuneLogger(container, attribute_name)
+    def __init__(self, container: NeptuneObject, attribute_name: str, stream: TextIO):
+        self._container = container
+        self._attribute_name = attribute_name
         self.stream = stream
         self._thread_local = threading.local()
         self.enabled = True
         self._log_data_queue = Queue()
         self._logging_thread = self.ReportingThread(self, "NeptuneThread_" + attribute_name)
         self._logging_thread.start()
 
+    def log_data(self, data):
+        self._container[self._attribute_name].append(data)
+
     def pause(self):
         self._log_data_queue.put_nowait(None)
         self._logging_thread.pause()
 
     def resume(self):
         self._logging_thread.resume()
 
@@ -63,28 +66,28 @@
 
         @Daemon.ConnectionRetryWrapper(kill_message="Killing Neptune STD capturing thread.")
         def work(self) -> None:
             while True:
                 data = self._logger._log_data_queue.get()
                 if data is None:
                     break
-                self._logger._logger.log(data)
+                self._logger.log_data(data)
 
 
 class StdoutCaptureLogger(StdStreamCaptureLogger):
-    def __init__(self, container: MetadataContainer, attribute_name: str):
+    def __init__(self, container: NeptuneObject, attribute_name: str):
         super().__init__(container, attribute_name, sys.stdout)
         sys.stdout = self
 
     def close(self):
         sys.stdout = self.stream
         super().close()
 
 
 class StderrCaptureLogger(StdStreamCaptureLogger):
-    def __init__(self, container: MetadataContainer, attribute_name: str):
+    def __init__(self, container: NeptuneObject, attribute_name: str):
         super().__init__(container, attribute_name, sys.stderr)
         sys.stderr = self
 
     def close(self, wait_for_all_logs=True):
         sys.stderr = self.stream
         super().close()
```

### Comparing `neptune-1.9.1/src/neptune/internal/threading/__init__.py` & `neptune-2.0.0a0/src/neptune/management/internal/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2021, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `neptune-1.9.1/src/neptune/internal/threading/daemon.py` & `neptune-2.0.0a0/src/neptune/internal/threading/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 __all__ = ["Daemon"]
 
 import abc
 import functools
 import threading
 from enum import Enum
 
-from neptune.common.exceptions import NeptuneConnectionLostException
+from neptune.internal.exceptions import NeptuneConnectionLostException
 from neptune.internal.utils.logger import get_logger
 
 logger = get_logger()
 
 
 class Daemon(threading.Thread):
     class DaemonState(Enum):
```

### Comparing `neptune-1.9.1/src/neptune/internal/types/file_types.py` & `neptune-2.0.0a0/src/neptune/internal/types/file_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from functools import wraps
 from io import IOBase
 from typing import (
     Optional,
     Union,
 )
 
-from neptune.common.exceptions import NeptuneException
 from neptune.exceptions import StreamAlreadyUsedException
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.utils import verify_type
 
 
 class FileType(enum.Enum):
     LOCAL_FILE = "LOCAL_FILE"
     IN_MEMORY = "IN_MEMORY"
     STREAM = "STREAM"
```

### Comparing `neptune-1.9.1/src/neptune/internal/types/stringify_value.py` & `neptune-2.0.0a0/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/types/utils.py` & `neptune-2.0.0a0/src/neptune/management/internal/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 #
-# Copyright (c) 2023, Neptune Labs Sp. z o.o.
+# Copyright (c) 2021, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__all__ = ["is_unsupported_float"]
+__all__ = (
+    "ProjectVisibility",
+    "ProjectMemberRole",
+    "MemberRole",
+    "WorkspaceMemberRole",
+)
 
-import math
 
+class ProjectVisibility:
+    PRIVATE = "priv"
+    PUBLIC = "pub"
+    WORKSPACE = "workspace"
 
-def is_unsupported_float(value: float) -> bool:
-    if isinstance(value, float):
-        return math.isinf(value) or math.isnan(value)
-    return False
+
+class ProjectMemberRole:
+    VIEWER = "viewer"
+    OWNER = "owner"
+    CONTRIBUTOR = "contributor"
+
+    # Deprecated
+    MEMBER = CONTRIBUTOR
+    MANAGER = OWNER
+
+
+MemberRole = ProjectMemberRole
+
+
+class WorkspaceMemberRole:
+    ADMIN = "admin"
+    MEMBER = "member"
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/__init__.py` & `neptune-2.0.0a0/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/dependency_tracking.py` & `neptune-2.0.0a0/src/neptune/internal/utils/dependency_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     from neptune import Run
 
 logger = get_logger()
 
 
 class DependencyTrackingStrategy(ABC):
     @abstractmethod
-    def log_dependencies(self, run: "Run") -> None:
-        ...
+    def log_dependencies(self, run: "Run") -> None: ...
 
 
 class InferDependenciesStrategy(DependencyTrackingStrategy):
     def log_dependencies(self, run: "Run") -> None:
         dependencies = []
 
         def sorting_key_func(d: Distribution) -> str:
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/deprecation.py` & `neptune-2.0.0a0/src/neptune/internal/utils/deprecation.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from functools import wraps
 from typing import Optional
 
-from neptune.common.warnings import warn_once
 from neptune.exceptions import NeptuneParametersCollision
+from neptune.internal.warnings import warn_once
 
 __all__ = ["deprecated", "deprecated_parameter"]
 
 
 def deprecated(*, alternative: Optional[str] = None):
     def deco(func):
         @wraps(func)
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/disk_utilization.py` & `neptune-2.0.0a0/src/neptune/internal/utils/disk_utilization.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     Callable,
     Optional,
 )
 
 import psutil
 from psutil import Error
 
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
 from neptune.constants import NEPTUNE_DATA_DIRECTORY
 from neptune.envs import (
     NEPTUNE_MAX_DISK_USAGE,
     NEPTUNE_RAISE_ERROR_ON_DISK_USAGE_EXCEEDED,
 )
 from neptune.exceptions import NeptuneMaxDiskUtilizationExceeded
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
 
 
 def get_neptune_data_directory() -> str:
     return os.getenv("NEPTUNE_DATA_DIRECTORY", NEPTUNE_DATA_DIRECTORY)
 
 
 def get_disk_utilization_percent(path: Optional[str] = None) -> Optional[float]:
@@ -82,28 +82,24 @@
     def __init__(self, max_disk_utilization: Optional[float], func: Callable[..., None], *args: Any, **kwargs: Any):
         self.max_disk_utilization = max_disk_utilization
         self.func = func
         self.args = args
         self.kwargs = kwargs
 
     @abstractmethod
-    def handle_limit_not_set(self) -> None:
-        ...  # pragma: no cover
+    def handle_limit_not_set(self) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    def handle_utilization_calculation_error(self) -> None:
-        ...  # pragma: no cover
+    def handle_utilization_calculation_error(self) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    def handle_limit_not_exceeded(self) -> None:
-        ...  # pragma: no cover
+    def handle_limit_not_exceeded(self) -> None: ...  # pragma: no cover
 
     @abstractmethod
-    def handle_limit_exceeded(self, current_utilization: float) -> None:
-        ...  # pragma: no cover
+    def handle_limit_exceeded(self, current_utilization: float) -> None: ...  # pragma: no cover
 
     def run(self) -> None:
         if not self.max_disk_utilization:
             return self.handle_limit_not_set()
 
         current_utilization = get_disk_utilization_percent()
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-2.0.0a0/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,50 +11,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["NoValue", "atomic_attribute_types_map", "map_attribute_result_to_value"]
 
-from neptune.internal.backends.api_model import AttributeType
+from neptune.api.models import FieldType
 
 
 class NoValue:
     pass
 
 
 VALUE = "value"
 LAST_VALUE = "last"
 VALUES = "values"
 
 atomic_attribute_types_map = {
-    AttributeType.FLOAT.value: "floatProperties",
-    AttributeType.INT.value: "intProperties",
-    AttributeType.BOOL.value: "boolProperties",
-    AttributeType.STRING.value: "stringProperties",
-    AttributeType.DATETIME.value: "datetimeProperties",
-    AttributeType.RUN_STATE.value: "experimentStateProperties",
-    AttributeType.NOTEBOOK_REF.value: "notebookRefProperties",
+    FieldType.FLOAT.value: "floatProperties",
+    FieldType.INT.value: "intProperties",
+    FieldType.BOOL.value: "boolProperties",
+    FieldType.STRING.value: "stringProperties",
+    FieldType.DATETIME.value: "datetimeProperties",
+    FieldType.OBJECT_STATE.value: "experimentStateProperties",
+    FieldType.NOTEBOOK_REF.value: "notebookRefProperties",
 }
 
 value_series_attribute_types_map = {
-    AttributeType.FLOAT_SERIES.value: "floatSeriesProperties",
-    AttributeType.STRING_SERIES.value: "stringSeriesProperties",
+    FieldType.FLOAT_SERIES.value: "floatSeriesProperties",
+    FieldType.STRING_SERIES.value: "stringSeriesProperties",
 }
 
 value_set_attribute_types_map = {
-    AttributeType.STRING_SET.value: "stringSetProperties",
+    FieldType.STRING_SET.value: "stringSetProperties",
 }
 
 # TODO: nicer mapping?
 _unmapped_attribute_types_map = {
-    AttributeType.FILE_SET.value: "fileSetProperties",  # TODO: return size?
-    AttributeType.FILE.value: "fileProperties",  # TODO: name? size?
-    AttributeType.IMAGE_SERIES.value: "imageSeriesProperties",  # TODO: return last step?
-    AttributeType.GIT_REF.value: "gitRefProperties",  # TODO: commit? branch?
+    FieldType.FILE_SET.value: "fileSetProperties",  # TODO: return size?
+    FieldType.FILE.value: "fileProperties",  # TODO: name? size?
+    FieldType.IMAGE_SERIES.value: "imageSeriesProperties",  # TODO: return last step?
+    FieldType.GIT_REF.value: "gitRefProperties",  # TODO: commit? branch?
 }
 
 
 def map_attribute_result_to_value(attribute):
     for attribute_map, value_key in [
         (atomic_attribute_types_map, VALUE),
         (value_series_attribute_types_map, LAST_VALUE),
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/git.py` & `neptune-2.0.0a0/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/hashing.py` & `neptune-2.0.0a0/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/images.py` & `neptune-2.0.0a0/src/neptune/internal/utils/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 __all__ = [
     "get_image_content",
     "get_html_content",
     "get_pickle_content",
     "is_numpy_array",
     "is_pil_image",
     "is_matplotlib_figure",
@@ -33,22 +35,24 @@
 import warnings
 from io import (
     BytesIO,
     StringIO,
 )
 from typing import Optional
 
+import numpy as np
 from packaging import version
 from pandas import DataFrame
 
 from neptune.exceptions import PlotlyIncompatibilityException
 from neptune.internal.utils.logger import get_logger
 
 logger = get_logger()
 SEABORN_GRID_CLASSES = {"FacetGrid", "PairGrid", "JointGrid"}
+ALLOWED_IMG_PIXEL_RANGES = ("[0, 255]", "[0.0, 1.0]")
 
 try:
     from numpy import array as numpy_array
     from numpy import ndarray as numpy_ndarray
     from numpy import uint8 as numpy_uint8
 except ImportError:
     numpy_ndarray = None
@@ -61,16 +65,16 @@
 except ImportError:
     PILImage = None
 
     def pilimage_fromarray():
         pass
 
 
-def get_image_content(image) -> Optional[bytes]:
-    content = _image_to_bytes(image)
+def get_image_content(image, autoscale=True) -> Optional[bytes]:
+    content = _image_to_bytes(image, autoscale)
 
     return content
 
 
 def get_html_content(chart) -> Optional[str]:
     content = _to_html(chart)
 
@@ -79,32 +83,32 @@
 
 def get_pickle_content(obj) -> Optional[bytes]:
     content = _export_pickle(obj)
 
     return content
 
 
-def _image_to_bytes(image) -> bytes:
+def _image_to_bytes(image, autoscale) -> bytes:
     if image is None:
         raise ValueError("image is None")
 
     elif is_numpy_array(image):
-        return _get_numpy_as_image(image)
+        return _get_numpy_as_image(image, autoscale)
 
     elif is_pil_image(image):
         return _get_pil_image_data(image)
 
     elif is_matplotlib_figure(image):
         return _get_figure_image_data(image)
 
     elif _is_torch_tensor(image):
-        return _get_numpy_as_image(image.detach().numpy())
+        return _get_numpy_as_image(image.detach().numpy(), autoscale)
 
     elif _is_tensorflow_tensor(image):
-        return _get_numpy_as_image(image.numpy())
+        return _get_numpy_as_image(image.numpy(), autoscale)
 
     elif is_seaborn_figure(image):
         return _get_figure_image_data(image.figure)
 
     raise TypeError("image is {}".format(type(image)))
 
 
@@ -192,46 +196,56 @@
 
 
 def _image_content_to_html(content: bytes) -> str:
     str_equivalent_image = base64.b64encode(content).decode()
     return "<img src='data:image/png;base64," + str_equivalent_image + "'/>"
 
 
-def _get_numpy_as_image(array):
+def _get_numpy_as_image(array: np.ndarray, autoscale: bool) -> bytes:
     array = array.copy()  # prevent original array from modifying
+    if autoscale:
+        array = _scale_array(array)
 
-    data_range_warnings = []
-    array_min = array.min()
-    array_max = array.max()
-    if array_min < 0:
-        data_range_warnings.append(f"the smallest value in the array is {array_min}")
-    if array_max > 1:
-        data_range_warnings.append(f"the largest value in the array is {array_max}")
-    if data_range_warnings:
-        data_range_warning_message = (" and ".join(data_range_warnings) + ".").capitalize()
-        logger.warning(
-            "%s To be interpreted as colors correctly values in the array need to be in the [0, 1] range.",
-            data_range_warning_message,
-        )
-    array *= 255
-    shape = array.shape
-    if len(shape) == 2:
+    if len(array.shape) == 2:
         return _get_pil_image_data(pilimage_fromarray(array.astype(numpy_uint8)))
-    if len(shape) == 3:
-        if shape[2] == 1:
+    if len(array.shape) == 3:
+        if array.shape[2] == 1:
             array2d = numpy_array([[col[0] for col in row] for row in array])
             return _get_pil_image_data(pilimage_fromarray(array2d.astype(numpy_uint8)))
-        if shape[2] in (3, 4):
+        if array.shape[2] in (3, 4):
             return _get_pil_image_data(pilimage_fromarray(array.astype(numpy_uint8)))
     raise ValueError(
         "Incorrect size of numpy.ndarray. Should be 2-dimensional or"
         "3-dimensional with 3rd dimension of size 1, 3 or 4."
     )
 
 
+def _scale_array(array: np.ndarray) -> np.ndarray:
+    array_min = array.min()
+    array_max = array.max()
+
+    if array_min >= 0 and 1 < array_max <= 255:
+        return array
+
+    if array_min >= 0 and array_max <= 1:
+        return array * 255
+
+    _warn_about_incorrect_image_data_range(array_min, array_max)
+    return array
+
+
+def _warn_about_incorrect_image_data_range(array_min: int | float, array_max: int | float) -> None:
+    msg = f"Image data is in range [{array_min}, {array_max}]."
+    logger.warning(
+        "%s To be interpreted as colors correctly values in the array need to be in the %s or %s range.",
+        msg,
+        *ALLOWED_IMG_PIXEL_RANGES,
+    )
+
+
 def _get_pil_image_data(image: PILImage) -> bytes:
     with io.BytesIO() as image_buffer:
         image.save(image_buffer, format="PNG")
         return image_buffer.getvalue()
 
 
 def _get_figure_image_data(figure) -> bytes:
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/iteration.py` & `neptune-2.0.0a0/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/limits.py` & `neptune-2.0.0a0/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/logger.py` & `neptune-2.0.0a0/src/neptune/internal/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["get_logger", "NEPTUNE_LOGGER_NAME"]
+__all__ = ["get_logger", "get_disabled_logger", "NEPTUNE_LOGGER_NAME"]
 
 import logging
 import sys
 
 NEPTUNE_LOGGER_NAME = "neptune"
 NEPTUNE_NO_PREFIX_LOGGER_NAME = "neptune_no_prefix"
+NEPTUNE_NOOP_LOGGER_NAME = "neptune_noop"
 LOG_FORMAT = "[%(name)s] [%(levelname)s] %(message)s"
 NO_PREFIX_FORMAT = "%(message)s"
 
 
 class CustomFormatter(logging.Formatter):
     def format(self, record):
         record.levelname = record.levelname.lower().ljust(len("warning"))
@@ -32,50 +33,63 @@
 
 
 class GrabbableStdoutHandler(logging.StreamHandler):
     """
     This class is like a StreamHandler using sys.stdout, but always uses
     whatever sys.stdout is currently set to rather than the value of
     sys.stderr at handler construction time.
-    This enables neptune-client to capture stdout regardless
+    This enables Neptune to capture stdout regardless
     of logging configuration time.
     Based on logging._StderrHandler from standard library.
     """
 
     def __init__(self, level=logging.NOTSET):
         logging.Handler.__init__(self, level)
 
     @property
     def stream(self):
         return sys.stdout
 
 
-def get_logger(with_prefix: bool = True):
-    if with_prefix:
-        return logging.getLogger(NEPTUNE_LOGGER_NAME)
-    return logging.getLogger(NEPTUNE_NO_PREFIX_LOGGER_NAME)
+def get_logger(with_prefix: bool = True) -> logging.Logger:
+    name = NEPTUNE_LOGGER_NAME if with_prefix else NEPTUNE_NO_PREFIX_LOGGER_NAME
+
+    return logging.getLogger(name)
+
+
+def get_disabled_logger() -> logging.Logger:
+    return logging.getLogger(NEPTUNE_NOOP_LOGGER_NAME)
 
 
 def _set_up_logging():
     # setup neptune logger so that logging.getLogger(NEPTUNE_LOGGER_NAME)
     # returns configured logger
     neptune_logger = logging.getLogger(NEPTUNE_LOGGER_NAME)
     neptune_logger.propagate = False
-    neptune_logger.setLevel(logging.DEBUG)
 
     stdout_handler = GrabbableStdoutHandler()
     stdout_handler.setFormatter(CustomFormatter())
     neptune_logger.addHandler(stdout_handler)
 
+    neptune_logger.setLevel(logging.INFO)
+
 
 def _set_up_no_prefix_logging():
     neptune_logger = logging.getLogger(NEPTUNE_NO_PREFIX_LOGGER_NAME)
     neptune_logger.propagate = False
-    neptune_logger.setLevel(logging.DEBUG)
 
     stdout_handler = GrabbableStdoutHandler()
     stdout_handler.setFormatter(logging.Formatter(NO_PREFIX_FORMAT))
     neptune_logger.addHandler(stdout_handler)
 
+    neptune_logger.setLevel(logging.INFO)
+
+
+def _set_up_disabled_logging():
+    neptune_logger = logging.getLogger(NEPTUNE_NOOP_LOGGER_NAME)
+
+    neptune_logger.setLevel(logging.CRITICAL)
+
 
 _set_up_logging()
 _set_up_no_prefix_logging()
+_set_up_disabled_logging()
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/paths.py` & `neptune-2.0.0a0/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/ping_background_job.py` & `neptune-2.0.0a0/src/neptune/internal/utils/ping_background_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 )
 
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.threading.daemon import Daemon
 from neptune.internal.utils.logger import get_logger
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 _logger = get_logger()
 
 
 class PingBackgroundJob(BackgroundJob):
     def __init__(self, period: float = 10):
         self._period = period
         self._thread: PingBackgroundJob.ReportingThread = None
         self._started = False
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         self._thread = self.ReportingThread(self._period, container)
         self._thread.start()
         self._started = True
 
     def stop(self):
         if not self._started:
             return
@@ -54,15 +54,15 @@
 
     def join(self, seconds: Optional[float] = None):
         if not self._started:
             return
         self._thread.join(seconds)
 
     class ReportingThread(Daemon):
-        def __init__(self, period: float, container: "MetadataContainer"):
+        def __init__(self, period: float, container: "NeptuneObject"):
             super().__init__(sleep_time=period, name="NeptunePing")
             self._container = container
 
         @Daemon.ConnectionRetryWrapper(
             kill_message=(
                 "Killing Neptune ping thread. Your run's status will not be updated and"
                 " the run will be shown as inactive."
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/process_killer.py` & `neptune-2.0.0a0/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/run_state.py` & `neptune-2.0.0a0/src/neptune/internal/utils/run_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["RunState"]
 
 import enum
 
-from neptune.common.exceptions import NeptuneException
+from neptune.internal.exceptions import NeptuneException
 
 
 class RunState(enum.Enum):
     active = "Active"
     inactive = "Inactive"
 
     _api_active = "running"
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/runningmode.py` & `neptune-2.0.0a0/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/s3.py` & `neptune-2.0.0a0/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/utils/source_code.py` & `neptune-2.0.0a0/src/neptune/internal/utils/source_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 from typing import (
     TYPE_CHECKING,
     List,
     Optional,
 )
 
 from neptune.attributes import constants as attr_consts
-from neptune.common.storage.storage_utils import normalize_file_name
-from neptune.common.utils import is_ipython
+from neptune.internal.storage import normalize_file_name
 from neptune.internal.utils import (
     does_paths_share_common_drive,
     get_absolute_paths,
     get_common_root,
 )
+from neptune.internal.utils.utils import is_ipython
 from neptune.vendor.lib_programname import (
     empty_path,
     get_path_executed_script,
 )
 
 if TYPE_CHECKING:
     from neptune import Run
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/traceback_job.py` & `neptune-2.0.0a0/src/neptune/internal/utils/traceback_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 
 from neptune.attributes.constants import SYSTEM_FAILED_ATTRIBUTE_PATH
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.utils.logger import get_logger
 from neptune.internal.utils.uncaught_exception_handler import instance as traceback_handler
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 _logger = get_logger()
 
 
 class TracebackJob(BackgroundJob):
     def __init__(self, path: str, fail_on_exception: bool = True):
         self._uuid = uuid.uuid4()
         self._started = False
         self._path = path
         self._fail_on_exception = fail_on_exception
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         if not self._started:
             path = self._path
             fail_on_exception = self._fail_on_exception
 
             def log_traceback(stacktrace_lines: List[str]):
                 container[path].log(stacktrace_lines)
                 if fail_on_exception:
```

### Comparing `neptune-1.9.1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-2.0.0a0/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-2.0.0a0/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 from neptune.types.series.file_series import FileSeries
 from neptune.types.series.float_series import FloatSeries
 from neptune.types.series.string_series import StringSeries
 from neptune.types.sets.string_set import StringSet
 from neptune.types.value_visitor import ValueVisitor
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 
 class ValueToAttributeVisitor(ValueVisitor[Attribute]):
-    def __init__(self, container: "MetadataContainer", path: List[str]):
+    def __init__(self, container: "NeptuneObject", path: List[str]):
         self._container = container
         self._path = path
 
     def visit_float(self, _: Float) -> Attribute:
         return FloatAttr(self._container, self._path)
 
     def visit_integer(self, _: Integer) -> Attribute:
```

### Comparing `neptune-1.9.1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-2.0.0a0/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,34 +26,34 @@
 from websocket import WebSocketConnectionClosedException
 
 from neptune.attributes.constants import (
     SIGNAL_TYPE_ABORT,
     SIGNAL_TYPE_STOP,
     SYSTEM_FAILED_ATTRIBUTE_PATH,
 )
-from neptune.common.websockets.reconnecting_websocket import ReconnectingWebsocket
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.threading.daemon import Daemon
 from neptune.internal.utils import process_killer
 from neptune.internal.utils.logger import get_logger
+from neptune.internal.websockets.reconnecting_websocket import ReconnectingWebsocket
 from neptune.internal.websockets.websockets_factory import WebsocketsFactory
 
 if TYPE_CHECKING:
-    from neptune.metadata_containers import MetadataContainer
+    from neptune.objects import NeptuneObject
 
 logger = get_logger()
 
 
 class WebsocketSignalsBackgroundJob(BackgroundJob):
     def __init__(self, ws_factory: WebsocketsFactory):
         self._ws_factory = ws_factory
         self._thread: "Optional[WebsocketSignalsBackgroundJob._ListenerThread]" = None
         self._started = False
 
-    def start(self, container: "MetadataContainer"):
+    def start(self, container: "NeptuneObject"):
         self._thread = self._ListenerThread(container, self._ws_factory.create())
         self._thread.start()
         self._started = True
 
     def stop(self):
         if not self._started:
             return
@@ -70,15 +70,15 @@
         if not self._started or threading.get_ident() == self._thread.ident:
             return
         self._thread.join(seconds)
         # Just in case. There is possible race condition when connection can be reestablished after being shutdown.
         self._thread.shutdown_ws_client()
 
     class _ListenerThread(Daemon):
-        def __init__(self, container: "MetadataContainer", ws_client: ReconnectingWebsocket):
+        def __init__(self, container: "NeptuneObject", ws_client: ReconnectingWebsocket):
             super().__init__(sleep_time=0, name="NeptuneWebhooks")
             self._container = container
             self._ws_client = ws_client
 
         def work(self) -> None:
             try:
                 raw_message = self._ws_client.recv()
```

### Comparing `neptune-1.9.1/src/neptune/internal/websockets/websockets_factory.py` & `neptune-2.0.0a0/src/neptune/internal/websockets/websockets_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 __all__ = ["WebsocketsFactory"]
 
 import threading
 from typing import Optional
 
 from requests_oauthlib import OAuth2Session
 
-from neptune.common.websockets.reconnecting_websocket import ReconnectingWebsocket
+from neptune.internal.websockets.reconnecting_websocket import ReconnectingWebsocket
 
 
 class WebsocketsFactory:
     def __init__(self, url: str, session: OAuth2Session, proxies: Optional[dict] = None):
         self._url = url
         self._session = session
         self._proxies = proxies
```

### Comparing `neptune-1.9.1/src/neptune/legacy/checkpoint.py` & `neptune-2.0.0a0/src/neptune/types/series/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+__all__ = [
+    "FileSeries",
+    "FloatSeries",
+    "StringSeries",
+]
 
-class Checkpoint(object):
-    def __init__(self, _id, name, path):
-        self.id = _id
-        self.name = name
-        self.path = path
+from .file_series import FileSeries
+from .float_series import FloatSeries
+from .string_series import StringSeries
```

### Comparing `neptune-1.9.1/src/neptune/legacy/constants.py` & `neptune-2.0.0a0/src/neptune/types/value.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 #
-# Copyright (c) 2020, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["Value"]
 
-"""Constants used by Neptune"""
+import abc
+from typing import (
+    TYPE_CHECKING,
+    TypeVar,
+)
 
-ANONYMOUS = "ANONYMOUS"
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
 
-ANONYMOUS_API_TOKEN = (
-    "eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vdWkubmVwdHVuZS5haSIsImFwaV91cmwiOiJodHRwczovL3VpLm5lcHR1bmUuYW"
-    "kiLCJhcGlfa2V5IjoiYjcwNmJjOGYtNzZmOS00YzJlLTkzOWQtNGJhMDM2ZjkzMmU0In0="
-)
+Ret = TypeVar("Ret")
+
+
+class Value:
+    @abc.abstractmethod
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        pass
```

### Comparing `neptune-1.9.1/src/neptune/legacy/git_info.py` & `neptune-2.0.0a0/src/neptune/integrations/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["GitInfo"]
+__all__ = ["join_paths", "verify_type", "RunType"]
 
-from neptune.common.git_info import GitInfo
+from typing import Union
+
+from neptune import Run
+from neptune.handler import Handler
+from neptune.internal.utils import verify_type
+from neptune.internal.utils.paths import join_paths
+
+RunType = Union[Run, Handler]
```

### Comparing `neptune-1.9.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune-2.0.0a0/src/neptune/integrations/sklearn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from neptune.internal.utils.requirement_check import require_installed
 
-from neptune.legacy.internal.api_clients import HostedNeptuneBackendApiClient
+require_installed("neptune-sklearn", suggestion="sklearn")
 
-# define deprecated HostedNeptuneBackend class
-HostedNeptuneBackend = HostedNeptuneBackendApiClient
+from neptune_sklearn.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune-2.0.0a0/src/neptune/types/atoms/artifact.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import threading
+__all__ = ["Artifact"]
 
-import six
+from dataclasses import dataclass
+from typing import (
+    TYPE_CHECKING,
+    Optional,
+    TypeVar,
+    Union,
+)
 
+from neptune.internal.artifacts.file_hasher import FileHasher
+from neptune.internal.types.stringify_value import (
+    StringifyValue,
+    extract_if_stringify_value,
+)
+from neptune.types.atoms.atom import Atom
 
-class NeptuneThread(threading.Thread):
-    def __init__(self, is_daemon):
-        super(NeptuneThread, self).__init__(target=self.run)
-        self.daemon = is_daemon
-        self._interrupted = threading.Event()
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
 
-    def should_continue_running(self):
-        if six.PY2:
-            all_threads = threading.enumerate()
+Ret = TypeVar("Ret")
 
-            main_thread_is_alive = any(t.__class__ is threading._MainThread and t.is_alive() for t in all_threads)
-        else:
-            main_thread_is_alive = threading.main_thread().is_alive()
 
-        return not self._interrupted.is_set() and main_thread_is_alive
+@dataclass
+class Artifact(Atom):
 
-    def interrupt(self):
-        self._interrupted.set()
+    hash: str
 
-    def run(self):
-        raise NotImplementedError()
+    def __init__(self, value: Union[Optional[str], StringifyValue] = None):
+        value = extract_if_stringify_value(value)
+
+        self.hash = str(value)
+        assert (
+            len(self.hash) == FileHasher.HASH_LENGTH or value is None
+        ), "Expected sha-256 string. E.g. 'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'"
+
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        return visitor.visit_artifact(self)
+
+    def __str__(self):
+        return "Artifact({})".format(self.hash)
```

### Comparing `neptune-1.9.1/src/neptune/legacy/internal/utils/deprecation.py` & `neptune-2.0.0a0/src/neptune/types/mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from functools import wraps
+__all__ = ["Mode"]
 
-from neptune.common.warnings import warn_once
+from enum import Enum
 
 
-def legacy_client_deprecation(func):
-    @wraps(func)
-    def inner(*args, **kwargs):
-        warn_once(
-            message="You're using a legacy version of Neptune client."
-            " It will be moved to `neptune.legacy` as of `neptune-client==1.0.0`."
-        )
-        return func(*args, **kwargs)
+class Mode(str, Enum):
+    OFFLINE = "offline"
+    DEBUG = "debug"
+    ASYNC = "async"
+    SYNC = "sync"
+    READ_ONLY = "read-only"
 
-    return inner
+    def __repr__(self):
+        return f'"{self.value}"'
```

### Comparing `neptune-1.9.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune-2.0.0a0/src/neptune/types/atoms/boolean.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,48 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["Boolean"]
 
-from neptune.common.websockets.reconnecting_websocket import ReconnectingWebsocket
+from dataclasses import dataclass
+from typing import (
+    TYPE_CHECKING,
+    TypeVar,
+)
 
+from neptune.internal.types.stringify_value import extract_if_stringify_value
+from neptune.types.atoms.atom import Atom
 
-class ReconnectingWebsocketFactory(object):
-    def __init__(self, backend, url):
-        self._backend = backend
-        self._url = url
-
-    def create(self, shutdown_condition):
-        return ReconnectingWebsocket(
-            url=self._url,
-            oauth2_session=self._backend.authenticator.auth.session,
-            shutdown_event=shutdown_condition,
-            proxies=self._backend.proxies,
-        )
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
+
+Ret = TypeVar("Ret")
+
+
+@dataclass
+class Boolean(Atom):
+
+    value: bool
+
+    def __init__(self, value):
+        self.value = bool(extract_if_stringify_value(value))
+
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        return visitor.visit_boolean(self)
+
+    def __str__(self):
+        return "Boolean({})".format(str(self.value))
+
+    def __bool__(self):
+        return self.value
```

### Comparing `neptune-1.9.1/src/neptune/legacy/oauth.py` & `neptune-2.0.0a0/src/neptune/integrations/xgboost/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# flake8: noqa
-from neptune.common.oauth import (
-    NeptuneAuth,
-    NeptuneAuthenticator,
-)
+from neptune.internal.utils.requirement_check import require_installed
+
+require_installed("neptune-xgboost", suggestion="xgboost")
+
+from neptune_xgboost.impl import *  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/legacy/patterns.py` & `neptune-2.0.0a0/src/neptune/types/atoms/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,9 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# flake8: noqa
-from neptune.common.patterns import PROJECT_QUALIFIED_NAME_PATTERN
+__all__ = ["Artifact", "Boolean", "Datetime", "File", "Float", "GitRef", "Integer", "String"]
+
+from .artifact import Artifact
+from .boolean import Boolean
+from .datetime import Datetime
+from .file import File
+from .float import Float
+from .git_ref import GitRef
+from .integer import Integer
+from .string import String
```

### Comparing `neptune-1.9.1/src/neptune/legacy/projects.py` & `neptune-2.0.0a0/src/neptune/objects/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,596 +1,591 @@
 #
-# Copyright (c) 2019, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["Run"]
 
-import atexit
-import logging
 import os
-import os.path
 import threading
 from platform import node as get_hostname
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
-import click
-import pandas as pd
-import six
-
-from neptune.common.utils import (
-    as_list,
-    discover_git_repo_location,
-    get_git_info,
-    map_keys,
-)
-from neptune.legacy.envs import (
-    NOTEBOOK_ID_ENV_NAME,
-    NOTEBOOK_PATH_ENV_NAME,
-)
-from neptune.legacy.exceptions import NeptuneNoExperimentContextException
-from neptune.legacy.experiments import Experiment
-from neptune.legacy.internal.abort import DefaultAbortImpl
-from neptune.legacy.internal.notebooks.notebooks import create_checkpoint
-from neptune.legacy.internal.utils.deprecation import legacy_client_deprecation
-from neptune.legacy.internal.utils.source_code import get_source_code_to_upload
-
-_logger = logging.getLogger(__name__)
+from typing_extensions import Literal
 
+from neptune.attributes.constants import (
+    SYSTEM_DESCRIPTION_ATTRIBUTE_PATH,
+    SYSTEM_FAILED_ATTRIBUTE_PATH,
+    SYSTEM_HOSTNAME_ATTRIBUTE_PATH,
+    SYSTEM_NAME_ATTRIBUTE_PATH,
+    SYSTEM_TAGS_ATTRIBUTE_PATH,
+)
+from neptune.envs import (
+    CONNECTION_MODE,
+    CUSTOM_RUN_ID_ENV_NAME,
+    MONITORING_NAMESPACE,
+    NEPTUNE_NOTEBOOK_ID,
+    NEPTUNE_NOTEBOOK_PATH,
+)
+from neptune.exceptions import (
+    InactiveRunException,
+    NeedExistingRunForReadOnlyMode,
+    NeptuneRunResumeAndCustomIdCollision,
+)
+from neptune.internal.backends.api_model import ApiExperiment
+from neptune.internal.backends.neptune_backend import NeptuneBackend
+from neptune.internal.container_type import ContainerType
+from neptune.internal.hardware.hardware_metric_reporting_job import HardwareMetricReportingJob
+from neptune.internal.id_formats import QualifiedName
+from neptune.internal.init.parameters import (
+    ASYNC_LAG_THRESHOLD,
+    ASYNC_NO_PROGRESS_THRESHOLD,
+    DEFAULT_FLUSH_PERIOD,
+    DEFAULT_NAME,
+    OFFLINE_PROJECT_QUALIFIED_NAME,
+)
+from neptune.internal.notebooks.notebooks import create_checkpoint
+from neptune.internal.state import ContainerState
+from neptune.internal.streams.std_capture_background_job import (
+    StderrCaptureBackgroundJob,
+    StdoutCaptureBackgroundJob,
+)
+from neptune.internal.utils import (
+    verify_collection_type,
+    verify_type,
+)
+from neptune.internal.utils.dependency_tracking import (
+    FileDependenciesStrategy,
+    InferDependenciesStrategy,
+)
+from neptune.internal.utils.git import (
+    to_git_info,
+    track_uncommitted_changes,
+)
+from neptune.internal.utils.hashing import generate_hash
+from neptune.internal.utils.limits import custom_run_id_exceeds_length
+from neptune.internal.utils.ping_background_job import PingBackgroundJob
+from neptune.internal.utils.runningmode import (
+    in_interactive,
+    in_notebook,
+)
+from neptune.internal.utils.source_code import upload_source_code
+from neptune.internal.utils.traceback_job import TracebackJob
+from neptune.internal.warnings import (
+    NeptuneWarning,
+    warn_once,
+)
+from neptune.internal.websockets.websocket_signals_background_job import WebsocketSignalsBackgroundJob
+from neptune.objects.abstract import NeptuneObjectCallback
+from neptune.objects.neptune_object import NeptuneObject
+from neptune.types import (
+    GitRef,
+    StringSeries,
+)
+from neptune.types.atoms.git_ref import GitRefDisabled
+from neptune.types.mode import Mode
 
-class Project(object):
-    """A class for storing information and managing Neptune project.
+if TYPE_CHECKING:
+    from neptune.internal.background_job import BackgroundJob
 
-    Args:
-        backend (:class:`~neptune.ApiClient`, required): A ApiClient object.
-        internal_id (:obj:`str`, required): ID of the project.
-        namespace (:obj:`str`, required): It can either be your workspace or user name.
-        name (:obj:`str`, required): project name.
 
-    Note:
-        ``namespace`` and ``name`` joined together with ``/`` form ``project_qualified_name``.
-    """
+T = TypeVar("T")
 
-    @legacy_client_deprecation
-    def __init__(self, backend, internal_id, namespace, name):
-        self._backend = backend
-        self.internal_id = internal_id
-        self.namespace = namespace
-        self.name = name
-
-        self._experiments_stack = []
-        self.__lock = threading.RLock()
-        atexit.register(self._shutdown_hook)
-
-    def get_members(self):
-        """Retrieve a list of project members.
-
-        Returns:
-            :obj:`list` of :obj:`str` - A list of usernames of project members.
-
-        Examples:
-
-            .. code:: python3
-
-                project = session.get_projects('neptune-ai')['neptune-ai/Salt-Detection']
-                project.get_members()
-
-        """
-        project_members = self._backend.get_project_members(self.internal_id)
-        return [member.registeredMemberInfo.username for member in project_members if member.registeredMemberInfo]
-
-    def get_experiments(self, id=None, state=None, owner=None, tag=None, min_running_time=None):
-        """Retrieve list of experiments matching the specified criteria.
-
-        All parameters are optional, each of them specifies a single criterion.
-        Only experiments matching all of the criteria will be returned.
-
-        Args:
-            id (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | An experiment id like ``'SAN-1'`` or list of ids like ``['SAN-1', 'SAN-2']``.
-                | Matching any element of the list is sufficient to pass criterion.
-            state (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | An experiment state like ``'succeeded'`` or list of states like ``['succeeded', 'running']``.
-                | Possible values: ``'running'``, ``'succeeded'``, ``'failed'``, ``'aborted'``.
-                | Matching any element of the list is sufficient to pass criterion.
-            owner (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | *Username* of the experiment owner (User who created experiment is an owner) like ``'josh'``
-                  or list of owners like ``['frederic', 'josh']``.
-                | Matching any element of the list is sufficient to pass criterion.
-            tag (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                 | An experiment tag like ``'lightGBM'`` or list of tags like ``['pytorch', 'cycleLR']``.
-                 | Only experiments that have all specified tags will match this criterion.
-            min_running_time (:obj:`int`, optional, default is ``None``):
-                Minimum running time of an experiment in seconds, like ``2000``.
-
-        Returns:
-            :obj:`list` of :class:`~neptune.experiments.Experiment` objects.
-
-        Examples:
-
-            .. code:: python3
-
-                # Fetch a project
-                project = session.get_projects('neptune-ai')['neptune-ai/Salt-Detection']
-
-                # Get list of experiments
-                project.get_experiments(state=['aborted'], owner=['neyo'], min_running_time=100000)
-
-                # Example output:
-                # [Experiment(SAL-1609),
-                #  Experiment(SAL-1765),
-                #  Experiment(SAL-1941),
-                #  Experiment(SAL-1960),
-                #  Experiment(SAL-2025)]
-        """
-        leaderboard_entries = self._fetch_leaderboard(id, state, owner, tag, min_running_time)
-        return [Experiment(self._backend, self, entry.id, entry.internal_id) for entry in leaderboard_entries]
-
-    def get_leaderboard(self, id=None, state=None, owner=None, tag=None, min_running_time=None):
-        """Fetch Neptune experiments view as pandas ``DataFrame``.
-
-        **returned DataFrame**
-
-        | In the returned ``DataFrame`` each *row* is an experiment and *columns* represent all system properties,
-          numeric and text logs, parameters and properties in these experiments.
-        | Note that, returned ``DataFrame`` does not contain all columns across the entire project.
-        | Some columns may be empty, since experiments may define various logs, properties, etc.
-        | For each log at most one (the last one) value is returned per experiment.
-        | Text values are trimmed to 255 characters.
-
-        **about parameters**
-
-        All parameters are optional, each of them specifies a single criterion.
-        Only experiments matching all of the criteria will be returned.
-
-        Args:
-            id (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | An experiment id like ``'SAN-1'`` or list of ids like ``['SAN-1', 'SAN-2']``.
-                | Matching any element of the list is sufficient to pass criterion.
-            state (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | An experiment state like ``'succeeded'`` or list of states like ``['succeeded', 'running']``.
-                | Possible values: ``'running'``, ``'succeeded'``, ``'failed'``, ``'aborted'``.
-                | Matching any element of the list is sufficient to pass criterion.
-            owner (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | *Username* of the experiment owner (User who created experiment is an owner) like ``'josh'``
-                  or list of owners like ``['frederic', 'josh']``.
-                | Matching any element of the list is sufficient to pass criterion.
-            tag (:obj:`str` or :obj:`list` of :obj:`str`, optional, default is ``None``):
-                | An experiment tag like ``'lightGBM'`` or list of tags like ``['pytorch', 'cycleLR']``.
-                | Only experiments that have all specified tags will match this criterion.
-            min_running_time (:obj:`int`, optional, default is ``None``):
-                Minimum running time of an experiment in seconds, like ``2000``.
-
-        Returns:
-            :obj:`pandas.DataFrame` - Fetched Neptune experiments view.
-
-        Examples:
-
-            .. code:: python3
-
-                # Fetch a project.
-                project = session.get_projects('neptune-ai')['neptune-ai/Salt-Detection']
-
-                # Get DataFrame that resembles experiment view.
-                project.get_leaderboard(state=['aborted'], owner=['neyo'], min_running_time=100000)
-        """
-
-        leaderboard_entries = self._fetch_leaderboard(id, state, owner, tag, min_running_time)
-
-        def make_row(entry):
-            channels = dict(("channel_{}".format(ch.name), ch.trimmed_y) for ch in entry.channels)
-
-            parameters = map_keys("parameter_{}".format, entry.parameters)
-            properties = map_keys("property_{}".format, entry.properties)
-
-            r = {}
-            r.update(entry.system_properties)
-            r.update(channels)
-            r.update(parameters)
-            r.update(properties)
-            return r
-
-        rows = ((n, make_row(e)) for (n, e) in enumerate(leaderboard_entries))
-
-        df = pd.DataFrame.from_dict(data=dict(rows), orient="index")
-        df = df.reindex(self._sort_leaderboard_columns(df.columns), axis="columns")
-        return df
 
-    def create_experiment(
-        self,
-        name=None,
-        description=None,
-        params=None,
-        properties=None,
-        tags=None,
-        upload_source_files=None,
-        abort_callback=None,
-        logger=None,
-        upload_stdout=True,
-        upload_stderr=True,
-        send_hardware_metrics=True,
-        run_monitoring_thread=True,
-        handle_uncaught_exceptions=True,
-        git_info=None,
-        hostname=None,
-        notebook_id=None,
-        notebook_path=None,
-    ):
-        """Create and start Neptune experiment.
+def temporarily_disabled(func: Callable[..., T]) -> Callable[..., T]:
+    def wrapper(*_, **__):
+        if func.__name__ == "_get_background_jobs":
+            return []
+        elif func.__name__ == "_write_initial_attributes":
+            return None
+        elif func.__name__ == "_write_initial_monitoring_attributes":
+            return None
 
-        Create experiment, set its status to `running` and append it to the top of the experiments view.
-        All parameters are optional, hence minimal invocation: ``neptune.create_experiment()``.
+    return wrapper
 
-        Args:
-            name (:obj:`str`, optional, default is ``'Untitled'``):
-                Editable name of the experiment.
-                Name is displayed in the experiment's `Details` (`Metadata` section)
-                and in `experiments view` as a column.
-
-            description (:obj:`str`, optional, default is ``''``):
-                Editable description of the experiment.
-                Description is displayed in the experiment's `Details` (`Metadata` section)
-                and can be displayed in the `experiments view` as a column.
-
-            params (:obj:`dict`, optional, default is ``{}``):
-                Parameters of the experiment.
-                After experiment creation ``params`` are read-only
-                (see: :meth:`~neptune.experiments.Experiment.get_parameters`).
-                Parameters are displayed in the experiment's `Details` (`Parameters` section)
-                and each key-value pair can be viewed in `experiments view` as a column.
-
-            properties (:obj:`dict`, optional, default is ``{}``):
-                Properties of the experiment.
-                They are editable after experiment is created.
-                Properties are displayed in the experiment's `Details` (`Properties` section)
-                and each key-value pair can be viewed in `experiments view` as a column.
-
-            tags (:obj:`list`, optional, default is ``[]``):
-                Must be list of :obj:`str`. Tags of the experiment.
-                They are editable after experiment is created
-                (see: :meth:`~neptune.experiments.Experiment.append_tag`
-                and :meth:`~neptune.experiments.Experiment.remove_tag`).
-                Tags are displayed in the experiment's `Details` (`Metadata` section)
-                and can be viewed in `experiments view` as a column.
-
-            upload_source_files (:obj:`list` or :obj:`str`, optional, default is ``None``):
-                List of source files to be uploaded. Must be list of :obj:`str` or single :obj:`str`.
-                Uploaded sources are displayed in the experiment's `Source code` tab.
-
-                | If ``None`` is passed, Python file from which experiment was created will be uploaded.
-                | Pass empty list (``[]``) to upload no files.
-                | Unix style pathname pattern expansion is supported. For example, you can pass ``'*.py'`` to upload
-                  all python source files from the current directory.
-                  For Python 3.5 or later, paths of uploaded files on server are resolved as relative to the
-                | calculated common root of all uploaded source  files. For older Python versions, paths on server are
-                | resolved always as relative to the current directory.
-                  For recursion lookup use ``'**/*.py'`` (for Python 3.5 and later).
-                  For more information see `glob library <https://docs.python.org/3/library/glob.html>`_.
-
-            abort_callback (:obj:`callable`, optional, default is ``None``):
-                Callback that defines how `abort experiment` action in the Web application should work.
-                Actual behavior depends on your setup:
-
-                    * (default) If ``abort_callback=None`` and `psutil <https://psutil.readthedocs.io/en/latest/>`_
-                      is installed, then current process and it's children are aborted by sending `SIGTERM`.
-                      If, after grace period, processes are not terminated, `SIGKILL` is sent.
-                    * If ``abort_callback=None`` and `psutil <https://psutil.readthedocs.io/en/latest/>`_
-                      is **not** installed, then `abort experiment` action just marks experiment as *aborted*
-                      in the Web application. No action is performed on the current process.
-                    * If ``abort_callback=callable``, then ``callable`` is executed when `abort experiment` action
-                      in the Web application is triggered.
-
-            logger (:obj:`logging.Logger` or `None`, optional, default is ``None``):
-                If Python's `Logger <https://docs.python.org/3/library/logging.html#logging.Logger>`_
-                is passed, new experiment's `text log`
-                (see: :meth:`~neptune.experiments.Experiment.log_text`) with name `"logger"` is created.
-                Each time `Python logger` logs new data, it is automatically sent to the `"logger"` in experiment.
-                As a results all data from `Python logger` are in the `Logs` tab in the experiment.
-
-            upload_stdout (:obj:`Boolean`, optional, default is ``True``):
-                Whether to send stdout to experiment's *Monitoring*.
-
-            upload_stderr (:obj:`Boolean`, optional, default is ``True``):
-                Whether to send stderr to experiment's *Monitoring*.
-
-            send_hardware_metrics (:obj:`Boolean`, optional, default is ``True``):
-                Whether to send hardware monitoring logs (CPU, GPU, Memory utilization) to experiment's *Monitoring*.
-
-            run_monitoring_thread (:obj:`Boolean`, optional, default is ``True``):
-                Whether to run thread that pings Neptune server in order to determine if experiment is responsive.
-
-            handle_uncaught_exceptions (:obj:`Boolean`, optional, default is ``True``):
-                Two options ``True`` and ``False`` are possible:
-
-                    * If set to ``True`` and uncaught exception occurs, then Neptune automatically place
-                      `Traceback` in the experiment's `Details` and change experiment status to `Failed`.
-                    * If set to ``False`` and uncaught exception occurs, then no action is performed
-                      in the Web application. As a consequence, experiment's status is `running` or `not responding`.
-
-            git_info (:class:`~neptune.git_info.GitInfo`, optional, default is ``None``):
-
-                | Instance of the class :class:`~neptune.git_info.GitInfo` that provides information about
-                  the git repository from which experiment was started.
-                | If ``None`` is passed,
-                  system attempts to automatically extract information about git repository in the following way:
-
-                      * System looks for `.git` file in the current directory and, if not found,
-                        goes up recursively until `.git` file will be found
-                        (see: :meth:`~neptune.utils.get_git_info`).
-                      * If there is no git repository,
-                        then no information about git is displayed in experiment details in Neptune web application.
-
-            hostname (:obj:`str`, optional, default is ``None``):
-                If ``None``, neptune.legacy automatically get `hostname` information.
-                User can also set `hostname` directly by passing :obj:`str`.
-
-        Returns:
-            :class:`~neptune.experiments.Experiment` object that is used to manage experiment and log data to it.
-
-        Raises:
-            `ExperimentValidationError`: When provided arguments are invalid.
-            `ExperimentLimitReached`: When experiment limit in the project has been reached.
-
-        Examples:
-
-            .. code:: python3
-
-                # minimal invoke
-                neptune.create_experiment()
-
-                # explicitly return experiment object
-                experiment = neptune.create_experiment()
-
-                # create experiment with name and two parameters
-                neptune.create_experiment(name='first-pytorch-ever',
-                                          params={'lr': 0.0005,
-                                                  'dropout': 0.2})
-
-                # create experiment with name and description, and no sources files uploaded
-                neptune.create_experiment(name='neural-net-mnist',
-                                          description='neural net trained on MNIST',
-                                          upload_source_files=[])
-
-                # Send all py files in cwd (excluding hidden files with names beginning with a dot)
-                neptune.create_experiment(upload_source_files='*.py')
-
-                # Send all py files from all subdirectories (excluding hidden files with names beginning with a dot)
-                # Supported on Python 3.5 and later.
-                neptune.create_experiment(upload_source_files='**/*.py')
-
-                # Send all files and directories in cwd (excluding hidden files with names beginning with a dot)
-                neptune.create_experiment(upload_source_files='*')
-
-                # Send all files and directories in cwd including hidden files
-                neptune.create_experiment(upload_source_files=['*', '.*'])
-
-                # Send files with names being a single character followed by '.py' extension.
-                neptune.create_experiment(upload_source_files='?.py')
-
-                # larger example
-                neptune.create_experiment(name='first-pytorch-ever',
-                                          params={'lr': 0.0005,
-                                                  'dropout': 0.2},
-                                          properties={'key1': 'value1',
-                                                      'key2': 17,
-                                                      'key3': 'other-value'},
-                                          description='write longer description here',
-                                          tags=['list-of', 'tags', 'goes-here', 'as-list-of-strings'],
-                                          upload_source_files=['training_with_pytorch.py', 'net.py'])
-        """
-
-        if name is None:
-            name = "Untitled"
-
-        if description is None:
-            description = ""
-
-        if params is None:
-            params = {}
-
-        if properties is None:
-            properties = {}
-
-        if tags is None:
-            tags = []
-
-        if git_info is None:
-            git_info = get_git_info(discover_git_repo_location())
-
-        if hostname is None:
-            hostname = get_hostname()
-
-        if notebook_id is None and os.getenv(NOTEBOOK_ID_ENV_NAME, None) is not None:
-            notebook_id = os.environ[NOTEBOOK_ID_ENV_NAME]
-
-        if isinstance(upload_source_files, six.string_types):
-            upload_source_files = [upload_source_files]
-
-        entrypoint, source_target_pairs = get_source_code_to_upload(upload_source_files=upload_source_files)
-
-        if notebook_path is None and os.getenv(NOTEBOOK_PATH_ENV_NAME, None) is not None:
-            notebook_path = os.environ[NOTEBOOK_PATH_ENV_NAME]
-
-        abortable = abort_callback is not None or DefaultAbortImpl.requirements_installed()
-
-        checkpoint_id = None
-        if notebook_id is not None and notebook_path is not None:
-            checkpoint = create_checkpoint(
-                backend=self._backend,
-                notebook_id=notebook_id,
-                notebook_path=notebook_path,
-            )
-            if checkpoint is not None:
-                checkpoint_id = checkpoint.id
 
-        experiment = self._backend.create_experiment(
-            project=self,
-            name=name,
-            description=description,
-            params=params,
-            properties=properties,
-            tags=tags,
-            abortable=abortable,
-            monitored=run_monitoring_thread,
-            git_info=git_info,
-            hostname=hostname,
-            entrypoint=entrypoint,
-            notebook_id=notebook_id,
-            checkpoint_id=checkpoint_id,
-        )
+class Run(NeptuneObject):
+    """Starts a new tracked run that logs ML model-building metadata to neptune.ai.
 
-        self._backend.upload_source_code(experiment, source_target_pairs)
+    You can log metadata by assigning it to the initialized Run object:
 
-        experiment._start(
-            abort_callback=abort_callback,
-            logger=logger,
-            upload_stdout=upload_stdout,
-            upload_stderr=upload_stderr,
-            send_hardware_metrics=send_hardware_metrics,
-            run_monitoring_thread=run_monitoring_thread,
-            handle_uncaught_exceptions=handle_uncaught_exceptions,
-        )
+    ```
+    run = neptune.init_run()
+    run["your/structure"] = some_metadata
+    ```
 
-        self._push_new_experiment(experiment)
+    Examples of metadata you can log: metrics, losses, scores, artifact versions, images, predictions,
+    model weights, parameters, checkpoints, and interactive visualizations.
 
-        click.echo(self._get_experiment_link(experiment))
+    By default, the run automatically tracks hardware consumption, stdout/stderr, source code, and Git information.
+    If you're using Neptune in an interactive session, however, some background monitoring needs to be enabled
+    explicitly.
 
-        return experiment
+    If you provide the ID of an existing run, that run is resumed and no new run is created. You may resume a run
+    either to log more metadata or to fetch metadata from it.
 
-    def _get_experiment_link(self, experiment):
-        return "{base_url}/{namespace}/{project}/e/{exp_id}".format(
-            base_url=self._backend.display_address,
-            namespace=self.namespace,
-            project=self.name,
-            exp_id=experiment.id,
-        )
+    The run ends either when its `stop()` method is called or when the script finishes execution.
 
-    def create_notebook(self):
-        """Create a new notebook object and return corresponding :class:`~neptune.notebook.Notebook` instance.
+    You can also use the Run object as a context manager (see examples).
 
-        Returns:
-            :class:`~neptune.notebook.Notebook` object.
+    Args:
+        project: Name of the project where the run should go, in the form `workspace-name/project_name`.
+            If left empty, the value of the NEPTUNE_PROJECT environment variable is used.
+        api_token: User's API token.
+            If left empty, the value of the NEPTUNE_API_TOKEN environment variable is used (recommended).
+        with_id: If you want to resume a run, pass the identifier of an existing run. For example, "SAN-1".
+            If left empty, a new run is created.
+        custom_run_id: A unique identifier to be used when running Neptune in distributed training jobs.
+            Make sure to use the same identifier throughout the whole pipeline execution.
+        mode: Connection mode in which the tracking will work.
+            If left empty, the value of the NEPTUNE_MODE environment variable is used.
+            If no value was set for the environment variable, "async" is used by default.
+            Possible values are `async`, `sync`, `offline`, `read-only`, and `debug`.
+        name: Custom name for the run. You can add it as a column in the runs table ("sys/name").
+            You can also edit the name in the app: Open the run menu and access the run information.
+        description:  Custom description of the run. You can add it as a column in the runs table
+            ("sys/description").
+            You can also edit the description in the app: Open the run menu and access the run information.
+        tags: Tags of the run as a list of strings.
+            You can edit the tags through the "sys/tags" field or in the app (run menu -> information).
+            You can also select multiple runs and manage their tags as a single action.
+        source_files: List of source files to be uploaded.
+            Uploaded source files are displayed in the "Source code" dashboard.
+            To not upload anything, pass an empty list (`[]`).
+            Unix style pathname pattern expansion is supported. For example, you can pass `*.py` to upload
+            all Python files from the current directory.
+            If None is passed, the Python file from which the run was created will be uploaded.
+        capture_stdout: Whether to log the stdout of the run.
+            Defaults to `False` in interactive sessions and `True` otherwise.
+            The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
+        capture_stderr: Whether to log the stderr of the run.
+            Defaults to `False` in interactive sessions and `True` otherwise.
+            The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
+        capture_hardware_metrics: Whether to send hardware monitoring logs (CPU, GPU, and memory utilization).
+            Defaults to `False` in interactive sessions and `True` otherwise.
+            The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
+        fail_on_exception: Whether to register an uncaught exception handler to this process and,
+            in case of an exception, set the "sys/failed" field of the run to `True`.
+            An exception is always logged.
+        monitoring_namespace: Namespace inside which all hardware monitoring logs are stored.
+            Defaults to "monitoring/<hash>", where the hash is generated based on environment information,
+            to ensure that it's unique for each process.
+        flush_period: In the asynchronous (default) connection mode, how often disk flushing is triggered
+            (in seconds).
+        proxies: Argument passed to HTTP calls made via the Requests library, as dictionary of strings.
+            For more information about proxies, see the Requests documentation.
+        capture_traceback: Whether to log the traceback of the run in case of an exception.
+            The tracked metadata is stored in the "<monitoring_namespace>/traceback" namespace (see the
+            `monitoring_namespace` parameter).
+        git_ref: GitRef object containing information about the Git repository path.
+            If None, Neptune looks for a repository in the path of the script that is executed.
+            To specify a different location, set to GitRef(repository_path="path/to/repo").
+            To turn off Git tracking for the run, set to False or GitRef.DISABLED.
+        dependencies: If you pass `"infer"`, Neptune logs dependencies installed in the current environment.
+            You can also pass a path to your dependency file directly.
+            If left empty, no dependencies are tracked.
+        async_lag_callback: Custom callback which is called if the lag between a queued operation and its
+            synchronization with the server exceeds the duration defined by `async_lag_threshold`. The callback
+            should take a Run object as the argument and can contain any custom code, such as calling `stop()` on
+            the object.
+            Note: Instead of using this argument, you can use Neptune's default callback by setting the
+            `NEPTUNE_ENABLE_DEFAULT_ASYNC_LAG_CALLBACK` environment variable to `TRUE`.
+        async_lag_threshold: In seconds, duration between the queueing and synchronization of an operation.
+            If a lag callback (default callback enabled via environment variable or custom callback passed to the
+            `async_lag_callback` argument) is enabled, the callback is called when this duration is exceeded.
+        async_no_progress_callback: Custom callback which is called if there has been no synchronization progress
+            whatsoever for the duration defined by `async_no_progress_threshold`. The callback
+            should take a Run object as the argument and can contain any custom code, such as calling `stop()` on
+            the object.
+            Note: Instead of using this argument, you can use Neptune's default callback by setting the
+            `NEPTUNE_ENABLE_DEFAULT_ASYNC_NO_PROGRESS_CALLBACK` environment variable to `TRUE`.
+        async_no_progress_threshold: In seconds, for how long there has been no synchronization progress since the
+            object was initialized. If a no-progress callback (default callback enabled via environment variable or
+            custom callback passed to the `async_no_progress_callback` argument) is enabled, the callback is called
+            when this duration is exceeded.
+
+    Returns:
+        Run object that is used to manage the tracked run and log metadata to it.
+
+    Examples:
+
+        Creating a new run:
+
+        >>> import neptune
+
+        >>> # Minimal invoke
+        ... # (creates a run in the project specified by the NEPTUNE_PROJECT environment variable)
+        ... run = neptune.init_run()
+
+        >>> # Or initialize with the constructor
+        ... run = Run(project="ml-team/classification")
+
+        >>> # Create a run with a name and description, with no sources files or Git info tracked:
+        >>> run = neptune.init_run(
+        ...     name="neural-net-mnist",
+        ...     description="neural net trained on MNIST",
+        ...     source_files=[],
+        ...     git_ref=False,
+        ... )
+
+        >>> # Log all .py files from all subdirectories, excluding hidden files
+        ... run = neptune.init_run(source_files="**/*.py")
+
+        >>> # Log all files and directories in the current working directory, excluding hidden files
+        ... run = neptune.init_run(source_files="*")
+
+        >>> # Larger example
+        ... run = neptune.init_run(
+        ...     project="ml-team/classification",
+        ...     name="first-pytorch-ever",
+        ...     description="Longer description of the run goes here",
+        ...     tags=["tags", "go-here", "as-list-of-strings"],
+        ...     source_files=["training_with_pytorch.py", "net.py"],
+        ...     dependencies="infer",
+        ...     capture_stderr=False,
+        ...     git_ref=GitRef(repository_path="/Users/Jackie/repos/cls_project"),
+        ... )
+
+        Connecting to an existing run:
+
+        >>> # Resume logging to an existing run with the ID "SAN-3"
+        ... run = neptune.init_run(with_id="SAN-3")
+        ... run["parameters/lr"] = 0.1  # modify or add metadata
+
+        >>> # Initialize an existing run in read-only mode (logging new data is not possible, only fetching)
+        ... run = neptune.init_run(with_id="SAN-4", mode="read-only")
+        ... learning_rate = run["parameters/lr"].fetch()
+
+        Using the Run object as context manager:
+
+        >>> with Run() as run:
+        ...     run["metric"].append(value)
+
+    For more, see the docs:
+        Initializing a run:
+            https://docs.neptune.ai/api/neptune#init_run
+        Run class reference:
+            https://docs.neptune.ai/api/run/
+        Essential logging methods:
+            https://docs.neptune.ai/logging/methods/
+        Resuming a run:
+            https://docs.neptune.ai/logging/to_existing_object/
+        Setting a custom run ID:
+            https://docs.neptune.ai/logging/custom_run_id/
+        Logging to multiple runs at once:
+            https://docs.neptune.ai/logging/to_multiple_objects/
+        Accessing the run from multiple places:
+            https://docs.neptune.ai/logging/from_multiple_places/
+    """
 
-        Examples:
+    container_type = ContainerType.RUN
 
-            .. code:: python3
+    def __init__(
+        self,
+        with_id: Optional[str] = None,
+        *,
+        project: Optional[str] = None,
+        api_token: Optional[str] = None,
+        custom_run_id: Optional[str] = None,
+        mode: Optional[Literal["async", "sync", "offline", "read-only", "debug"]] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        tags: Optional[Union[List[str], str]] = None,
+        source_files: Optional[Union[List[str], str]] = None,
+        capture_stdout: Optional[bool] = None,
+        capture_stderr: Optional[bool] = None,
+        capture_hardware_metrics: Optional[bool] = None,
+        fail_on_exception: bool = True,
+        monitoring_namespace: Optional[str] = None,
+        flush_period: float = DEFAULT_FLUSH_PERIOD,
+        proxies: Optional[dict] = None,
+        capture_traceback: bool = True,
+        git_ref: Optional[Union[GitRef, GitRefDisabled, bool]] = None,
+        dependencies: Optional[Union[str, os.PathLike]] = None,
+        async_lag_callback: Optional[NeptuneObjectCallback] = None,
+        async_lag_threshold: float = ASYNC_LAG_THRESHOLD,
+        async_no_progress_callback: Optional[NeptuneObjectCallback] = None,
+        async_no_progress_threshold: float = ASYNC_NO_PROGRESS_THRESHOLD,
+        **kwargs,
+    ):
+        check_for_extra_kwargs("Run", kwargs)
 
-                # Instantiate a session and fetch a project
-                project = neptune.init()
+        verify_type("with_id", with_id, (str, type(None)))
+        verify_type("project", project, (str, type(None)))
+        verify_type("custom_run_id", custom_run_id, (str, type(None)))
+        verify_type("mode", mode, (str, type(None)))
+        verify_type("name", name, (str, type(None)))
+        verify_type("description", description, (str, type(None)))
+        verify_type("capture_stdout", capture_stdout, (bool, type(None)))
+        verify_type("capture_stderr", capture_stderr, (bool, type(None)))
+        verify_type("capture_hardware_metrics", capture_hardware_metrics, (bool, type(None)))
+        verify_type("fail_on_exception", fail_on_exception, bool)
+        verify_type("monitoring_namespace", monitoring_namespace, (str, type(None)))
+        verify_type("capture_traceback", capture_traceback, bool)
+        verify_type("git_ref", git_ref, (GitRef, str, bool, type(None)))
+        verify_type("dependencies", dependencies, (str, os.PathLike, type(None)))
+
+        if tags is not None:
+            if isinstance(tags, str):
+                tags = [tags]
+            else:
+                verify_collection_type("tags", tags, str)
+        if source_files is not None:
+            if isinstance(source_files, str):
+                source_files = [source_files]
+            else:
+                verify_collection_type("source_files", source_files, str)
 
-                # Create a notebook in Neptune
-                notebook = project.create_notebook()
-        """
-        return self._backend.create_notebook(self)
+        self._with_id: Optional[str] = with_id
+        self._name: Optional[str] = DEFAULT_NAME if with_id is None and name is None else name
+        self._description: Optional[str] = "" if with_id is None and description is None else description
+        self._custom_run_id: Optional[str] = custom_run_id or os.getenv(CUSTOM_RUN_ID_ENV_NAME)
+        self._hostname: str = get_hostname()
+        self._pid: int = os.getpid()
+        self._tid: int = threading.get_ident()
+        self._tags: Optional[List[str]] = tags
+        self._source_files: Optional[List[str]] = source_files
+        self._fail_on_exception: bool = fail_on_exception
+        self._capture_traceback: bool = capture_traceback
+
+        if type(git_ref) is bool:
+            git_ref = GitRef() if git_ref else GitRef.DISABLED
+
+        self._git_ref: Optional[GitRef, GitRefDisabled] = git_ref or GitRef()
+        self._dependencies: Optional[str, os.PathLike] = dependencies
+
+        self._monitoring_namespace: str = (
+            monitoring_namespace
+            or os.getenv(MONITORING_NAMESPACE)
+            or generate_monitoring_namespace(self._hostname, self._pid, self._tid)
+        )
 
-    def get_notebook(self, notebook_id):
-        """Get a :class:`~neptune.notebook.Notebook` object with given ``notebook_id``.
+        # for backward compatibility imports
+        mode = Mode(mode or os.getenv(CONNECTION_MODE) or Mode.ASYNC.value)
 
-        Returns:
-            :class:`~neptune.notebook.Notebook` object.
+        self._stdout_path: str = "{}/stdout".format(self._monitoring_namespace)
+        self._capture_stdout: bool = capture_stdout
+        if capture_stdout is None:
+            self._capture_stdout = capture_only_if_non_interactive(mode=mode)
+
+        self._stderr_path: str = "{}/stderr".format(self._monitoring_namespace)
+        self._capture_stderr: bool = capture_stderr
+        if capture_stderr is None:
+            self._capture_stderr = capture_only_if_non_interactive(mode=mode)
+
+        self._capture_hardware_metrics: bool = capture_hardware_metrics
+        if capture_hardware_metrics is None:
+            self._capture_hardware_metrics = capture_only_if_non_interactive(mode=mode)
+
+        if with_id and custom_run_id:
+            raise NeptuneRunResumeAndCustomIdCollision()
+
+        if mode == Mode.OFFLINE or mode == Mode.DEBUG:
+            project = OFFLINE_PROJECT_QUALIFIED_NAME
+
+        super().__init__(
+            project=project,
+            api_token=api_token,
+            mode=mode,
+            flush_period=flush_period,
+            proxies=proxies,
+            async_lag_callback=async_lag_callback,
+            async_lag_threshold=async_lag_threshold,
+            async_no_progress_callback=async_no_progress_callback,
+            async_no_progress_threshold=async_no_progress_threshold,
+        )
 
-        Examples:
+    def _get_or_create_api_object(self) -> ApiExperiment:
+        project_workspace = self._project_api_object.workspace
+        project_name = self._project_api_object.name
+        project_qualified_name = f"{project_workspace}/{project_name}"
+
+        if self._with_id:
+            return self._backend.get_metadata_container(
+                container_id=QualifiedName(project_qualified_name + "/" + self._with_id),
+                expected_container_type=Run.container_type,
+            )
+        else:
+            if self._mode == Mode.READ_ONLY:
+                raise NeedExistingRunForReadOnlyMode()
+
+            git_info = to_git_info(git_ref=self._git_ref)
+
+            custom_run_id = self._custom_run_id
+            if custom_run_id_exceeds_length(self._custom_run_id):
+                custom_run_id = None
+
+            notebook_id, checkpoint_id = create_notebook_checkpoint(backend=self._backend)
+
+            return self._backend.create_run(
+                project_id=self._project_api_object.id,
+                git_info=git_info,
+                custom_run_id=custom_run_id,
+                notebook_id=notebook_id,
+                checkpoint_id=checkpoint_id,
+            )
 
-            .. code:: python3
+    @temporarily_disabled
+    def _get_background_jobs(self) -> List["BackgroundJob"]:
+        background_jobs = [PingBackgroundJob()]
+
+        websockets_factory = self._backend.websockets_factory(self._project_api_object.id, self._id)
+        if websockets_factory:
+            background_jobs.append(WebsocketSignalsBackgroundJob(websockets_factory))
+
+        if self._capture_stdout:
+            background_jobs.append(StdoutCaptureBackgroundJob(attribute_name=self._stdout_path))
+
+        if self._capture_stderr:
+            background_jobs.append(StderrCaptureBackgroundJob(attribute_name=self._stderr_path))
+
+        if self._capture_hardware_metrics:
+            background_jobs.append(HardwareMetricReportingJob(attribute_namespace=self._monitoring_namespace))
+
+        if self._capture_traceback:
+            background_jobs.append(
+                TracebackJob(path=f"{self._monitoring_namespace}/traceback", fail_on_exception=self._fail_on_exception)
+            )
 
-                # Instantiate a session and fetch a project
-                project = neptune.init()
+        return background_jobs
 
-                # Get a notebook object
-                notebook = project.get_notebook('d1c1b494-0620-4e54-93d5-29f4e848a51a')
-        """
-        return self._backend.get_notebook(project=self, notebook_id=notebook_id)
+    @temporarily_disabled
+    def _write_initial_monitoring_attributes(self) -> None:
+        if self._hostname is not None:
+            self[f"{self._monitoring_namespace}/hostname"] = self._hostname
+            if self._with_id is None:
+                self[SYSTEM_HOSTNAME_ATTRIBUTE_PATH] = self._hostname
+
+        if self._pid is not None:
+            self[f"{self._monitoring_namespace}/pid"] = str(self._pid)
+
+        if self._tid is not None:
+            self[f"{self._monitoring_namespace}/tid"] = str(self._tid)
+
+    @temporarily_disabled
+    def _write_initial_attributes(self):
+        if self._name is not None:
+            self[SYSTEM_NAME_ATTRIBUTE_PATH] = self._name
+
+        if self._description is not None:
+            self[SYSTEM_DESCRIPTION_ATTRIBUTE_PATH] = self._description
+
+        if any((self._capture_stderr, self._capture_stdout, self._capture_traceback, self._capture_hardware_metrics)):
+            self._write_initial_monitoring_attributes()
+
+        if self._tags is not None:
+            self[SYSTEM_TAGS_ATTRIBUTE_PATH].add(self._tags)
+
+        if self._with_id is None:
+            self[SYSTEM_FAILED_ATTRIBUTE_PATH] = False
+
+        if self._capture_stdout and not self.exists(self._stdout_path):
+            self.define(self._stdout_path, StringSeries([]))
+
+        if self._capture_stderr and not self.exists(self._stderr_path):
+            self.define(self._stderr_path, StringSeries([]))
+
+        if self._with_id is None or self._source_files is not None:
+            # upload default sources ONLY if creating a new run
+            upload_source_code(source_files=self._source_files, run=self)
+
+        if self._dependencies:
+            try:
+                if self._dependencies == "infer":
+                    dependency_strategy = InferDependenciesStrategy()
+
+                else:
+                    dependency_strategy = FileDependenciesStrategy(path=self._dependencies)
+
+                dependency_strategy.log_dependencies(run=self)
+            except Exception as e:
+                warn_once(
+                    "An exception occurred in automatic dependency tracking."
+                    "Skipping upload of requirement files."
+                    "Exception: " + str(e),
+                    exception=NeptuneWarning,
+                )
+
+        try:
+            track_uncommitted_changes(
+                git_ref=self._git_ref,
+                run=self,
+            )
+        except Exception as e:
+            warn_once(
+                "An exception occurred in tracking uncommitted changes."
+                "Skipping upload of patch files."
+                "Exception: " + str(e),
+                exception=NeptuneWarning,
+            )
 
     @property
-    def full_id(self):
-        """Project qualified name as :obj:`str`, for example `john/sandbox`."""
-        return "{}/{}".format(self.namespace, self.name)
-
-    def __str__(self):
-        return "Project({})".format(self.full_id)
-
-    def __repr__(self):
-        return str(self)
-
-    def __eq__(self, o):
-        return self.__dict__ == o.__dict__
-
-    def __ne__(self, o):
-        return not self.__eq__(o)
-
-    def _fetch_leaderboard(self, id, state, owner, tag, min_running_time):
-        return self._backend.get_leaderboard_entries(
-            project=self,
-            ids=as_list(id),
-            states=as_list(state),
-            owners=as_list(owner),
-            tags=as_list(tag),
-            min_running_time=min_running_time,
+    def monitoring_namespace(self) -> str:
+        return self._monitoring_namespace
+
+    def _raise_if_stopped(self):
+        if self._state == ContainerState.STOPPED:
+            raise InactiveRunException(label=self._sys_id)
+
+    def get_url(self) -> str:
+        """Returns the URL that can be accessed within the browser"""
+        return self._backend.get_run_url(
+            run_id=self._id,
+            workspace=self._workspace,
+            project_name=self._project_name,
+            sys_id=self._sys_id,
         )
 
-    @staticmethod
-    def _sort_leaderboard_columns(column_names):
-        user_defined_weights = {"channel": 1, "parameter": 2, "property": 3}
-
-        system_properties_weights = {
-            "id": 0,
-            "name": 1,
-            "created": 2,
-            "finished": 3,
-            "owner": 4,
-            "worker_type": 5,
-            "environment": 6,
-        }
-
-        def key(c):
-            """A sorting key for a column name.
-
-            Sorts by the system properties first, then channels, parameters, user-defined properties.
-
-            Within each group columns are sorted alphabetically, except for system properties,
-            where order is custom.
-            """
-            parts = c.split("_", 1)
-            if parts[0] in user_defined_weights.keys():
-                name = parts[1]
-                weight = user_defined_weights.get(parts[0], 99)
-                system_property_weight = None
-            else:
-                name = c
-                weight = 0
-                system_property_weight = system_properties_weights.get(name, 99)
-
-            return weight, system_property_weight, name
-
-        return sorted(column_names, key=key)
-
-    def _get_current_experiment(self):
-        with self.__lock:
-            if self._experiments_stack:
-                return self._experiments_stack[-1]
-            else:
-                raise NeptuneNoExperimentContextException()
 
-    def _push_new_experiment(self, new_experiment):
-        with self.__lock:
-            self._experiments_stack.append(new_experiment)
-            return new_experiment
-
-    def _remove_stopped_experiment(self, experiment):
-        with self.__lock:
-            if self._experiments_stack:
-                self._experiments_stack = [exp for exp in self._experiments_stack if exp != experiment]
-
-    def _shutdown_hook(self):
-        if self._experiments_stack:
-            # stopping experiment removes it from list, co we copy it
-            copied_experiment_list = [exp for exp in self._experiments_stack]
-            for exp in copied_experiment_list:
-                exp.stop()
+def capture_only_if_non_interactive(mode) -> bool:
+    if in_interactive() or in_notebook():
+        if mode in {Mode.OFFLINE, Mode.SYNC, Mode.ASYNC}:
+            warn_once(
+                "The following monitoring options are disabled by default in interactive sessions:"
+                " 'capture_stdout', 'capture_stderr', 'capture_traceback', and 'capture_hardware_metrics'."
+                " To enable them, set each parameter to 'True' when initializing the run. The monitoring will"
+                " continue until you call run.stop() or the kernel stops."
+                " Also note: Your source files can only be tracked if you pass the path(s) to the 'source_code'"
+                " argument. For help, see the Neptune docs: https://docs.neptune.ai/logging/source_code/",
+                exception=NeptuneWarning,
+            )
+        return False
+    return True
+
+
+def generate_monitoring_namespace(*descriptors) -> str:
+    return f"monitoring/{generate_hash(*descriptors, length=8)}"
+
+
+def check_for_extra_kwargs(caller_name: str, kwargs: dict):
+    if kwargs:
+        first_key = next(iter(kwargs.keys()))
+        raise TypeError(f"{caller_name}() got an unexpected keyword argument '{first_key}'")
+
+
+def create_notebook_checkpoint(backend: NeptuneBackend) -> Tuple[Optional[str], Optional[str]]:
+    notebook_id = os.getenv(NEPTUNE_NOTEBOOK_ID, None)
+    notebook_path = os.getenv(NEPTUNE_NOTEBOOK_PATH, None)
+
+    checkpoint_id = None
+    if notebook_id is not None and notebook_path is not None:
+        checkpoint_id = create_checkpoint(backend=backend, notebook_id=notebook_id, notebook_path=notebook_path)
+
+    return notebook_id, checkpoint_id
```

### Comparing `neptune-1.9.1/src/neptune/logging/logger.py` & `neptune-2.0.0a0/src/neptune/types/atoms/float.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,23 +9,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+__all__ = ["Float"]
 
-# backwards compatibility
-__all__ = [
-    "Logger",
-]
+from dataclasses import dataclass
+from typing import (
+    TYPE_CHECKING,
+    TypeVar,
+)
 
-from neptune.metadata_containers import MetadataContainer
+from neptune.internal.types.stringify_value import extract_if_stringify_value
+from neptune.types.atoms.atom import Atom
 
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
 
-class Logger(object):
-    def __init__(self, container: MetadataContainer, attribute_name: str):
-        self._container = container
-        self._attribute_name = attribute_name
+Ret = TypeVar("Ret")
 
-    def log(self, msg: str):
-        self._container[self._attribute_name].log(msg)
+
+@dataclass
+class Float(Atom):
+
+    value: float
+
+    def __init__(self, value):
+        self.value = float(extract_if_stringify_value(value))
+
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        return visitor.visit_float(self)
+
+    def __str__(self):
+        return "Float({})".format(str(self.value))
+
+    def __float__(self):
+        return self.value
```

### Comparing `neptune-1.9.1/src/neptune/management/__init__.py` & `neptune-2.0.0a0/src/neptune/management/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     get_project_service_account_list()
     get_workspace_service_account_list()
     trash_objects()
 
 Usage examples
 --------------
 
+Import management API
+>>> from neptune import management
+
 Getting projects in a workspace as a list:
 >>> projects = management.get_project_list()
 
 Creating a new project:
 >>> management.create_project(
 ...     name="ml-team/classification",
 ...     key="CLS",
@@ -91,14 +94,17 @@
 >>> # Fetch runs tagged as "trash":
 ... runs_to_trash_df = project.fetch_runs_table(tag="trash").to_pandas()
 >>> # Turn run IDs into a list:
 ... runs_to_trash = runs_to_trash_df["sys/id"].tolist()
 >>> # Move the runs to trash:
 ... management.trash_objects(project=project_name, ids=runs_to_trash)
 
+Get information about a workspace, including storage usage and limits:
+>>> management.get_workspace_status(workspace="ml-team")
+
 ---
 
 See also the API reference in the docs: https://docs.neptune.ai/api/management
 """
 from .internal.api import (
     WorkspaceMemberRole,
     add_project_member,
@@ -108,14 +114,15 @@
     delete_objects_from_trash,
     delete_project,
     get_project_list,
     get_project_member_list,
     get_project_service_account_list,
     get_workspace_member_list,
     get_workspace_service_account_list,
+    get_workspace_status,
     invite_to_workspace,
     remove_project_member,
     remove_project_service_account,
     trash_objects,
 )
 from .internal.types import (
     MemberRole,
@@ -134,11 +141,12 @@
     "get_workspace_member_list",
     "invite_to_workspace",
     "WorkspaceMemberRole",
     "add_project_service_account",
     "remove_project_service_account",
     "get_project_service_account_list",
     "get_workspace_service_account_list",
+    "get_workspace_status",
     "trash_objects",
     "MemberRole",
     "ProjectVisibility",
 ]
```

### Comparing `neptune-1.9.1/src/neptune/management/exceptions.py` & `neptune-2.0.0a0/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/management/internal/api.py` & `neptune-2.0.0a0/src/neptune/management/internal/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     "invite_to_workspace",
     "WorkspaceMemberRole",
     "add_project_service_account",
     "remove_project_service_account",
     "get_project_service_account_list",
     "get_workspace_service_account_list",
     "trash_objects",
+    "get_workspace_status",
 ]
 
 import os
 from typing import (
     Dict,
     Iterable,
     List,
@@ -46,28 +47,28 @@
     HTTPBadRequest,
     HTTPConflict,
     HTTPForbidden,
     HTTPNotFound,
     HTTPUnprocessableEntity,
 )
 
-from neptune.common.backends.utils import with_api_exceptions_handler
-from neptune.common.envs import API_TOKEN_ENV_NAME
 from neptune.internal.backends.hosted_client import (
     DEFAULT_REQUEST_KWARGS,
     create_backend_client,
     create_http_client_with_auth,
     create_leaderboard_client,
 )
 from neptune.internal.backends.swagger_client_wrapper import SwaggerClientWrapper
 from neptune.internal.backends.utils import (
     parse_validation_errors,
     ssl_verify,
+    with_api_exceptions_handler,
 )
 from neptune.internal.credentials import Credentials
+from neptune.internal.envs import API_TOKEN_ENV_NAME
 from neptune.internal.id_formats import QualifiedName
 from neptune.internal.utils import (
     verify_collection_type,
     verify_type,
 )
 from neptune.internal.utils.iteration import get_batches
 from neptune.internal.utils.logger import get_logger
@@ -1029,7 +1030,70 @@
         **DEFAULT_REQUEST_KWARGS,
     }
 
     response = leaderboard_client.api.deleteAllExperiments(**params).response()
 
     for error in response.result.errors:
         logger.warning(error)
+
+
+def get_workspace_status(workspace: str, *, api_token: Optional[str] = None) -> Dict[str, int]:
+    """Retrieves status information about a Neptune workspace.
+
+    Includes the following:
+
+    - Storage usage and limit
+    - Active project count and limit
+    - Member count
+
+    Args:
+        workspace: Name of the Neptune workspace.
+        api_token: Account's API token.
+            If None, the value of the NEPTUNE_API_TOKEN environment variable is used.
+            Note: To keep your token secure, use the NEPTUNE_API_TOKEN environment variable rather than placing your
+            API token in plain text in your source code.
+
+    Returns:
+        Dictionary with metric name as keys and float values
+
+    Example:
+        >>> from neptune import management
+        >>> management.get_workspace_status(workspace="ml-team")
+        ... {'storageBytesAvailable': 214747451765,
+        ... 'storageBytesLimit': 214748364800,
+        ... 'storageBytesUsed': 913035,
+        ... 'activeProjectsUsage': 1,
+        ... 'activeProjectsLimit': 1,
+        ... 'membersCount': 1}
+
+    You may also want to check the management API reference:
+    https://docs.neptune.ai/api/management/#get_workspace_status
+    """
+    verify_type("workspace", workspace, str)
+    verify_type("api_token", api_token, (str, type(None)))
+
+    backend_client = _get_backend_client(api_token=api_token)
+
+    params = {
+        "organizationIdentifier": workspace,
+        **DEFAULT_REQUEST_KWARGS,
+    }
+
+    try:
+        response = backend_client.api.workspaceStatus(**params).response()
+
+        result = dict()
+        if hasattr(response.result, "storageBytesAvailable"):
+            result["storageBytesAvailable"] = response.result.storageBytesAvailable
+        if hasattr(response.result, "storageBytesLimit"):
+            result["storageBytesLimit"] = response.result.storageBytesLimit
+        if hasattr(response.result, "storageBytesAvailable") and hasattr(response.result, "storageBytesLimit"):
+            result["storageBytesUsed"] = response.result.storageBytesLimit - response.result.storageBytesAvailable
+        if hasattr(response.result, "activeProjectsUsage"):
+            result["activeProjectsUsage"] = response.result.activeProjectsUsage
+        if hasattr(response.result, "activeProjectsLimit"):
+            result["activeProjectsLimit"] = response.result.activeProjectsLimit
+        if hasattr(response.result, "membersCount"):
+            result["membersCount"] = response.result.membersCount
+        return result
+    except HTTPNotFound as e:
+        raise WorkspaceNotFound(workspace=workspace) from e
```

### Comparing `neptune-1.9.1/src/neptune/management/internal/dto.py` & `neptune-2.0.0a0/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/management/internal/utils.py` & `neptune-2.0.0a0/src/neptune/management/internal/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import re
 from enum import Enum
 from typing import Optional
 
-from neptune.common.patterns import PROJECT_QUALIFIED_NAME_PATTERN
+from neptune.internal.utils.patterns import PROJECT_QUALIFIED_NAME_PATTERN
 from neptune.management.exceptions import (
     ConflictingWorkspaceName,
     InvalidProjectName,
     MissingWorkspaceName,
 )
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/abstract.py` & `neptune-2.0.0a0/src/neptune/objects/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["SupportsNamespaces", "NeptuneObject", "NeptuneObjectCallback"]
+__all__ = ["SupportsNamespaces", "AbstractNeptuneObject", "NeptuneObjectCallback"]
 
 from abc import (
     ABC,
     abstractmethod,
 )
 from typing import (
     TYPE_CHECKING,
@@ -51,30 +51,25 @@
         >>> callback.log_accuracy(0.8)
         >>> # or
         ... callback = NeptuneCallback(start_from=run["some/random/path"])
         >>> callback.log_accuracy(0.8)
     """
 
     @abstractmethod
-    def __getitem__(self, path: str) -> "Handler":
-        ...
+    def __getitem__(self, path: str) -> "Handler": ...
 
     @abstractmethod
-    def __setitem__(self, key: str, value) -> None:
-        ...
+    def __setitem__(self, key: str, value) -> None: ...
 
     @abstractmethod
-    def __delitem__(self, path) -> None:
-        ...
+    def __delitem__(self, path) -> None: ...
 
     @abstractmethod
-    def get_root_object(self) -> "SupportsNamespaces":
-        ...
+    def get_root_object(self) -> "SupportsNamespaces": ...
 
 
-class NeptuneObject(SupportsNamespaces, ABC):
+class AbstractNeptuneObject(SupportsNamespaces, ABC):
     @abstractmethod
-    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None:
-        ...
+    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None: ...
 
 
-NeptuneObjectCallback = Callable[[NeptuneObject], None]
+NeptuneObjectCallback = Callable[[AbstractNeptuneObject], None]
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/metadata_container.py` & `neptune-2.0.0a0/src/neptune/objects/neptune_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,120 +9,120 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["MetadataContainer"]
+__all__ = ["NeptuneObject"]
 
 import abc
 import atexit
 import itertools
+import logging
 import os
 import threading
 import time
 import traceback
 from contextlib import AbstractContextManager
-from functools import wraps
+from functools import (
+    partial,
+    wraps,
+)
 from queue import Queue
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
     Union,
 )
 
+from neptune.api.models import FieldType
 from neptune.attributes import create_attribute_from_type
 from neptune.attributes.attribute import Attribute
 from neptune.attributes.namespace import Namespace as NamespaceAttr
 from neptune.attributes.namespace import NamespaceBuilder
-from neptune.common.exceptions import UNIX_STYLES
-from neptune.common.utils import reset_internal_ssl_state
-from neptune.common.warnings import warn_about_unsupported_type
 from neptune.envs import (
     NEPTUNE_ENABLE_DEFAULT_ASYNC_LAG_CALLBACK,
     NEPTUNE_ENABLE_DEFAULT_ASYNC_NO_PROGRESS_CALLBACK,
 )
-from neptune.exceptions import (
-    MetadataInconsistency,
-    NeptunePossibleLegacyUsageException,
-)
+from neptune.exceptions import MetadataInconsistency
 from neptune.handler import Handler
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    AttributeType,
     Project,
 )
 from neptune.internal.backends.factory import get_backend
 from neptune.internal.backends.neptune_backend import NeptuneBackend
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.backends.project_name_lookup import project_name_lookup
 from neptune.internal.backgroud_job_list import BackgroundJobList
 from neptune.internal.background_job import BackgroundJob
 from neptune.internal.container_structure import ContainerStructure
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import UNIX_STYLES
 from neptune.internal.id_formats import (
     QualifiedName,
     SysId,
     UniqueId,
     conform_optional,
 )
 from neptune.internal.init.parameters import (
     ASYNC_LAG_THRESHOLD,
     ASYNC_NO_PROGRESS_THRESHOLD,
     DEFAULT_FLUSH_PERIOD,
 )
 from neptune.internal.operation import DeleteAttribute
 from neptune.internal.operation_processors.factory import get_operation_processor
+from neptune.internal.operation_processors.lazy_operation_processor_wrapper import LazyOperationProcessorWrapper
 from neptune.internal.operation_processors.operation_processor import OperationProcessor
 from neptune.internal.signals_processing.background_job import CallbacksMonitor
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import (
     verify_optional_callable,
     verify_type,
 )
-from neptune.internal.utils.logger import get_logger
+from neptune.internal.utils.logger import (
+    get_disabled_logger,
+    get_logger,
+)
 from neptune.internal.utils.paths import parse_path
 from neptune.internal.utils.uncaught_exception_handler import instance as uncaught_exception_handler
+from neptune.internal.utils.utils import reset_internal_ssl_state
 from neptune.internal.value_to_attribute_visitor import ValueToAttributeVisitor
-from neptune.metadata_containers.abstract import (
-    NeptuneObject,
+from neptune.internal.warnings import warn_about_unsupported_type
+from neptune.objects.abstract import (
+    AbstractNeptuneObject,
     NeptuneObjectCallback,
 )
-from neptune.metadata_containers.metadata_containers_table import Table
-from neptune.metadata_containers.utils import parse_dates
+from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.types.type_casting import cast_value
 from neptune.typing import ProgressBarType
 from neptune.utils import stop_synchronization_callback
 
 if TYPE_CHECKING:
     from neptune.internal.signals_processing.signals import Signal
 
-logger = get_logger()
-
 
 def ensure_not_stopped(fun):
     @wraps(fun)
-    def inner_fun(self: "MetadataContainer", *args, **kwargs):
+    def inner_fun(self: "NeptuneObject", *args, **kwargs):
         self._raise_if_stopped()
         return fun(self, *args, **kwargs)
 
     return inner_fun
 
 
-class MetadataContainer(AbstractContextManager, NeptuneObject):
+class NeptuneObject(AbstractContextManager, AbstractNeptuneObject):
     container_type: ContainerType
 
-    LEGACY_METHODS = set()
-
     def __init__(
         self,
         *,
         project: Optional[str] = None,
         api_token: Optional[str] = None,
         mode: Mode = Mode.ASYNC,
         flush_period: float = DEFAULT_FLUSH_PERIOD,
@@ -145,14 +145,15 @@
         self._mode: Mode = mode
         self._flush_period = flush_period
         self._lock: threading.RLock = threading.RLock()
         self._forking_cond: threading.Condition = threading.Condition()
         self._forking_state: bool = False
         self._state: ContainerState = ContainerState.CREATED
         self._signals_queue: "Queue[Signal]" = Queue()
+        self._logger: logging.Logger = get_logger()
 
         self._backend: NeptuneBackend = get_backend(mode=mode, api_token=api_token, proxies=proxies)
 
         self._project_qualified_name: Optional[str] = conform_optional(project, QualifiedName)
         self._project_api_object: Project = project_name_lookup(
             backend=self._backend, name=self._project_qualified_name
         )
@@ -161,33 +162,34 @@
         self._api_object: ApiExperiment = self._get_or_create_api_object()
         self._id: UniqueId = self._api_object.id
         self._sys_id: SysId = self._api_object.sys_id
         self._workspace: str = self._api_object.workspace
         self._project_name: str = self._api_object.project_name
 
         self._async_lag_threshold = async_lag_threshold
-        self._async_lag_callback = MetadataContainer._get_callback(
+        self._async_lag_callback = NeptuneObject._get_callback(
             provided=async_lag_callback,
             env_name=NEPTUNE_ENABLE_DEFAULT_ASYNC_LAG_CALLBACK,
         )
         self._async_no_progress_threshold = async_no_progress_threshold
-        self._async_no_progress_callback = MetadataContainer._get_callback(
+        self._async_no_progress_callback = NeptuneObject._get_callback(
             provided=async_no_progress_callback,
             env_name=NEPTUNE_ENABLE_DEFAULT_ASYNC_NO_PROGRESS_CALLBACK,
         )
 
         self._op_processor: OperationProcessor = get_operation_processor(
             mode=mode,
             container_id=self._id,
             container_type=self.container_type,
             backend=self._backend,
             lock=self._lock,
             flush_period=flush_period,
             queue=self._signals_queue,
         )
+
         self._bg_job: BackgroundJobList = self._prepare_background_jobs_if_non_read_only()
         self._structure: ContainerStructure[Attribute, NamespaceAttr] = ContainerStructure(NamespaceBuilder(self))
 
         if self._mode != Mode.OFFLINE:
             self.sync(wait=False)
 
         if self._mode != Mode.READ_ONLY:
@@ -229,43 +231,44 @@
 
         with self._forking_cond:
             self._forking_state = False
             self._forking_cond.notify_all()
 
     def _handle_fork_in_child(self):
         reset_internal_ssl_state()
+        self._logger = get_disabled_logger()
         if self._state == ContainerState.STARTED:
             self._op_processor.close()
             self._signals_queue = Queue()
-            self._op_processor = get_operation_processor(
-                mode=self._mode,
-                container_id=self._id,
-                container_type=self.container_type,
-                backend=self._backend,
-                lock=self._lock,
-                flush_period=self._flush_period,
-                queue=self._signals_queue,
+            self._op_processor = LazyOperationProcessorWrapper(
+                operation_processor_getter=partial(
+                    get_operation_processor,
+                    mode=self._mode,
+                    container_id=self._id,
+                    container_type=self.container_type,
+                    backend=self._backend,
+                    lock=self._lock,
+                    flush_period=self._flush_period,
+                    queue=self._signals_queue,
+                ),
             )
-
             # TODO: Every implementation of background job should handle fork by itself.
             jobs = []
             if self._mode == Mode.ASYNC:
                 jobs.append(
                     CallbacksMonitor(
                         queue=self._signals_queue,
                         async_lag_threshold=self._async_lag_threshold,
                         async_no_progress_threshold=self._async_no_progress_threshold,
                         async_lag_callback=self._async_lag_callback,
                         async_no_progress_callback=self._async_no_progress_callback,
                     )
                 )
             self._bg_job = BackgroundJobList(jobs)
 
-            self._op_processor.start()
-
         with self._forking_cond:
             self._forking_state = False
             self._forking_cond.notify_all()
 
     def _before_fork(self):
         with self._forking_cond:
             self._forking_cond.wait_for(lambda: self._state != ContainerState.STOPPING)
@@ -306,16 +309,14 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_tb is not None:
             traceback.print_exception(exc_type, exc_val, exc_tb)
         self.stop()
 
     def __getattr__(self, item):
-        if item in self.LEGACY_METHODS:
-            raise NeptunePossibleLegacyUsageException()
         raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{item}'")
 
     @abc.abstractmethod
     def _raise_if_stopped(self):
         raise NotImplementedError
 
     def _get_subpath_suggestions(self, path_prefix: str = None, limit: int = 1000) -> List[str]:
@@ -441,25 +442,25 @@
             return
 
         with self._forking_cond:
             self._forking_cond.wait_for(lambda: not self._forking_state)
             self._state = ContainerState.STOPPING
 
         ts = time.time()
-        logger.info("Shutting down background jobs, please wait a moment...")
+        self._logger.info("Shutting down background jobs, please wait a moment...")
         self._bg_job.stop()
         self._bg_job.join(seconds)
-        logger.info("Done!")
+        self._logger.info("Done!")
 
         sec_left = None if seconds is None else seconds - (time.time() - ts)
         self._op_processor.stop(sec_left)
 
         if self._mode not in {Mode.OFFLINE, Mode.DEBUG}:
             metadata_url = self.get_url().rstrip("/") + "/metadata"
-            logger.info(f"Explore the metadata in the Neptune app: {metadata_url}")
+            self._logger.info(f"Explore the metadata in the Neptune app: {metadata_url}")
         self._backend.close()
 
         with self._forking_cond:
             self._state = ContainerState.STOPPED
             self._forking_cond.notify_all()
 
     def get_state(self) -> str:
@@ -624,15 +625,15 @@
             if wait:
                 self._op_processor.wait()
             attributes = self._backend.get_attributes(self._id, self.container_type)
             self._structure.clear()
             for attribute in attributes:
                 self._define_attribute(parse_path(attribute.path), attribute.type)
 
-    def _define_attribute(self, _path: List[str], _type: AttributeType):
+    def _define_attribute(self, _path: List[str], _type: FieldType):
         attr = create_attribute_from_type(_type, self, _path)
         self._structure.set(_path, attr)
 
     def _get_root_handler(self):
         return Handler(self, "")
 
     @abc.abstractmethod
@@ -643,15 +644,15 @@
 
         API reference: https://docs.neptune.ai/api/universal/#get_url
         """
         ...
 
     def _startup(self, debug_mode):
         if not debug_mode:
-            logger.info(f"Neptune initialized. Open in the app: {self.get_url()}")
+            self._logger.info(f"Neptune initialized. Open in the app: {self.get_url()}")
 
         self.start()
 
         uncaught_exception_handler.activate()
 
     def _shutdown_hook(self):
         self.stop()
@@ -679,18 +680,16 @@
             columns=columns,
             limit=limit,
             sort_by=sort_by,
             ascending=ascending,
             progress_bar=progress_bar,
         )
 
-        leaderboard_entries = parse_dates(leaderboard_entries)
-
         return Table(
             backend=self._backend,
             container_type=child_type,
             entries=leaderboard_entries,
         )
 
-    def get_root_object(self) -> "MetadataContainer":
+    def get_root_object(self) -> "NeptuneObject":
         """Returns the same Neptune object."""
         return self
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/model.py` & `neptune-2.0.0a0/src/neptune/objects/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,57 +22,59 @@
     List,
     Optional,
 )
 
 from typing_extensions import Literal
 
 from neptune.attributes.constants import SYSTEM_NAME_ATTRIBUTE_PATH
-from neptune.common.exceptions import NeptuneException
 from neptune.envs import CONNECTION_MODE
 from neptune.exceptions import (
     InactiveModelException,
     NeedExistingModelForReadOnlyMode,
     NeptuneMissingRequiredInitParameter,
     NeptuneModelKeyAlreadyExistsError,
     NeptuneObjectCreationConflict,
+    NeptuneUnsupportedFunctionalityException,
 )
 from neptune.internal.backends.api_model import ApiExperiment
 from neptune.internal.backends.nql import (
     NQLAggregator,
     NQLAttributeOperator,
     NQLAttributeType,
     NQLQueryAggregate,
     NQLQueryAttribute,
 )
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.id_formats import QualifiedName
 from neptune.internal.init.parameters import (
     ASYNC_LAG_THRESHOLD,
     ASYNC_NO_PROGRESS_THRESHOLD,
     DEFAULT_FLUSH_PERIOD,
     DEFAULT_NAME,
     OFFLINE_PROJECT_QUALIFIED_NAME,
 )
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import verify_type
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
-from neptune.metadata_containers import MetadataContainer
-from neptune.metadata_containers.abstract import NeptuneObjectCallback
-from neptune.metadata_containers.metadata_containers_table import Table
+from neptune.objects.abstract import NeptuneObjectCallback
+from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.utils import build_raw_query
+from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.typing import (
     ProgressBarCallback,
     ProgressBarType,
 )
 
 if TYPE_CHECKING:
     from neptune.internal.background_job import BackgroundJob
 
 
-class Model(MetadataContainer):
+class Model(NeptuneObject):
     """Initializes a Model object from an existing or new model.
 
     You can use this to create a new model from code or to perform actions on existing models.
 
     A Model object is suitable for storing model metadata that is common to all versions (you can use ModelVersion
     objects to track version-specific metadata). It does not track background metrics or logs automatically,
     but you can assign metadata to the Model object just like you can for runs.
@@ -176,14 +178,17 @@
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
         async_lag_callback: Optional[NeptuneObjectCallback] = None,
         async_lag_threshold: float = ASYNC_LAG_THRESHOLD,
         async_no_progress_callback: Optional[NeptuneObjectCallback] = None,
         async_no_progress_threshold: float = ASYNC_NO_PROGRESS_THRESHOLD,
     ):
+        # not yet supported by the backend
+        raise NeptuneUnsupportedFunctionalityException
+
         verify_type("with_id", with_id, (str, type(None)))
         verify_type("name", name, (str, type(None)))
         verify_type("key", key, (str, type(None)))
         verify_type("project", project, (str, type(None)))
         verify_type("mode", mode, (str, type(None)))
 
         self._key: Optional[str] = key
@@ -260,26 +265,30 @@
             project_name=self._project_name,
             sys_id=self._sys_id,
         )
 
     def fetch_model_versions_table(
         self,
         *,
+        query: Optional[str] = None,
         columns: Optional[Iterable[str]] = None,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
     ) -> Table:
         """Retrieve all versions of the given model.
 
         Args:
+            query: NQL query string. Syntax: https://docs.neptune.ai/usage/nql/
+                Example: `"(model_size: float > 100) AND (backbone: string = VGG)"`.
             columns: Names of columns to include in the table, as a list of field names.
                 The Neptune ID ("sys/id") is included automatically.
-                If `None` (default), all the columns of the model versions table are included.
+                If `None` (default), all the columns of the model versions table are included,
+                    up to a maximum of 10 000 columns.
             limit: How many entries to return at most. If `None`, all entries are returned.
             sort_by: Name of the field to sort the results by.
                 The field must represent a simple type (string, float, datetime, integer, or Boolean).
             ascending: Whether to sort the entries in ascending order of the sorting column values.
             progress_bar: Set to `False` to disable the download progress bar,
                 or pass a `ProgressBarCallback` class to use your own progress bar callback.
 
@@ -299,43 +308,48 @@
             ... model_versions_df = model.fetch_model_versions_table(columns=["params/lr", "val/loss"]).to_pandas()
 
             >>> # Sort model versions by size (space they take up in Neptune)
             ... model_versions_df = model.fetch_model_versions_table(sort_by="sys/size").to_pandas()
             ... # Extract the ID of the largest model version object
             ... largest_model_version_id = model_versions_df["sys/id"].values[0]
 
+            >>> # Fetch model versions with VGG backbone
+            ... models_table_df = project.fetch_model_versions_table(
+            ...     query="(backbone: string = VGG)"
+            ... ).to_pandas()
+
         See also the API referene:
             https://docs.neptune.ai/api/model/#fetch_model_versions_table
         """
+        verify_type("query", query, (str, type(None)))
         verify_type("limit", limit, (int, type(None)))
         verify_type("sort_by", sort_by, str)
         verify_type("ascending", ascending, bool)
         verify_type("progress_bar", progress_bar, (type(None), bool, type(ProgressBarCallback)))
 
         if isinstance(limit, int) and limit <= 0:
             raise ValueError(f"Parameter 'limit' must be a positive integer or None. Got {limit}.")
-        return MetadataContainer._fetch_entries(
+
+        query = query if query is not None else ""
+        nql = build_raw_query(query=query, trashed=False)
+        nql = NQLQueryAggregate(
+            items=[
+                nql,
+                NQLQueryAttribute(
+                    name="sys/model_id",
+                    value=self._sys_id,
+                    operator=NQLAttributeOperator.EQUALS,
+                    type=NQLAttributeType.STRING,
+                ),
+            ],
+            aggregator=NQLAggregator.AND,
+        )
+        return NeptuneObject._fetch_entries(
             self,
             child_type=ContainerType.MODEL_VERSION,
-            query=NQLQueryAggregate(
-                items=[
-                    NQLQueryAttribute(
-                        name="sys/model_id",
-                        value=self._sys_id,
-                        operator=NQLAttributeOperator.EQUALS,
-                        type=NQLAttributeType.STRING,
-                    ),
-                    NQLQueryAttribute(
-                        name="sys/trashed",
-                        type=NQLAttributeType.BOOLEAN,
-                        operator=NQLAttributeOperator.EQUALS,
-                        value=False,
-                    ),
-                ],
-                aggregator=NQLAggregator.AND,
-            ),
+            query=nql,
             columns=columns,
             limit=limit,
             sort_by=sort_by,
             ascending=ascending,
             progress_bar=progress_bar,
         )
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/model_version.py` & `neptune-2.0.0a0/src/neptune/objects/model_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,46 +24,47 @@
 
 from typing_extensions import Literal
 
 from neptune.attributes.constants import (
     SYSTEM_NAME_ATTRIBUTE_PATH,
     SYSTEM_STAGE_ATTRIBUTE_PATH,
 )
-from neptune.common.exceptions import NeptuneException
 from neptune.envs import CONNECTION_MODE
 from neptune.exceptions import (
     InactiveModelVersionException,
     NeedExistingModelVersionForReadOnlyMode,
     NeptuneMissingRequiredInitParameter,
     NeptuneOfflineModeChangeStageException,
+    NeptuneUnsupportedFunctionalityException,
 )
 from neptune.internal.backends.api_model import ApiExperiment
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.id_formats import QualifiedName
 from neptune.internal.init.parameters import (
     ASYNC_LAG_THRESHOLD,
     ASYNC_NO_PROGRESS_THRESHOLD,
     DEFAULT_FLUSH_PERIOD,
     DEFAULT_NAME,
     OFFLINE_PROJECT_QUALIFIED_NAME,
 )
 from neptune.internal.operation_processors.offline_operation_processor import OfflineOperationProcessor
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import verify_type
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
-from neptune.metadata_containers import MetadataContainer
-from neptune.metadata_containers.abstract import NeptuneObjectCallback
+from neptune.objects.abstract import NeptuneObjectCallback
+from neptune.objects.neptune_object import NeptuneObject
 from neptune.types.mode import Mode
 from neptune.types.model_version_stage import ModelVersionStage
 
 if TYPE_CHECKING:
     from neptune.internal.background_job import BackgroundJob
 
 
-class ModelVersion(MetadataContainer):
+class ModelVersion(NeptuneObject):
     """Initializes a ModelVersion object from an existing or new model version.
 
     Before creating model versions, you must first register a model by creating a Model object.
 
     A ModelVersion object is suitable for storing model metadata that is version-specific. It does not track
     background metrics or logs automatically, but you can assign metadata to the model version just like you can
     for runs. You can use the parent Model object to store metadata that is common to all versions of the model.
@@ -172,14 +173,17 @@
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
         async_lag_callback: Optional[NeptuneObjectCallback] = None,
         async_lag_threshold: float = ASYNC_LAG_THRESHOLD,
         async_no_progress_callback: Optional[NeptuneObjectCallback] = None,
         async_no_progress_threshold: float = ASYNC_NO_PROGRESS_THRESHOLD,
     ) -> None:
+
+        raise NeptuneUnsupportedFunctionalityException
+
         verify_type("with_id", with_id, (str, type(None)))
         verify_type("name", name, (str, type(None)))
         verify_type("model", model, (str, type(None)))
         verify_type("project", project, (str, type(None)))
         verify_type("mode", mode, (str, type(None)))
 
         self._model: Optional[str] = model
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/project.py` & `neptune-2.0.0a0/src/neptune/objects/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,49 +20,49 @@
     Iterable,
     Optional,
     Union,
 )
 
 from typing_extensions import Literal
 
-from neptune.common.exceptions import NeptuneException
 from neptune.envs import CONNECTION_MODE
-from neptune.exceptions import InactiveProjectException
-from neptune.internal.backends.api_model import ApiExperiment
-from neptune.internal.backends.nql import (
-    NQLAttributeOperator,
-    NQLAttributeType,
-    NQLEmptyQuery,
-    NQLQueryAttribute,
+from neptune.exceptions import (
+    InactiveProjectException,
+    NeptuneUnsupportedFunctionalityException,
 )
+from neptune.internal.backends.api_model import ApiExperiment
 from neptune.internal.container_type import ContainerType
+from neptune.internal.exceptions import NeptuneException
 from neptune.internal.init.parameters import (
     ASYNC_LAG_THRESHOLD,
     ASYNC_NO_PROGRESS_THRESHOLD,
     DEFAULT_FLUSH_PERIOD,
 )
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import (
     as_list,
     verify_collection_type,
     verify_type,
     verify_value,
 )
-from neptune.metadata_containers import MetadataContainer
-from neptune.metadata_containers.abstract import NeptuneObjectCallback
-from neptune.metadata_containers.metadata_containers_table import Table
-from neptune.metadata_containers.utils import prepare_nql_query
+from neptune.objects.abstract import NeptuneObjectCallback
+from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.utils import (
+    build_raw_query,
+    prepare_nql_query,
+)
+from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.typing import (
     ProgressBarCallback,
     ProgressBarType,
 )
 
 
-class Project(MetadataContainer):
+class Project(NeptuneObject):
     """Starts a connection to an existing Neptune project.
 
     You can use the Project object to retrieve information about runs, models, and model versions
     within the project.
 
     You can also log (and fetch) metadata common to the whole project, such as information about datasets,
     links to documents, or key project metrics.
@@ -148,14 +148,17 @@
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
         async_lag_callback: Optional[NeptuneObjectCallback] = None,
         async_lag_threshold: float = ASYNC_LAG_THRESHOLD,
         async_no_progress_callback: Optional[NeptuneObjectCallback] = None,
         async_no_progress_threshold: float = ASYNC_NO_PROGRESS_THRESHOLD,
     ):
+        if mode in {Mode.ASYNC.value, Mode.SYNC.value}:
+            raise NeptuneUnsupportedFunctionalityException
+
         verify_type("mode", mode, (str, type(None)))
 
         # make mode proper Enum instead of string
         mode = Mode(mode or os.getenv(CONNECTION_MODE) or Mode.ASYNC.value)
 
         if mode == Mode.OFFLINE:
             raise NeptuneException("Project can't be initialized in OFFLINE mode")
@@ -192,14 +195,15 @@
             workspace=self._workspace,
             project_name=self._project_name,
         )
 
     def fetch_runs_table(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[Union[str, Iterable[str]]] = None,
         state: Optional[Union[Literal["inactive", "active"], Iterable[Literal["inactive", "active"]]]] = None,
         owner: Optional[Union[str, Iterable[str]]] = None,
         tag: Optional[Union[str, Iterable[str]]] = None,
         columns: Optional[Iterable[str]] = None,
         trashed: Optional[bool] = False,
         limit: Optional[int] = None,
@@ -209,14 +213,17 @@
     ) -> Table:
         """Retrieve runs matching the specified criteria.
 
         All parameters are optional. Each of them specifies a single criterion.
         Only runs matching all of the criteria will be returned.
 
         Args:
+            query: NQL query string. Syntax: https://docs.neptune.ai/usage/nql/
+                Example: `"(accuracy: float > 0.88) AND (loss: float < 0.2)"`.
+                Exclusive with the `id`, `state`, `owner`, and `tag` parameters.
             id: Neptune ID of a run, or list of several IDs.
                 Example: `"SAN-1"` or `["SAN-1", "SAN-2"]`.
                 Matching any element of the list is sufficient to pass the criterion.
             state: Run state, or list of states.
                 Example: `"active"`.
                 Possible values: `"inactive"`, `"active"`.
                 Matching any element of the list is sufficient to pass the criterion.
@@ -225,15 +232,15 @@
                 The owner is the user who created the run.
                 Matching any element of the list is sufficient to pass the criterion.
             tag: A tag or list of tags applied to the run.
                 Example: `"lightGBM"` or `["pytorch", "cycleLR"]`.
                 Only runs that have all specified tags will match this criterion.
             columns: Names of columns to include in the table, as a list of field names.
                 The Neptune ID ("sys/id") is included automatically.
-                If `None` (default), all the columns of the runs table are included.
+                If `None` (default), all the columns of the runs table are included, up to a maximum of 10 000 columns.
             trashed: Whether to retrieve trashed runs.
                 If `True`, only trashed runs are retrieved.
                 If `False` (default), only not-trashed runs are retrieved.
                 If `None`, both trashed and not-trashed runs are retrieved.
             limit: How many entries to return at most. If `None`, all entries are returned.
             sort_by: Name of the field to sort the results by.
                 The field must represent a simple type (string, float, datetime, integer, or Boolean).
@@ -284,65 +291,78 @@
 
             >>> # You can combine conditions. Runs satisfying all conditions will be fetched
             ... runs_table_df = project.fetch_runs_table(state="inactive", tag="Exploration").to_pandas()
 
         See also the API reference in the docs:
             https://docs.neptune.ai/api/project#fetch_runs_table
         """
+
+        if any((id, state, owner, tag)) and query is not None:
+            raise ValueError(
+                "You can't use the 'query' parameter together with the 'id', 'state', 'owner', or 'tag' parameters."
+            )
+
         ids = as_list("id", id)
         states = as_list("state", state)
         owners = as_list("owner", owner)
         tags = as_list("tag", tag)
 
+        verify_type("query", query, (str, type(None)))
         verify_type("trashed", trashed, (bool, type(None)))
         verify_type("limit", limit, (int, type(None)))
         verify_type("sort_by", sort_by, str)
         verify_type("ascending", ascending, bool)
         verify_type("progress_bar", progress_bar, (type(None), bool, type(ProgressBarCallback)))
         verify_collection_type("state", states, str)
 
-        for state in states:
-            verify_value("state", state.lower(), ("inactive", "active"))
-
         if isinstance(limit, int) and limit <= 0:
             raise ValueError(f"Parameter 'limit' must be a positive integer or None. Got {limit}.")
 
-        nql_query = prepare_nql_query(ids, states, owners, tags, trashed)
+        for state in states:
+            verify_value("state", state.lower(), ("inactive", "active"))
+
+        if query is not None:
+            nql_query = build_raw_query(query, trashed=trashed)
+        else:
+            nql_query = prepare_nql_query(ids, states, owners, tags, trashed)
 
-        return MetadataContainer._fetch_entries(
+        return NeptuneObject._fetch_entries(
             self,
             child_type=ContainerType.RUN,
             query=nql_query,
             columns=columns,
             limit=limit,
             sort_by=sort_by,
             ascending=ascending,
             progress_bar=progress_bar,
         )
 
     def fetch_models_table(
         self,
         *,
+        query: Optional[str] = None,
         columns: Optional[Iterable[str]] = None,
         trashed: Optional[bool] = False,
         limit: Optional[int] = None,
         sort_by: str = "sys/creation_time",
         ascending: bool = False,
         progress_bar: Optional[ProgressBarType] = None,
     ) -> Table:
         """Retrieve models stored in the project.
 
         Args:
+            query: NQL query string. Syntax: https://docs.neptune.ai/usage/nql/
+                Example: `"(model_size: float > 100) AND (backbone: string = VGG)"`.
             trashed: Whether to retrieve trashed models.
                 If `True`, only trashed models are retrieved.
                 If `False`, only not-trashed models are retrieved.
                 If `None`, both trashed and not-trashed models are retrieved.
             columns: Names of columns to include in the table, as a list of field names.
                 The Neptune ID ("sys/id") is included automatically.
-                If `None`, all the columns of the models table are included.
+                If `None`, all the columns of the models table are included, up to a maximum of 10 000 columns.
             limit: How many entries to return at most. If `None`, all entries are returned.
             sort_by: Name of the field to sort the results by.
                 The field must represent a simple type (string, float, datetime, integer, or Boolean).
             ascending: Whether to sort the entries in ascending order of the sorting column values.
             progress_bar: Set to `False` to disable the download progress bar,
                 or pass a `ProgressBarCallback` class to use your own progress bar callback.
 
@@ -365,35 +385,36 @@
             >>> # Fetch 10 oldest model objects
             ... models_table_df = project.fetch_models_table(
             ...     sort_by="sys/creation_time", ascending=True, limit=10
             ...  ).to_pandas()
             ... # Extract the ID of the first listed (oldest) model object
             ... last_model_id = models_table_df["sys/id"].values[0]
 
+            >>> # Fetch models with VGG backbone
+            ... models_table_df = project.fetch_models_table(
+                    query="(backbone: string = VGG)"
+                ).to_pandas()
+
         See also the API reference in the docs:
             https://docs.neptune.ai/api/project#fetch_models_table
         """
+        verify_type("query", query, (str, type(None)))
         verify_type("limit", limit, (int, type(None)))
         verify_type("sort_by", sort_by, str)
         verify_type("ascending", ascending, bool)
         verify_type("progress_bar", progress_bar, (type(None), bool, type(ProgressBarCallback)))
 
         if isinstance(limit, int) and limit <= 0:
             raise ValueError(f"Parameter 'limit' must be a positive integer or None. Got {limit}.")
 
-        return MetadataContainer._fetch_entries(
+        query = query if query is not None else ""
+        nql = build_raw_query(query=query, trashed=trashed)
+        return NeptuneObject._fetch_entries(
             self,
             child_type=ContainerType.MODEL,
-            query=NQLQueryAttribute(
-                name="sys/trashed",
-                type=NQLAttributeType.BOOLEAN,
-                operator=NQLAttributeOperator.EQUALS,
-                value=trashed,
-            )
-            if trashed is not None
-            else NQLEmptyQuery,
+            query=nql,
             columns=columns,
             limit=limit,
             sort_by=sort_by,
             ascending=ascending,
             progress_bar=progress_bar,
         )
```

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/structure_version.py` & `neptune-2.0.0a0/src/neptune/objects/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/metadata_containers/utils.py` & `neptune-2.0.0a0/src/neptune/objects/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,48 +11,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 __all__ = [
-    "DATE_FORMAT",
-    "parse_dates",
     "prepare_nql_query",
 ]
 
-from datetime import datetime
 from typing import (
-    Generator,
     Iterable,
     List,
     Optional,
     Union,
 )
 
-from neptune.common.warnings import (
-    NeptuneWarning,
-    warn_once,
-)
-from neptune.internal.backends.api_model import (
-    AttributeType,
-    AttributeWithProperties,
-    LeaderboardEntry,
-)
 from neptune.internal.backends.nql import (
     NQLAggregator,
     NQLAttributeOperator,
     NQLAttributeType,
+    NQLQuery,
     NQLQueryAggregate,
     NQLQueryAttribute,
+    RawNQLQuery,
 )
 from neptune.internal.utils.run_state import RunState
 
-DATE_FORMAT: str = "%Y-%m-%dT%H:%M:%S.%fZ"
-
 
 def prepare_nql_query(
     ids: Optional[Iterable[str]],
     states: Optional[Iterable[str]],
     owners: Optional[Iterable[str]],
     tags: Optional[Iterable[str]],
     trashed: Optional[bool],
@@ -133,39 +120,23 @@
             )
         )
 
     query = NQLQueryAggregate(items=query_items, aggregator=NQLAggregator.AND)
     return query
 
 
-def parse_dates(leaderboard_entries: Iterable[LeaderboardEntry]) -> Generator[LeaderboardEntry, None, None]:
-    yield from [_parse_entry(entry) for entry in leaderboard_entries]
+def build_raw_query(query: str, trashed: Optional[bool]) -> NQLQuery:
+    raw_nql = RawNQLQuery(query)
 
+    if trashed is None:
+        return raw_nql
 
-def _parse_entry(entry: LeaderboardEntry) -> LeaderboardEntry:
-    try:
-        return LeaderboardEntry(
-            entry.id,
-            attributes=[
-                AttributeWithProperties(
-                    attribute.path,
-                    attribute.type,
-                    {
-                        **attribute.properties,
-                        "value": datetime.strptime(attribute.properties["value"], DATE_FORMAT),
-                    },
-                )
-                if attribute.type == AttributeType.DATETIME
-                else attribute
-                for attribute in entry.attributes
-            ],
-        )
-    except TypeError:
-        # date is already in the right format
-        return entry
-    except ValueError:
-        # the parsing format is incorrect
-        warn_once(
-            "Date parsing failed. The date format is incorrect. Returning as string instead of datetime.",
-            exception=NeptuneWarning,
-        )
-        return entry
+    nql = NQLQueryAggregate(
+        items=[
+            raw_nql,
+            NQLQueryAttribute(
+                name="sys/trashed", type=NQLAttributeType.BOOLEAN, operator=NQLAttributeOperator.EQUALS, value=trashed
+            ),
+        ],
+        aggregator=NQLAggregator.AND,
+    )
+    return nql
```

### Comparing `neptune-1.9.1/src/neptune/new/utils.py` & `neptune-2.0.0a0/src/neptune/types/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,10 +9,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["stringify_unsupported"]
+__all__ = [
+    "Artifact",
+    "Boolean",
+    "Datetime",
+    "File",
+    "Float",
+    "GitRef",
+    "Integer",
+    "String",
+    "FileSet",
+    "StringSet",
+    "FileSeries",
+    "FloatSeries",
+    "StringSeries",
+]
 
-from neptune.utils import stringify_unsupported
+
+from .atoms import (
+    Artifact,
+    Boolean,
+    Datetime,
+    File,
+    Float,
+    GitRef,
+    Integer,
+    String,
+)
+from .file_set import FileSet
+from .series import (
+    FileSeries,
+    FloatSeries,
+    StringSeries,
+)
+from .sets import StringSet
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/artifact.py` & `neptune-2.0.0a0/src/neptune/types/atoms/datetime.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,48 +9,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Artifact"]
+__all__ = ["Datetime"]
 
 from dataclasses import dataclass
+from datetime import datetime
 from typing import (
     TYPE_CHECKING,
-    Optional,
     TypeVar,
     Union,
 )
 
-from neptune.internal.artifacts.file_hasher import FileHasher
 from neptune.internal.types.stringify_value import (
     StringifyValue,
     extract_if_stringify_value,
 )
 from neptune.types.atoms.atom import Atom
 
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
 @dataclass
-class Artifact(Atom):
+class Datetime(Atom):
+    value: datetime
 
-    hash: str
-
-    def __init__(self, value: Union[Optional[str], StringifyValue] = None):
+    def __init__(self, value: Union[datetime, StringifyValue]):
         value = extract_if_stringify_value(value)
-
-        self.hash = str(value)
-        assert (
-            len(self.hash) == FileHasher.HASH_LENGTH or value is None
-        ), "Expected sha-256 string. E.g. 'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'"
+        self.value = value.replace(microsecond=1000 * int(value.microsecond / 1000))
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_artifact(self)
+        return visitor.visit_datetime(self)
 
     def __str__(self):
-        return "Artifact({})".format(self.hash)
+        return "Datetime({})".format(str(self.value))
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/atom.py` & `neptune-2.0.0a0/src/neptune/types/series/series.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Atom"]
+__all__ = ["Series"]
 
 import abc
 from typing import (
     TYPE_CHECKING,
     TypeVar,
 )
 
@@ -25,11 +25,29 @@
 
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
-class Atom(Value):
+class Series(Value):
     @abc.abstractmethod
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
         pass
+
+    @property
+    @abc.abstractmethod
+    def values(self):
+        pass
+
+    @property
+    @abc.abstractmethod
+    def steps(self):
+        pass
+
+    @property
+    @abc.abstractmethod
+    def timestamps(self):
+        pass
+
+    def __len__(self):
+        return len(self.values)
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/boolean.py` & `neptune-2.0.0a0/src/neptune/types/atoms/integer.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Boolean"]
+__all__ = ["Integer"]
 
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     TypeVar,
 )
 
@@ -27,22 +27,22 @@
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
 @dataclass
-class Boolean(Atom):
+class Integer(Atom):
 
-    value: bool
+    value: int
 
     def __init__(self, value):
-        self.value = bool(extract_if_stringify_value(value))
+        self.value = int(extract_if_stringify_value(value))
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_boolean(self)
+        return visitor.visit_integer(self)
 
     def __str__(self):
-        return "Boolean({})".format(str(self.value))
+        return "Integer({})".format(str(self.value))
 
-    def __bool__(self):
+    def __int__(self):
         return self.value
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/datetime.py` & `neptune-2.0.0a0/src/neptune/types/namespace.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,42 +9,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Datetime"]
+__all__ = ["Namespace"]
 
 from dataclasses import dataclass
-from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     TypeVar,
-    Union,
 )
 
-from neptune.internal.types.stringify_value import (
-    StringifyValue,
-    extract_if_stringify_value,
-)
-from neptune.types.atoms.atom import Atom
+from neptune.internal.utils.logger import get_logger
+from neptune.internal.utils.paths import parse_path
+from neptune.types.value import Value
 
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
+logger = get_logger()
 Ret = TypeVar("Ret")
 
 
 @dataclass
-class Datetime(Atom):
-    value: datetime
+class Namespace(Value):
+
+    value: dict
 
-    def __init__(self, value: Union[datetime, StringifyValue]):
-        value = extract_if_stringify_value(value)
-        self.value = value.replace(microsecond=1000 * int(value.microsecond / 1000))
+    def __init__(self, value):
+        self.value = value
+        empty_keys = [k for k in self.value.keys() if not parse_path(k)]
+        if empty_keys:
+            all_keys = ", ".join(['"' + k + '"' for k in empty_keys])
+            logger.warning(
+                f"Key(s) {all_keys} can't be used in Namespaces and dicts stored in Neptune. Please use non-empty "
+                f"keys instead. The value(s) will be dropped.",
+            )
+            self.value = value.copy()
+            [self.value.pop(key) for key in empty_keys]
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_datetime(self)
+        return visitor.visit_namespace(self)
 
     def __str__(self):
-        return "Datetime({})".format(str(self.value))
+        return "Namespace({})".format(str(self.value))
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/file.py` & `neptune-2.0.0a0/src/neptune/types/atoms/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,26 +167,29 @@
         verify_type("seek", seek, (int, type(None)))
         verify_type("extension", extension, (str, type(None)))
 
         file_composite = StreamComposite(stream, seek, extension)
         return File(file_composite=file_composite)
 
     @staticmethod
-    def as_image(image) -> "File":
+    def as_image(image, autoscale: bool = True) -> "File":
         """Static method for converting image objects or image-like objects to an image File value object.
 
-        This way you can upload `Matplotlib` figures, `Seaborn` figures, `PIL` images, `NumPy` arrays, as static images.
+        This way you can upload Matplotlib figures, Seaborn figures, PIL images, and NumPy arrays as static images.
 
         Args:
             image: Image-like object to be converted.
-                Supported are `PyTorch` tensors, `TensorFlow/Keras` tensors, `NumPy` arrays, `PIL` images,
-                `Matplotlib` figures and `Seaborn` figures.
+                The input image pixel must be either in range [0.0, 1.0] (float) or [0, 255] (integer).
+                Supported are PyTorch tensors, TensorFlow/Keras tensors, NumPy arrays, PIL images,
+                Matplotlib figures and Seaborn figures.
+            autoscale: Whether Neptune should try to detect the pixel range automatically
+                and scale it to an acceptable format.
 
         Returns:
-            ``File``: value object with converted image
+            `File`: value object with converted image
 
         Examples:
             >>> import neptune
             >>> from neptune.types import File
             >>> run = neptune.init_run()
 
             Convert NumPy array to File value object and upload it
@@ -194,24 +197,23 @@
             >>> run["train/prediction_example"].upload(File.as_image(numpy_array))
 
             Convert PIL image to File value object and upload it
 
             >>> pil_file = File.as_image(pil_image)
             >>> run["dataset/data_sample/img1"].upload(pil_file)
 
-            You can upload PIL image without explicit conversion
+            You can upload PIL images without explicit conversion
 
             >>> run["dataset/data_sample/img2"].upload(pil_image)
 
-        You may also want to check `as_image docs page`_.
-
-        .. _as_image docs page:
-           https://docs.neptune.ai/api/field_types#as_image
+        See also the docs:
+            - How to log images: https://docs.neptune.ai/logging/images/
+            - API referene: https://docs.neptune.ai/api/field_types#as_image
         """
-        content_bytes = get_image_content(image)
+        content_bytes = get_image_content(image, autoscale=autoscale)
         return File.from_content(content_bytes if content_bytes is not None else b"", extension="png")
 
     @staticmethod
     def as_html(chart) -> "File":
         """Converts an object to an HTML File value object.
 
         This way you can upload `Altair`, `Bokeh`, `Plotly`, `Matplotlib`, `Seaborn` interactive charts
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/float.py` & `neptune-2.0.0a0/src/neptune/types/value_copy.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,40 +9,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Float"]
+__all__ = ["ValueCopy"]
 
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     TypeVar,
 )
 
-from neptune.internal.types.stringify_value import extract_if_stringify_value
-from neptune.types.atoms.atom import Atom
+from neptune.internal.utils.paths import parse_path
+from neptune.types.value import Value
 
 if TYPE_CHECKING:
+    from neptune.handler import Handler
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
 @dataclass
-class Float(Atom):
+class ValueCopy(Value):
 
-    value: float
+    source_handler: "Handler"
 
-    def __init__(self, value):
-        self.value = float(extract_if_stringify_value(value))
+    def __init__(self, source_handler: "Handler"):
+        self.source_handler = source_handler
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_float(self)
+        source_path = self.source_handler._path
+        source_attr = self.source_handler._container.get_attribute(source_path)
+        if source_attr and source_attr.supports_copy:
+            return visitor.copy_value(source_type=type(source_attr), source_path=parse_path(source_path))
+        else:
+            raise Exception(f"{type(source_attr).__name__} doesn't support copying")
 
     def __str__(self):
-        return "Float({})".format(str(self.value))
-
-    def __float__(self):
-        return self.value
+        return "Copy({})".format(str(self.source_handler))
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/git_ref.py` & `neptune-2.0.0a0/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/atoms/integer.py` & `neptune-2.0.0a0/src/neptune/types/file_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,40 +9,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Integer"]
+__all__ = [
+    "FileSet",
+]
 
-from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
+    Iterable,
+    List,
     TypeVar,
+    Union,
 )
 
-from neptune.internal.types.stringify_value import extract_if_stringify_value
-from neptune.types.atoms.atom import Atom
+from neptune.internal.utils import (
+    verify_collection_type,
+    verify_type,
+)
+from neptune.types.value import Value
 
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
-@dataclass
-class Integer(Atom):
-
-    value: int
-
-    def __init__(self, value):
-        self.value = int(extract_if_stringify_value(value))
+class FileSet(Value):
+    def __init__(self, file_globs: Union[str, Iterable[str]]):
+        verify_type("file_globs", file_globs, (str, Iterable))
+        if isinstance(file_globs, str):
+            file_globs = [file_globs]
+        else:
+            verify_collection_type("file_globs", file_globs, str)
+        self.file_globs: List[str] = list(file_globs)
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_integer(self)
+        return visitor.visit_file_set(self)
 
     def __str__(self):
-        return "Integer({})".format(str(self.value))
-
-    def __int__(self):
-        return self.value
+        return "FileSet({})".format(str(self.file_globs))
```

### Comparing `neptune-1.9.1/src/neptune/types/atoms/string.py` & `neptune-2.0.0a0/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/mode.py` & `neptune-2.0.0a0/src/neptune/integrations/mosaicml/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2024, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Mode"]
+__all__ = ["NeptuneLogger"]
 
-from enum import Enum
+from neptune.internal.utils.requirement_check import require_installed
 
+require_installed("mosaicml")
 
-class Mode(str, Enum):
-    OFFLINE = "offline"
-    DEBUG = "debug"
-    ASYNC = "async"
-    SYNC = "sync"
-    READ_ONLY = "read-only"
-
-    def __repr__(self):
-        return f'"{self.value}"'
+from composer.loggers import NeptuneLogger  # noqa: F401,F403,E402
```

### Comparing `neptune-1.9.1/src/neptune/types/series/file_series.py` & `neptune-2.0.0a0/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/series/float_series.py` & `neptune-2.0.0a0/src/neptune/types/series/float_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     TYPE_CHECKING,
     Optional,
     Sequence,
     TypeVar,
     Union,
 )
 
-from neptune.common.warnings import (
-    NeptuneUnsupportedValue,
-    warn_once,
-)
 from neptune.internal.types.stringify_value import extract_if_stringify_value
 from neptune.internal.types.utils import is_unsupported_float
 from neptune.internal.utils import is_collection
+from neptune.internal.warnings import (
+    NeptuneUnsupportedValue,
+    warn_once,
+)
 from neptune.types.series.series import Series
 
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
```

### Comparing `neptune-1.9.1/src/neptune/types/series/series_value.py` & `neptune-2.0.0a0/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/series/string_series.py` & `neptune-2.0.0a0/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/type_casting.py` & `neptune-2.0.0a0/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/types/value_visitor.py` & `neptune-2.0.0a0/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/typing.py` & `neptune-2.0.0a0/src/neptune/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["SupportsNamespaces", "NeptuneObject", "NeptuneObjectCallback", "ProgressBarCallback", "ProgressBarType"]
+__all__ = [
+    "SupportsNamespaces",
+    "AbstractNeptuneObject",
+    "NeptuneObjectCallback",
+    "ProgressBarCallback",
+    "ProgressBarType",
+]
 
 import abc
 import contextlib
 from typing import (
     Any,
     Optional,
     Type,
     Union,
 )
 
 from typing_extensions import TypeAlias
 
-from neptune.metadata_containers.abstract import (
-    NeptuneObject,
+from neptune.objects.abstract import (
+    AbstractNeptuneObject,
     NeptuneObjectCallback,
     SupportsNamespaces,
 )
 
 
 class ProgressBarCallback(contextlib.AbstractContextManager):
     """Abstract base class for progress bar callbacks.
@@ -74,16 +80,14 @@
         ...     project.fetch_runs_table(progress_bar=ClickProgressBar)
         ...     project.fetch_models_table(progress_bar=ClickProgressBar)
 
         IMPORTANT: Pass a type, not an instance to the `progress_bar` argument.
         That is, `ClickProgressBar`, not `ClickProgressBar()`.
     """
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        ...
+    def __init__(self, *args: Any, **kwargs: Any) -> None: ...
 
     @abc.abstractmethod
-    def update(self, *, by: int, total: Optional[int] = None) -> None:
-        ...
+    def update(self, *, by: int, total: Optional[int] = None) -> None: ...
 
 
 ProgressBarType: TypeAlias = Union[bool, Type[ProgressBarCallback]]
```

### Comparing `neptune-1.9.1/src/neptune/utils.py` & `neptune-2.0.0a0/src/neptune/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,16 @@
     Type,
     Union,
 )
 
 from neptune.internal.init.parameters import DEFAULT_STOP_TIMEOUT
 from neptune.internal.types.stringify_value import StringifyValue
 from neptune.internal.utils.logger import get_logger
-from neptune.internal.utils.runningmode import (
-    in_interactive,
-    in_notebook,
-)
 from neptune.typing import (
-    NeptuneObject,
+    AbstractNeptuneObject,
     ProgressBarCallback,
 )
 
 logger = get_logger()
 
 
 def stringify_unsupported(value: Any) -> Union[StringifyValue, Mapping]:
@@ -56,25 +52,22 @@
         >>> import neptune
         >>> run = neptune.init_run()
         >>> complex_dict = {"tuple": ("hi", 1), "metric": 0.87}
         >>> run["complex_dict"] = complex_dict
         >>> # (as of 1.0.0) error - tuple is not a supported type
         ... from neptune.utils import stringify_unsupported
         >>> run["complex_dict"] = stringify_unsupported(complex_dict)
-
-        For more information, see:
-        https://docs.neptune.ai/setup/neptune-client_1-0_release_changes/#no-more-implicit-casting-to-string
     """
     if isinstance(value, MutableMapping):
         return {str(k): stringify_unsupported(v) for k, v in value.items()}
 
     return StringifyValue(value=value)
 
 
-def stop_synchronization_callback(neptune_object: NeptuneObject) -> None:
+def stop_synchronization_callback(neptune_object: AbstractNeptuneObject) -> None:
     """Default callback function that stops a Neptune object's synchronization with the server.
 
     Args:
         neptune_object: A Neptune object (Run, Model, ModelVersion, or Project) to be stopped.
 
     Example:
         >>> import neptune
@@ -114,20 +107,16 @@
         *args: Any,
         description: Optional[str] = None,
         unit: Optional[str] = None,
         unit_scale: bool = False,
         **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
-        interactive = in_interactive() or in_notebook()
 
-        if interactive:
-            from tqdm.notebook import tqdm
-        else:
-            from tqdm import tqdm  # type: ignore
+        from tqdm.auto import tqdm
 
         unit = unit if unit else ""
 
         self._progress_bar = tqdm(desc=description, unit=unit, unit_scale=unit_scale, **kwargs)
 
     def __enter__(self) -> "TqdmProgressBar":
         self._progress_bar.__enter__()
```

### Comparing `neptune-1.9.1/src/neptune/vendor/lib_programname.py` & `neptune-2.0.0a0/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/vendor/pynvml.py` & `neptune-2.0.0a0/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-1.9.1/src/neptune/version.py` & `neptune-2.0.0a0/src/neptune/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 __all__ = ["version", "__version__"]
 
 import sys
 from typing import Optional
 
 from packaging.version import parse
 
-from neptune.common.warnings import warn_once
-
 if sys.version_info >= (3, 8):
     from importlib.metadata import PackageNotFoundError
     from importlib.metadata import version as version_parser
 else:
     from importlib_metadata import PackageNotFoundError
     from importlib_metadata import version as version_parser
 
@@ -36,29 +34,16 @@
     except PackageNotFoundError:
         # package is not installed
         return None
 
 
 def detect_version() -> str:
     neptune_version = check_version("neptune")
-    neptune_client_version = check_version("neptune-client")
 
-    if neptune_version is not None and neptune_client_version is not None:
-        raise RuntimeError(
-            "We've detected that the 'neptune' and 'neptune-client' packages are both installed. "
-            "Uninstall each of them and then install only the new 'neptune' package. For more information, "
-            "see https://docs.neptune.ai/setup/upgrading/"
-        )
-    elif neptune_version is not None:
+    if neptune_version is not None:
         return neptune_version
-    elif neptune_client_version is not None:
-        warn_once(
-            "The 'neptune-client' package has been deprecated and will be removed in the future. Install "
-            "the 'neptune' package instead. For more, see https://docs.neptune.ai/setup/upgrading/"
-        )
-        return neptune_client_version
 
     raise PackageNotFoundError("neptune")
 
 
 __version__ = detect_version()
 version = parse(__version__)
```

### Comparing `neptune-1.9.1/PKG-INFO` & `neptune-2.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 1.9.1
+Version: 2.0.0a0
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -32,14 +32,15 @@
 Provides-Extra: aws
 Provides-Extra: detectron2
 Provides-Extra: experimental
 Provides-Extra: fastai
 Provides-Extra: kedro
 Provides-Extra: lightgbm
 Provides-Extra: mlflow
+Provides-Extra: mosaicml
 Provides-Extra: optuna
 Provides-Extra: prophet
 Provides-Extra: pytorch
 Provides-Extra: pytorch-lightning
 Provides-Extra: sacred
 Provides-Extra: sklearn
 Provides-Extra: tensorboard
@@ -49,17 +50,17 @@
 Provides-Extra: zenml
 Requires-Dist: GitPython (>=2.0.8)
 Requires-Dist: Pillow (>=1.1.6)
 Requires-Dist: PyJWT
 Requires-Dist: boto3 (>=1.28.0)
 Requires-Dist: bravado (>=11.0.0,<12.0.0)
 Requires-Dist: click (>=7.0)
-Requires-Dist: future (>=0.17.1)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
-Requires-Dist: kedro-neptune ; (python_version < "3.11") and (extra == "kedro")
+Requires-Dist: kedro-neptune ; (python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
+Requires-Dist: mosaicml ; extra == "mosaicml"
 Requires-Dist: neptune-airflow ; extra == "airflow"
 Requires-Dist: neptune-aws ; extra == "aws"
 Requires-Dist: neptune-detectron2 ; (python_version >= "3.7") and (extra == "detectron2")
 Requires-Dist: neptune-fastai ; extra == "fastai"
 Requires-Dist: neptune-lightgbm ; extra == "lightgbm"
 Requires-Dist: neptune-mlflow ; extra == "mlflow"
 Requires-Dist: neptune-optuna ; extra == "optuna"
@@ -69,19 +70,20 @@
 Requires-Dist: neptune-sklearn ; extra == "sklearn"
 Requires-Dist: neptune-tensorboard ; extra == "tensorboard"
 Requires-Dist: neptune-tensorflow-keras ; extra == "tensorflow-keras"
 Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0)
 Requires-Dist: packaging
 Requires-Dist: pandas
+Requires-Dist: protobuf (>=4.0.0,<5.0.0)
 Requires-Dist: psutil
 Requires-Dist: pytorch-lightning ; extra == "pytorch-lightning"
 Requires-Dist: requests (>=2.20.0)
 Requires-Dist: requests-oauthlib (>=1.0.0)
-Requires-Dist: six (>=1.12.0)
+Requires-Dist: setuptools ; python_version >= "3.12"
 Requires-Dist: swagger-spec-validator (>=2.7.4)
 Requires-Dist: transformers ; extra == "transformers"
 Requires-Dist: typing-extensions (>=3.10.0)
 Requires-Dist: urllib3
 Requires-Dist: websocket-client (>=0.35.0,!=1.0.0)
 Requires-Dist: zenml ; extra == "zenml"
 Project-URL: Documentation, https://docs.neptune.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neptune Version: 1.9.1 Summary: Neptune Client
+Metadata-Version: 2.1 Name: neptune Version: 2.0.0a0 Summary: Neptune Client
 Home-page: https://neptune.ai/ License: Apache-2.0 Keywords: MLOps,ML
 Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store Author:
 neptune.ai Author-email: contact@neptune.ai Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
@@ -14,44 +14,45 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Provides-Extra: airflow Provides-
 Extra: aws Provides-Extra: detectron2 Provides-Extra: experimental Provides-
 Extra: fastai Provides-Extra: kedro Provides-Extra: lightgbm Provides-Extra:
-mlflow Provides-Extra: optuna Provides-Extra: prophet Provides-Extra: pytorch
-Provides-Extra: pytorch-lightning Provides-Extra: sacred Provides-Extra:
-sklearn Provides-Extra: tensorboard Provides-Extra: tensorflow-keras Provides-
-Extra: transformers Provides-Extra: xgboost Provides-Extra: zenml Requires-
-Dist: GitPython (>=2.0.8) Requires-Dist: Pillow (>=1.1.6) Requires-Dist: PyJWT
-Requires-Dist: boto3 (>=1.28.0) Requires-Dist: bravado (>=11.0.0,<12.0.0)
-Requires-Dist: click (>=7.0) Requires-Dist: future (>=0.17.1) Requires-Dist:
-importlib-metadata ; python_version < "3.8" Requires-Dist: kedro-neptune ;
-(python_version < "3.11") and (extra == "kedro") Requires-Dist: neptune-airflow
-; extra == "airflow" Requires-Dist: neptune-aws ; extra == "aws" Requires-Dist:
+mlflow Provides-Extra: mosaicml Provides-Extra: optuna Provides-Extra: prophet
+Provides-Extra: pytorch Provides-Extra: pytorch-lightning Provides-Extra:
+sacred Provides-Extra: sklearn Provides-Extra: tensorboard Provides-Extra:
+tensorflow-keras Provides-Extra: transformers Provides-Extra: xgboost Provides-
+Extra: zenml Requires-Dist: GitPython (>=2.0.8) Requires-Dist: Pillow (>=1.1.6)
+Requires-Dist: PyJWT Requires-Dist: boto3 (>=1.28.0) Requires-Dist: bravado
+(>=11.0.0,<12.0.0) Requires-Dist: click (>=7.0) Requires-Dist: importlib-
+metadata ; python_version < "3.8" Requires-Dist: kedro-neptune ;
+(python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
+Requires-Dist: mosaicml ; extra == "mosaicml" Requires-Dist: neptune-airflow ;
+extra == "airflow" Requires-Dist: neptune-aws ; extra == "aws" Requires-Dist:
 neptune-detectron2 ; (python_version >= "3.7") and (extra == "detectron2")
 Requires-Dist: neptune-fastai ; extra == "fastai" Requires-Dist: neptune-
 lightgbm ; extra == "lightgbm" Requires-Dist: neptune-mlflow ; extra ==
 "mlflow" Requires-Dist: neptune-optuna ; extra == "optuna" Requires-Dist:
 neptune-prophet ; extra == "prophet" Requires-Dist: neptune-pytorch ; extra ==
 "pytorch" Requires-Dist: neptune-sacred ; extra == "sacred" Requires-Dist:
 neptune-sklearn ; extra == "sklearn" Requires-Dist: neptune-tensorboard ; extra
 == "tensorboard" Requires-Dist: neptune-tensorflow-keras ; extra ==
 "tensorflow-keras" Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0) Requires-Dist: packaging Requires-Dist:
-pandas Requires-Dist: psutil Requires-Dist: pytorch-lightning ; extra ==
-"pytorch-lightning" Requires-Dist: requests (>=2.20.0) Requires-Dist: requests-
-oauthlib (>=1.0.0) Requires-Dist: six (>=1.12.0) Requires-Dist: swagger-spec-
-validator (>=2.7.4) Requires-Dist: transformers ; extra == "transformers"
-Requires-Dist: typing-extensions (>=3.10.0) Requires-Dist: urllib3 Requires-
-Dist: websocket-client (>=0.35.0,!=1.0.0) Requires-Dist: zenml ; extra ==
-"zenml" Project-URL: Documentation, https://docs.neptune.ai/ Project-URL:
-Repository, https://github.com/neptune-ai/neptune-client Project-URL: Tracker,
-https://github.com/neptune-ai/neptune-client/issues Description-Content-Type:
-text/markdown
+pandas Requires-Dist: protobuf (>=4.0.0,<5.0.0) Requires-Dist: psutil Requires-
+Dist: pytorch-lightning ; extra == "pytorch-lightning" Requires-Dist: requests
+(>=2.20.0) Requires-Dist: requests-oauthlib (>=1.0.0) Requires-Dist: setuptools
+; python_version >= "3.12" Requires-Dist: swagger-spec-validator (>=2.7.4)
+Requires-Dist: transformers ; extra == "transformers" Requires-Dist: typing-
+extensions (>=3.10.0) Requires-Dist: urllib3 Requires-Dist: websocket-client
+(>=0.35.0,!=1.0.0) Requires-Dist: zenml ; extra == "zenml" Project-URL:
+Documentation, https://docs.neptune.ai/ Project-URL: Repository, https://
+github.com/neptune-ai/neptune-client Project-URL: Tracker, https://github.com/
+neptune-ai/neptune-client/issues Description-Content-Type: text/markdown
   [https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/
                                Github-cover.png]
                            ************ nneeppttuunnee..aaii ************
    _Q_u_i_c_k_s_t_a_r_t   â¢   _W_e_b_s_i_t_e   â¢   _D_o_c_s   â¢   _E_x_a_m_p_l_e_s   â¢   _R_e_s_o_u_r_c_e
                              _c_e_n_t_e_r   â¢   _B_l_o_g  
 ===============================================================================
 ## What is neptune.ai? Neptune is a lightweight experiment tracker for ML teams
```

