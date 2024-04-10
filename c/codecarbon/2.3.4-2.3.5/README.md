# Comparing `tmp/codecarbon-2.3.4.tar.gz` & `tmp/codecarbon-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.3.4.tar", last modified: Tue Jan 30 19:21:45 2024, max compression
+gzip compressed data, was "codecarbon-2.3.5.tar", last modified: Wed Apr 10 07:19:31 2024, max compression
```

## Comparing `codecarbon-2.3.4.tar` & `codecarbon-2.3.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.444359 codecarbon-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-30 19:21:34.000000 codecarbon-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-01-30 19:21:45.444359 codecarbon-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-01-30 19:21:34.000000 codecarbon-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.424359 codecarbon-2.3.4/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.424359 codecarbon-2.3.4/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.428360 codecarbon-2.3.4/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.428360 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.428360 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.428360 codecarbon-2.3.4/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-30 19:21:34.000000 codecarbon-2.3.4/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.432360 codecarbon-2.3.4/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.432360 codecarbon-2.3.4/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.432360 codecarbon-2.3.4/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/powermetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.424359 codecarbon-2.3.4/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.432360 codecarbon-2.3.4/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)    49615 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (127)   124267 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (127)    46586 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/external/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.436360 codecarbon-2.3.4/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.440359 codecarbon-2.3.4/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    29734 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    29874 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27995 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-01-30 19:21:34.000000 codecarbon-2.3.4/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.440359 codecarbon-2.3.4/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 19:21:45.000000 codecarbon-2.3.4/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 19:21:45.444359 codecarbon-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-30 19:21:34.000000 codecarbon-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:21:45.440359 codecarbon-2.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_powermetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_tracking_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/test_viz_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-01-30 19:21:34.000000 codecarbon-2.3.4/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.858790 codecarbon-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 07:19:23.000000 codecarbon-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-10 07:19:31.858790 codecarbon-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-10 07:19:23.000000 codecarbon-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/powermetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.834790 codecarbon-2.3.5/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)    49665 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49591 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46544 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29734 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29874 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28035 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.854790 codecarbon-2.3.5/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:19:31.858790 codecarbon-2.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-10 07:19:23.000000 codecarbon-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.854790 codecarbon-2.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_powermetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_tracking_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_viz_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/testutils.py
```

### Comparing `codecarbon-2.3.4/LICENSE` & `codecarbon-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/PKG-INFO` & `codecarbon-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.3.4
+Version: 2.3.5
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.3.4/README.md` & `codecarbon-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 
 class EmptyResultException(Exception):
     """
     The request return an empty result.
     """
 
-    pass
-
 
 @dataclass
 class ErrorBase:
     code: str
     message: str
```

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.3.5/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/carbonserver/database/database.py` & `codecarbon-2.3.5/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/container.py` & `codecarbon-2.3.5/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/main.py` & `codecarbon-2.3.5/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/carbonserver/setup.py` & `codecarbon-2.3.5/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/cli/cli_utils.py` & `codecarbon-2.3.5/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/cli/main.py` & `codecarbon-2.3.5/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/api_client.py` & `codecarbon-2.3.5/codecarbon/core/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 
 Based on https://kernelpanic.io/the-modern-way-to-call-apis-in-python
 
 TODO : use async call to API
 """
+
 # from httpx import AsyncClient
 import dataclasses
 import json
 import time
 from datetime import timedelta, tzinfo
 
 import arrow
@@ -170,15 +171,14 @@
             f"ApiClient API return http code {response.status_code} and answer : {response.text}"
         )
 
     def close_experiment(self):
         """
         Tell the API that the experiment has ended.
         """
-        pass
 
 
 class simple_utc(tzinfo):
     def tzname(self, **kwargs):
         return "UTC"
 
     def utcoffset(self, dt):
```

### Comparing `codecarbon-2.3.4/codecarbon/core/cloud.py` & `codecarbon-2.3.5/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/co2_signal.py` & `codecarbon-2.3.5/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/config.py` & `codecarbon-2.3.5/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/cpu.py` & `codecarbon-2.3.5/codecarbon/core/cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """
 Implements tracking Intel CPU Power Consumption on Mac and Windows
 using Intel Power Gadget
 https://software.intel.com/content/www/us/en/develop/articles/intel-power-gadget.html
 """
+
 import os
 import shutil
 import subprocess
 import sys
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 
 import pandas as pd
 from rapidfuzz import fuzz, process, utils
 
 from codecarbon.core.rapl import RAPLFile
 from codecarbon.core.units import Time
 from codecarbon.core.util import detect_cpu_model
 from codecarbon.external.logger import logger
 from codecarbon.input import DataSource
 
 
-def is_powergadget_available():
+def is_powergadget_available() -> bool:
     try:
         IntelPowerGadget()
         return True
     except Exception as e:
         logger.debug(
             "Not using PowerGadget, an exception occurred while instantiating"
             + f" IntelPowerGadget : {e}",
         )
         return False
 
 
-def is_rapl_available():
+def is_rapl_available() -> bool:
     try:
         IntelRAPL()
         return True
     except Exception as e:
         logger.debug(
             "Not using the RAPL interface, an exception occurred while instantiating "
             + f"IntelRAPL : {e}",
@@ -57,15 +58,15 @@
     ):
         self._log_file_path = os.path.join(output_dir, log_file_name)
         self._system = sys.platform.lower()
         self._duration = duration
         self._resolution = resolution
         self._setup_cli()
 
-    def _setup_cli(self):
+    def _setup_cli(self) -> None:
         """
         Setup cli command to run Intel Power Gadget
         """
         if self._system.startswith("win"):
             self._get_windows_exec_backup()
             if shutil.which(self._windows_exec):
                 self._cli = shutil.which(
@@ -106,15 +107,15 @@
         if desired_folder:
             self._windows_exec_backup = os.path.join(
                 parent_folder, desired_folder, self._windows_exec
             )
         else:
             self._windows_exec_backup = None
 
-    def _log_values(self):
+    def _log_values(self) -> None:
         """
         Logs output from Intel Power Gadget command line to a file
         """
         returncode = None
         if self._system.startswith("win"):
             returncode = subprocess.call(
                 [
@@ -139,15 +140,14 @@
             return None
 
         if returncode != 0:
             logger.warning(
                 "Returncode while logging power values using "
                 + f"Intel Power Gadget: {returncode}"
             )
-        return
 
     def get_cpu_details(self, **kwargs) -> Dict:
         """
         Fetches the CPU Power Details by fetching values from a logged csv file
         in _log_values function
         """
         self._log_values()
@@ -183,26 +183,25 @@
         self._cpu_details: Dict = dict()
 
         self._last_mesure = 0
 
     def _is_platform_supported(self) -> bool:
         return self._system.startswith("lin")
 
-    def _setup_rapl(self):
+    def _setup_rapl(self) -> None:
         if self._is_platform_supported():
             if os.path.exists(self._lin_rapl_dir):
                 self._fetch_rapl_files()
             else:
                 raise FileNotFoundError(
                     f"Intel RAPL files not found at {self._lin_rapl_dir} "
                     + f"on {self._system}"
                 )
         else:
             raise SystemError("Platform not supported by Intel RAPL Interface")
-        return
 
     def _fetch_rapl_files(self):
         """
         Fetches RAPL files from the RAPL directory
         """
 
         # consider files like `intel-rapl:$i`
@@ -233,32 +232,31 @@
                     logger.debug(f"We will read Intel RAPL files at {rapl_file}")
                 except PermissionError as e:
                     raise PermissionError(
                         "Unable to read Intel RAPL files for CPU power, we will use a constant for your CPU power."
                         + " Please view https://github.com/mlco2/codecarbon/issues/244"
                         + f" for workarounds : {e}"
                     )
-        return
 
     def get_cpu_details(self, duration: Time, **kwargs) -> Dict:
         """
         Fetches the CPU Energy Deltas by fetching values from RAPL files
         """
         cpu_details = dict()
         try:
             list(map(lambda rapl_file: rapl_file.delta(duration), self._rapl_files))
 
             for rapl_file in self._rapl_files:
                 logger.debug(rapl_file)
                 cpu_details[rapl_file.name] = rapl_file.energy_delta.kWh
                 # We fake the name used by Power Gadget when using RAPL
                 if "Energy" in rapl_file.name:
-                    cpu_details[
-                        rapl_file.name.replace("Energy", "Power")
-                    ] = rapl_file.power.W
+                    cpu_details[rapl_file.name.replace("Energy", "Power")] = (
+                        rapl_file.power.W
+                    )
         except Exception as e:
             logger.info(
                 f"Unable to read Intel RAPL files at {self._rapl_files}\n \
                 Exception occurred {e}",
                 exc_info=True,
             )
         self.cpu_details = cpu_details
@@ -283,15 +281,15 @@
         self.model, self.tdp = self._main()
 
     @staticmethod
     def _get_cpu_constant_power(match: str, cpu_power_df: pd.DataFrame) -> int:
         """Extract constant power from matched CPU"""
         return cpu_power_df[cpu_power_df["Name"] == match]["TDP"].values[0]
 
-    def _get_cpu_power_from_registry(self, cpu_model_raw: str) -> int:
+    def _get_cpu_power_from_registry(self, cpu_model_raw: str) -> Optional[int]:
         cpu_power_df = DataSource().get_cpu_power_data()
         cpu_matching = self._get_matching_cpu(cpu_model_raw, cpu_power_df)
         if cpu_matching:
             power = self._get_cpu_constant_power(cpu_matching, cpu_power_df)
             return power
         return None
```

### Comparing `codecarbon-2.3.4/codecarbon/core/emissions.py` & `codecarbon-2.3.5/codecarbon/core/emissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             )  # kgs
 
         country_energy_mix: Dict = energy_mix[geo.country_iso_code]
         emissions_per_kWh = self._global_energy_mix_to_emissions_rate(
             country_energy_mix
         )
         logger.debug(
-            f"We apply an energy mix of {emissions_per_kWh.kgs_per_kWh*1000:.0f}"
+            f"We apply an energy mix of {emissions_per_kWh.kgs_per_kWh * 1000:.0f}"
             + f" g.CO2eq/kWh for {geo.country_name}"
         )
 
         return emissions_per_kWh.kgs_per_kWh * energy.kWh  # kgs
 
     @staticmethod
     def _global_energy_mix_to_emissions_rate(energy_mix: Dict) -> EmissionsPerKWh:
```

### Comparing `codecarbon-2.3.4/codecarbon/core/gpu.py` & `codecarbon-2.3.5/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/measure.py` & `codecarbon-2.3.5/codecarbon/core/measure.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/powermetrics.py` & `codecarbon-2.3.5/codecarbon/core/powermetrics.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/rapl.py` & `codecarbon-2.3.5/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/schemas.py` & `codecarbon-2.3.5/codecarbon/core/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Here is the schemas used to communicate with the API.
 """
+
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional
 from uuid import UUID
 
 
 @dataclass
```

### Comparing `codecarbon-2.3.4/codecarbon/core/units.py` & `codecarbon-2.3.5/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/core/util.py` & `codecarbon-2.3.5/codecarbon/core/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         yield
     except exceptions:
         logger.warning("graceful shutdown. Exceptions:")
         logger.warning(
             exceptions if len(exceptions) != 1 else exceptions[0], exc_info=True
         )
         logger.warning("stopping.")
-        pass
 
 
 def resolve_path(path: Union[str, Path]) -> Path:
     """
     Fully resolve a path:
     resolve env vars ($HOME etc.) -> expand user (~) -> make absolute
 
@@ -57,22 +56,22 @@
     file_path = resolve_path(file_path)
     if not file_path.exists():
         return
     assert file_path.is_file()
     idx = 0
     parent = file_path.parent
     file_name = f"{file_path.name}{ext}"
-    backup = parent / file_name
+    backup_path = parent / file_name
 
-    while backup.exists():
+    while backup_path.exists():
         file_name = f"{file_path.name}_{idx}{ext}"
-        backup = parent / file_name
+        backup_path = parent / file_name
         idx += 1
 
-    file_path.rename(backup)
+    file_path.rename(backup_path)
 
 
 def detect_cpu_model() -> str:
     cpu_info = cpuinfo.get_cpu_info()
     if cpu_info:
         cpu_model_detected = cpu_info.get("brand_raw", "")
         return cpu_model_detected
```

### Comparing `codecarbon-2.3.4/codecarbon/data/cloud/impact.csv` & `codecarbon-2.3.5/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.3.5/codecarbon/data/hardware/cpu_power.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1488,14 +1488,15 @@
 Intel Core i7-10710U,25
 Intel Core i7-10750H,45
 Intel Core i7-10810U,25
 Intel Core i7-10850H,45
 Intel Core i7-10870H,45
 Intel Core i7-10875H,45
 Intel Core i7-10885H,45
+Intel Core i7-11370H,28
 Intel Core i7-1160G7,15
 Intel Core i7-1165G7,28
 Intel Core i7-11700,65
 Intel Core i7-11700F,65
 Intel Core i7-11700K,125
 Intel Core i7-11700KF,125
 Intel Core i7-11700T,35
@@ -2015,14 +2016,15 @@
 Intel Xeon E5-2650L v2,70
 Intel Xeon E5-2660 v2,95
 Intel Xeon E5-2667 v2,130
 Intel Xeon E5-2670 v2,115
 Intel Xeon E5-2673 v3,110
 Intel Xeon E5-2660 v4,105
 Intel Xeon E5-2680 v2,115
+Intel Xeon E5-2680 v3,120
 Intel Xeon E5-2680 v4,120
 Intel Xeon E5-2687W v2,130
 Intel Xeon E5-2690 v2,130
 Intel Xeon E5-2692 v2,100
 Intel Xeon E5-2695 v2,115
 Intel Xeon E5-2697 v2,130
 Intel Xeon E5-4607,95
```

### Comparing `codecarbon-2.3.4/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.3.5/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.3.5/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.3.5/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/emissions_tracker.py` & `codecarbon-2.3.5/codecarbon/emissions_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Contains implementations of the Public facing API: EmissionsTracker,
 OfflineEmissionsTracker and @track_emissions
 """
+
 import dataclasses
 import os
 import platform
 import time
 import uuid
 from abc import ABC, abstractmethod
 from collections import Counter
@@ -471,19 +472,19 @@
                 task_name: Task(
                     task_name=task_name,
                 )
             }
         )
         self._active_task = task_name
 
-    def stop_task(self, task_name: str = None) -> EmissionsData:
+    def stop_task(self, task_name: str = None) -> float:
         """
         Stop tracking a dedicated execution task. Delta energy is computed by task, to isolate its contribution to total
         emissions.
-        :return: EmissionsData
+        :return: None
         """
         task_name = task_name if task_name else self._active_task
         self._measure_power_and_energy()
 
         emissions_data = self._prepare_emissions_data(delta=True)
 
         task_duration = Time.from_seconds(
@@ -639,22 +640,20 @@
         return total_emissions
 
     @abstractmethod
     def _get_geo_metadata(self) -> GeoMetadata:
         """
         :return: Metadata containing geographical info
         """
-        pass
 
     @abstractmethod
     def _get_cloud_metadata(self) -> CloudMetadata:
         """
         :return: Metadata containing cloud info
         """
-        pass
 
     def _do_measurements(self) -> None:
         for hardware in self._hardware:
             h_time = time.time()
             # Compute last_duration again for more accuracy
             last_duration = time.time() - self._last_measured_time
             (
```

### Comparing `codecarbon-2.3.4/codecarbon/external/geography.py` & `codecarbon-2.3.5/codecarbon/external/geography.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Encapsulates external dependencies to retrieve cloud and geographical metadata
 """
 
 import re
+import urllib.parse
 from dataclasses import dataclass
 from typing import Callable, Dict, Optional
 
 import requests
 
 from codecarbon.core.cloud import get_env_cloud_details
 from codecarbon.external.logger import logger
@@ -81,28 +82,58 @@
             self.region,
         )
 
     @classmethod
     def from_geo_js(cls, url: str) -> "GeoMetadata":
         try:
             response: Dict = requests.get(url, timeout=0.5).json()
+
+            return cls(
+                country_iso_code=response["country_code3"].upper(),
+                country_name=response["country"],
+                region=response.get("region", "").lower(),
+                latitude=float(response.get("latitude")),
+                longitude=float(response.get("longitude")),
+                country_2letter_iso_code=response.get("country_code"),
+            )
         except Exception as e:
-            # If there is a timeout, we default to Canada
+            # If there is a timeout, we will try using a backup API
+            logger.warning(
+                f"Unable to access geographical location through primary API. Will resort to using the backup API - Exception : {e} - url={url}"
+            )
+
+        geo_url_backup = "https://ip-api.com/json/"
+
+        try:
+            geo_response: Dict = requests.get(geo_url_backup, timeout=0.5).json()
+            country_name = geo_response["country"]
+
+            # The previous request does not return the three-letter country code
+            country_code_3_url = f"https://api.first.org/data/v1/countries?q={urllib.parse.quote_plus(country_name)}&scope=iso"
+            country_code_response: Dict = requests.get(
+                country_code_3_url, timeout=0.5
+            ).json()
+
+            return cls(
+                country_iso_code=next(
+                    iter(country_code_response["data"].keys())
+                ).upper(),
+                country_name=country_name,
+                region=geo_response.get("regionName", "").lower(),
+                latitude=float(geo_response.get("lat")),
+                longitude=float(geo_response.get("lon")),
+                country_2letter_iso_code=geo_response.get("countryCode"),
+            )
+        except Exception as e:
+            # If both API calls fail, default to Canada
             logger.warning(
                 f"Unable to access geographical location. Using 'Canada' as the default value - Exception : {e} - url={url}"
             )
+
             return cls(
                 country_iso_code="CAN",
                 country_name="Canada",
                 region="Quebec",
                 latitude=46.8,
                 longitude=-71.2,
                 country_2letter_iso_code="CA",
             )
-        return cls(
-            country_iso_code=response["country_code3"].upper(),
-            country_name=response["country"],
-            region=response.get("region", "").lower(),
-            latitude=float(response.get("latitude")),
-            longitude=float(response.get("longitude")),
-            country_2letter_iso_code=response.get("country_code"),
-        )
```

### Comparing `codecarbon-2.3.4/codecarbon/external/hardware.py` & `codecarbon-2.3.5/codecarbon/external/hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Encapsulates external dependencies to retrieve hardware metadata
 """
+
 import re
 import subprocess
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Iterable, List, Optional, Tuple
 
 import psutil
@@ -167,15 +168,14 @@
 
         power = 0
         for metric, value in all_cpu_details.items():
             # "^Processor Power_\d+\(Watt\)$" for Intel Power Gadget
             if re.match(r"^Processor Power", metric):
                 power += value
                 logger.debug(f"_get_power_from_cpus - MATCH {metric} : {value}")
-
             else:
                 logger.debug(f"_get_power_from_cpus - DONT MATCH {metric} : {value}")
         return Power.from_watts(power)
 
     def _get_energy_from_cpus(self, delay: Time) -> Energy:
         """
         Get CPU energy deltas from RAPL files
@@ -201,15 +201,14 @@
             return power, energy
         # If not intel_rapl
         return super().measure_power_and_energy(last_duration=last_duration)
 
     def start(self):
         if self._mode in ["intel_power_gadget", "intel_rapl", "apple_powermetrics"]:
             self._intel_interface.start()
-        pass
 
     def get_model(self):
         return self._model
 
     @classmethod
     def from_utils(
         cls,
```

### Comparing `codecarbon-2.3.4/codecarbon/external/logger.py` & `codecarbon-2.3.5/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/external/scheduler.py` & `codecarbon-2.3.5/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/external/task.py` & `codecarbon-2.3.5/codecarbon/external/task.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/input.py` & `codecarbon-2.3.5/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/output.py` & `codecarbon-2.3.5/codecarbon/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,17 +178,17 @@
                 logger.warning(
                     f"CSV contains more than 1 ({len(df_run)})"
                     + f" rows with current run ID ({data.run_id})."
                     + "Appending instead of updating."
                 )
                 df = pd.concat([df, pd.DataFrame.from_records([dict(data.values)])])
             else:
-                df.at[
-                    df.run_id == data.run_id, data.values.keys()
-                ] = data.values.values()
+                df.at[df.run_id == data.run_id, data.values.keys()] = (
+                    data.values.values()
+                )
 
         df.to_csv(self.save_file_path, index=False)
 
     def task_out(self, data: List[TaskEmissionsData], experiment_name: str, output_dir):
         run_id = data[0].run_id
         save_task_file_path = os.path.join(
             output_dir, "emissions_" + experiment_name + "_" + run_id + ".csv"
```

### Comparing `codecarbon-2.3.4/codecarbon/prometheus/metric_definitions.py` & `codecarbon-2.3.5/codecarbon/prometheus/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/prometheus/prometheus.py` & `codecarbon-2.3.5/codecarbon/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.3.5/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.3.5/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.3.5/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon/viz/carbonboard.py` & `codecarbon-2.3.5/codecarbon/viz/carbonboard_on_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import dash
 import dash_bootstrap_components as dbc
+import dash_core_components as dcc
+import dash_table as dt
 import fire
 import pandas as pd
-from dash import dash_table as dt
-from dash import dcc
 from dash.dependencies import Input, Output
 
+from codecarbon.core.config import get_hierarchical_config
 from codecarbon.viz.components import Components
 from codecarbon.viz.data import Data
 
 
 def render_app(df: pd.DataFrame):
     app = dash.Dash(__name__, external_stylesheets=[dbc.themes.COSMO])
 
@@ -82,18 +83,18 @@
         if {project_summary["region"]} == "":
             project_infrastructure_location = f"{project_summary['country_name']}"
         else:
             project_infrastructure_location = (
                 f"{project_summary['region']}, {project_summary['country_name']}"
             )
         project_power_consumption = (
-            f"{round(project_summary['total']['energy_consumed'],1)} kWh"
+            f"{round(project_summary['total']['energy_consumed'], 1)} kWh"
         )
         project_carbon_equivalent = (
-            f"{round(project_summary['total']['emissions'],1)} kg"
+            f"{round(project_summary['total']['emissions'], 1)} kg"
         )
         last_run_power_consumption = (
             f"{project_summary['last_run']['energy_consumed']} kWh"
         )
         last_run_carbon_equivalent = f"{project_summary['last_run']['emissions']} kg"
 
         return (
@@ -263,16 +264,17 @@
                 on_cloud, cloud_provider_name, cloud_emissions_barchart_data
             ),
         )
 
     return app
 
 
-def viz(filepath: str, port: int = 8050, debug: bool = False) -> None:
-    df = pd.read_csv(filepath)
+def viz(port: int = 8051, debug: bool = False) -> None:
+    conf = get_hierarchical_config()
+    df = Data.get_data_from_api(conf.get("api_endpoint", "http://localhost:8000"))
     app = render_app(df)
     app.run_server(port=port, debug=debug)
 
 
 def main():
     fire.Fire(viz)
```

### Comparing `codecarbon-2.3.4/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.3.5/codecarbon/viz/carbonboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import dash
 import dash_bootstrap_components as dbc
-import dash_core_components as dcc
-import dash_table as dt
 import fire
 import pandas as pd
+from dash import dash_table as dt
+from dash import dcc
 from dash.dependencies import Input, Output
 
-from codecarbon.core.config import get_hierarchical_config
 from codecarbon.viz.components import Components
 from codecarbon.viz.data import Data
 
 
 def render_app(df: pd.DataFrame):
     app = dash.Dash(__name__, external_stylesheets=[dbc.themes.COSMO])
 
@@ -83,18 +82,18 @@
         if {project_summary["region"]} == "":
             project_infrastructure_location = f"{project_summary['country_name']}"
         else:
             project_infrastructure_location = (
                 f"{project_summary['region']}, {project_summary['country_name']}"
             )
         project_power_consumption = (
-            f"{round(project_summary['total']['energy_consumed'],1)} kWh"
+            f"{round(project_summary['total']['energy_consumed'], 1)} kWh"
         )
         project_carbon_equivalent = (
-            f"{round(project_summary['total']['emissions'],1)} kg"
+            f"{round(project_summary['total']['emissions'], 1)} kg"
         )
         last_run_power_consumption = (
             f"{project_summary['last_run']['energy_consumed']} kWh"
         )
         last_run_carbon_equivalent = f"{project_summary['last_run']['emissions']} kg"
 
         return (
@@ -264,17 +263,16 @@
                 on_cloud, cloud_provider_name, cloud_emissions_barchart_data
             ),
         )
 
     return app
 
 
-def viz(port: int = 8051, debug: bool = False) -> None:
-    conf = get_hierarchical_config()
-    df = Data.get_data_from_api(conf.get("api_endpoint", "http://localhost:8000"))
+def viz(filepath: str, port: int = 8050, debug: bool = False) -> None:
+    df = pd.read_csv(filepath)
     app = render_app(df)
     app.run_server(port=port, debug=debug)
 
 
 def main():
     fire.Fire(viz)
```

### Comparing `codecarbon-2.3.4/codecarbon/viz/components.py` & `codecarbon-2.3.5/codecarbon/viz/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,17 +523,19 @@
                 "country": "Country",
                 "emissions": "Carbon Equivalent (KgCO2)",
                 "iso_code": "Country Code",
                 energy_type: energy_labels[energy_type],
             },
             width=1400,
             height=600,
-            color_continuous_scale=list(reversed(self.colorscale))
-            if energy_type == "low_carbon"
-            else self.colorscale,
+            color_continuous_scale=(
+                list(reversed(self.colorscale))
+                if energy_type == "low_carbon"
+                else self.colorscale
+            ),
         )
 
     @staticmethod
     def get_regional_emissions_comparison():
         return html.Div(
             dbc.Col(
                 [
```

### Comparing `codecarbon-2.3.4/codecarbon/viz/data.py` & `codecarbon-2.3.5/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.3.5/codecarbon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.3.4
+Version: 2.3.5
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.3.4/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.3.5/codecarbon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/setup.py` & `codecarbon-2.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.3.4",
+    version="2.3.5",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.3.4/tests/test_api_call.py` & `codecarbon-2.3.5/tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_cloud.py` & `codecarbon-2.3.5/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_co2_signal.py` & `codecarbon-2.3.5/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_config.py` & `codecarbon-2.3.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_core_util.py` & `codecarbon-2.3.5/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_cpu.py` & `codecarbon-2.3.5/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_emissions.py` & `codecarbon-2.3.5/tests/test_emissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,29 +62,29 @@
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=1),
             GeoMetadata(country_iso_code="FRA", country_name="France"),
         )
 
         # THEN
         assert isinstance(emissions, float)
-        self.assertAlmostEqual(emissions, 67.39 / 1000, places=2)
+        self.assertAlmostEqual(emissions, 84.87 / 1000, places=2)
 
     def test_get_emissions_PRIVATE_INFRA_JOR(self):
         """
         Jordania use fossil energy
         """
         # WHEN
 
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=1_000),
             GeoMetadata(country_iso_code="JOR", country_name="Jordan"),
         )
 
         # THEN
-        jor_emissions = 399.909  # Emissions in Kgs of CO2 For 1 000 kWh of energy
+        jor_emissions = 475  # Emissions in Kgs of CO2 For 1 000 kWh of energy
         assert isinstance(emissions, float)
         self.assertAlmostEqual(emissions, jor_emissions, places=2)
 
     def test_get_emissions_PRIVATE_INFRA_NOR(self):
         """
         Norway utilises hydropower more than any other country around the globe
         """
@@ -137,15 +137,15 @@
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=3),
             GeoMetadata(country_iso_code="CAN", country_name="Canada"),
         )
 
         # THEN
         assert isinstance(emissions, float)
-        self.assertAlmostEqual(emissions, 0.3869, places=2)
+        self.assertAlmostEqual(emissions, 0.3775, places=2)
 
     def test_get_emissions_PRIVATE_INFRA_CANADA_WITH_REGION(self):
         # WHEN
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=3),
             GeoMetadata(
                 country_iso_code="CAN", country_name="Canada", region="ontario"
```

### Comparing `codecarbon-2.3.4/tests/test_emissions_tracker.py` & `codecarbon-2.3.5/tests/test_emissions_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
         tracker = EmissionsTracker(measure_power_secs=1, save_to_file=False)
 
         # WHEN
         tracker.start()
         heavy_computation(run_time_secs=2)
         emissions = tracker.stop()
-        self.assertEqual(1, mocked_requests_get.call_count)
+        self.assertEqual(2, mocked_requests_get.call_count)
         self.assertIsInstance(emissions, float)
         self.assertAlmostEqual(1.1037980397280433e-05, emissions, places=2)
 
     def test_graceful_start_failure(
         self,
         mock_setup_intel_cli,
         mock_log_values,
```

### Comparing `codecarbon-2.3.4/tests/test_emissions_tracker_constant.py` & `codecarbon-2.3.5/tests/test_emissions_tracker_constant.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_emissions_tracker_flush.py` & `codecarbon-2.3.5/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_energy.py` & `codecarbon-2.3.5/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_geography.py` & `codecarbon-2.3.5/tests/test_geography.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import responses
 
 from codecarbon.external.geography import CloudMetadata, GeoMetadata
 from tests.testdata import (
     CLOUD_METADATA_AWS,
     CLOUD_METADATA_AZURE,
     CLOUD_METADATA_GCP,
+    COUNTRY_METADATA_USA,
     GEO_METADATA_CANADA,
     GEO_METADATA_USA,
+    GEO_METADATA_USA_BACKUP,
 )
 
 
 class TestCloudMetadata(unittest.TestCase):
     @mock.patch(
         "codecarbon.external.geography.get_env_cloud_details",
         return_value=CLOUD_METADATA_AWS,
@@ -66,14 +68,36 @@
         responses.add(responses.GET, self.geo_js_url, json=GEO_METADATA_USA, status=200)
         geo = GeoMetadata.from_geo_js(self.geo_js_url)
         self.assertEqual("USA", geo.country_iso_code)
         self.assertEqual("United States", geo.country_name)
         self.assertEqual("illinois", geo.region)
 
     @responses.activate
+    def test_geo_metadata_USA_backup(self):
+        responses.add(
+            responses.GET, self.geo_js_url, json={"error": "not found"}, status=404
+        )
+        responses.add(
+            responses.GET,
+            "https://ip-api.com/json/",
+            json=GEO_METADATA_USA_BACKUP,
+            status=200,
+        )
+        responses.add(
+            responses.GET,
+            "https://api.first.org/data/v1/countries?q=United%20States&scope=iso",
+            json=COUNTRY_METADATA_USA,
+            status=200,
+        )
+        geo = GeoMetadata.from_geo_js(self.geo_js_url)
+        self.assertEqual("USA", geo.country_iso_code)
+        self.assertEqual("United States", geo.country_name)
+        self.assertEqual("illinois", geo.region)
+
+    @responses.activate
     def test_geo_metadata_CANADA(self):
         responses.add(
             responses.GET, self.geo_js_url, json=GEO_METADATA_CANADA, status=200
         )
         geo = GeoMetadata.from_geo_js(self.geo_js_url)
         self.assertEqual("CAN", geo.country_iso_code)
         self.assertEqual("Canada", geo.country_name)
```

### Comparing `codecarbon-2.3.4/tests/test_gpu.py` & `codecarbon-2.3.5/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_logging_output.py` & `codecarbon-2.3.5/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_powermetrics.py` & `codecarbon-2.3.5/tests/test_powermetrics.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_ram.py` & `codecarbon-2.3.5/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_tracking_inference.py` & `codecarbon-2.3.5/tests/test_tracking_inference.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/test_viz_data.py` & `codecarbon-2.3.5/tests/test_viz_data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.4/tests/testdata.py` & `codecarbon-2.3.5/tests/testdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,48 @@
     "city": "Chicago",
     "country": "United States",
     "continent_code": "NA",
     "country_code": "US",
     "latitude": "0",
 }
 
+GEO_METADATA_USA_BACKUP = {
+    "organization_name": "foobar",
+    "regionName": "Illinois",
+    "accuracy": 1,
+    "asn": 0,
+    "organization": "foobar",
+    "timezone": "America/Chicago",
+    "lon": "88",
+    "area_code": "0",
+    "ip": "foobar",
+    "city": "Chicago",
+    "country": "United States",
+    "countryCode": "US",
+    "lat": "0",
+}
+
+COUNTRY_METADATA_USA = {
+    "status": "OK",
+    "status-code": 200,
+    "version": "1.0",
+    "access": "public",
+    "data": {
+        "USA": {
+            "id": "USA",
+            "country": "United States of America (the)",
+            "region": "North America",
+        },
+        "UMI": {
+            "id": "UMI",
+            "country": "United States Minor Outlying Islands (the)",
+            "region": "Oceania",
+        },
+    },
+}
 
 GEO_METADATA_CANADA = {
     "organization_name": "foobar",
     "region": "Ontario",
     "accuracy": 100,
     "asn": 0,
     "organization": "foobar",
```

### Comparing `codecarbon-2.3.4/tests/testutils.py` & `codecarbon-2.3.5/tests/testutils.py`

 * *Files identical despite different names*

