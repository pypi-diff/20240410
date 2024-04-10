# Comparing `tmp/navigate-micro-0.0.4.tar.gz` & `tmp/navigate-micro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigate-micro-0.0.4.tar", last modified: Thu Feb  8 19:24:02 2024, max compression
+gzip compressed data, was "navigate-micro-0.0.5.tar", last modified: Wed Apr 10 12:01:58 2024, max compression
```

## Comparing `navigate-micro-0.0.4.tar` & `navigate-micro-0.0.5.tar`

### file list

```diff
@@ -1,291 +1,291 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/
--rw-rw-rw-   0        0        0     2114 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0      132 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6595 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/README.md
--rw-rw-rw-   0        0        0     1995 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.971159 navigate-micro-0.0.4/src/
--rw-rw-rw-   0        0        0        0 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.971159 navigate-micro-0.0.4/src/navigate/
--rw-rw-rw-   0        0        0        7 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/VERSION
--rw-rw-rw-   0        0        0      225 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/__init__.py
--rw-rw-rw-   0        0        0     3993 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/_commit.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.971159 navigate-micro-0.0.4/src/navigate/config/
--rw-rw-rw-   0        0        0       98 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/__init__.py
--rw-rw-rw-   0        0        0    36476 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/config.py
--rw-rw-rw-   0        0        0    11736 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/configuration.yaml
--rw-rw-rw-   0        0        0     2385 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/experiment.yml
--rw-rw-rw-   0        0        0       66 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/rest_api_config.yml
--rw-rw-rw-   0        0        0     6914 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/synthetic_configuration.yaml
--rw-rw-rw-   0        0        0     7197 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/waveform_constants.yml
--rw-rw-rw-   0        0        0      146 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/config/waveform_templates.yml
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.971159 navigate-micro-0.0.4/src/navigate/controller/
--rw-rw-rw-   0        0        0       62 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/__init__.py
--rw-rw-rw-   0        0        0    12782 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/configuration_controller.py
--rw-rw-rw-   0        0        0    48672 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/controller.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.986786 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/
--rw-rw-rw-   0        0        0     1427 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/__init__.py
--rw-rw-rw-   0        0        0    17550 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/acquire_bar_controller.py
--rw-rw-rw-   0        0        0    15957 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py
--rw-rw-rw-   0        0        0    10817 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/autofocus_popup_controller.py
--rw-rw-rw-   0        0        0     6105 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py
--rw-rw-rw-   0        0        0    23255 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_setting_controller.py
--rw-rw-rw-   0        0        0    44619 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_view_controller.py
--rw-rw-rw-   0        0        0    17711 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/channel_setting_controller.py
--rw-rw-rw-   0        0        0    34590 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/channels_tab_controller.py
--rw-rw-rw-   0        0        0     9611 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py
--rw-rw-rw-   0        0        0    29415 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/features_popup_controller.py
--rw-rw-rw-   0        0        0     3894 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/gui_controller.py
--rw-rw-rw-   0        0        0     9430 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/ilastik_popup_controller.py
--rw-rw-rw-   0        0        0     8431 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/keystroke_controller.py
--rw-rw-rw-   0        0        0    40031 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/menu_controller.py
--rw-rw-rw-   0        0        0     9717 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/microscope_popup_controller.py
--rw-rw-rw-   0        0        0    11435 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/multi_position_controller.py
--rw-rw-rw-   0        0        0    12864 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/plugins_controller.py
--rw-rw-rw-   0        0        0    22523 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/stage_controller.py
--rw-rw-rw-   0        0        0    16629 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/tiling_wizard_controller.py
--rw-rw-rw-   0        0        0    21786 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py
--rw-rw-rw-   0        0        0    31003 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/waveform_popup_controller.py
--rw-rw-rw-   0        0        0    12799 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/sub_controllers/waveform_tab_controller.py
--rw-rw-rw-   0        0        0    16135 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/controller/thread_pool.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:01.986786 navigate-micro-0.0.4/src/navigate/log_files/
--rw-rw-rw-   0        0        0       58 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/log_files/__init__.py
--rw-rw-rw-   0        0        0     3721 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/log_files/filters.py
--rw-rw-rw-   0        0        0     6749 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/log_files/log_functions.py
--rw-rw-rw-   0        0        0     1305 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/log_files/logging.yml
--rw-rw-rw-   0        0        0     1315 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/log_files/model_logging.yml
--rw-rw-rw-   0        0        0     4445 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/main.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/
--rw-rw-rw-   0        0        0       76 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/analysis/
--rw-rw-rw-   0        0        0       82 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/analysis/__init__.py
--rw-rw-rw-   0        0        0    14091 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/analysis/boundary_detect.py
--rw-rw-rw-   0        0        0     5547 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/analysis/camera.py
--rw-rw-rw-   0        0        0     2858 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/analysis/image_contrast.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/concurrency/
--rw-rw-rw-   0        0        0       67 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/concurrency/__init__.py
--rw-rw-rw-   0        0        0    26823 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/concurrency/concurrency_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/data_sources/
--rw-rw-rw-   0        0        0      922 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/data_sources/__init__.py
--rw-rw-rw-   0        0        0    20357 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/data_sources/bdv_data_source.py
--rw-rw-rw-   0        0        0    12940 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/data_sources/data_source.py
--rw-rw-rw-   0        0        0    10817 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/data_sources/tiff_data_source.py
--rw-rw-rw-   0        0        0    41926 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/device_startup_functions.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/
--rw-rw-rw-   0        0        0       34 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/asi/
--rw-rw-rw-   0        0        0       69 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/asi/__init__.py
--rw-rw-rw-   0        0        0    25001 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/coherent/
--rw-rw-rw-   0        0        0     6497 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/coherent/ObisLaser.py
--rw-rw-rw-   0        0        0       38 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/coherent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/dynamixel/
--rw-rw-rw-   0        0        0       40 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/dynamixel/__init__.py
--rw-rw-rw-   0        0        0    10609 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/hamamatsu/
--rw-rw-rw-   0        0        0    41464 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py
--rw-rw-rw-   0        0        0       36 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/hamamatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.002408 navigate-micro-0.0.4/src/navigate/model/devices/APIs/imagineoptics/
--rw-rw-rw-   0        0        0       51 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/imagineoptics/__init__.py
--rw-rw-rw-   0        0        0      481 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/imagineoptics/enums.py
--rw-rw-rw-   0        0        0    32812 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/imagineoptics/imop.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/mcl/
--rw-rw-rw-   0        0        0       55 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/mcl/__init__.py
--rw-rw-rw-   0        0        0     5681 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/mcl/madlib.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/omicron/
--rw-rw-rw-   0        0        0    12303 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/omicron/LuxxLaser.py
--rw-rw-rw-   0        0        0       39 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/omicron/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/
--rw-rw-rw-   0        0        0     4461 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/
--rw-rw-rw-   0        0        0    10711 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/
--rw-rw-rw-   0        0        0        0 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/__init__.py
--rw-rw-rw-   0        0        0    43400 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py
--rw-rw-rw-   0        0        0    29219 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/
--rw-rw-rw-   0        0        0      413 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/camera_settings.py
--rw-rw-rw-   0        0        0     1239 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py
--rw-rw-rw-   0        0        0     2525 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py
--rw-rw-rw-   0        0        0     2692 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py
--rw-rw-rw-   0        0        0      940 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py
--rw-rw-rw-   0        0        0     2288 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py
--rw-rw-rw-   0        0        0     1927 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py
--rw-rw-rw-   0        0        0     1319 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py
--rw-rw-rw-   0        0        0     1595 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py
--rw-rw-rw-   0        0        0      494 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling.py
--rw-rw-rw-   0        0        0      395 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling_show.py
--rw-rw-rw-   0        0        0     3654 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py
--rw-rw-rw-   0        0        0     1873 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py
--rw-rw-rw-   0        0        0    15288 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py
--rw-rw-rw-   0        0        0       39 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/sutter/
--rw-rw-rw-   0        0        0    20712 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/sutter/MP285.py
--rw-rw-rw-   0        0        0       48 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/sutter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.018036 navigate-micro-0.0.4/src/navigate/model/devices/APIs/thorlabs/
--rw-rw-rw-   0        0        0       45 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/thorlabs/__init__.py
--rw-rw-rw-   0        0        0    18113 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py
--rw-rw-rw-   0        0        0      671 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/camera/
--rw-rw-rw-   0        0        0       25 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/camera/__init__.py
--rw-rw-rw-   0        0        0     8172 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_base.py
--rw-rw-rw-   0        0        0    24538 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_hamamatsu.py
--rw-rw-rw-   0        0        0    23409 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_photometrics.py
--rw-rw-rw-   0        0        0    11519 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/daq/
--rw-rw-rw-   0        0        0       40 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/daq/__init__.py
--rw-rw-rw-   0        0        0     6627 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_base.py
--rw-rw-rw-   0        0        0    20176 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_ni.py
--rw-rw-rw-   0        0        0     6165 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/
--rw-rw-rw-   0        0        0       31 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/__init__.py
--rw-rw-rw-   0        0        0     7169 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py
--rw-rw-rw-   0        0        0     3650 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_base.py
--rw-rw-rw-   0        0        0    11305 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py
--rw-rw-rw-   0        0        0     4140 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/galvo/
--rw-rw-rw-   0        0        0       31 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/galvo/__init__.py
--rw-rw-rw-   0        0        0     9266 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_base.py
--rw-rw-rw-   0        0        0     4389 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_ni.py
--rw-rw-rw-   0        0        0     2704 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/lasers/
--rw-rw-rw-   0        0        0       24 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/lasers/__init__.py
--rw-rw-rw-   0        0        0     3321 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/lasers/laser_base.py
--rw-rw-rw-   0        0        0     7294 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/lasers/laser_ni.py
--rw-rw-rw-   0        0        0     2786 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/lasers/laser_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/mirrors/
--rw-rw-rw-   0        0        0       36 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/mirrors/__init__.py
--rw-rw-rw-   0        0        0     3141 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_base.py
--rw-rw-rw-   0        0        0     5128 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_imop.py
--rw-rw-rw-   0        0        0     2840 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_synthetic.py
--rw-rw-rw-   0        0        0     5222 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/objectives.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.033656 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/
--rw-rw-rw-   0        0        0       31 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/__init__.py
--rw-rw-rw-   0        0        0     9959 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_base.py
--rw-rw-rw-   0        0        0    10671 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py
--rw-rw-rw-   0        0        0     4592 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_ni.py
--rw-rw-rw-   0        0        0     3052 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.049282 navigate-micro-0.0.4/src/navigate/model/devices/shutter/
--rw-rw-rw-   0        0        0       26 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/shutter/__init__.py
--rw-rw-rw-   0        0        0     3074 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_base.py
--rw-rw-rw-   0        0        0     2729 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_synthetic.py
--rw-rw-rw-   0        0        0     4183 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_ttl.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.049282 navigate-micro-0.0.4/src/navigate/model/devices/stages/
--rw-rw-rw-   0        0        0       24 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/__init__.py
--rw-rw-rw-   0        0        0    18031 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_asi.py
--rw-rw-rw-   0        0        0     8375 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_base.py
--rw-rw-rw-   0        0        0    12142 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_galvo.py
--rw-rw-rw-   0        0        0     6855 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_mcl.py
--rw-rw-rw-   0        0        0     9756 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_pi.py
--rw-rw-rw-   0        0        0    10457 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_sutter.py
--rw-rw-rw-   0        0        0     7728 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_synthetic.py
--rw-rw-rw-   0        0        0     8657 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.049282 navigate-micro-0.0.4/src/navigate/model/devices/zoom/
--rw-rw-rw-   0        0        0       23 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/zoom/__init__.py
--rw-rw-rw-   0        0        0     5967 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_base.py
--rw-rw-rw-   0        0        0     9014 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_dynamixel.py
--rw-rw-rw-   0        0        0     2894 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.049282 navigate-micro-0.0.4/src/navigate/model/features/
--rw-rw-rw-   0        0        0       62 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/__init__.py
--rw-rw-rw-   0        0        0    21608 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/adaptive_optics.py
--rw-rw-rw-   0        0        0     8529 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/auto_tile_scan.py
--rw-rw-rw-   0        0        0    20037 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/autofocus.py
--rw-rw-rw-   0        0        0    55561 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/common_features.py
--rw-rw-rw-   0        0        0    23202 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/cva_conpro.py
--rw-rw-rw-   0        0        0    42808 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/feature_container.py
--rw-rw-rw-   0        0        0    14931 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/feature_related_functions.py
--rw-rw-rw-   0        0        0    13532 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/image_writer.py
--rw-rw-rw-   0        0        0    19751 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/remove_empty_tiles.py
--rw-rw-rw-   0        0        0     9274 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/restful_features.py
--rw-rw-rw-   0        0        0    16368 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/features/volume_search.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.064913 navigate-micro-0.0.4/src/navigate/model/metadata_sources/
--rw-rw-rw-   0        0        0       43 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/metadata_sources/__init__.py
--rw-rw-rw-   0        0        0    20659 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/metadata_sources/bdv_metadata.py
--rw-rw-rw-   0        0        0    12574 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/metadata_sources/metadata.py
--rw-rw-rw-   0        0        0    10605 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/metadata_sources/ome_tiff_metadata.py
--rw-rw-rw-   0        0        0    35875 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/microscope.py
--rw-rw-rw-   0        0        0    55737 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/model.py
--rw-rw-rw-   0        0        0    10200 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/plugins_model.py
--rw-rw-rw-   0        0        0    11679 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/model/waveforms.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.064913 navigate-micro-0.0.4/src/navigate/plugins/
--rw-rw-rw-   0        0        0       25 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.064913 navigate-micro-0.0.4/src/navigate/tools/
--rw-rw-rw-   0        0        0       66 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/__init__.py
--rw-rw-rw-   0        0        0     2394 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/common_dict_tools.py
--rw-rw-rw-   0        0        0     4277 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/common_functions.py
--rw-rw-rw-   0        0        0     2887 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/decorators.py
--rw-rw-rw-   0        0        0     6897 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/file_functions.py
--rw-rw-rw-   0        0        0     4135 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/image.py
--rw-rw-rw-   0        0        0     5696 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/linear_algebra.py
--rw-rw-rw-   0        0        0     7854 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/main_functions.py
--rw-rw-rw-   0        0        0     8376 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/multipos_table_tools.py
--rw-rw-rw-   0        0        0     4004 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/sdf.py
--rw-rw-rw-   0        0        0     3268 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/waveform_template_funcs.py
--rw-rw-rw-   0        0        0     4254 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/tools/xml_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.064913 navigate-micro-0.0.4/src/navigate/view/
--rw-rw-rw-   0        0        0       46 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.064913 navigate-micro-0.0.4/src/navigate/view/custom_widgets/
--rw-rw-rw-   0        0        0     3286 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/ArrowLabel.py
--rw-rw-rw-   0        0        0     7028 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/DockableNotebook.py
--rw-rw-rw-   0        0        0    11451 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py
--rw-rw-rw-   0        0        0       67 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/hover.py
--rw-rw-rw-   0        0        0     8768 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/hoverbar.py
--rw-rw-rw-   0        0        0     4905 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/hovermixin.py
--rw-rw-rw-   0        0        0     6301 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/popup.py
--rw-rw-rw-   0        0        0     5675 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/scrollbars.py
--rw-rw-rw-   0        0        0    38828 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/custom_widgets/validation.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.080534 navigate-micro-0.0.4/src/navigate/view/icon/
--rw-rw-rw-   0        0        0    67646 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/icon/mic.ico
--rw-rw-rw-   0        0        0   127742 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/icon/mic.png
--rw-rw-rw-   0        0        0   256647 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/icon/mic_orig.png
--rw-rw-rw-   0        0        0   364584 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/icon/splash_screen_image.png
--rw-rw-rw-   0        0        0     7364 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_application_window.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.080534 navigate-micro-0.0.4/src/navigate/view/main_window_content/
--rw-rw-rw-   0        0        0       46 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/__init__.py
--rw-rw-rw-   0        0        0     5490 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/acquire_notebook.py
--rw-rw-rw-   0        0        0    20237 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/camera_tab.py
--rw-rw-rw-   0        0        0    31196 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/channels_tab.py
--rw-rw-rw-   0        0        0    20004 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/display_notebook.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.080534 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/
--rw-rw-rw-   0        0        0    11248 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greydown.png
--rw-rw-rw-   0        0        0     5729 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greydown_disabled.png
--rw-rw-rw-   0        0        0    11254 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyleft.png
--rw-rw-rw-   0        0        0     5882 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyleft_disabled.png
--rw-rw-rw-   0        0        0    11078 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyright.png
--rw-rw-rw-   0        0        0     5883 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyright_disabled.png
--rw-rw-rw-   0        0        0    10935 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyup.png
--rw-rw-rw-   0        0        0     5636 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyup_disabled.png
--rw-rw-rw-   0        0        0     8912 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/images/wa_right.png
--rw-rw-rw-   0        0        0     3874 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/menus.py
--rw-rw-rw-   0        0        0    15198 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/multiposition_tab.py
--rw-rw-rw-   0        0        0     4246 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/settings_notebook.py
--rw-rw-rw-   0        0        0    30950 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/main_window_content/stage_tab.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/src/navigate/view/popups/
--rw-rw-rw-   0        0        0       59 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/__init__.py
--rw-rw-rw-   0        0        0     8160 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/acquire_popup.py
--rw-rw-rw-   0        0        0    14713 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/adaptiveoptics_popup.py
--rw-rw-rw-   0        0        0     8164 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/autofocus_setting_popup.py
--rw-rw-rw-   0        0        0     4976 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/camera_map_setting_popup.py
--rw-rw-rw-   0        0        0     5352 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/camera_view_popup_window.py
--rw-rw-rw-   0        0        0    18655 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/feature_list_popup.py
--rw-rw-rw-   0        0        0     6068 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/ilastik_setting_popup.py
--rw-rw-rw-   0        0        0     8312 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/microscope_setting_popup_window.py
--rw-rw-rw-   0        0        0     4554 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/plugins_popup.py
--rw-rw-rw-   0        0        0     8481 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/tiling_wizard_popup.py
--rw-rw-rw-   0        0        0    10122 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/tiling_wizard_popup2.py
--rw-rw-rw-   0        0        0    11696 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/popups/waveform_parameter_popup_window.py
--rw-rw-rw-   0        0        0     3667 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/src/navigate/view/splash_screen.py
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/src/navigate_micro.egg-info/
--rw-rw-rw-   0        0        0     6595 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12235 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      623 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-08 19:24:01.000000 navigate-micro-0.0.4/src/navigate_micro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-08 19:24:02.096163 navigate-micro-0.0.4/test/
--rw-rw-rw-   0        0        0     2198 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/test/test_commit.py
--rw-rw-rw-   0        0        0     2834 2024-02-08 19:23:28.000000 navigate-micro-0.0.4/test/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/
+-rw-rw-rw-   0        0        0     2114 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0      132 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6595 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1995 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/
+-rw-rw-rw-   0        0        0        0 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/
+-rw-rw-rw-   0        0        0        7 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/VERSION
+-rw-rw-rw-   0        0        0      225 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/__init__.py
+-rw-rw-rw-   0        0        0     3993 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/_commit.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/config/
+-rw-rw-rw-   0        0        0       98 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/__init__.py
+-rw-rw-rw-   0        0        0    37570 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/config.py
+-rw-rw-rw-   0        0        0    11736 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/configuration.yaml
+-rw-rw-rw-   0        0        0     2385 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/experiment.yml
+-rw-rw-rw-   0        0        0       66 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/rest_api_config.yml
+-rw-rw-rw-   0        0        0     6914 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/synthetic_configuration.yaml
+-rw-rw-rw-   0        0        0     7197 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/waveform_constants.yml
+-rw-rw-rw-   0        0        0      218 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/waveform_templates.yml
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/controller/
+-rw-rw-rw-   0        0        0       62 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/__init__.py
+-rw-rw-rw-   0        0        0    12782 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/configuration_controller.py
+-rw-rw-rw-   0        0        0    49646 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/controller.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.927802 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/
+-rw-rw-rw-   0        0        0     1427 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/__init__.py
+-rw-rw-rw-   0        0        0    17550 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/acquire_bar_controller.py
+-rw-rw-rw-   0        0        0    15957 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py
+-rw-rw-rw-   0        0        0    10817 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/autofocus_popup_controller.py
+-rw-rw-rw-   0        0        0     6105 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py
+-rw-rw-rw-   0        0        0    22294 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_setting_controller.py
+-rw-rw-rw-   0        0        0    44619 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_view_controller.py
+-rw-rw-rw-   0        0        0    17711 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channel_setting_controller.py
+-rw-rw-rw-   0        0        0    35208 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channels_tab_controller.py
+-rw-rw-rw-   0        0        0     9611 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py
+-rw-rw-rw-   0        0        0    29415 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/features_popup_controller.py
+-rw-rw-rw-   0        0        0     3894 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/gui_controller.py
+-rw-rw-rw-   0        0        0     9430 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/ilastik_popup_controller.py
+-rw-rw-rw-   0        0        0     8431 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/keystroke_controller.py
+-rw-rw-rw-   0        0        0    42034 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/menu_controller.py
+-rw-rw-rw-   0        0        0     9733 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/microscope_popup_controller.py
+-rw-rw-rw-   0        0        0    11435 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/multi_position_controller.py
+-rw-rw-rw-   0        0        0    12864 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/plugins_controller.py
+-rw-rw-rw-   0        0        0    22523 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/stage_controller.py
+-rw-rw-rw-   0        0        0    16629 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller.py
+-rw-rw-rw-   0        0        0    21786 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py
+-rw-rw-rw-   0        0        0    31409 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_popup_controller.py
+-rw-rw-rw-   0        0        0    12872 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_tab_controller.py
+-rw-rw-rw-   0        0        0    16135 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/thread_pool.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.927802 navigate-micro-0.0.5/src/navigate/log_files/
+-rw-rw-rw-   0        0        0       58 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/__init__.py
+-rw-rw-rw-   0        0        0     3721 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/filters.py
+-rw-rw-rw-   0        0        0     7471 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/log_functions.py
+-rw-rw-rw-   0        0        0     1305 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/logging.yml
+-rw-rw-rw-   0        0        0     1315 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/model_logging.yml
+-rw-rw-rw-   0        0        0     4445 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/main.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/
+-rw-rw-rw-   0        0        0       76 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/analysis/
+-rw-rw-rw-   0        0        0       82 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/__init__.py
+-rw-rw-rw-   0        0        0    14091 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/boundary_detect.py
+-rw-rw-rw-   0        0        0     5547 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/camera.py
+-rw-rw-rw-   0        0        0     2858 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/image_contrast.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/concurrency/
+-rw-rw-rw-   0        0        0       67 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/concurrency/__init__.py
+-rw-rw-rw-   0        0        0    26823 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/concurrency/concurrency_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/data_sources/
+-rw-rw-rw-   0        0        0      922 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/__init__.py
+-rw-rw-rw-   0        0        0    20357 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/bdv_data_source.py
+-rw-rw-rw-   0        0        0    12940 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/data_source.py
+-rw-rw-rw-   0        0        0    10817 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/tiff_data_source.py
+-rw-rw-rw-   0        0        0    42546 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/device_startup_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/
+-rw-rw-rw-   0        0        0       34 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/
+-rw-rw-rw-   0        0        0       69 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/__init__.py
+-rw-rw-rw-   0        0        0    25001 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/
+-rw-rw-rw-   0        0        0     6497 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/ObisLaser.py
+-rw-rw-rw-   0        0        0       38 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/
+-rw-rw-rw-   0        0        0       40 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/__init__.py
+-rw-rw-rw-   0        0        0    10609 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/
+-rw-rw-rw-   0        0        0    41704 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py
+-rw-rw-rw-   0        0        0       36 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/
+-rw-rw-rw-   0        0        0       51 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/__init__.py
+-rw-rw-rw-   0        0        0      481 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/enums.py
+-rw-rw-rw-   0        0        0    32812 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/imop.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/
+-rw-rw-rw-   0        0        0       55 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/__init__.py
+-rw-rw-rw-   0        0        0     5681 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/madlib.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/
+-rw-rw-rw-   0        0        0    12303 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/LuxxLaser.py
+-rw-rw-rw-   0        0        0       39 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/
+-rw-rw-rw-   0        0        0     4461 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/
+-rw-rw-rw-   0        0        0    10711 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/
+-rw-rw-rw-   0        0        0        0 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/__init__.py
+-rw-rw-rw-   0        0        0    43400 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py
+-rw-rw-rw-   0        0        0    29219 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/
+-rw-rw-rw-   0        0        0      413 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/camera_settings.py
+-rw-rw-rw-   0        0        0     1239 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py
+-rw-rw-rw-   0        0        0     2525 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py
+-rw-rw-rw-   0        0        0     2692 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py
+-rw-rw-rw-   0        0        0      940 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py
+-rw-rw-rw-   0        0        0     2288 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py
+-rw-rw-rw-   0        0        0     1927 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py
+-rw-rw-rw-   0        0        0     1319 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py
+-rw-rw-rw-   0        0        0     1595 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py
+-rw-rw-rw-   0        0        0      494 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling.py
+-rw-rw-rw-   0        0        0      395 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling_show.py
+-rw-rw-rw-   0        0        0     3654 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py
+-rw-rw-rw-   0        0        0     1873 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py
+-rw-rw-rw-   0        0        0    15288 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py
+-rw-rw-rw-   0        0        0       39 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/
+-rw-rw-rw-   0        0        0    20712 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/MP285.py
+-rw-rw-rw-   0        0        0       48 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/
+-rw-rw-rw-   0        0        0       45 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/__init__.py
+-rw-rw-rw-   0        0        0    18113 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py
+-rw-rw-rw-   0        0        0      671 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/camera/
+-rw-rw-rw-   0        0        0       25 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/__init__.py
+-rw-rw-rw-   0        0        0     8334 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_base.py
+-rw-rw-rw-   0        0        0    23489 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_hamamatsu.py
+-rw-rw-rw-   0        0        0    23173 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_photometrics.py
+-rw-rw-rw-   0        0        0    11490 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/daq/
+-rw-rw-rw-   0        0        0       40 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/__init__.py
+-rw-rw-rw-   0        0        0     6238 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_base.py
+-rw-rw-rw-   0        0        0    20126 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_ni.py
+-rw-rw-rw-   0        0        0     6165 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/
+-rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/__init__.py
+-rw-rw-rw-   0        0        0     7169 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py
+-rw-rw-rw-   0        0        0     3650 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_base.py
+-rw-rw-rw-   0        0        0    11305 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py
+-rw-rw-rw-   0        0        0     4140 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/galvo/
+-rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/__init__.py
+-rw-rw-rw-   0        0        0     8952 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_base.py
+-rw-rw-rw-   0        0        0     4389 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_ni.py
+-rw-rw-rw-   0        0        0     2704 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/lasers/
+-rw-rw-rw-   0        0        0       24 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/__init__.py
+-rw-rw-rw-   0        0        0     3321 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_base.py
+-rw-rw-rw-   0        0        0     7294 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_ni.py
+-rw-rw-rw-   0        0        0     2786 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/
+-rw-rw-rw-   0        0        0       36 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/__init__.py
+-rw-rw-rw-   0        0        0     3141 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_base.py
+-rw-rw-rw-   0        0        0     5128 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_imop.py
+-rw-rw-rw-   0        0        0     2840 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_synthetic.py
+-rw-rw-rw-   0        0        0     5222 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/objectives.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/
+-rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/__init__.py
+-rw-rw-rw-   0        0        0     9992 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_base.py
+-rw-rw-rw-   0        0        0    10671 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py
+-rw-rw-rw-   0        0        0     4592 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_ni.py
+-rw-rw-rw-   0        0        0     3052 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/shutter/
+-rw-rw-rw-   0        0        0       26 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/__init__.py
+-rw-rw-rw-   0        0        0     3074 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_base.py
+-rw-rw-rw-   0        0        0     2729 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_synthetic.py
+-rw-rw-rw-   0        0        0     4183 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_ttl.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/stages/
+-rw-rw-rw-   0        0        0       24 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/__init__.py
+-rw-rw-rw-   0        0        0    18031 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_asi.py
+-rw-rw-rw-   0        0        0     8375 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_base.py
+-rw-rw-rw-   0        0        0    11617 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_galvo.py
+-rw-rw-rw-   0        0        0     6855 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_mcl.py
+-rw-rw-rw-   0        0        0     9756 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_pi.py
+-rw-rw-rw-   0        0        0    10457 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_sutter.py
+-rw-rw-rw-   0        0        0     7634 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_synthetic.py
+-rw-rw-rw-   0        0        0     8657 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/zoom/
+-rw-rw-rw-   0        0        0       23 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/__init__.py
+-rw-rw-rw-   0        0        0     5967 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_base.py
+-rw-rw-rw-   0        0        0     9014 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_dynamixel.py
+-rw-rw-rw-   0        0        0     2894 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/model/features/
+-rw-rw-rw-   0        0        0       62 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/__init__.py
+-rw-rw-rw-   0        0        0    21608 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/adaptive_optics.py
+-rw-rw-rw-   0        0        0     8529 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/auto_tile_scan.py
+-rw-rw-rw-   0        0        0    20037 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/autofocus.py
+-rw-rw-rw-   0        0        0    55561 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/common_features.py
+-rw-rw-rw-   0        0        0    22979 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/cva_conpro.py
+-rw-rw-rw-   0        0        0    42808 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/feature_container.py
+-rw-rw-rw-   0        0        0    14931 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/feature_related_functions.py
+-rw-rw-rw-   0        0        0    13532 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/image_writer.py
+-rw-rw-rw-   0        0        0    19751 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/remove_empty_tiles.py
+-rw-rw-rw-   0        0        0     9274 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/restful_features.py
+-rw-rw-rw-   0        0        0    16368 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/volume_search.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/model/metadata_sources/
+-rw-rw-rw-   0        0        0       43 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/__init__.py
+-rw-rw-rw-   0        0        0    20659 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/bdv_metadata.py
+-rw-rw-rw-   0        0        0    12574 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/metadata.py
+-rw-rw-rw-   0        0        0    10605 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/ome_tiff_metadata.py
+-rw-rw-rw-   0        0        0    35870 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/microscope.py
+-rw-rw-rw-   0        0        0    57127 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/model.py
+-rw-rw-rw-   0        0        0    10117 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/plugins_model.py
+-rw-rw-rw-   0        0        0    14067 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/waveforms.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/plugins/
+-rw-rw-rw-   0        0        0       25 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/tools/
+-rw-rw-rw-   0        0        0       66 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/__init__.py
+-rw-rw-rw-   0        0        0     3332 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/common_dict_tools.py
+-rw-rw-rw-   0        0        0     4277 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/common_functions.py
+-rw-rw-rw-   0        0        0     2887 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/decorators.py
+-rw-rw-rw-   0        0        0     6897 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/file_functions.py
+-rw-rw-rw-   0        0        0     4135 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/image.py
+-rw-rw-rw-   0        0        0     5696 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/linear_algebra.py
+-rw-rw-rw-   0        0        0     7854 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/main_functions.py
+-rw-rw-rw-   0        0        0     8376 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/multipos_table_tools.py
+-rw-rw-rw-   0        0        0     4004 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/sdf.py
+-rw-rw-rw-   0        0        0     3268 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/waveform_template_funcs.py
+-rw-rw-rw-   0        0        0     4254 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/xml_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/view/
+-rw-rw-rw-   0        0        0       46 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/custom_widgets/
+-rw-rw-rw-   0        0        0     3286 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/ArrowLabel.py
+-rw-rw-rw-   0        0        0     7028 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/DockableNotebook.py
+-rw-rw-rw-   0        0        0    11451 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py
+-rw-rw-rw-   0        0        0       67 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hover.py
+-rw-rw-rw-   0        0        0     8768 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hoverbar.py
+-rw-rw-rw-   0        0        0     4905 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hovermixin.py
+-rw-rw-rw-   0        0        0     6301 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/popup.py
+-rw-rw-rw-   0        0        0     5675 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/scrollbars.py
+-rw-rw-rw-   0        0        0    39055 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/validation.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/icon/
+-rw-rw-rw-   0        0        0    67646 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic.ico
+-rw-rw-rw-   0        0        0   127742 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic.png
+-rw-rw-rw-   0        0        0   256647 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic_orig.png
+-rw-rw-rw-   0        0        0   364584 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/splash_screen_image.png
+-rw-rw-rw-   0        0        0     7364 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_application_window.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/main_window_content/
+-rw-rw-rw-   0        0        0       46 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/__init__.py
+-rw-rw-rw-   0        0        0     5490 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/acquire_notebook.py
+-rw-rw-rw-   0        0        0    20237 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/camera_tab.py
+-rw-rw-rw-   0        0        0    31198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/channels_tab.py
+-rw-rw-rw-   0        0        0    20004 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/display_notebook.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/
+-rw-rw-rw-   0        0        0    11248 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown.png
+-rw-rw-rw-   0        0        0     5729 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown_disabled.png
+-rw-rw-rw-   0        0        0    11254 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft.png
+-rw-rw-rw-   0        0        0     5882 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft_disabled.png
+-rw-rw-rw-   0        0        0    11078 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright.png
+-rw-rw-rw-   0        0        0     5883 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright_disabled.png
+-rw-rw-rw-   0        0        0    10935 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup.png
+-rw-rw-rw-   0        0        0     5636 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup_disabled.png
+-rw-rw-rw-   0        0        0     8912 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/wa_right.png
+-rw-rw-rw-   0        0        0     3874 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/menus.py
+-rw-rw-rw-   0        0        0    15198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/multiposition_tab.py
+-rw-rw-rw-   0        0        0     4246 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/settings_notebook.py
+-rw-rw-rw-   0        0        0    30950 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/stage_tab.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/src/navigate/view/popups/
+-rw-rw-rw-   0        0        0       59 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/__init__.py
+-rw-rw-rw-   0        0        0     8160 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/acquire_popup.py
+-rw-rw-rw-   0        0        0    14713 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/adaptiveoptics_popup.py
+-rw-rw-rw-   0        0        0     8164 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/autofocus_setting_popup.py
+-rw-rw-rw-   0        0        0     4976 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/camera_map_setting_popup.py
+-rw-rw-rw-   0        0        0     5352 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/camera_view_popup_window.py
+-rw-rw-rw-   0        0        0    18655 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/feature_list_popup.py
+-rw-rw-rw-   0        0        0     6068 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/ilastik_setting_popup.py
+-rw-rw-rw-   0        0        0     8312 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/microscope_setting_popup_window.py
+-rw-rw-rw-   0        0        0     4554 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/plugins_popup.py
+-rw-rw-rw-   0        0        0     8481 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup.py
+-rw-rw-rw-   0        0        0    10122 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup2.py
+-rw-rw-rw-   0        0        0    11807 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/waveform_parameter_popup_window.py
+-rw-rw-rw-   0        0        0     3667 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/splash_screen.py
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/src/navigate_micro.egg-info/
+-rw-rw-rw-   0        0        0     6595 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12235 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      623 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/test/
+-rw-rw-rw-   0        0        0     2198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/test/test_commit.py
+-rw-rw-rw-   0        0        0     2834 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/test/test_main.py
```

### Comparing `navigate-micro-0.0.4/LICENSE.md` & `navigate-micro-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/PKG-INFO` & `navigate-micro-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigate-micro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Open source, smart, light-sheet microscopy control software.
 Author: The Dean Lab, UT Southwestern Medical Center
 License: Copyright (c) 2021-2023 The University of Texas Southwestern Medical Center.
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are
```

### Comparing `navigate-micro-0.0.4/README.md` & `navigate-micro-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/pyproject.toml` & `navigate-micro-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/_commit.py` & `navigate-micro-0.0.5/src/navigate/_commit.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/config/config.py` & `navigate-micro-0.0.5/src/navigate/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -764,26 +764,26 @@
                         waveform_dict[microscope_name][zoom],
                         laser,
                         {
                             "amplitude": config_dict["remote_focus_device"][
                                 "amplitude"
                             ],
                             "offset": config_dict["remote_focus_device"]["offset"],
-                            "percent_smoothing": "0",
-                            "percent_delay": config_dict["remote_focus_device"][
-                                "delay_percent"
-                            ],
+                            # "percent_smoothing": "0",
+                            # "delay": config_dict["remote_focus_device"][
+                            #     "delay"
+                            # ],
                         },
                     )
                 else:
                     for k in [
                         "amplitude",
                         "offset",
-                        "percent_smoothing",
-                        "percent_delay",
+                        # "percent_smoothing",
+                        # "delay",
                     ]:
                         if k not in waveform_dict[microscope_name][zoom][laser].keys():
                             waveform_dict[microscope_name][zoom][laser][
                                 k
                             ] = config_dict["remote_focus_device"].get(k, "0")
                         else:
                             try:
@@ -889,24 +889,52 @@
         # delete non-exist microscope
         for k in waveform_dict.keys():
             if k not in configuration["configuration"]["microscopes"].keys():
                 waveform_dict.pop(k)
 
     # other_constants
     waveform_dict = configuration["waveform_constants"]
+    other_constants_dict = {
+        "remote_focus_settle_duration": "0",
+        "percent_smoothing": "0",
+        "remote_focus_delay": config_dict["remote_focus_device"][
+            "delay"
+        ],
+        "remote_focus_ramp_falling": config_dict["remote_focus_device"][
+            "ramp_falling"
+        ]
+    }
     if (
         "other_constants" not in waveform_dict.keys()
         or type(waveform_dict["other_constants"]) is not DictProxy
     ):
         update_config_dict(
             manager,
             waveform_dict,
             "other_constants",
-            {"remote_focus_settle_duration": "0"},
+            other_constants_dict,
         )
-    if "remote_focus_settle_duration" not in waveform_dict["other_constants"].keys():
-        waveform_dict["other_constants"]["remote_focus_settle_duration"] = "0"
-    else:
+    for k in other_constants_dict.keys():
         try:
-            float(waveform_dict["other_constants"]["remote_focus_settle_duration"])
-        except ValueError:
-            waveform_dict["other_constants"]["remote_focus_settle_duration"] = "0"
+            float(waveform_dict["other_constants"][k])
+        except (ValueError, KeyError):
+            waveform_dict["other_constants"][k] = "0"
+
+def verify_configuration(manager, configuration):
+    """Verify configuration files.
+    
+    Supports old version of configurations.
+    """
+    device_config = configuration["configuration"]["microscopes"]
+    for microscope_name in device_config.keys():
+        # camera
+        # delay_percent -> delay
+        camera_config = device_config[microscope_name]["camera"]
+        if "delay" not in camera_config.keys():
+            camera_config["delay"] = camera_config.get("delay_percent", 2)
+        # remote focus
+        # ramp_falling_percent -> ramp_falling
+        remote_focus_config = device_config[microscope_name]["remote_focus_device"]
+        if "ramp_falling" not in remote_focus_config.keys():
+            remote_focus_config["ramp_falling"] = remote_focus_config.get("ramp_falling_percent", 5)
+        if "delay" not in remote_focus_config.keys():
+            remote_focus_config["delay"] = remote_focus_config.get("delay_percent", 0)
```

### Comparing `navigate-micro-0.0.4/src/navigate/config/configuration.yaml` & `navigate-micro-0.0.5/src/navigate/config/configuration.yaml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/config/experiment.yml` & `navigate-micro-0.0.5/src/navigate/config/experiment.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/config/synthetic_configuration.yaml` & `navigate-micro-0.0.5/src/navigate/config/synthetic_configuration.yaml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/config/waveform_constants.yml` & `navigate-micro-0.0.5/src/navigate/config/waveform_constants.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/configuration_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/configuration_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/controller.py` & `navigate-micro-0.0.5/src/navigate/controller/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) 2021-2022  The University of Texas Southwestern Medical Center.
 # All rights reserved.
-import platform
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted for academic and research use only
 # (subject to the limitations in the disclaimer below)
 # provided that the following conditions are met:
 
 #      * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
@@ -36,14 +35,15 @@
 import tkinter
 from tkinter import messagebox
 import multiprocessing as mp
 import threading
 import sys
 import os
 import time
+import platform
 
 # Third Party Imports
 
 # Local View Imports
 from navigate.view.main_application_window import MainApp as view
 from navigate.view.popups.camera_view_popup_window import CameraViewPopupWindow
 from navigate.view.popups.feature_list_popup import FeatureListPopup
@@ -74,14 +74,15 @@
 
 # Misc. Local Imports
 from navigate.config.config import (
     load_configs,
     update_config_dict,
     verify_experiment_config,
     verify_waveform_constants,
+    verify_configuration,
     get_navigate_path,
 )
 from navigate.tools.file_functions import create_save_path, save_yaml_file
 from navigate.tools.common_dict_tools import update_stage_dict
 from navigate.tools.multipos_table_tools import update_table
 from navigate.tools.common_functions import combine_funcs
 
@@ -138,24 +139,26 @@
         self.threads_pool = SynchronizedThreadPool()
 
         #: mp.Queue: Queue for retrieving events ('event_name', value) from model
         self.event_queue = mp.Queue(100)
 
         #: Manager: A shared memory manager
         self.manager = Manager()
+
         #: dict: Configuration dictionary
         self.configuration = load_configs(
             self.manager,
             configuration=configuration_path,
             experiment=experiment_path,
             waveform_constants=waveform_constants_path,
             rest_api_config=rest_api_path,
             waveform_templates=waveform_templates_path,
         )
 
+        verify_configuration(self.manager, self.configuration)
         verify_experiment_config(self.manager, self.configuration)
         verify_waveform_constants(self.manager, self.configuration)
 
         # Initialize the Model
         #: ObjectInSubprocess: Model object in MVC architecture.
         self.model = ObjectInSubprocess(
             Model, args, self.configuration, event_queue=self.event_queue
@@ -184,17 +187,15 @@
 
         # Initialize the View
         #: View: View object in MVC architecture.
         self.view = view(root)
 
         # Sub Gui Controllers
         #: AcquireBarController: Acquire Bar Sub-Controller.
-        self.acquire_bar_controller = AcquireBarController(
-            self.view.acqbar, self
-        )
+        self.acquire_bar_controller = AcquireBarController(self.view.acqbar, self)
         #: ChannelsTabController: Channels Tab Sub-Controller.
         self.channels_tab_controller = ChannelsTabController(
             self.view.settings.channels_tab, self
         )
         #: MultiPositionController: Multi-Position Tab Sub-Controller.
         self.multiposition_tab_controller = MultiPositionController(
             self.view.settings.multiposition_tab.multipoint_list, self
@@ -235,46 +236,55 @@
         # self.microscope = self.configuration['configuration']
         # ['microscopes'].keys()[0]  # Default to the first microscope
 
         # Initialize the menus
         #: MenuController: Menu Sub-Controller.
         self.menu_controller = MenuController(view=self.view, parent_controller=self)
         self.menu_controller.initialize_menus()
+
         #: dict: acquisition modes from plugins
         self.plugin_acquisition_modes = {}
+
         # add plugin menus
         #: PluginsController: Plugin Sub-Controller
-        self.plugin_controller = PluginsController(view=self.view, parent_controller=self)
+        self.plugin_controller = PluginsController(
+            view=self.view, parent_controller=self
+        )
         self.plugin_controller.load_plugins()
 
         # Create default data buffer
         #: int: Number of x_pixels from microscope configuration file.
         self.img_width = 0
+
         #: int: Number of y_pixels from microscope configuration file.
         self.img_height = 0
+
         #: SharedNDArray: Pre-allocated shared memory array.
         self.data_buffer = None
+
         #: dict: Additional microscopes.
         self.additional_microscopes = {}
+
         #: dict: Additional microscope configurations.
         self.additional_microscopes_configs = {}
+
         #: bool: Flag for stopping acquisition.
         self.stop_acquisition_flag = False
 
         # Set view based on model.experiment
         self.populate_experiment_setting(in_initialize=True)
 
         # Camera View Tab
         self.initialize_cam_view()
 
         # destroy splash screen and show main screen
         splash_screen.destroy()
         root.deiconify()
 
-        #: event: Event for resizing the GUI. Only works on Windows OS.
+        #: int: ID for the resize event.Only works on Windows OS.
         self.resize_event_id = None
         if platform.system() == "Windows":
             self.view.root.bind("<Configure>", self.resize)
 
     def update_buffer(self):
         """Update the buffer size according to the camera
         dimensions listed in the experimental parameters.
@@ -299,14 +309,20 @@
         if img_width == self.img_width and img_height == self.img_height:
             return
 
         self.data_buffer = self.model.get_data_buffer(img_width, img_height)
         self.img_width = img_width
         self.img_height = img_height
 
+        # virtual microscopes
+        for microscope_name in self.additional_microscopes:
+            self.model.destroy_virtual_microscope(microscope_name)
+            # TODO: destroy the popup window
+            self.additional_microscopes.pop(microscope_name)
+
     def update_acquire_control(self):
         """Update the acquire control based on the current experiment parameters."""
         self.view.acqbar.stop_stage.config(
             command=self.stage_controller.stop_button_handler
         )
 
     def change_microscope(self, microscope_name, zoom=None):
@@ -451,15 +467,15 @@
         Parameters
         __________
         event : event
             event = <Configure x=0 y=0 width=1200 height=600>
         """
 
         def refresh(width, height):
-            """ Refresh the GUI.
+            """Refresh the GUI.
 
             Parameters
             __________
             width : int
                 Width of the GUI.
             height : int
                 Height of the GUI.
@@ -675,33 +691,32 @@
                 self.threads_pool.createThread(
                     "camera",
                     self.capture_image,
                     args=("autofocus", "live", *args),
                 )
             elif self.acquire_bar_controller.mode == "live":
                 self.threads_pool.createThread(
-                    "model",
-                    lambda: self.model.run_command("autofocus", *args)
+                    "model", lambda: self.model.run_command("autofocus", *args)
                 )
 
         elif command == "eliminate_tiles":
             """Execute eliminate tiles routine."""
 
             self.acquire_bar_controller.set_mode(mode="customized")
             feature_list = self.menu_controller.feature_list_names
             feature_name = "Remove Empty Tiles"
             try:
                 # feature_id_val has a trace, and setting the menu item triggers it.
                 feature_id = feature_list.index(feature_name)
                 self.menu_controller.feature_id_val.set(feature_id)
             except ValueError:
                 logger.debug("No feature named 'Remove Empty Tiles' found.")
-                messagebox.showwarning(title="Navigate",
-                                       message="Feature 'Remove Empty Tiles' not found."
-                                       )
+                messagebox.showwarning(
+                    title="Navigate", message="Feature 'Remove Empty Tiles' not found."
+                )
                 return
             self.execute("acquire")
 
         elif command == "load_feature":
             """Tell model to load/unload features."""
 
             work_thread = self.threads_pool.createThread(
@@ -724,19 +739,27 @@
 
             """
             if not self.prepare_acquire_data():
                 self.acquire_bar_controller.stop_acquire()
                 return
             saving_settings = self.configuration["experiment"]["Saving"]
             file_directory = create_save_path(saving_settings)
+
+            # Save the experiment.yaml file.
             save_yaml_file(
-                file_directory,
-                self.configuration["experiment"],
+                file_directory=file_directory,
+                content_dict=self.configuration["experiment"],
                 filename="experiment.yml",
             )
+
+            # Save the waveform_constants.yaml file.
+            save_yaml_file(file_directory=file_directory,
+                           content_dict=self.configuration['waveform_constants'],
+                           filename="waveform_constants.yml")
+
             self.camera_setting_controller.solvent = self.configuration["experiment"][
                 "Saving"
             ]["solvent"]
             self.camera_setting_controller.calculate_physical_dimensions()
             self.execute("acquire")
 
         elif command == "acquire":
@@ -749,24 +772,25 @@
             Parameters
             __________
             args[0] : string
                 string = 'continuous', 'z-stack', 'single', or 'projection'
             """
             # acquisition mode from plugin
             plugin_obj = self.plugin_acquisition_modes.get(
-                self.acquire_bar_controller.mode, None)
+                self.acquire_bar_controller.mode, None
+            )
 
             if plugin_obj and hasattr(plugin_obj, "prepare_acquisition_controller"):
                 getattr(plugin_obj, "prepare_acquisition_controller")(self)
 
             # Prepare data
             if not self.prepare_acquire_data():
                 self.acquire_bar_controller.stop_acquire()
                 return
-            
+
             # set the display segmentation flag to False
             self.camera_view_controller.display_mask_flag = False
 
             # ask user to verify feature list parameters if in "customized" mode
             if self.acquire_bar_controller.mode == "customized":
                 feature_id = self.menu_controller.feature_id_val.get()
                 if feature_id > 0:
@@ -938,14 +962,16 @@
         self.camera_view_controller.initialize_non_live_display(
             self.data_buffer,
             self.configuration["experiment"]["MicroscopeState"],
             self.configuration["experiment"]["CameraParameters"],
         )
 
         self.stop_acquisition_flag = False
+        start_time = time.time()
+        self.camera_setting_controller.update_readout_time()
 
         while True:
             if self.stop_acquisition_flag:
                 break
             # Receive the Image and log it.
             image_id = self.show_img_pipe.recv()
             logger.info(f"Navigate Controller - Received Image: {image_id}")
@@ -955,25 +981,37 @@
             if not isinstance(image_id, int):
                 logger.debug(
                     f"Navigate Controller - Something wrong happened, stop the model!, "
                     f"{image_id}"
                 )
                 self.execute("stop_acquire")
 
+
             # Display the Image in the View
             self.camera_view_controller.try_to_display_image(image_id=image_id)
             images_received += 1
 
             # Update progress bar.
             self.acquire_bar_controller.progress_bar(
                 images_received=images_received,
                 microscope_state=self.configuration["experiment"]["MicroscopeState"],
                 mode=mode,
                 stop=False,
             )
+            # update framerate
+            stop_time = time.time()
+            frames_per_second = images_received / (stop_time - start_time)
+            # Update the Framerate in the Camera Settings Tab
+            self.camera_setting_controller.framerate_widgets["max_framerate"].set(
+                frames_per_second
+            )
+
+            # Update the Framerate in the Acquire Bar to provide an estimate of
+            # the duration of time remaining.
+            self.acquire_bar_controller.framerate = frames_per_second
 
         logger.info(
             f"Navigate Controller - Captured {images_received}, " f"{mode} Images"
         )
 
         # acquisition mode from plugin
         plugin_obj = self.plugin_acquisition_modes.get(mode, None)
@@ -1211,26 +1249,18 @@
                 for _ in range(10):
                     try:
                         self.update_stage_controller_silent(value)
                         break
                     except RuntimeError:
                         time.sleep(0.001)
                         pass
-
-            elif event == "framerate":
-                # Update the Framerate in the Camera Settings Tab
-                self.camera_setting_controller.framerate_widgets["max_framerate"].set(
-                    value
-                )
-
-                # Update the Framerate in the Acquire Bar to provide an estimate of
-                # the duration of time remaining.
-                self.acquire_bar_controller.framerate = value
             elif event == "remove_positions":
                 self.multiposition_tab_controller.remove_positions(value)
+            elif event == "exposure_time":
+                self.channels_tab_controller.set_exposure_time(value[0], value[1])
 
     # def exit_program(self):
     #     """Exit the program.
 
     #     This function is called when the user clicks the exit button in the GUI.
     #     """
     #     if messagebox.askyesno("Exit", "Are you sure?"):
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/__init__.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/acquire_bar_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/acquire_bar_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/autofocus_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/autofocus_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_setting_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_setting_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         self.framerate_widgets["frames_to_average"].set(
             self.camera_setting_dict["frames_to_average"]
         )
 
         # Physical Dimensions
         self.calculate_physical_dimensions()
         # readout time
-        self.calculate_readout_time()
+        self.update_readout_time()
 
         # after initialization
         self.in_initialization = False
 
     def update_experiment_values(self, *args):
         """Updates experiment yaml file according to the values in View.
 
@@ -345,26 +345,25 @@
             )
             self.mode_widgets["Pixels"].widget.trigger_focusout_validation()
             self.mode_widgets["Pixels"].widget["state"] = "normal"
 
             self.show_verbose_info("Light Sheet Camera Readout Mode")
 
         # calculate readout time
-        self.calculate_readout_time()
+        self.update_readout_time()
 
     def update_exposure_time(self, exposure_time):
         """When camera exposure time is changed, recalculate readout time
 
         Parameters
         ----------
         exposure_time : float
             exposure time in seconds
         """
         self.framerate_widgets["exposure_time"].set(exposure_time)
-        self.calculate_readout_time()
 
     def update_roi(self, btn_name):
         """Update ROI width and height.
 
         Parameters
         ----------
         btn_name : roi button name
@@ -460,51 +459,31 @@
 
         physical_dimensions_x = x_pixel * pixel_size
         physical_dimensions_y = y_pixel * pixel_size
 
         self.roi_widgets["FOV_X"].set(physical_dimensions_x)
         self.roi_widgets["FOV_Y"].set(physical_dimensions_y)
 
-    def calculate_readout_time(self):
-        """Calculate camera readout time.
+    def update_readout_time(self):
+        """Update camera readout time.
 
 
         TODO: Highly specific to Hamamatsu Orca Flash 4.0.
         Should find a way to pass this from the camera to here.
         This should be moved to the camera device/API,
         ideally by calling a command from the camera.
         """
-
-        h = 9.74436e-6  # Readout timing constant
         sensor_mode = self.mode_widgets["Sensor"].get()
-        if (self.readout_speed == 1) and (sensor_mode == "Normal"):
-            h = 32.4812e-6
-        # the ROI height 'subarray_vsize'
-        vn = float(self.roi_widgets["Height"].get())
-        exposure_time = float(self.framerate_widgets["exposure_time"].get())
 
         if sensor_mode == "Normal":
-            #  Area sensor mode operation
-            if self.trigger_source == 1:
-                # Internal Trigger Source
-                readout_time = exposure_time - ((vn / 2) * h)
-
-            if self.trigger_active in [1, 2]:
-                #  External Trigger Source
-                #  Edge == 1, Level == 2
-                readout_time = exposure_time - ((vn / 2) * h + 10 * h)
-
-            elif self.trigger_active == 3:
-                #  External Trigger Source
-                #  Synchronous Readout == 3
-                readout_time = exposure_time - ((vn / 2) * h + 5 * h)
+            readout_time = self.camera_setting_dict["readout_time"]
 
         elif sensor_mode == "Light-Sheet":
             #  Progressive sensor mode operation
-            readout_time = exposure_time - 1 / (exposure_time + (vn + 10) * h)
+            readout_time = 0
 
         # return readout_time
         self.framerate_widgets["readout_time"].set(readout_time)
 
     def update_number_of_pixels(self, *args):
         """Update the number of pixels in the ROI.
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/camera_view_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_view_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/channel_setting_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channel_setting_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/channels_tab_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channels_tab_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,7 +844,22 @@
             try:
                 float(self.microscope_state_dict["stack_pause"])
             except:
                 return "Stack pause should be a valid number!"
             if self.microscope_state_dict["timepoints"] < 1:
                 return "Timepoints should be at least 1!"
         return None
+    
+    def set_exposure_time(self, channel, exposure_time):
+        """Set exposure time for a specified channel
+        
+        Parameters
+        ----------
+        channel : str
+            Channel name, such as "channel_1", "channel_2",...
+        exposure_time : float
+            Exposure time in miliseconds.
+        """
+        idx = int(channel[channel.index('_')+1:]) - 1
+        self.channel_setting_controller.in_initialization = True
+        self.channel_setting_controller.view.exptime_variables[idx].set(exposure_time)
+        self.channel_setting_controller.in_initialization = False
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/features_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/features_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/gui_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/gui_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/ilastik_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/ilastik_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/keystroke_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/keystroke_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/menu_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/menu_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,23 @@
     FeatureAdvancedSettingController,
     AdaptiveOpticsPopupController,
     UninstallPluginController,
 )
 from navigate.tools.file_functions import save_yaml_file, load_yaml_file
 from navigate.tools.decorators import FeatureList
 from navigate.tools.common_functions import load_module_from_file
-from navigate.config.config import get_navigate_path
 
 
+# Misc. Local Imports
+from navigate.config.config import (
+    update_config_dict,
+    verify_waveform_constants,
+    get_navigate_path,
+)
+
 # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
 class FakeEvent:
     """Fake event class for keyboard shortcuts"""
@@ -84,16 +90,18 @@
         char: str
             The character that was pressed.
         keysym: str
             The key that was pressed.
         """
         #: str: The character that was pressed.
         self.char = char
+
         #: str: The key that was pressed.
         self.keysym = keysym
+
         #: int: The state of the keyboard.
         self.state = 0
 
 
 class MenuController(GUIController):
     """Menu controller class."""
 
@@ -104,32 +112,42 @@
         ----------
         view: class
             The view class.
         parent_controller
             The parent controller.
         """
         super().__init__(view, parent_controller)
+
         #: Controller: The parent controller.
         self.parent_controller = parent_controller
+
         #: tk.canvas: The view class.
         self.view = view
+
         #: tkinter.StringVar: Resolution value.
         self.resolution_value = tk.StringVar()
+
         #: tkinter.IntVar: Feature id value.
         self.feature_id_val = tk.IntVar()
+
         #: tkinter.IntVar: Disable stage limits.
         self.disable_stage_limits = tk.IntVar()
+
         #: FakeEvent: Fake event.
         self.fake_event = None
+
         #: list: List of feature list names.
         self.feature_list_names = []
+
         #: int: System feature list count.
         self.system_feature_list_count = 0
+
         #: int: Feature list count.
         self.feature_list_count = 0
+
         #: str: Feature list file name.
         self.feature_list_file_name = "feature_lists.yaml"
 
     def initialize_menus(self):
         """Initialize menus
         This function defines all the menus in the menubar
 
@@ -182,14 +200,28 @@
                 "Save Experiment": [
                     "standard",
                     self.save_experiment,
                     "Ctrl+Shift+S",
                     "<Control-S>",
                     "<Control_L-S>",
                 ],
+                "Load Waveform Constants": [
+                    "standard",
+                    self.load_waveform_constants,
+                    None,
+                    None,
+                    None,
+                ],
+                "Save Waveform Constants": [
+                    "standard",
+                    self.save_waveform_constants,
+                    None,
+                    None,
+                    None,
+                ],
                 "add_separator": [None],
                 "Toggle Save Data": [
                     "standard",
                     self.toggle_save,
                     "Ctrl+s",
                     "<Control-s>",
                     "<Control_L-s>",
@@ -686,14 +718,53 @@
         filename = filedialog.asksaveasfilename(
             defaultextension=".yml", filetypes=[("Yaml file", "*.yml *.yaml")]
         )
         if not filename:
             return
         save_yaml_file("", self.parent_controller.configuration["experiment"], filename)
 
+    def save_waveform_constants(self):
+        """Save a waveform constants file
+
+        Updates model.waveform_constants and saves it to file
+
+        """
+        filename = filedialog.asksaveasfilename(
+            defaultextension=".yml", filetypes=[("Yaml file", "*.yml *.yaml")]
+        )
+        if not filename:
+            return
+        save_yaml_file(
+            "", self.parent_controller.configuration["waveform_constants"], filename
+        )
+
+    def load_waveform_constants(self):
+        """Load a waveform constants file"""
+
+        filename = filedialog.askopenfilename(
+            defaultextension=".yml", filetypes=[("Yaml files", "*.yml *.yaml")]
+        )
+        if not filename:
+            return
+
+        update_config_dict(
+            self.parent_controller.manager,
+            self.parent_controller.configuration,
+            "waveform_constants",
+            filename,
+        )
+        verify_waveform_constants(
+            self.parent_controller.manager, self.parent_controller.configuration
+        )
+
+        if hasattr(self.parent_controller, "waveform_popup_controller"):
+            self.parent_controller.waveform_popup_controller.populate_experiment_values(
+                force_update=True
+            )
+
     def load_images(self):
         """Load images from a file."""
         filenames = filedialog.askopenfilenames(
             defaultextension=".tif", filetypes=[("tiff files", "*.tif *.tiff")]
         )
         if not filenames:
             return
@@ -758,17 +829,21 @@
             return
         af_popup = AutofocusPopup(self.view)
         self.parent_controller.af_popup_controller = AutofocusPopupController(
             af_popup, self.parent_controller
         )
 
     def popup_waveform_setting(self):
+        """Pop up the Waveform setting window.
+
+        If the window is already open, show it. Otherwise, create a new one."""
         if hasattr(self.parent_controller, "waveform_popup_controller"):
             self.parent_controller.waveform_popup_controller.showup()
             return
+
         waveform_constants_popup = WaveformParameterPopupWindow(
             self.view, self.parent_controller.configuration_controller
         )
         waveform_popup_controller = WaveformPopupController(
             waveform_constants_popup,
             self.parent_controller,
             self.parent_controller.waveform_constants_path,
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/microscope_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/microscope_popup_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             ] = self.primary_microscope
             zoom = self.parent_controller.configuration["waveform_constants"][
                 "remote_focus_constants"
             ][self.primary_microscope].keys()[0]
             self.parent_controller.configuration["experiment"]["MicroscopeState"][
                 "zoom"
             ] = zoom
-            self.parent_controller.resolution_value.set(
+            self.parent_controller.menu_controller.resolution_value.set(
                 f"{self.primary_microscope} {zoom}"
             )
 
         has_multi_cameras = False
         for microscope_name in self.microscope_info.keys():
             if self.variables[microscope_name].get() == "Additional Microscope":
                 config = {}
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/multi_position_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/multi_position_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/plugins_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/plugins_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/stage_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/stage_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/tiling_wizard_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/waveform_popup_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_popup_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,52 +71,65 @@
         # Microscope information
         #: dict: Waveform constants for the microscope.
         self.resolution_info = self.parent_controller.configuration[
             "waveform_constants"
         ]
         #: dict: Galvo constants for the microscope.
         self.galvo_setting = self.resolution_info["galvo_constants"]
+
         #: ConfigurationController: The configuration controller.
         self.configuration_controller = self.parent_controller.configuration_controller
+
         #: str: The path to the waveform constants file.
         self.waveform_constants_path = waveform_constants_path
 
         # Get mode and mag widgets
         #: dict: The widgets for the mode and magnification.
         self.widgets = self.view.get_widgets()
+
         #: dict: The variables for the mode and magnification.
         self.variables = self.view.get_variables()
 
         # Get configuration
         #: list: The lasers.
         self.lasers = self.configuration_controller.lasers_info
 
-        # Initialize
         #: str: The current resolution.
         self.resolution = None
+
         #: str: The current magnification.
         self.mag = None
+
         #: str: The current microscope operation mode.
         self.mode = "stop"
+
         #: dict: Remote focus experiment dictionary.
         self.remote_focus_experiment_dict = None
+
         #: bool: Flag to update galvo device.
         self.update_galvo_device_flag = None
+
         #: bool: Flag to update waveform parameters.
         self.update_waveform_parameters_flag = False
+
         #: bool: Flag to enable/disable waveforms.
         self.waveforms_enabled = True
+
         #: dict: Dictionary of amplitude values.
         self.amplitude_dict = None
+
         #: float: the minimum value of remote focus device
         self.laser_min = 0
+
         #: float: the maximum value of remote focus device
         self.laser_max = 1.0
+
         #: dict: Dictionary of galvo minimum values
         self.galvo_min = {}
+
         #: dict: Dictionary of galvo maximum values
         self.galvo_max = {}
 
         # event id list
         #: int: The event id.
         self.event_id = None
 
@@ -157,14 +170,17 @@
             )
 
         # Changes in the delay, duty cycle, and smoothing waveform parameters
         # Delay, Duty, and Smoothing
         self.variables["Delay"].trace_add("write", self.update_waveform_parameters)
         self.variables["Duty"].trace_add("write", self.update_waveform_parameters)
         self.variables["Smoothing"].trace_add("write", self.update_waveform_parameters)
+        self.variables["Ramp_falling"].trace_add(
+            "write", self.update_waveform_parameters
+        )
 
         # Save waveform constants
         self.view.get_buttons()["Save"].configure(command=self.save_waveform_constants)
 
         # Temporarily disable waveforms
         self.view.get_buttons()["toggle_waveform_button"].configure(
             command=self.toggle_waveform_state
@@ -200,27 +216,37 @@
 
         This function updates the widget ranges and precisions based on the current
         resolution mode. The precision is set to -3 for high and nanoscale modes and -2
         for low mode. The increment is set to 0.001 for high and nanoscale modes and
         0.01 for low mode.
 
         """
-        self.laser_min = self.configuration_controller.remote_focus_dict["hardware"]["min"]
-        self.laser_max = self.configuration_controller.remote_focus_dict["hardware"]["max"]
-        
-        precision = int(self.configuration_controller.remote_focus_dict["hardware"].get("precision", 0))
-        increment = int(self.configuration_controller.remote_focus_dict["hardware"].get("step", 0))
+        self.laser_min = self.configuration_controller.remote_focus_dict["hardware"][
+            "min"
+        ]
+        self.laser_max = self.configuration_controller.remote_focus_dict["hardware"][
+            "max"
+        ]
+
+        precision = int(
+            self.configuration_controller.remote_focus_dict["hardware"].get(
+                "precision", 0
+            )
+        )
+        increment = int(
+            self.configuration_controller.remote_focus_dict["hardware"].get("step", 0)
+        )
         if precision == 0:
             precision = -4 if self.laser_max < 1 else -3
         elif precision > 0:
-            precision = - precision
+            precision = -precision
         if increment == 0:
             increment = 0.0001 if self.laser_max < 1 else 0.001
         elif increment < 0:
-            increment = - increment
+            increment = -increment
 
         # set ranges of value for those lasers
         for laser in self.lasers:
             self.widgets[laser + " Amp"].widget.configure(from_=self.laser_min)
             self.widgets[laser + " Amp"].widget.configure(to=self.laser_max)
             self.widgets[laser + " Amp"].widget.configure(increment=increment)
             self.widgets[laser + " Amp"].widget.set_precision(precision)
@@ -272,27 +298,33 @@
         # However, sometimes we have a resonant galvo.
         # In the case of the resonant galvo, amplitude is zero and only the offset
         # can be controlled. We only define the offset in the configuration.yml file.
         # If only the offset is defined for galvo_{focus_prefix}, we disable the
         # amplitude.
         #
 
-    def populate_experiment_values(self):
+    def populate_experiment_values(self, force_update=False):
         """Set experiment values."""
         self.remote_focus_experiment_dict = self.parent_controller.configuration[
             "experiment"
         ]["MicroscopeState"]
         resolution_value = self.remote_focus_experiment_dict["microscope_name"]
         zoom_value = self.remote_focus_experiment_dict["zoom"]
         mag = zoom_value
-        if (
-            self.widgets["Mode"].get() == resolution_value
+        if (not force_update
+            and self.widgets["Mode"].get() == resolution_value
             and self.widgets["Mag"].get() == mag
         ):
             return
+
+        # Microscope information
+        self.resolution_info = self.parent_controller.configuration[
+            "waveform_constants"
+        ]
+        self.galvo_setting = self.resolution_info["galvo_constants"]
         self.widgets["Mode"].set(resolution_value)
         self.show_magnification(mag)
 
     def showup(self):
         """This function will let the popup window show in front."""
         self.view.popup.deiconify()
         self.view.popup.attributes("-topmost", 1)
@@ -366,34 +398,30 @@
         self.update_galvo_device_flag = True
 
         # Load waveform parameters from configuration - Smooth, Delay, Duty Cycle.
         # Provide defaults should loading fail.
         # Currently pulls from the original microscope configuration YAML file, not the
         # current microscope configuration according to the model
         self.update_waveform_parameters_flag = False
-        waveform_configuration = self.resolution_info["remote_focus_constants"][
-            self.resolution
-        ][self.mag][self.lasers[0]]
         self.widgets["Smoothing"].set(
-            waveform_configuration.get("percent_smoothing", 0)
+            self.resolution_info["other_constants"].get("percent_smoothing", 0)
         )
         self.widgets["Smoothing"].widget.trigger_focusout_validation()
-        self.widgets["Delay"].set(waveform_configuration.get("percent_delay", 7.5))
+        self.widgets["Delay"].set(
+            self.resolution_info["other_constants"].get("remote_focus_delay", 7.5)
+        )
         self.widgets["Delay"].widget.trigger_focusout_validation()
-        if "other_constants" not in self.resolution_info:
-            update_config_dict(
-                self.parent_controller.manager,
-                self.resolution_info,
-                "other_constants",
-                {"remote_focus_settle_duration": 0},
-            )
         self.widgets["Duty"].set(
             self.resolution_info["other_constants"]["remote_focus_settle_duration"]
         )
         self.widgets["Duty"].widget.trigger_focusout_validation()
+        self.widgets["Ramp_falling"].set(
+            self.resolution_info["other_constants"]["remote_focus_ramp_falling"]
+        )
+        self.widgets["Ramp_falling"].widget.trigger_focusout_validation()
         self.update_waveform_parameters_flag = True
 
         # update resolution value in central controller (menu)
         value = f"{self.resolution} {self.mag}"
         if self.parent_controller.menu_controller.resolution_value.get() != value:
             self.parent_controller.menu_controller.resolution_value.set(value)
 
@@ -431,15 +459,15 @@
                 f"Remote Focus Amplitude/Offset Changed pre if statement: "
                 f"{variable_value}"
             )
             if value != variable_value and variable_value != "":
                 # tell parent controller (the device)
                 if self.event_id:
                     self.view.popup.after_cancel(self.event_id)
-                
+
                 try:
                     value = float(variable_value)
                 except ValueError:
                     return
                 if value < self.laser_min or value > self.laser_max:
                     return
                 self.resolution_info["remote_focus_constants"][self.resolution][
@@ -469,92 +497,97 @@
         *args : tuple
             The first element is the new waveform.
         **wargs : dict
             The key is the name of the waveform and the value is the waveform
         """
         if not self.update_waveform_parameters_flag:
             return
-        
+
         if self.event_id:
             self.view.popup.after_cancel(self.event_id)
         # Get the values from the widgets.
         try:
             delay = float(self.widgets["Delay"].widget.get())
             duty_cycle = float(self.widgets["Duty"].widget.get())
             smoothing = float(self.widgets["Smoothing"].widget.get())
+            ramp_falling = float(self.widgets["Ramp_falling"].widget.get())
         except ValueError:
             return
 
         # Update the waveform parameters
         # all the lasers use the same delay, smoothing value
-        for laser in self.lasers:
-            self.resolution_info["remote_focus_constants"][self.resolution][self.mag][
-                laser
-            ]["percent_delay"] = delay
-            self.resolution_info["remote_focus_constants"][self.resolution][self.mag][
-                laser
-            ]["percent_smoothing"] = smoothing
         self.resolution_info["other_constants"][
             "remote_focus_settle_duration"
         ] = duty_cycle
+        self.resolution_info["other_constants"][
+            "remote_focus_ramp_falling"
+        ] = ramp_falling
+        self.resolution_info["other_constants"]["remote_focus_delay"] = delay
+        self.resolution_info["other_constants"]["percent_smoothing"] = smoothing
 
         # Pass the values to the parent controller.
         self.event_id = self.view.popup.after(
             500,
             lambda: self.parent_controller.execute(
                 "update_setting", "waveform_parameters"
             ),
         )
 
     def estimate_galvo_setting(self, *args, **kwargs):
-        """Estimate galvo settings according to the acquisition parameters.
+        """Digitally scanned light-sheet frequency estimation.
 
-        Will only work if all channels have the same exposure duration.
-        Gets the line interval from the camera, number of pixels from the light-sheet
-        mode, and estimates the frequency as 1 / (line interval * number of pixels).
+        When imaging in a digitally scanned light-sheet mode, the galvo must
+        operate at a specific frequency, otherwise periodic lines will appear in
+        the image. This function estimates the frequency of the galvo based on the
+        line interval and the number of pixels in the light-sheet mode.
+
+        Note
+        ----
+            Will only work if all channels have the same exposure duration.
+            The framerate widget doesn't update unless you change the
+            exposure time in the channel settings. Default is 100ms.
 
         Parameters
         ----------
         *args : tuple
             The first element is the name of the galvo.
         **kwargs : dict
             The key is the name of the galvo and the value is the galvo setting.
         """
 
+        # Get the name of the galvo.
         galvo_name = args[0]
 
+        # Get the number of pixels in the light-sheet mode.
         number_of_pixels = (
             self.parent_controller.camera_setting_controller.mode_widgets[
                 "Pixels"
             ].get()
         )
+
+        # If not in the light-sheet mode, widget returns an empty string.
         if number_of_pixels == "":
-            # If we are not in the light-sheet mode, widget returns an empty string.
             return
 
-        # TODO: Worth noting that this doesn't matter because it cancels out in the
-        # frequency bit, but this is often not the right value. The framerate widget
-        # doesn't update unless you change the exposure time in the channel settings.
-        # It launches as a default of 100 ms every time.
+        # Get the exposure time. Convert to seconds.
         exposure_time = (
             self.parent_controller.camera_setting_controller.framerate_widgets[
                 "exposure_time"
             ].get()
         )
+        exposure_time = exposure_time / 1000
 
-        # The camera line interval won't be set until starting acquisition,
-        # we need to calculate it directly
-        # exposure_time and light_sheet_exposure_time are both ms
+        # Get the light sheet exposure time.
         (
-            light_sheet_exposure_time,
-            _,
+            light_sheet_exposure_time, _, _,
         ) = self.parent_controller.model.get_camera_line_interval_and_exposure_time(
             exposure_time, int(number_of_pixels) + 1
-        )  # TODO: Unclear why we need the +1. Figure out the reason.
+        )
 
+        # Calculate the frequency of the galvo.
         frequency = 2 / light_sheet_exposure_time * exposure_time
 
         # Update the GUI
         self.view.inputs[galvo_name].widget.set(round(frequency, 3))
 
     def update_galvo_setting(self, galvo_name, widget_name, parameter):
         """Update galvo settings in memory.
@@ -591,26 +624,29 @@
                 f"Galvo parameter {parameter} changed: "
                 f"{variable_value} pre if statement"
             )
             if value != variable_value and variable_value != "":
                 # change any galvo parameters as one event
                 if self.event_id:
                     self.view.popup.after_cancel(self.event_id)
-                
+
                 try:
                     value = float(variable_value)
                 except ValueError:
                     return
-                if value < self.galvo_min[galvo_name] or value > self.galvo_max[galvo_name]:
+                if "Freq" not in widget_name and (
+                    value < self.galvo_min[galvo_name]
+                    or value > self.galvo_max[galvo_name]
+                ):
                     return
                 self.galvo_setting[galvo_name][self.resolution][self.mag][
                     parameter
                 ] = variable_value
                 logger.debug(f"Galvo parameter {parameter} changed: {variable_value}")
-                
+
                 self.event_id = self.view.popup.after(
                     500,
                     lambda: self.parent_controller.execute("update_setting", "galvo"),
                 )
 
         return func_galvo
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/sub_controllers/waveform_tab_controller.py` & `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_tab_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,16 @@
         max_camera_waveform = 0
         min_camera_waveform = 1000000
         max_remote_focus_waveform = 0
         min_remote_focus_waveform = 1000000
         # two pass
         for k in self.waveform_dict["camera_waveform"].keys():
             remote_focus_waveform = self.waveform_dict["remote_focus_waveform"][k]
+            if remote_focus_waveform is None:
+                continue
             max_remote_focus_waveform = np.maximum(max_remote_focus_waveform, np.max(remote_focus_waveform))
             min_remote_focus_waveform = np.minimum(min_remote_focus_waveform, np.min(remote_focus_waveform))
             camera_waveform = self.waveform_dict["camera_waveform"][k]
             max_camera_waveform = np.maximum(max_camera_waveform, np.max(camera_waveform))
             min_camera_waveform = np.minimum(min_camera_waveform, np.min(camera_waveform))
             for galvo_waveform in self.waveform_dict["galvo_waveform"]:
                 max_galvo_waveform = np.maximum(max_galvo_waveform, np.max(galvo_waveform[k]))
```

### Comparing `navigate-micro-0.0.4/src/navigate/controller/thread_pool.py` & `navigate-micro-0.0.5/src/navigate/controller/thread_pool.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/log_files/filters.py` & `navigate-micro-0.0.5/src/navigate/log_files/filters.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/log_files/log_functions.py` & `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_ni.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,179 +27,158 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 # Standard Library Imports
-import logging.config
-import logging.handlers
-from pathlib import Path
-import os
-import sys
-import traceback
-from datetime import datetime
+import logging
 
 # Third Party Imports
-import yaml
+import nidaqmx
+from nidaqmx.errors import DaqError
+from nidaqmx.constants import LineGrouping
 
 # Local Imports
-from navigate.config.config import get_navigate_path
+from navigate.model.devices.lasers.laser_base import LaserBase
 
+# Logger Setup
+p = __name__.split(".")[1]
+logger = logging.getLogger(p)
 
-def update_nested_dict(d, find_func, apply_func):
-    """Update a nested dictionary by applying a function to a value
 
-    Loops through a nested dictionary and if find_func() conditions are met,
-    run apply_func on that key.
+class LaserNI(LaserBase):
+    """LaserNI Class
 
-    TODO: This is highly general and doesn't belong here.
-    TODO: It might be nice to make this non-recursive.
-
-    Parameters
-    ----------
-    d : dict
-        Dictionary to be updated
-    find_func : func
-        Accepts key, value pair and matches a condition based on these. Returns bool.
-    apply_func : func
-        Accepts a value returns the new value.
-
-    Returns
-    -------
-    d2 : dict
-        An version of d, updated according to the passed functions.
+    This class is used to control a laser connected to a National Instruments DAQ.
     """
-    d2 = {}
-    for k, v in d.items():
-        if find_func(k, v):
-            d2[k] = apply_func(v)
-        else:
-            d2[k] = v
-        if isinstance(v, dict):
-            d2[k] = update_nested_dict(v, find_func, apply_func)
-    return d2
-
-
-def find_filename(k, v):
-    """Check that we've met the condition dictionary key == 'filename'
-
-    Parameters
-    ----------
-    k : str
-        Dictionary key
-    v : str
-        Dictionary value
-
-    Returns
-    -------
-    bool
-        True if k == 'filename', False otherwise
-
-    Examples
-    --------
-    >>> find_filename('filename', 'test')
-    """
-    if k == "filename":
-        return True
-    return False
-
-
-def log_setup(logging_configuration, logging_path=None):
-    """Setup logging configuration
-
-    Initialize a logger from a YAML file containing information in the Python logging
-    dictionary format.
-
-    Note
-    ----
-        Additional information here:
-        https://docs.python.org/3/library/logging.config.html#logging-config-dictschema
-
-    Parameters
-    ----------
-    logging_configuration : str
-        Path to file to be loaded.
-        Relative to the location of the folder containing this file.
-    logging_path : str, optional
-        Path to store logs. Defaults to navigate_path/logs
-    """
-
-    # path to logging_configuration is set relative
-    # to the location of the folder containing this file (log_functions.py)
-    base_directory = Path(__file__).resolve().parent
-    logging_configuration_path = Path.joinpath(base_directory, logging_configuration)
-
-    # Save directory for logging information.
-    time = datetime.now()
-    time_stamp = Path(
-        "%s-%s-%s-%s%s"
-        % (
-            f"{time.year:04d}",
-            f"{time.month:02d}",
-            f"{time.day:02d}",
-            f"{time.hour:02d}",
-            f"{time.minute:02d}",
-        )
-    )
-
-    if logging_path is None:
-        logging_path = Path.joinpath(Path(get_navigate_path()), "logs")
-    todays_path = Path.joinpath(logging_path, time_stamp)
-    if not os.path.exists(logging_path):
-        os.mkdir(logging_path)
-    if not os.path.exists(todays_path):
-        os.mkdir(todays_path)
 
-    def update_filename(v):
-        """Function to map filename to base_directory/filename in the dictionary
+    def __init__(self, microscope_name, device_connection, configuration, laser_id):
+        """Initialize the LaserNI class.
 
         Parameters
         ----------
-        v : str
-            Value to be updated
-
-        Returns
-        -------
-        Path : str
-            Path to the log file
+        microscope_name : str
+            The microscope name.
+        device_connection : object
+            The device connection object.
+        configuration : dict
+            The device configuration.
+        laser_id : str
+            The laser id.
         """
-        return Path.joinpath(todays_path, v)
+        super().__init__(microscope_name, device_connection, configuration, laser_id)
+
+        #: str: Modulation type of the laser - Analog or Digital.
+        self.on_off_type = None
+
+        # Digital out (if using mixed modulation mode)
+        try:
+            laser_do_port = self.device_config["onoff"]["hardware"]["channel"]
+
+            #: float: The minimum digital modulation voltage.
+            self.laser_min_do = self.device_config["onoff"]["hardware"]["min"]
+
+            #: float: The maximum digital modulation voltage.
+            self.laser_max_do = self.device_config["onoff"]["hardware"]["max"]
+
+            #: object: The laser analog or digital modulation task.
+            self.laser_do_task = nidaqmx.Task()
+
+            if "/ao" in laser_do_port:
+                # Artificial Digital Modulation via an Analog Port
+                self.laser_do_task.ao_channels.add_ao_voltage_chan(
+                    laser_do_port, min_val=self.laser_min_do, max_val=self.laser_max_do
+                )
+                self.on_off_type = "analog"
+
+            else:
+                # Digital Modulation via a Digital Port
+                self.laser_do_task.do_channels.add_do_chan(
+                    laser_do_port, line_grouping=LineGrouping.CHAN_FOR_ALL_LINES
+                )
+                self.on_off_type = "digital"
+        except (KeyError, DaqError) as e:
+            self.laser_do_task = None
+            if isinstance(e, DaqError):
+                logger.exception(e)
+                logger.debug(e.error_code)
+                logger.debug(e.error_type)
+                print(e)
+                print(e.error_code)
+                print(e.error_type)
 
-    # Read the logging configuration file.
-    with open(logging_configuration_path, "r") as f:
+        #: float: Current laser intensity.
+        self._current_intensity = 0
+
+        # Analog out
         try:
-            config_data = yaml.load(f.read(), Loader=yaml.FullLoader)
+            laser_ao_port = self.device_config["power"]["hardware"]["channel"]
+
+            #: float: The minimum analog modulation voltage.
+            self.laser_min_ao = self.device_config["power"]["hardware"]["min"]
+
+            #: float: The maximum analog modulation voltage.
+            self.laser_max_ao = self.device_config["power"]["hardware"]["max"]
 
-            # Force all log files to be created relative to logging_path
-            config_data2 = update_nested_dict(
-                config_data, find_filename, update_filename
+            #: object: The laser analog modulation task.
+            self.laser_ao_task = nidaqmx.Task()
+            self.laser_ao_task.ao_channels.add_ao_voltage_chan(
+                laser_ao_port, min_val=self.laser_min_ao, max_val=self.laser_max_ao
             )
-            logging.config.dictConfig(config_data2)
+        except DaqError as e:
+            logger.exception(e)
+            logger.debug(e.error_code)
+            logger.debug(e.error_type)
+            print(e)
+            print(e.error_code)
+            print(e.error_type)
 
-            # Configures our loggers from updated logging.yml
-        except yaml.YAMLError as yaml_error:
-            print(yaml_error)
+    def set_power(self, laser_intensity):
+        """Sets the laser power.
 
+        Parameters
+        ----------
+        laser_intensity : float
+            The laser intensity.
+        """
+        try:
+            scaled_laser_voltage = (int(laser_intensity) / 100) * self.laser_max_ao
+            self.laser_ao_task.write(scaled_laser_voltage, auto_start=True)
+            self._current_intensity = laser_intensity
+        except DaqError as e:
+            logger.exception(e)
 
-def main_process_listener(queue):
-    """Listener function for the main process
+    def turn_on(self):
+        """Turns on the laser."""
+        try:
+            self.set_power(self._current_intensity)
+            if self.laser_do_task is not None:
+                if self.on_off_type == "digital":
+                    self.laser_do_task.write(True, auto_start=True)
+                elif self.on_off_type == "analog":
+                    self.laser_do_task.write(self.laser_max_do, auto_start=True)
+        except DaqError as e:
+            logger.exception(e)
 
-    This function will listen for new logs put in queue from sub processes,
-    it will then log via the main process.
+    def turn_off(self):
+        """Turns off the laser."""
+        try:
+            tmp = self._current_intensity
+            self.set_power(0)
+            self._current_intensity = tmp
+            if self.laser_do_task is not None:
+                if self.on_off_type == "digital":
+                    self.laser_do_task.write(False, auto_start=True)
+                elif self.on_off_type == "analog":
+                    self.laser_do_task.write(self.laser_min_do, auto_start=True)
+        except DaqError as e:
+            logger.exception(e)
 
-    Parameters
-    ----------
-    queue : multiprocessing.Queue
-        Queue to listen for new logs
-    """
-    while True:
+    def close(self):
+        """Close the NI Task before exit."""
         try:
-            record = queue.get()
-            if record is None:
-                # Sentinel to tell listener to stop
-                break
-            logger = logging.getLogger(record.name)
-            logger.handle(record)
-        except Exception:
-            print("Whoops! Problem: ", file=sys.stderr)
-            traceback.print_exc(file=sys.stderr)
+            self.laser_ao_task.close()
+            if self.laser_do_task is not None:
+                self.laser_do_task.close()
+        except DaqError as e:
+            logger.exception(e)
```

### Comparing `navigate-micro-0.0.4/src/navigate/log_files/logging.yml` & `navigate-micro-0.0.5/src/navigate/log_files/logging.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/log_files/model_logging.yml` & `navigate-micro-0.0.5/src/navigate/log_files/model_logging.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/main.py` & `navigate-micro-0.0.5/src/navigate/main.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/analysis/boundary_detect.py` & `navigate-micro-0.0.5/src/navigate/model/analysis/boundary_detect.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/analysis/camera.py` & `navigate-micro-0.0.5/src/navigate/model/analysis/camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/analysis/image_contrast.py` & `navigate-micro-0.0.5/src/navigate/model/analysis/image_contrast.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/concurrency/concurrency_tools.py` & `navigate-micro-0.0.5/src/navigate/model/concurrency/concurrency_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/data_sources/__init__.py` & `navigate-micro-0.0.5/src/navigate/model/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/data_sources/bdv_data_source.py` & `navigate-micro-0.0.5/src/navigate/model/data_sources/bdv_data_source.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/data_sources/data_source.py` & `navigate-micro-0.0.5/src/navigate/model/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/data_sources/tiff_data_source.py` & `navigate-micro-0.0.5/src/navigate/model/data_sources/tiff_data_source.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/device_startup_functions.py` & `navigate-micro-0.0.5/src/navigate/model/device_startup_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1230,17 +1230,30 @@
             except RuntimeError as e:
                 if "camera" in plugin_devices:
                     camera = plugin_devices["camera"]["load_device"](
                         configuration, id, is_synthetic
                     )
 
             if (not is_synthetic) and device["type"].startswith("Hamamatsu"):
+                camera_serial_number = str(camera._serial_number)
                 device_ref_name = build_ref_name(
-                    "_", device["type"], str(camera._serial_number)
+                    "_", device["type"], camera_serial_number
                 )
+                # if the serial number has leading zeros,
+                # the yaml reader will convert it to an octal number
+                if camera_serial_number.startswith("0"):
+                    try:
+                        oct_num = int(camera_serial_number, 8)
+                        devices["camera"][build_ref_name(
+                            "_",
+                            device["type"],
+                            oct_num
+                        )] = camera
+                    except ValueError:
+                        pass
             else:
                 device_ref_name = build_ref_name(
                     "_", device["type"], device["serial_number"]
                 )
             devices["camera"][device_ref_name] = camera
 
     # load mirror
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/coherent/ObisLaser.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/ObisLaser.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,24 +637,25 @@
 
 
 property_dict = {
     "exposure_time": 2031888,  # 0x001F0110, R/W, sec, "EXPOSURE TIME"
     "sensor_mode": 4194832,  # 0x00400210, R/W, mode,  "SENSOR MODE"
     "defect_correct_mode": 4653072,  # 0x00470010, R/W, mode,  "DEFECT CORRECT MODE"
     "binning": 4198672,  # 0x00401110, R/W, mode, "BINNING"
+    "subarray_mode": 4202832,  # 0x00402150, R/W, mode,   "SUBARRAY MODE"
     "readout_speed": 4194576,  # 0x00400110, R/W, long,    "READOUT SPEED"
     "readout_direction": 4194608,  # 0x00400130, R/W, mode,   "READOUT DIRECTION"
     "readout_time": 4206608,  # 0x00403010, R/O, sec,   "TIMING READOUT TIME"
     "trigger_active": 1048864,  # 0x00100120, R/W, mode,   "TRIGGER ACTIVE"
     "trigger_mode": 1049104,  # 0x00100210, R/W, mode,    "TRIGGER MODE"
     "trigger_polarity": 1049120,  # 0x00100220, R/W, mode, "TRIGGER POLARITY"
     "trigger_source": 1048848,  # 0x00100110, R/W, mode,   "TRIGGER SOURCE"
     "trigger_delay": 1049184,  # 0x00100260,	/* R/W, sec,	"TRIGGER DELAY"
-    "internal_line_interval": 4208720,  # 0x00403850, R/W, sec,
-    # "INTERNAL LINE INTERVAL"
+    "internal_line_interval": 4208720,  # 0x00403850, R/W, sec,    "INTERNAL LINE INTERVAL"
+    "internal_line_speed": 4208704,  # 0x00403840, R/W, m/sec,    "INTERNAL LINE SPEED"
     "image_width": 4325904,  # 0x00420210, R/O, long, "IMAGE WIDTH"
     "image_height": 4325920,  # 0x00420220, R/O, long,    "IMAGE HEIGHT"
     "exposuretime_control": 2031920,  # 0x001F0130, R/W, mode,
     # "EXPOSURE TIME CONTROL"
     "subarray_hpos": 4202768,  # 0x00402110, R/W, long,    "SUBARRAY HPOS"
     "subarray_hsize": 4202784,  # 0x00402120, R/W, long,   "SUBARRAY HSIZE"
     "subarray_vpos": 4202800,  # 0x00402130, R/W, long,    "SUBARRAY VPOS"
@@ -1009,16 +1010,17 @@
 
         if property_value_min is None:
             print("Could not set attribute", name)
             print("property range:", name, property_value_min, property_value_max)
             return False
 
         # Cast value to a multiple of step size
-        if property_value_step > 0:
-            value = int(value // property_value_step) * property_value_step
+        # The cast will cause accuracy problems when setting exposure time
+        # if property_value_step > 0:
+        #     value = int(value // property_value_step) * property_value_step
 
         if value < property_value_min:
             print(
                 " The property value of ",
                 value,
                 "is less than minimum of",
                 property_value_min,
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/imagineoptics/imop.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/imop.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/mcl/madlib.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/madlib.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/omicron/LuxxLaser.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/LuxxLaser.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/sutter/MP285.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/MP285.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py` & `navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/__init__.py` & `navigate-micro-0.0.5/src/navigate/model/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,32 +79,32 @@
             microscope_name
         ]["camera"]
 
         #: bool: Whether the camera is currently acquiring
         self.is_acquiring = False
 
         # Initialize Pixel Information
-        #: int: Maximum image width
-        self.max_image_width = 2048
-        #: int: Maximum image height
-        self.max_image_height = 2048
         #: int: Minimum image width
         self.min_image_width = 4
         #: int: Minimum image height
         self.min_image_height = 4
         #: int: Minimum step size for image width.
         self.step_image_width = 4
         #: int: Minimum step size for image height.
         self.step_image_height = 4
         #: int: Number of pixels in the x direction
-        self.x_pixels = self.max_image_width
+        self.x_pixels = 2048
         #: int: Number of pixels in the y direction
-        self.y_pixels = self.max_image_height
-        self.camera_parameters["x_pixels"] = self.max_image_width
-        self.camera_parameters["y_pixels"] = self.max_image_height
+        self.y_pixels = 2048
+        #: float: minimum exposure time
+        self.minimum_exposure_time = 0.001
+        self.camera_parameters["x_pixels"] = 2048
+        self.camera_parameters["y_pixels"] = 2048
+        # TODO: trigger_source, readout_speed, trigger_active, trigger_mode and trigger_polarity
+        # can be removed after updating how we get the readout time in model and controller
         self.camera_parameters["trigger_source"] = 2.0
         self.camera_parameters["readout_speed"] = 1.0
         self.camera_parameters["pixel_size_in_microns"] = 6.5
         self.camera_parameters["trigger_active"] = 1.0
         self.camera_parameters["trigger_mode"] = 1.0
         self.camera_parameters["trigger_polarity"] = 2.0
         self.camera_parameters["supported_readout_directions"] = [
@@ -190,34 +190,36 @@
     ):
         """Convert normal mode exposure time to light-sheet mode exposure time.
         Calculate the parameters for an acquisition
 
         Parameters
         ----------
         full_chip_exposure_time : float
-            Normal mode exposure time.
+            Normal mode exposure time in seconds.
         shutter_width : int
             Width of light-sheet rolling shutter.
 
         Returns
         -------
         exposure_time : float
-            Light-sheet mode exposure time (ms).
+            Light-sheet mode exposure time (s).
         camera_line_interval : float
             HamamatsuOrca line interval duration (s).
+        full_chip_exposure time : float
+            Full chip exposure time (s).
         """
 
-        camera_line_interval = (full_chip_exposure_time / 1000) / (
+        camera_line_interval = full_chip_exposure_time / (
             shutter_width + self.y_pixels - 1
         )
 
         self.camera_parameters["line_interval"] = camera_line_interval
 
-        exposure_time = camera_line_interval * shutter_width * 1000
-        return exposure_time, camera_line_interval
+        exposure_time = camera_line_interval * shutter_width
+        return exposure_time, camera_line_interval, full_chip_exposure_time
 
     def close_camera(self):
         """Close camera."""
         pass
 
     def get_line_interval(self):
         """Return stored camera line interval.
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_hamamatsu.py` & `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_hamamatsu.py`

 * *Files 26% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 from navigate.model.devices.camera.camera_base import CameraBase
 
 # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
-class HamamatsuOrca(CameraBase):
+class HamamatsuBase(CameraBase):
     """HamamatsuOrca camera class.
 
-    This is by default for an Orca Flash 4.0, Fusion, and Lightning cameras.
+    This is the default parent class for Hamamatsu Cameras.
+    This includes the ORCA Flash 4.0, Fusion, Lightning, and Fire.
 
     **Configuration**::
 
         hardware:
           camera:
             -
                 type: HamamatsuOrca
@@ -88,27 +89,28 @@
 
         Parameters
         ----------
         microscope_name : str
             Name of microscope in configuration
         device_connection : object
             Hardware device to connect to
-        configuration : multiprocesing.managers.DictProxy
+        configuration : multiprocessing.managers.DictProxy
             Global configuration of the microscope
         """
         super().__init__(microscope_name, device_connection, configuration)
 
         #: dict: Camera parameters
-        self.camera_parameters["x_pixels"] = self.max_image_width
-        self.camera_parameters["y_pixels"] = self.max_image_height
-        self.camera_parameters["x_pixels_min"] = self.min_image_width
-        self.camera_parameters["y_pixels_min"] = self.min_image_height
-        self.camera_parameters["x_pixels_step"] = self.step_image_width
-        self.camera_parameters["y_pixels_step"] = self.step_image_height
-        self.camera_parameters["supported_readout_directions"] = ["Top-to-Bottom", "Bottom-to-Top"]
+        self.camera_parameters["x_pixels"] = self.camera_controller.max_image_width
+        self.camera_parameters["y_pixels"] = self.camera_controller.max_image_height
+        self.camera_parameters["x_pixels_min"] = self.camera_controller.min_image_width
+        self.camera_parameters["y_pixels_min"] = self.camera_controller.min_image_height
+        self.camera_parameters["x_pixels_step"] = self.camera_controller.step_image_width
+        self.camera_parameters["y_pixels_step"] = self.camera_controller.step_image_height
+        self.minimum_exposure_time, _, _ = self.camera_controller.get_property_range("exposure_time")
+
         #: object: Camera controller
         if self.camera_controller.get_property_value("readout_speed"):
             _, speed_max, _ = self.camera_controller.get_property_range("readout_speed")
             if speed_max is not None:
                 self.camera_controller.set_property_value("readout_speed", int(speed_max))
                 self.camera_parameters["readout_speed"] = int(speed_max)
             else:
@@ -151,158 +153,43 @@
         Returns
         -------
         serial_number : str
             Serial number for the camera.
         """
         return self.camera_controller._serial_number
 
-    # The pass statements get around camera base calls
-    @property
-    def max_image_width(self):
-        """Get maximum image width.
-
-        Returns
-        -------
-        max_image_width : int
-            Maximum image width.
-        """
-        return self.camera_controller.max_image_width
-
-    @max_image_width.setter
-    def max_image_width(self, value):
-        """Set maximum image width."""
-        pass
-
-    @property
-    def min_image_width(self):
-        """Get minimum image width.
-
-        Returns
-        -------
-        min_image_width : int
-            Minimum image width.
-        """
-        return self.camera_controller.min_image_width
-
-    @min_image_width.setter
-    def min_image_width(self, value):
-        """Set minimum image width.
-
-        Parameters
-        ----------
-        value : int
-            Minimum image width.
-        """
-        pass
-
-    @property
-    def max_image_height(self):
-        """Get maximum image height.
-
-        Returns
-        -------
-        max_image_height : int
-            Maximum image height.
-        """
-        return self.camera_controller.max_image_height
-
-    @max_image_height.setter
-    def max_image_height(self, value):
-        """Set maximum image height.
-
-        Parameters
-        ----------
-        value : int
-            Maximum image height.
-        """
-        pass
-
-    @property
-    def min_image_height(self):
-        """Get minimum image height.
-
-        Returns
-        -------
-        min_image_height : int
-            Minimum image height.
-        """
-        return self.camera_controller.min_image_height
-
-    @min_image_height.setter
-    def min_image_height(self, value):
-        """Set minimum image height.
-
-        Parameters
-        ----------
-        value : int
-            Minimum image height.
-        """
-        pass
-
-    @property
-    def step_image_width(self):
-        """Get step image width.
-
-        Returns
-        -------
-        step_image_width : int
-            Step image width.
-        """
-        return self.camera_controller.step_image_width
-
-    @step_image_width.setter
-    def step_image_width(self, value):
-        """Set step image width.
-
-        Parameters
-        ----------
-        value : int
-            Step image width.
-        """
-        pass
-
-    @property
-    def step_image_height(self):
-        """Get step image height.
-
-        Returns
-        -------
-        step_image_height : int
-            Step image height.
-        """
-        return self.camera_controller.step_image_height
-
-    @step_image_height.setter
-    def step_image_height(self, value):
-        """Step image height."""
-
-        pass
-
     def report_settings(self):
         """Print Camera Settings.
 
         Prints the current camera settings to the console and the log file."""
         params = [
             "defect_correct_mode",
             "sensor_mode",
             "binning",
+            "subarray_mode",
+            "subarray_vsize",
+            "subarray_hsize",
             "readout_speed",
             "trigger_active",
             "trigger_mode",
             "trigger_polarity",
             "trigger_source",
             "internal_line_interval",
+            "internal_line_speed",
             "image_height",
             "image_width",
             "exposure_time",
+            "readout_time"
         ]
         for param in params:
             print(param, self.camera_controller.get_property_value(param))
             logger.info(f"{param}, {self.camera_controller.get_property_value(param)}")
 
+        print("*** exposure time range:", self.camera_controller.get_property_range("exposure_time"))
+
     def close_camera(self):
         """Close HamamatsuOrca Camera"""
         self.camera_controller.dev_close()
 
     def set_sensor_mode(self, mode):
         """Set HamamatsuOrca sensor mode.
 
@@ -322,14 +209,19 @@
                 self.camera_controller.step_image_width,
             ) = self.camera_controller.get_property_range("subarray_hsize")
             (
                 self.camera_controller.min_image_height,
                 _,
                 self.camera_controller.step_image_height,
             ) = self.camera_controller.get_property_range("subarray_vsize")
+            # update configuration dict
+            self.camera_parameters["x_pixels_min"] = self.camera_controller.min_image_width
+            self.camera_parameters["y_pixels_min"] = self.camera_controller.min_image_height
+            self.camera_parameters["x_pixels_step"] = self.camera_controller.step_image_width
+            self.camera_parameters["y_pixels_step"] = self.camera_controller.step_image_height
         else:
             print("Camera mode not supported")
             logger.info("Camera mode not supported")
 
     def set_readout_direction(self, mode):
         """Set HamamatsuOrca readout direction.
 
@@ -361,76 +253,35 @@
         Assumes model C13440 with Camera Link communication from Hamamatsu.
         Currently pulling values directly from the camera.
 
         Returns
         -------
         readout_time : float
             Duration of time needed to readout an image.
-        max_frame_rate : float
-            Maximum framerate for a given camera acquisition mode.
 
-        TODO: I think self.camera_controller.get_property_value("readout_time") pulls
-              out the actual readout_time
-              calculated here (i.e. we don't need to do the calculations).
-        """
-        h = self.camera_controller.get_property_value("readout_time")
-        vn = self.camera_controller.get_property_value("subarray_vsize")
-        sensor_mode = self.camera_controller.get_property_value("sensor_mode")
-        exposure_time = self.camera_controller.get_property_value("exposure_time")
-        trigger_source = self.camera_controller.get_property_value("trigger_source")
-        trigger_active = self.camera_controller.get_property_value("trigger_active")
-
-        if sensor_mode == 1:
-            #  Area sensor mode operation
-            if trigger_source == 1:
-                # Internal Trigger Source
-                max_frame_rate = 1 / ((vn / 2) * h)
-                readout_time = exposure_time - ((vn / 2) * h)
-
-            if trigger_active == 1 or 2:
-                #  External Trigger Source
-                #  Edge == 1, Level == 2
-                max_frame_rate = 1 / ((vn / 2) * h + exposure_time + 10 * h)
-                readout_time = exposure_time - ((vn / 2) * h + exposure_time + 10 * h)
-
-            if trigger_active == 3:
-                #  External Trigger Source
-                #  Synchronous Readout == 3
-                max_frame_rate = 1 / ((vn / 2) * h + 5 * h)
-                readout_time = exposure_time - ((vn / 2) * h + 5 * h)
-
-            readout_time = h
-            max_frame_rate = 1.0 / (exposure_time + readout_time)
-
-        elif sensor_mode == 12:
-            #  Progressive sensor mode operation
-            max_frame_rate = 1 / (exposure_time + (vn + 10) * h)
-            readout_time = exposure_time - 1 / (exposure_time + (vn + 10) * h)
+        """
+        readout_time = self.camera_controller.get_property_value("readout_time")
 
-        else:
-            print(f"Hamamatsu Camera. Sensor mode {sensor_mode} not supported")
-            logger.error(f"Hamamatsu Camera. Sensor mode {sensor_mode} not supported")
-            max_frame_rate = 0
-            readout_time = 0
-        return readout_time, max_frame_rate
+        # with camera internal delay
+        return readout_time + 4 * self.minimum_exposure_time
 
     def set_exposure_time(self, exposure_time):
         """Set HamamatsuOrca exposure time.
 
         Note
         ----
             Units of the Hamamatsu API are in seconds.
             Units for the software are in milliseconds. Conversion is done here.
 
         Parameters
         ----------
         exposure_time : float
-            Exposure time in milliseconds.
+            Exposure time in seconds.
         """
-        exposure_time = exposure_time / 1000
+        exposure_time = exposure_time
         return self.camera_controller.set_property_value("exposure_time", exposure_time)
 
     def set_line_interval(self, line_interval_time):
         """Set HamamatsuOrca line interval.
 
         Parameters
         ----------
@@ -479,23 +330,14 @@
         if binning_string not in binning_dict.keys():
             logger.debug(f"can't set binning to {binning_string}")
             print(f"can't set binning to {binning_string}")
             return False
         self.camera_controller.set_property_value(
             "binning", binning_dict[binning_string]
         )
-        # idx = binning_string.index("x")
-        # x_binning = int(binning_string[:idx])
-        # y_binning = int(binning_string[idx + 1 :])
-        # self.x_pixels = int(self.x_pixels / x_binning)
-        # self.y_pixels = int(self.y_pixels / y_binning)
-
-        # should update experiment in controller side
-        # self.configuration['experiment']['CameraParameters']['camera_binning'] =
-        #   str(self.x_binning) + 'x' + str(self.y_binning)
         return True
 
     def set_ROI(self, roi_height=2048, roi_width=2048):
         """Change the size of the active region on the camera.
 
         Parameters
         ----------
@@ -506,16 +348,16 @@
 
         Returns
         -------
         result: bool
             True if successful, False otherwise.
         """
         # Get the Maximum Number of Pixels from the Configuration File
-        camera_height = self.max_image_height
-        camera_width = self.max_image_width
+        camera_height = self.camera_parameters["y_pixels"]
+        camera_width = self.camera_parameters["x_pixels"]
 
         if (
             roi_height > camera_height
             or roi_width > camera_width
             or roi_height < 1
             or roi_width < 1
         ):
@@ -604,116 +446,191 @@
             "minimum_trigger_blank"
         )
         # trigger_interval =
         #   self.camera_controller.get_property_value('minimum_trigger_interval')
         return trigger_blank
 
 
-class HamamatsuOrcaLightning(HamamatsuOrca):
+class HamamatsuOrcaLightning(HamamatsuBase):
     """HamamatsuOrcaLightning camera class."""
 
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrcaLightning class.
 
         Parameters
         ----------
         microscope_name : str
             Name of microscope in configuration
         device_connection : object
             Hardware device to connect to
-        configuration : multiprocesing.managers.DictProxy
+        configuration : multiprocessing.managers.DictProxy
             Global configuration of the microscope
         """
-        HamamatsuOrca.__init__(self, microscope_name, device_connection, configuration)
+        HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
+
         self.camera_parameters["supported_readout_directions"] = ["Top-to-Bottom"]
 
+        # self.minimum_exposure_time = 6.304 * 10 ** -6
+
         logger.info("HamamatsuOrcaLightning Initialized")
 
     def calculate_light_sheet_exposure_time(
         self, full_chip_exposure_time, shutter_width
     ):
         """Calculate light sheet exposure time.
 
         Parameters
         ----------
         full_chip_exposure_time : float
-            Full chip exposure time.
+            Full chip exposure time in seconds.
         shutter_width : int
             Shutter width.
 
         Returns
         -------
         exposure_time : float
-            Exposure time.
+            Exposure time in seconds.
         camera_line_interval : float
-            Camera line interval.
+            Camera line interval in seconds.
+        full_chip_exposure_time : float
+            Full chip exposure time in seconds.
         """
 
-        camera_line_interval = (full_chip_exposure_time / 1000) / (
-            (shutter_width + self.y_pixels - 1) / 4
+        camera_line_interval = full_chip_exposure_time / (
+            6 + (shutter_width + self.y_pixels) / 4
         )
-
         self.camera_parameters["line_interval"] = camera_line_interval
 
-        exposure_time = camera_line_interval * (shutter_width / 4) * 1000
-        return exposure_time, camera_line_interval
+        maximum_internal_line_interval = 0.0002 # 200.0 us
+        if camera_line_interval > maximum_internal_line_interval:
+            camera_line_interval = maximum_internal_line_interval
+            full_chip_exposure_time = camera_line_interval * (6 + (shutter_width + self.y_pixels) / 4)
+        
+        exposure_time = camera_line_interval * ((shutter_width + 3) // 4)
+        return exposure_time, camera_line_interval, full_chip_exposure_time
 
 
-class HamamatsuOrcaFire(HamamatsuOrca):
+class HamamatsuOrcaFire(HamamatsuBase):
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrcaFire class.
 
         Parameters
         ----------
         microscope_name : str
             Name of microscope in configuration
         device_connection : object
             Hardware device to connect to
-        configuration : multiprocesing.managers.DictProxy
+        configuration : multiprocessing.managers.DictProxy
             Global configuration of the microscope
         """
-        HamamatsuOrca.__init__(self, microscope_name, device_connection, configuration)
-        self.camera_parameters["supported_readout_directions"] = ["Top-to-Bottom", "Bottom-to-Top", "Bidirectional", "Rev. Bidirectional"]
-        # get the max image width and height from the camera
-        # it seems the camera will reset to its default value when close the connection with the camera.
-        self.camera_parameters["x_pixels"] = self.camera_controller.get_property_value("image_width")
-        self.camera_parameters["y_pixels"] = self.camera_controller.get_property_value("image_height")
+        HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
+        self.camera_parameters["supported_readout_directions"] = [
+            "Top-to-Bottom", "Bottom-to-Top", "Bidirectional", "Rev. Bidirectional"]
+
+        # self.minimum_exposure_time = 7.309 * 10 ** -6  # 7.309 us
+
+        self.camera_parameters["x_pixels"] = self.camera_controller.get_property_value(
+            "image_width")
+
+        self.camera_parameters["y_pixels"] = self.camera_controller.get_property_value(
+            "image_height")
 
         logger.info("HamamatsuOrcaFire Initialized")
 
-    @property
-    def max_image_width(self):
-        """Get maximum image width.
+
+    def calculate_light_sheet_exposure_time(
+        self, full_chip_exposure_time, shutter_width
+    ):
+        """Convert normal mode exposure time to light-sheet mode exposure time.
+        Calculate the parameters for an acquisition
+
+        Parameters
+        ----------
+        full_chip_exposure_time : float
+            Normal mode exposure time in seconds.
+        shutter_width : int
+            Width of light-sheet rolling shutter.
 
         Returns
         -------
-        max_image_width : int
-            Maximum image width.
+        exposure_time : float
+            Light-sheet mode exposure time (s).
+        camera_line_interval : float
+            HamamatsuOrca line interval duration (s).
+        full_chip_exposure_time : float
+            Updated full chip exposure time (s).
         """
-        return self.camera_parameters["x_pixels"]
+        # 4H delay, (Vn/2+5)H readout
+        camera_line_interval = full_chip_exposure_time / (
+            9 + (shutter_width + self.y_pixels) / 2
+        )
+        
+        maximum_internal_line_interval = 0.0002339 # 233.9 us
+        if camera_line_interval > maximum_internal_line_interval:
+            camera_line_interval = maximum_internal_line_interval
+            full_chip_exposure_time = camera_line_interval * (9 + (shutter_width + self.y_pixels) / 2)
 
-    @max_image_width.setter
-    def max_image_width(self, value):
-        """Set maximum image width."""
-        pass
+        self.camera_parameters["line_interval"] = camera_line_interval
 
-    @property
-    def max_image_height(self):
-        """Get maximum image height.
+        # round up exposure time
+        exposure_time = camera_line_interval * ((shutter_width+1) // 2)
+        return exposure_time, camera_line_interval, full_chip_exposure_time
 
-        Returns
-        -------
-        max_image_height : int
-            Maximum image height.
+
+class HamamatsuOrca(HamamatsuBase):
+    def __init__(self, microscope_name, device_connection, configuration):
+        """Initialize HamamatsuOrca class.
+
+        This is for controlling the Orca Flash 4.0.
+
+        Parameters
+        ----------
+        microscope_name : str
+            Name of microscope in configuration
+        device_connection : object
+            Hardware device to connect to
+        configuration : multiprocessing.managers.DictProxy
+            Global configuration of the microscope
         """
-        return self.camera_parameters["y_pixels"]
+        HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
+
+        self.camera_parameters["supported_readout_directions"] = [
+            "Top-to-Bottom", "Bottom-to-Top"]
 
-    @max_image_height.setter
-    def max_image_height(self, value):
-        """Set maximum image height.
+        # self.minimum_exposure_time = 9.74436 * 10 ** -6
+
+        logger.info("HamamatsuOrca Initialized")
+
+    def calculate_light_sheet_exposure_time(
+        self, full_chip_exposure_time, shutter_width
+    ):
+        """Convert normal mode exposure time to light-sheet mode exposure time.
+        Calculate the parameters for an acquisition
 
         Parameters
         ----------
-        value : int
-            Maximum image height.
+        full_chip_exposure_time : float
+            Normal mode exposure time in seconds.
+        shutter_width : int
+            Width of light-sheet rolling shutter.
+
+        Returns
+        -------
+        exposure_time : float
+            Light-sheet mode exposure time (s).
+        camera_line_interval : float
+            HamamatsuOrca line interval duration (s).
+        full_chip_exposure_time : float
+            Updated full chip exposure time (s).
         """
-        pass
+        camera_line_interval = full_chip_exposure_time / (4 + shutter_width + self.y_pixels)
+        
+        maximum_internal_line_interval = 963.8e-6 # 963.8 us
+        if camera_line_interval > maximum_internal_line_interval:
+            camera_line_interval = maximum_internal_line_interval
+            full_chip_exposure_time = camera_line_interval * (4 + shutter_width + self.y_pixels)
+
+        self.camera_parameters["line_interval"] = camera_line_interval
+
+        # round up exposure time
+        exposure_time = camera_line_interval * shutter_width
+        return exposure_time, camera_line_interval, full_chip_exposure_time
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_photometrics.py` & `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_photometrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,21 +82,17 @@
         self._databuffer = None
         #: int: Number of frames received
         self._frames_received = 0
         #: float: Unit for line delay
         self._unitforlinedelay = 0.00375  # 3.75  us for dynamic mode kinetix
         #: list: Frame IDs
         self._frame_ids = []
-        #: int: Max image width
-        self.max_image_width = self.camera_controller.sensor_size[0]
-        #: int: Max image height
-        self.max_image_height = self.camera_controller.sensor_size[1]
         #: dict: Camera parameters
-        self.camera_parameters["x_pixels"] = self.max_image_width
-        self.camera_parameters["y_pixels"] = self.max_image_height
+        self.camera_parameters["x_pixels"] = self.camera_controller.sensor_size[0]
+        self.camera_parameters["y_pixels"] = self.camera_controller.sensor_size[1]
 
         # todo: complete first init of parameters to default values
 
         # Values are pulled from the CameraParameters section of the
         # configuration.yml file.
         # Exposure time converted here from milliseconds to seconds.
         self.set_sensor_mode("Normal")
@@ -224,32 +220,28 @@
         ----
             Not implemented. Currently hard-coded for Hamamatsu Orca Flash 4.0.
 
         Returns
         -------
         readout_time : float
             Duration of time needed to readout an image.
-        max_frame_rate : float
-            Maximum framerate for a given camera acquisition mode.
         """
 
         # todo
         h = 3.75 * 10**-6  # Readout timing constant
         # h = self.camera_controller.get_property_value("readout_time")
         vn = self.y_pixels
         exposure_time = self._exposuretime
         # trigger_source = self.camera_controller.get_property_value('trigger_source')
         # trigger_active = self.camera_controller.get_property_value('trigger_active')
         #
         if self._scanmode == 0:  # normal/static light-sheet
-            max_frame_rate = 1 / ((vn + 10) * h + exposure_time)
             readout_time = exposure_time - ((vn + 10) * h + exposure_time)
         else:
             # todo: not sure if these equations are correct
-            max_frame_rate = 1 / ((vn + 10) * h * self._scandelay + exposure_time)
             readout_time = exposure_time - (
                 (vn + 10) * h * self._scandelay + exposure_time
             )
 
             #
         #     #  Area sensor mode operation
         #     if trigger_source == 1:
@@ -270,15 +262,15 @@
         #         readout_time = exposure_time - ((vn / 2) * h + 5 * h)
         #
         # if sensor_mode == 12:
         #     #  Progressive sensor mode operation
         #     max_frame_rate = 1 / (exposure_time + (vn + 10) * h)
         #     readout_time = exposure_time - 1 / (exposure_time + (vn + 10) * h)
         #
-        return readout_time, max_frame_rate
+        return readout_time
 
     def set_exposure_time(self, exposure_time):
         """Set Photometrics exposure time.
 
         Units of the Photometrics API are in seconds.
         All of our units are in milliseconds.
 
@@ -320,15 +312,19 @@
 
         Returns
         -------
         exposure_time : float
             Light-sheet mode exposure time.
         camera_line_interval : float
             HamamatsuOrca line interval duration.
+        full_chip_exposure_time : float
+            Full chip exposure time (s)
         """
+        # TODO: what's the units of the input full_chip_exposure_time? miliseconds or seconds?
+
         linedelay = self._unitforlinedelay  # 10.16us
         nbrows = self.y_pixels
         ASLM_scanWidth = 70
 
         ASLM_lineExposure = int(
             np.ceil(full_chip_exposure_time / (1 + nbrows / ASLM_scanWidth))
         )
@@ -356,15 +352,15 @@
                 ASLM_lineExposure,
                 ASLM_line_delay,
                 ASLM_acquisition_time,
                 ASLM_scanWidth,
             )
         )
 
-        return ASLM_lineExposure, ASLM_line_delay
+        return ASLM_lineExposure, ASLM_line_delay, full_chip_exposure_time
 
     def _calculate_ASLMparameters(self, desired_exposuretime):
         """Calculate the parameters for an ASLM acquisition
 
         Parameters
         ----------
         desired_exposuretime : float
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/camera/camera_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_synthetic.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,18 @@
         self.pre_frame_idx = None
         #: bool: whether to use random image
         self.random_image = True
         #: int: serial number
         self.serial_number = "synthetic"
         #: float: exposure time
         self.camera_exposure_time = 0.2
+        #: int: width
+        self.x_pixels = self.camera_parameters["x_pixels"]
+        #: int: height
+        self.y_pixels = self.camera_parameters["y_pixels"]
 
         logger.info("SyntheticCamera Class Initialized")
 
     def __del__(self):
         """Delete SyntheticCamera class."""
         logger.info("SyntheticCamera Shutdown")
         pass
@@ -150,18 +154,18 @@
         """Set SyntheticCamera exposure time.
 
         All of our units are in milliseconds. Function converts to seconds.
 
         Parameters
         ----------
         exposure_time : float
-            Exposure time in milliseconds.
+            Exposure time in seconds.
 
         """
-        self.camera_exposure_time = exposure_time / 1000
+        self.camera_exposure_time = exposure_time
 
     def set_line_interval(self, line_interval_time):
         """Set SyntheticCamera line interval.
 
         Parameters
         ----------
         line_interval_time : float
@@ -270,15 +274,15 @@
         )
 
         self.current_frame_idx = (self.current_frame_idx + 1) % self.num_of_frame
 
     def get_new_frame(self):
         """Get frame from SyntheticCamera camera."""
 
-        time.sleep(self.camera_exposure_time / 1000)
+        time.sleep(self.camera_exposure_time)
         timeout = 500
         while self.pre_frame_idx == self.current_frame_idx and timeout:
             time.sleep(0.001)
             timeout -= 1
         if timeout <= 0:
             return []
         if self.pre_frame_idx < self.current_frame_idx:
@@ -317,15 +321,12 @@
         """Calculate duration of time needed to readout an image. Calculates the readout
         time and maximum frame rate according to the camera configuration settings.
 
         Returns
         -------
         readout_time : float
             Duration of time needed to readout an image.
-        max_frame_rate : float
-            Maximum framerate for a given camera acquisition mode.
 
         """
         exposure_time = self.camera_controller.get_property_value("exposure_time")
         readout_time = 0.01  # 10 milliseconds.
-        max_frame_rate = 1 / (exposure_time + readout_time)
-        return readout_time, max_frame_rate
+        return readout_time
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,31 +73,23 @@
 
         # Initialize Variables
         #: float: Sample rate of the DAQ
         self.sample_rate = self.daq_parameters["sample_rate"]
 
         #: dict: Sweep times for different channels
         self.sweep_times = None
-        
+
         #: dict: exposure times for different channels
         self.exposure_times = None
 
-        # Remote Focus Parameters
-        #: dict: Dictionary of remote focus ramp falling percentages
-        self.remote_focus_ramp_falling = {}
-        for m in self.configuration["configuration"]["microscopes"].keys():
-            self.remote_focus_ramp_falling[m] = self.configuration["configuration"][
-                "microscopes"
-            ][m]["remote_focus_device"]["ramp_falling_percent"]
-
         # Camera Parameters
         #: float: Camera delay percentage
-        self.camera_delay_percent = self.configuration["configuration"]["microscopes"][
+        self.camera_delay = self.configuration["configuration"]["microscopes"][
             self.microscope_name
-        ]["camera"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
 
         #: dict: Dictionary of waveforms.
         self.waveform_dict = {}
 
         #: int: Number of times to repeat the waveform
         self.waveform_repeat_num = 1
 
@@ -136,19 +128,20 @@
             channel = microscope_state["channels"][channel_key]
 
             # Only proceed if it is enabled in the GUI
             if channel["is_selected"] is True:
                 exposure_time = exposure_times[channel_key]
                 sweep_time = sweep_times[channel_key]
 
+                # Create 5V TTL for 1 camera exposure.
                 self.waveform_dict[channel_key] = camera_exposure(
                     sample_rate=self.sample_rate,
                     sweep_time=sweep_time,
                     exposure=exposure_time,
-                    camera_delay=self.camera_delay_percent,
+                    camera_delay=self.camera_delay,
                 )
 
         return self.waveform_dict
 
     def enable_microscope(self, microscope_name):
         """Enables the microscope.
 
@@ -156,13 +149,13 @@
         ----------
         microscope_name : str
             Name of the active microscope
         """
         if microscope_name != self.microscope_name:
             self.microscope_name = microscope_name
 
-        self.camera_delay_percent = self.configuration["configuration"]["microscopes"][
+        self.camera_delay = self.configuration["configuration"]["microscopes"][
             microscope_name
-        ]["camera"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
         self.sample_rate = self.configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sample_rate"]
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_ni.py` & `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_ni.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         camera_trigger_out_line = self.configuration["configuration"]["microscopes"][
             self.microscope_name
         ]["daq"]["camera_trigger_out_line"]
         camera_high_time = 0.004
         exposure_time = self.exposure_times[channel_key]
         sweep_time = self.sweep_times[channel_key]
         camera_low_time = sweep_time - camera_high_time
-        camera_delay = (self.camera_delay_percent / 100) * (exposure_time / 1000)
+        camera_delay = self.camera_delay
 
         self.camera_trigger_task.co_channels.add_co_pulse_chan_time(
             camera_trigger_out_line,
             high_time=camera_high_time,
             low_time=camera_low_time,
             initial_delay=camera_delay,
         )
@@ -426,17 +426,17 @@
             Name of microscope to enable.
         """
         if microscope_name != self.microscope_name:
             self.microscope_name = microscope_name
             self.analog_outputs = {}
             self.analog_output_tasks = {}
         
-        self.camera_delay_percent = self.configuration["configuration"]["microscopes"][
+        self.camera_delay = self.configuration["configuration"]["microscopes"][
             microscope_name
-        ]["camera"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
         self.sample_rate = self.configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sample_rate"]
 
         try:
             switching_port = self.configuration["configuration"]["microscopes"][
                 self.microscope_name
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/daq/daq_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py` & `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py` & `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,30 +81,25 @@
         ]["daq"]["sample_rate"]
 
         #: float: Sweep time.
         self.sweep_time = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sweep_time"]
 
-        #: float: Camera delay percent.
-        self.camera_delay_percent = configuration["configuration"]["microscopes"][
+        #: float: Camera delay
+        self.camera_delay = configuration["configuration"]["microscopes"][
             microscope_name
-        ]["camera"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
 
         #: float: Galvo max voltage.
         self.galvo_max_voltage = self.device_config["hardware"]["max"]
 
         #: float: Galvo min voltage.
         self.galvo_min_voltage = self.device_config["hardware"]["min"]
 
-        #: float: Percent galvo ramp rising percent.
-        self.remote_focus_ramp_falling = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["remote_focus_device"]["ramp_falling_percent"]
-
         # Galvo Waveform Information
         #: str: Galvo waveform. Waveform or Sawtooth.
         self.galvo_waveform = self.device_config.get("waveform", "sawtooth")
 
         #: dict: Dictionary of galvo waveforms.
         self.waveform_dict = {}
 
@@ -170,15 +165,15 @@
                 if self.galvo_waveform == "sawtooth":
                     self.waveform_dict[channel_key] = sawtooth(
                         sample_rate=self.sample_rate,
                         sweep_time=self.sweep_time,
                         frequency=galvo_frequency,
                         amplitude=galvo_amplitude,
                         offset=galvo_offset,
-                        phase=(self.camera_delay_percent / 100) * exposure_time,
+                        phase=self.camera_delay,
                     )
                 elif self.galvo_waveform == "sine":
                     self.waveform_dict[channel_key] = sine_wave(
                         sample_rate=self.sample_rate,
                         sweep_time=self.sweep_time,
                         frequency=galvo_frequency,
                         amplitude=galvo_amplitude,
@@ -188,15 +183,15 @@
                 elif self.galvo_waveform == "halfsaw":
                     new_wave = sawtooth(
                         sample_rate=self.sample_rate,
                         sweep_time=self.sweep_time,
                         frequency=galvo_frequency,
                         amplitude=galvo_amplitude,
                         offset=galvo_offset,
-                        phase=(self.camera_delay_percent / 100) * exposure_time,
+                        phase=self.camera_delay,
                     )
                     half_samples = (
                         new_wave.argmax() if galvo_amplitude > 0 else new_wave.argmin()
                     )
                     new_wave[:half_samples] = -galvo_offset
                     self.waveform_dict[channel_key] = new_wave
                 else:
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_ni.py` & `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/galvo/galvo_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/lasers/laser_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/lasers/laser_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_imop.py` & `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_imop.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/mirrors/mirror_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/objectives.py` & `navigate-micro-0.0.5/src/navigate/model/devices/objectives.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 
 #  Standard Library Imports
 import logging
 
 # Third Party Imports
 
 # Local Imports
-from navigate.model.waveforms import remote_focus_ramp, smooth_waveform
+from navigate.model.waveforms import (
+    remote_focus_ramp,
+    smooth_waveform,
+    remote_focus_ramp_triangular,
+)
 
 # # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
 class RemoteFocusBase:
@@ -77,28 +81,19 @@
 
         #: float: Sweep time of the DAQ.
         self.sweep_time = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sweep_time"]
 
         #: float: Camera delay percent.
-        self.camera_delay_percent = configuration["configuration"]["microscopes"][
+        self.camera_delay = configuration["configuration"]["microscopes"][
             microscope_name
-        ]["camera"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
 
         # Waveform Parameters
-        #: float: Remote focus delay.
-        self.remote_focus_delay = self.device_config.get("delay_percent", 7.5)
-
-        #: float: Percent smoothing.
-        self.percent_smoothing = self.device_config.get("smoothing", 0)
-
-        #: float: Remote focus ramp falling.
-        self.remote_focus_ramp_falling = self.device_config["ramp_falling_percent"]
-
         #: float: Remote focus max voltage.
         self.remote_focus_max_voltage = self.device_config["hardware"]["max"]
 
         #: float: Remote focus min voltage.
         self.remote_focus_min_voltage = self.device_config["hardware"]["min"]
 
         #: dict: Waveform dictionary.
@@ -119,31 +114,41 @@
             Dictionary of sweep times for each selected channel
 
         Returns
         -------
         waveform : numpy.ndarray
             Waveform for the remote focus device.
         """
+        # to determine if the waveform has to be triangular
+        sensor_mode = self.configuration["experiment"]["CameraParameters"][
+            "sensor_mode"
+        ]
+        readout_direction = self.configuration["experiment"]["CameraParameters"][
+            "readout_direction"
+        ]
 
         self.waveform_dict = dict.fromkeys(self.waveform_dict, None)
         microscope_state = self.configuration["experiment"]["MicroscopeState"]
         waveform_constants = self.configuration["waveform_constants"]
         imaging_mode = microscope_state["microscope_name"]
         zoom = microscope_state["zoom"]
+        # ramp_type = self.configuration["configuration"]["microscopes"][
+        #     self.microscope_name]['remote focus device']['ramp_type']
         self.sample_rate = self.configuration["configuration"]["microscopes"][
             self.microscope_name
         ]["daq"]["sample_rate"]
 
-        duty_cycle_wait_duration = (
-            float(
-                self.configuration["waveform_constants"]
-                .get("other_constants", {})
-                .get("remote_focus_settle_duration", 0)
-            )
-            / 1000
+        remote_focus_ramp_falling = float(
+            waveform_constants["other_constants"]["remote_focus_ramp_falling"]
+        ) / 1000
+        remote_focus_delay = float(
+            waveform_constants["other_constants"]["remote_focus_delay"]
+        ) / 1000
+        percent_smoothing = float(
+            waveform_constants["other_constants"]["percent_smoothing"]
         )
 
         for channel_key in microscope_state["channels"].keys():
             # channel includes 'is_selected', 'laser', 'filter', 'camera_exposure'...
             channel = microscope_state["channels"][channel_key]
 
             # Only proceed if it is enabled in the GUI
@@ -153,25 +158,14 @@
                 # Should Assert.
                 laser = channel["laser"]
                 exposure_time = exposure_times[channel_key]
                 self.sweep_time = sweep_times[channel_key]
 
                 samples = int(self.sample_rate * self.sweep_time)
 
-                # Make sure the smoothing results in a waveform of length sweep time
-                ps = float(
-                    waveform_constants["remote_focus_constants"][self.microscope_name][
-                        zoom
-                    ][channel["laser"]].get("percent_smoothing", 0.0)
-                )
-                if ps > 0:
-                    self.sweep_time = (self.sweep_time - duty_cycle_wait_duration) / (
-                        1 + ps / 100
-                    ) + duty_cycle_wait_duration
-
                 # Remote Focus Parameters
                 temp = waveform_constants["remote_focus_constants"][imaging_mode][zoom][
                     laser
                 ]["amplitude"]
                 if temp == "-" or temp == ".":
                     waveform_constants["remote_focus_constants"][imaging_mode][zoom][
                         laser
@@ -179,25 +173,14 @@
 
                 remote_focus_amplitude = float(
                     waveform_constants["remote_focus_constants"][imaging_mode][zoom][
                         laser
                     ]["amplitude"]
                 )
 
-                self.remote_focus_delay = float(
-                    waveform_constants["remote_focus_constants"][imaging_mode][zoom][
-                        laser
-                    ]["percent_delay"]
-                )
-                self.percent_smoothing = float(
-                    waveform_constants["remote_focus_constants"][imaging_mode][zoom][
-                        laser
-                    ]["percent_smoothing"]
-                )
-
                 # Validation for when user puts a '-' in spinbox
                 temp = waveform_constants["remote_focus_constants"][imaging_mode][zoom][
                     laser
                 ]["offset"]
                 if temp == "-" or temp == ".":
                     waveform_constants["remote_focus_constants"][imaging_mode][zoom][
                         laser
@@ -208,35 +191,50 @@
                         laser
                     ]["offset"]
                 )
                 if offset is not None:
                     remote_focus_offset += offset
 
                 # Calculate the Waveforms
-                self.waveform_dict[channel_key] = remote_focus_ramp(
-                    sample_rate=self.sample_rate,
-                    exposure_time=exposure_time,
-                    sweep_time=self.sweep_time,
-                    remote_focus_delay=self.remote_focus_delay,
-                    camera_delay=self.camera_delay_percent,
-                    fall=self.remote_focus_ramp_falling,
-                    amplitude=remote_focus_amplitude,
-                    offset=remote_focus_offset,
-                )
+                if sensor_mode == "Light-Sheet" and (
+                    readout_direction == "Bidirectional"
+                    or readout_direction == "Rev. Bidirectional"
+                ):
+                    self.waveform_dict[channel_key] = remote_focus_ramp_triangular(
+                        sample_rate=self.sample_rate,
+                        exposure_time=exposure_time,
+                        sweep_time=self.sweep_time,
+                        remote_focus_delay=remote_focus_delay,
+                        camera_delay=self.camera_delay,
+                        amplitude=remote_focus_amplitude,
+                        offset=remote_focus_offset,
+                    )
+                    samples *= 2
+
+                else:
+                    self.waveform_dict[channel_key] = remote_focus_ramp(
+                        sample_rate=self.sample_rate,
+                        exposure_time=exposure_time,
+                        sweep_time=self.sweep_time,
+                        remote_focus_delay=remote_focus_delay,
+                        camera_delay=self.camera_delay,
+                        fall=remote_focus_ramp_falling,
+                        amplitude=remote_focus_amplitude,
+                        offset=remote_focus_offset,
+                    )
 
                 # Smooth the Waveform if specified
-                if self.percent_smoothing > 0:
+                if percent_smoothing > 0:
                     self.waveform_dict[channel_key] = smooth_waveform(
                         waveform=self.waveform_dict[channel_key],
-                        percent_smoothing=self.percent_smoothing,
+                        percent_smoothing=percent_smoothing,
                     )[: samples]
 
                 # Clip any values outside of the hardware limits
                 self.waveform_dict[channel_key][
                     self.waveform_dict[channel_key] > self.remote_focus_max_voltage
                 ] = self.remote_focus_max_voltage
                 self.waveform_dict[channel_key][
                     self.waveform_dict[channel_key] < self.remote_focus_min_voltage
                 ] = self.remote_focus_min_voltage
 
         return self.waveform_dict
-
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py` & `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_ni.py` & `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/shutter/laser_shutter_ttl.py` & `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_ttl.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_asi.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_asi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_galvo.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_galvo.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 # Third Party Imports
 import numpy as np
 import nidaqmx
 
 # Local Imports
 from navigate.model.devices.stages.stage_base import StageBase
-from navigate.model.waveforms import dc_value, remote_focus_ramp
 
 # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
 class GalvoNIStage(StageBase):
@@ -124,27 +123,17 @@
 
         #: str: Trigger source for the DAQ.
         self.trigger_source = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["trigger_source"]
 
         #: float: Percent of the camera delay.
-        self.camera_delay_percent = configuration["configuration"]["microscopes"][
+        self.camera_delay = configuration["configuration"]["microscopes"][
             microscope_name
-        ]["camera"]["delay_percent"]
-
-        #: float: Percent of the remote focus delay.
-        self.remote_focus_ramp_falling = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["remote_focus_device"]["ramp_falling_percent"]
-
-        #: float: Percent of the remote focus delay.
-        self.remote_focus_delay = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["remote_focus_device"]["delay_percent"]
+        ]["camera"]["delay"] / 1000
 
         #: float: Sample rate of the DAQ.
         self.sample_rate = self.configuration["configuration"]["microscopes"][
             self.microscope_name
         ]["daq"]["sample_rate"]
 
         #: dict: Dictionary of exposure times for each channel.
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_mcl.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_mcl.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_pi.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_pi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_sutter.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_sutter.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,15 @@
             #: dict: Dictionary mapping software axes to hardware axes.
             self.axes_mapping = {
                 axis: axes_mapping[axis] for axis in self.axes if axis in axes_mapping
             }
 
         self.sample_rate = 10000
         self.volts_per_micron = "0.1 * x"
-        self.remote_focus_delay = 0.05
-        self.camera_delay_percent = 0.01
-        self.remote_focus_ramp_falling = 0.1
+        self.camera_delay = 0.01
 
     def report_position(self):
         """Report the current position of the stage.
 
         Returns
         -------
         position_dict : dict
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py` & `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_base.py` & `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_dynamixel.py` & `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_dynamixel.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/devices/zoom/zoom_synthetic.py` & `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/adaptive_optics.py` & `navigate-micro-0.0.5/src/navigate/model/features/adaptive_optics.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/auto_tile_scan.py` & `navigate-micro-0.0.5/src/navigate/model/features/auto_tile_scan.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/autofocus.py` & `navigate-micro-0.0.5/src/navigate/model/features/autofocus.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/common_features.py` & `navigate-micro-0.0.5/src/navigate/model/features/common_features.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/cva_conpro.py` & `navigate-micro-0.0.5/src/navigate/model/features/cva_conpro.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,18 @@
         print(f"current channel = {self.channels}")
 
         self.end_acquisition = False
         self.received_frames = 0
         self.end_signal_temp = 0
 
         # get the current exposure time for channel channel.
-        readout_time = self.model.active_microscope.get_readout_time()
-        print("readout time calculated")
-        print(f"*** readout time = {readout_time} s")
         (
             exposure_times,
             sweep_times,
-        ) = self.model.active_microscope.calculate_exposure_sweep_times(readout_time)
+        ) = self.model.active_microscope.calculate_exposure_sweep_times()
         print("sweep times and exposure times calculated")
         print(f"exposure time = {exposure_times}")
         print(f"sweep time = {sweep_times}")
         channel_name = next(iter(sweep_times))
 
         channel_num = int(channel_name.split("_")[1])
         self.model.active_microscope.current_channel = channel_num
@@ -133,15 +130,14 @@
             f"channel_{self.model.active_microscope.current_channel}"
         ]
         current_expsure_time = exposure_times[
             f"channel_{self.model.active_microscope.current_channel}"
         ]
         self.current_sweep_time = current_sweep_time
         self.current_exposure_time = current_expsure_time
-        self.readout_time = readout_time
         print("sweep time calculated")
         scaling_factor = 1
         print("*** current sweep time before scaling:", current_sweep_time)
 
         # Provide just a bit of breathing room for the sweep time...
         current_sweep_time = current_sweep_time * scaling_factor
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/feature_container.py` & `navigate-micro-0.0.5/src/navigate/model/features/feature_container.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/feature_related_functions.py` & `navigate-micro-0.0.5/src/navigate/model/features/feature_related_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/image_writer.py` & `navigate-micro-0.0.5/src/navigate/model/features/image_writer.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/remove_empty_tiles.py` & `navigate-micro-0.0.5/src/navigate/model/features/remove_empty_tiles.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/restful_features.py` & `navigate-micro-0.0.5/src/navigate/model/features/restful_features.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/features/volume_search.py` & `navigate-micro-0.0.5/src/navigate/model/features/volume_search.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/metadata_sources/bdv_metadata.py` & `navigate-micro-0.0.5/src/navigate/model/metadata_sources/bdv_metadata.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/metadata_sources/metadata.py` & `navigate-micro-0.0.5/src/navigate/model/metadata_sources/metadata.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/metadata_sources/ome_tiff_metadata.py` & `navigate-micro-0.0.5/src/navigate/model/metadata_sources/ome_tiff_metadata.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/model/microscope.py` & `navigate-micro-0.0.5/src/navigate/model/microscope.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 import importlib  # noqa: F401
 from multiprocessing.managers import ListProxy
 
 from navigate.model.device_startup_functions import (
     start_stage,
 )
 from navigate.tools.common_functions import build_ref_name
-from navigate.model.devices.stages.stage_galvo import GalvoNIStage
 
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
 class Microscope:
     """Microscope Class - Used to control the microscope."""
@@ -402,39 +401,42 @@
         if self.camera.is_acquiring:
             self.camera.close_image_series()
 
         # Set Camera Sensor Mode - Must be done before camera is initialized.
         sensor_mode = self.configuration["experiment"]["CameraParameters"][
             "sensor_mode"
         ]
+
         self.camera.set_sensor_mode(sensor_mode)
         if sensor_mode == "Light-Sheet":
             self.camera.set_readout_direction(
                 self.configuration["experiment"]["CameraParameters"][
                     "readout_direction"
                 ]
             )
+
         # set binning
         self.camera.set_binning(
             self.configuration["experiment"]["CameraParameters"]["binning"]
         )
         # Initialize Image Series - Attaches camera buffer and start imaging
         self.camera.initialize_image_series(self.data_buffer, self.number_of_frames)
 
         # calculate all the waveform
         self.shutter.open_shutter()
+
         return self.calculate_all_waveform()
 
     def end_acquisition(self):
         """End the acquisition."""
         self.daq.stop_acquisition()
         # set NI Galvo stage to normal stage mode
         if self.configuration["experiment"]["MicroscopeState"]["image_mode"] == "confocal-projection":
             for stage, _ in self.stages_list:
-                if type(stage) == GalvoNIStage:
+                if type(stage).__name__ == "GalvoNIStage":
                     stage.switch_mode("normal")
         self.stop_stage()
         if self.central_focus is not None:
             self.move_stage({"f_abs": self.central_focus})
         if self.camera.is_acquiring:
             self.camera.close_image_series()
         self.shutter.close_shutter()
@@ -455,113 +457,122 @@
         """Calculate all the waveforms.
 
         Returns
         -------
         waveform : dict
             Dictionary of all the waveforms.
         """
-        readout_time = self.get_readout_time()
-        exposure_times, sweep_times = self.calculate_exposure_sweep_times(readout_time)
+        exposure_times, sweep_times = self.calculate_exposure_sweep_times()
         camera_waveform = self.daq.calculate_all_waveforms(
             self.microscope_name, exposure_times, sweep_times
         )
         remote_focus_waveform = self.remote_focus_device.adjust(
             exposure_times, sweep_times
         )
         galvo_waveform = [
             self.galvo[k].adjust(exposure_times, sweep_times) for k in self.galvo
         ]
 
         # calculate waveform for galvo stage
         for stage, _ in self.stages_list:
-            if type(stage) == GalvoNIStage:
+            if type(stage).__name__ == "GalvoNIStage":
                 stage.switch_mode("normal", exposure_times, sweep_times)
         waveform_dict = {
             "camera_waveform": camera_waveform,
             "remote_focus_waveform": remote_focus_waveform,
             "galvo_waveform": galvo_waveform,
         }
         return waveform_dict
 
-    def calculate_exposure_sweep_times(self, readout_time):
+    def calculate_exposure_sweep_times(self):
         """Calculate the exposure and sweep times for all channels.
 
         The `calculate_exposure_sweep_times` function calculates and returns exposure
         times and sweep times for all channels in a microscope configuration. It takes
         the camera's readout time as an input parameter and considers various parameters
         such as camera exposure time, delay percentages, and smoothing to compute these
         times. The function iterates through the channels, performs calculations, and
         returns the results as dictionaries containing exposure times and sweep times
         for each channel.
 
-        Parameters
-        ----------
-        readout_time : float
-            Readout time of the camera (seconds) if we are operating the camera in
-            Normal mode, otherwise -1.
-
         Returns
         -------
         exposure_times : dict
             Dictionary of exposure times.
         sweep_times : dict
             Dictionary of sweep times.
 
         """
         exposure_times = {}
         sweep_times = {}
         microscope_state = self.configuration["experiment"]["MicroscopeState"]
         zoom = microscope_state["zoom"]
         waveform_constants = self.configuration["waveform_constants"]
-        camera_delay_percent = self.configuration["configuration"]["microscopes"][
+        camera_delay = self.configuration["configuration"]["microscopes"][
             self.microscope_name
-        ]["camera"]["delay_percent"]
-        remote_focus_ramp_falling = self.configuration["configuration"]["microscopes"][
+        ]["camera"]["delay"] / 1000
+        camera_settle_duration = self.configuration["configuration"]["microscopes"][
             self.microscope_name
-        ]["remote_focus_device"]["ramp_falling_percent"]
+        ]["camera"].get("settle_duration", 0) / 1000
+        remote_focus_ramp_falling = float(
+                waveform_constants["other_constants"]["remote_focus_ramp_falling"]
+            ) / 1000
 
         duty_cycle_wait_duration = (
             float(
-                self.configuration["waveform_constants"]
-                .get("other_constants", {})
-                .get("remote_focus_settle_duration", 0)
-            )
-            / 1000
+                waveform_constants["other_constants"]["remote_focus_settle_duration"]
+            ) / 1000
         )
+        ps = float(
+            waveform_constants["other_constants"].get("percent_smoothing", 0.0)
+        )
+
+        readout_time = 0
+        readout_mode = self.configuration["experiment"]["CameraParameters"]["sensor_mode"]
+        if readout_mode == "Normal":
+            readout_time = self.camera.calculate_readout_time()
+        elif (
+            self.configuration["experiment"]["CameraParameters"]["readout_direction"] in ["Bidirectional", "Rev. Bidirectional"]
+        ):
+            remote_focus_ramp_falling = 0
+        # set readout out time
+        self.configuration["experiment"]["CameraParameters"]["readout_time"] = readout_time * 1000
+
         for channel_key in microscope_state["channels"].keys():
             channel = microscope_state["channels"][channel_key]
             if channel["is_selected"] is True:
                 exposure_time = float(channel["camera_exposure_time"]) / 1000
 
+                if readout_mode == "Light-Sheet":
+                    _, _, updated_exposure_time = self.camera.calculate_light_sheet_exposure_time(
+                        exposure_time,
+                        int(
+                            self.configuration["experiment"]["CameraParameters"][
+                                "number_of_pixels"
+                            ]
+                        )
+                    )
+                    if updated_exposure_time != exposure_time:
+                        print(f"*** Notice: The actual exposure time of the camera for {channel_key} is {round(updated_exposure_time*1000, 1)}ms, not {exposure_time*1000}ms!")
+                        exposure_time = round(updated_exposure_time, 4)
+                        # update the experiment file
+                        channel["camera_exposure_time"] = round(updated_exposure_time * 1000, 1)
+                        self.output_event_queue.put(("exposure_time", (channel_key, channel["camera_exposure_time"])))
+
                 sweep_time = (
                     exposure_time
-                    + exposure_time
-                    * (camera_delay_percent + remote_focus_ramp_falling)
-                    / 100
-                )
-                if readout_time > 0:
-                    # This addresses the dovetail nature of the camera readout in normal
-                    # mode. The camera reads middle out, and the delay in start of the
-                    # last lines compared to the first lines causes the exposure to be
-                    # net longer than exposure_time. This helps the galvo keep sweeping
-                    # for the full camera exposure time.
-                    sweep_time += readout_time  # we could set it to 0.14 instead of
-                    # 0.16384 according to the test
-
-                ps = float(
-                    waveform_constants["remote_focus_constants"][self.microscope_name][
-                        zoom
-                    ][channel["laser"]].get("percent_smoothing", 0.0)
-                )
+                    + readout_time
+                    + camera_delay
+                    + max(remote_focus_ramp_falling + duty_cycle_wait_duration, camera_settle_duration, camera_delay) - camera_delay
+                )        
+                # TODO: should we keep the percent_smoothing?
                 if ps > 0:
                     sweep_time = (1 + ps / 100) * sweep_time
 
-                sweep_time += duty_cycle_wait_duration
-
-                exposure_times[channel_key] = exposure_time
+                exposure_times[channel_key] = exposure_time + readout_time
                 sweep_times[channel_key] = sweep_time
 
         self.exposure_times = exposure_times
         self.sweep_times = sweep_times
 
         return exposure_times, sweep_times
 
@@ -610,22 +621,23 @@
         channel = self.configuration["experiment"]["MicroscopeState"]["channels"][
             channel_key
         ]
         # Filter Wheel Settings.
         self.filter_wheel.set_filter(channel["filter"])
 
         # Camera Settings
-        self.current_exposure_time = float(channel["camera_exposure_time"])
+        self.current_exposure_time = float(channel["camera_exposure_time"]) / 1000
         if (
             self.configuration["experiment"]["CameraParameters"]["sensor_mode"]
             == "Light-Sheet"
         ):
             (
                 self.current_exposure_time,
                 camera_line_interval,
+                _
             ) = self.camera.calculate_light_sheet_exposure_time(
                 self.current_exposure_time,
                 int(
                     self.configuration["experiment"]["CameraParameters"][
                         "number_of_pixels"
                     ]
                 ),
@@ -658,34 +670,14 @@
         if self.central_focus is not None:
             self.move_stage(
                 {"f_abs": self.central_focus + float(channel["defocus"])},
                 wait_until_done=True,
                 update_focus=False,
             )
 
-    def get_readout_time(self):
-        """Get readout time from camera.
-
-        Get the camera readout time if we are in normal mode.
-        Return a -1 to indicate when we are not in normal mode.
-        This is needed in daq.calculate_all_waveforms()
-
-        Returns
-        -------
-        readout_time : float
-            Camera readout time in seconds or -1 if not in Normal mode.
-        """
-        readout_time = 0
-        if (
-            self.configuration["experiment"]["CameraParameters"]["sensor_mode"]
-            == "Normal"
-        ):
-            readout_time, _ = self.camera.calculate_readout_time()
-        return readout_time
-
     def move_stage(self, pos_dict, wait_until_done=False, update_focus=True):
         """Move stage to a position.
 
         Parameters
         ----------
         pos_dict : dict
             Dictionary of stage positions.
@@ -755,16 +747,15 @@
         """Move remote focus.
 
         Parameters
         ----------
         offset : float, optional
             Offset, by default None
         """
-        readout_time = self.get_readout_time()
-        exposure_times, sweep_times = self.calculate_exposure_sweep_times(readout_time)
+        exposure_times, sweep_times = self.calculate_exposure_sweep_times()
         self.remote_focus_device.move(exposure_times, sweep_times, offset)
 
     def update_stage_limits(self, limits_flag=True):
         """Update stage limits.
 
         Parameters
         ----------
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/model.py` & `navigate-micro-0.0.5/src/navigate/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     convert_str_to_feature_list,
     convert_feature_list_to_str,
     SharedList,
     load_dynamic_parameter_functions,
 )
 from navigate.log_files.log_functions import log_setup
 from navigate.tools.common_dict_tools import update_stage_dict
-from navigate.tools.common_functions import load_module_from_file
+from navigate.tools.common_functions import load_module_from_file, VariableWithLock
 from navigate.tools.file_functions import load_yaml_file, save_yaml_file
 from navigate.model.device_startup_functions import load_devices
 from navigate.model.microscope import Microscope
 from navigate.config.config import get_navigate_path
 from navigate.model.plugins_model import PluginsModel
 
 
@@ -203,16 +203,16 @@
         self.event_queue = event_queue
 
         # frame signal id
         #: int: Frame ID.
         self.frame_id = 0
 
         # flags
-        #: bool: Autofocus on?
-        self.autofocus_on = False  # autofocus
+        #: bool: Inject a feature list?
+        self.injected_flag = VariableWithLock(bool)  # autofocus
         #: bool: Is the model live?
         self.is_live = False  # need to clear up data buffer after acquisition
         #: bool: Is the model saving the data?
         self.is_save = False  # save data
         #: bool: Stop signal and data threads?
         self.stop_acquisition = False  # stop signal and data threads
         #: bool: Stop signal thread?
@@ -499,14 +499,15 @@
             "Navigate Model - Received command from controller:", command, args
         )
         if not self.data_buffer:
             logging.debug("Navigate Model - Shared Memory Buffer Not Set Up.")
             return
 
         if command == "acquire":
+            """ Begin an acquisition."""
             self.is_acquiring = True
             self.imaging_mode = self.configuration["experiment"]["MicroscopeState"][
                 "image_mode"
             ]
             self.is_save = self.configuration["experiment"]["MicroscopeState"][
                 "is_save"
             ]
@@ -640,24 +641,28 @@
 
             Parameters
             ----------
             Args[0]: device name
             Args[1]: device reference
             """
             if self.is_acquiring and self.imaging_mode == "live":
-                if hasattr(self, "signal_container"):
-                    self.signal_container.cleanup()
-                if hasattr(self, "data_container"):
-                    self.data_container.cleanup()
-                self.signal_container, self.data_container = load_features(
-                    self,
-                    [{"name": Autofocus}],
-                )
+                with self.injected_flag as injected_flag:
+                    if hasattr(self, "signal_container"):
+                        self.signal_container.cleanup()
+                    if hasattr(self, "data_container"):
+                        self.data_container.cleanup()
+                    self.signal_container, self.data_container = load_features(
+                        self,
+                        [{"name": Autofocus}],
+                    )
+                    injected_flag.value = True
+
             elif not self.is_acquiring:
                 self.is_acquiring = True
+                self.imaging_mode = "autofocus"
                 autofocus = Autofocus(self, *args)
                 autofocus.run()
 
         elif command == "flatten_mirror":
             self.update_mirror(coef=[], flatten=True)
         elif command == "zero_mirror":
             self.active_microscope.mirror.zero_flatness()
@@ -749,15 +754,15 @@
         #     print(f"Using new camera >> {new_camera.camera_controller._serial_number}")
         #     self.active_microscope.camera = new_camera
 
         elif command == "exit":
             for camera in self.active_microscope.cameras.values():
                 camera.camera_controller.dev_close()
         else:
-            self.active_microscope.run_command(command, args)
+            self.active_microscope.run_command(command, *args)
 
     # main function to update mirror/set experiment mode values
     def update_mirror(self, coef=[], flatten=False):
         """Update the mirror.
 
         Parameters
         ----------
@@ -860,15 +865,14 @@
             Function to run on the acquired data.
         """
         wait_num = self.camera_wait_iterations
         acquired_frame_num = 0
 
         # whether acquire specific number of frames.
         count_frame = num_of_frames > 0
-        start_time = time.time()
 
         while not self.stop_acquisition:
             if self.ask_to_pause_data_thread:
                 self.pause_data_ready_lock.release()
                 self.pause_data_event.clear()
                 self.pause_data_event.wait()
             frame_ids = self.active_microscope.camera.get_new_frame()
@@ -881,17 +885,14 @@
                 wait_num -= 1
                 if wait_num <= 0:
                     # Camera timeout, abort acquisition.
                     break
                 continue
 
             acquired_frame_num += len(frame_ids)
-            stop_time = time.time()
-            frames_per_second = acquired_frame_num / (stop_time - start_time)
-            self.event_queue.put(("framerate", frames_per_second))
 
             wait_num = self.camera_wait_iterations
 
             if hasattr(self, "data_container") and not self.data_container.end_flag:
                 if self.data_container.is_closed:
                     self.logger.info("Navigate Model - Data container is closed.")
                     self.stop_acquisition = True
@@ -1010,15 +1011,15 @@
         turn_off_flags : bool
             Turn off the flags.
         """
         # turn off flags
         if turn_off_flags:
             self.stop_acquisition = False
             self.stop_send_signal = False
-            self.autofocus_on = False
+            self.injected_flag.value = False
             self.is_live = False
 
         plugin_obj = self.plugin_acquisition_modes.get(self.imaging_mode, None)
         if plugin_obj and hasattr(plugin_obj, "prepare_acquisition_model"):
             getattr(plugin_obj, "prepare_acquisition_model")(self)
 
         for m in self.virtual_microscopes:
@@ -1086,21 +1087,25 @@
 
         Recalculates the waveforms for each image, thereby allowing people to adjust
         acquisition parameters in real-time.
         """
         self.stop_acquisition = False
         while self.stop_acquisition is False and self.stop_send_signal is False:
             self.run_acquisition()
+            if not self.injected_flag.value:
+                self.signal_container.reset()
+            else:
+                self.reset_feature_list()
         # Update the stage position.
         # Allows the user to externally move the stage in the continuous mode.
         self.get_stage_position()
 
     def run_acquisition(self):
         """Run acquisition along with a feature list one time."""
-        if not hasattr(self, "signal_container") or self.signal_container.end_flag:
+        if not hasattr(self, "signal_container"):
             self.snap_image()
             return
 
         while (
             not self.signal_container.end_flag
             and not self.stop_send_signal
             and not self.stop_acquisition
@@ -1111,14 +1116,47 @@
             if self.signal_container.is_closed:
                 self.logger.info("Navigate Model - Signal container is closed.")
                 self.stop_acquisition = True
                 return
         if self.imaging_mode != "live":
             self.stop_acquisition = True
 
+    def reset_feature_list(self):
+        """Reset live mode feature list."""
+        with self.injected_flag as injected_flag:
+            # wait for datathread ends
+            waiting_num = 30
+            while (
+                hasattr(self, "data_container")
+                and not self.data_container.end_flag
+                and waiting_num > 0
+            ):
+                if self.stop_acquisition:
+                    return
+                time.sleep(0.01)
+                waiting_num -= 1
+            if hasattr(self, "signal_container"):
+                self.signal_container.cleanup()
+            if hasattr(self, "data_container"):
+                self.data_container.cleanup()
+            self.signal_container, self.data_container = load_features(
+                self,
+                [
+                    (
+                        {"name": PrepareNextChannel},
+                        {
+                            "name": LoopByCount,
+                            "args": ("experiment.MicroscopeState.selected_channels",),
+                        },
+                    )
+                ],
+            )
+            injected_flag.value = False
+
+
     def change_resolution(self, resolution_value):
         """Switch resolution mode of the microscope.
 
         Parameters
         ----------
         resolution_value : str
             Resolution mode.
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/plugins_model.py` & `navigate-micro-0.0.5/src/navigate/model/plugins_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,27 +26,31 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
+# Standard library imports
 import os
 from pathlib import Path
 import inspect
 
+# Third-party imports
+
+# Local application imports
 from navigate.tools.common_functions import load_module_from_file
 from navigate.tools.file_functions import load_yaml_file, save_yaml_file
 from navigate.tools.decorators import FeatureList, AcquisitionMode
 from navigate.model.features import feature_related_functions
 from navigate.config.config import get_navigate_path
 
 
 class PluginsModel:
-    """Plugins manaager in the model side"""
+    """Plugins manager in the model side"""
 
     def __init__(self):
         """Initialize plugins manager class"""
         #: str: plugins default path.
         self.plugins_path = os.path.join(
             Path(__file__).resolve().parent.parent, "plugins"
         )
@@ -54,20 +58,14 @@
     def load_plugins(self):
         """Load plugins"""
         devices_dict = {}
         plugin_acquisition_modes = {}
         feature_lists_path = os.path.join(get_navigate_path(), "feature_lists")
         if not os.path.exists(feature_lists_path):
             os.makedirs(feature_lists_path)
-        feature_list_files = [
-            temp
-            for temp in os.listdir(feature_lists_path)
-            if (temp.endswith(".yml") or temp.endswith(".yaml"))
-            and os.path.isfile(os.path.join(feature_lists_path, temp))
-        ]
         plugins = os.listdir(self.plugins_path)
         plugins_dict = {}
         # load plugins form plugins folder
         for f in plugins:
             if not os.path.isdir(os.path.join(self.plugins_path, f)):
                 continue
             # read "plugin_config.yml"
@@ -89,27 +87,30 @@
             )
         else:
             plugins_config = load_yaml_file(plugins_config_path)
             verified_plugins_config = {}
             for plugin_name, plugin_path in plugins_config.items():
                 if not plugin_path:
                     print(
-                        f"Plugin '{plugin_name}' is not installed correctly. Please reinstall it if necessary."
+                        f"Plugin '{plugin_name}' is not installed correctly. "
+                        f"Please reinstall it if necessary."
                     )
                     continue
                 if os.path.exists(plugin_path):
                     if plugin_name in plugins_dict:
                         print(
-                            f"There are two plugins named '{plugin_name}'. Please rename Plugin '{plugin_name}' in plugins folder!"
+                            f"There are two plugins named '{plugin_name}'. Please "
+                            f"rename Plugin '{plugin_name}' in plugins folder!"
                         )
                     plugins_dict[plugin_name] = plugin_path
                     verified_plugins_config[plugin_name] = plugin_path
                 else:
                     print(
-                        f"Couldn't load plugin '{plugin_name}', please make sure it exits!"
+                        f"Couldn't load plugin '{plugin_name}' please make sure "
+                        f"it exists!"
                     )
             save_yaml_file(
                 os.path.join(get_navigate_path(), "config"),
                 verified_plugins_config,
                 "plugins_config.yml",
             )
```

### Comparing `navigate-micro-0.0.4/src/navigate/model/waveforms.py` & `navigate-micro-0.0.5/src/navigate/model/waveforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 # Local Imports
 
 # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
-def camera_exposure(sample_rate=100000, sweep_time=0.4, exposure=0.4, camera_delay=10):
+def camera_exposure(sample_rate=100000, sweep_time=0.4, exposure=0.4, camera_delay=0.001):
     """Calculates timing and duration of camera exposure.
     Not actually used to trigger the camera.  Only meant for visualization.
 
     Parameters
     ----------
     sample_rate : Integer
         Unit - Hz
     sweep_time : Float
         Unit - Seconds
     exposure : Float
         Unit - Seconds
     camera_delay : Float
-        Unit - Percent
+        Unit - Seconds
 
     Returns
     -------
     exposure_start : Float
         Unit - Seconds
     exposure_end : Float
         Unit - Seconds
@@ -77,15 +77,15 @@
     # get an integer number of samples
     samples = int(np.multiply(sample_rate, sweep_time))
 
     # create an array just containing the offset voltage:
     array = np.zeros(samples)
 
     # convert pulse width and delay in % into number of samples
-    pulse_delay_samples = int((exposure * camera_delay / 100) * sample_rate)
+    pulse_delay_samples = int(camera_delay * sample_rate)
     pulse_samples = int(exposure * sample_rate)
 
     # modify the array
     array[pulse_delay_samples : (pulse_samples + pulse_delay_samples)] = amplitude
     return np.array(array)
 
 
@@ -135,17 +135,17 @@
     return np.array(array)
 
 
 def remote_focus_ramp(
     sample_rate=100000,
     exposure_time=0.2,
     sweep_time=0.24,
-    remote_focus_delay=7.5,
-    camera_delay=10,
-    fall=2.5,
+    remote_focus_delay=0.005,
+    camera_delay=0.001,
+    fall=0.05,
     amplitude=1,
     offset=0,
 ):
     """Returns a numpy array with a sawtooth ramp - typically used for remote focusing.
 
     The waveform starts at offset and stays there for the delay period, then
     rises linearly to 2x amplitude (amplitude here refers to 1/2 peak-to-peak)
@@ -159,19 +159,19 @@
     sample_rate : Integer
         Unit - Hz
     exposure_time : Float
         Unit - Seconds
     sweep_time : Float
         Unit - Seconds
     remote_focus_delay : Float
-        Unit - Percent
+        Unit - seconds
     camera_delay : Float
-        Unit - Percent
+        Unit - seconds
     fall : Float
-        Unit - Percent
+        Unit - seconds
     amplitude : Float
         Unit - Volts
     offset : Float
         Unit - Volts
 
     Returns
     -------
@@ -179,44 +179,119 @@
 
     Examples
     --------
     >>> etl_ramp = tunable_lens_ramp(sample_rate, exposure_time, sweep_time, etl_delay,
         camera_delay, fall, amplitude, offset)
 
     """
-
     # create an array just containing the negative amplitude voltage:
-    delay_samples = int(remote_focus_delay * exposure_time * sample_rate / 100)
+    delay_samples = int(remote_focus_delay * sample_rate)
     delay_array = np.zeros(delay_samples) + offset - amplitude
 
     # 10-7.5 -> 1.025 * .2
     #
     ramp_samples = int(
-        (exposure_time + exposure_time * (camera_delay - remote_focus_delay) / 100)
+        (exposure_time + camera_delay - remote_focus_delay)
         * sample_rate
     )
     ramp_array = np.linspace(offset - amplitude, offset + amplitude, ramp_samples)
 
     # fall_samples = .025 * .2 * 100000 = 500
-    fall_samples = int(fall * exposure_time * sample_rate / 100)
+    fall_samples = int(fall * sample_rate)
     fall_array = np.linspace(offset + amplitude, offset - amplitude, fall_samples)
 
     extra_samples = int(
         int(np.multiply(sample_rate, sweep_time))
         - (delay_samples + ramp_samples + fall_samples)
     )
     if extra_samples > 0:
         extra_array = np.zeros(extra_samples) + offset - amplitude
         waveform = np.hstack([delay_array, ramp_array, fall_array, extra_array])
     else:
         waveform = np.hstack([delay_array, ramp_array, fall_array])
 
+
     return waveform
 
 
+def remote_focus_ramp_triangular(
+        sample_rate=100000,
+        exposure_time=0.2,
+        sweep_time=0.24,
+        remote_focus_delay=0.005,
+        camera_delay=0.001,
+        amplitude=1,
+        offset=0,
+        ramp_type='Rising'
+):
+    """Returns a numpy array with a triangular ramp typically used for remote focusing
+
+    The waveform starts at offset and stays there for the delay period, then
+    rises linearly to 2x amplitude (amplitude here refers to 1/2 peak-to-peak).
+
+    Switching from a left to right remote focus ramp is possible by exchanging the
+    rise and fall periods.
+
+    Parameters
+    ----------
+    sample_rate : Integer
+        Unit - Hz
+    exposure_time : Float
+        Unit - Seconds
+    sweep_time : Float
+        Unit - Seconds
+    remote_focus_delay : Float
+        Unit - Seconds
+    camera_delay : Float
+        Unit - Seconds
+    amplitude : Float
+        Unit - Volts
+    offset : Float
+        Unit - Volts
+    ramp_type : String
+
+
+    Returns
+    -------
+    waveform : np.array
+
+    Examples
+    --------
+    >>> etl_ramp = tunable_lens_ramp(sample_rate, exposure_time, sweep_time, etl_delay,
+        camera_delay, fall, amplitude, offset)
+
+    """
+    # create an array just containing the negative amplitude voltage:
+    # In theory, delay here should be 4H.
+    delay_samples = int(remote_focus_delay  * sample_rate)
+    delay_array = np.zeros(delay_samples) + offset
+
+    # ramp samples
+    ramp_samples = int(
+        (exposure_time + camera_delay - remote_focus_delay)
+        * sample_rate
+    )
+    rise_ramp_array = np.linspace(offset - amplitude, offset + amplitude, ramp_samples)
+    fall_ramp_array = np.linspace(offset + amplitude, offset - amplitude, ramp_samples)
+
+    settle_samples = int(
+        int(np.multiply(sample_rate, sweep_time))
+        - (delay_samples + ramp_samples)
+    )
+    settle_array = np.zeros(settle_samples) + offset
+
+    if ramp_type == 'Rising':
+        waveform = np.hstack([delay_array - amplitude, rise_ramp_array, settle_array + amplitude,
+                                delay_array + amplitude, fall_ramp_array, settle_array - amplitude])
+    elif ramp_type == 'Falling':
+        waveform = np.hstack([delay_array + amplitude, fall_ramp_array, settle_array - amplitude,
+                                delay_array - amplitude, rise_ramp_array, settle_array + amplitude])
+
+    return waveform
+
 def sawtooth(
     sample_rate=100000,
     sweep_time=0.4,
     frequency=10,
     amplitude=1,
     offset=0,
     duty_cycle=50,
```

### Comparing `navigate-micro-0.0.4/src/navigate/tools/common_dict_tools.py` & `navigate-micro-0.0.5/src/navigate/tools/decorators.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,25 +26,51 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-def update_stage_dict(target, pos_dict):
-    """Update dictionary entries common to the model and controller.
+from time import time
+
+
+def function_timer(func):
+    """Decorator for evaluating the duration of time necessary to execute a statement.
 
     Parameters
     ----------
-    target : navigate.model.Model or navigate.controller.Controller
-        The object that is being updated.
-    pos_dict : dict
-        The dictionary of positions to update.
+    func : function
+        The function to be timed.
 
     Returns
     -------
-    None
+    wrap_func : function
+        The wrapped function.
     """
-    # Update our local experiment parameters
-    for axis, val in pos_dict.items():
-        ax = axis.split("_")[0]
-        target.configuration["experiment"]["StageParameters"][ax] = val
+
+    def wrap_func(*args, **kwargs):
+        t1 = time()
+        result = func(*args, **kwargs)
+        t2 = time()
+        print(f"Function {func.__name__!r} executed in {(t2 - t1):.4f}s")
+        return result
+
+    return wrap_func
+
+
+class FeatureList(object):
+    def __init__(self, func):
+        self._feature_list = func
+        temp = func.__name__
+        self.feature_list_name = str.title(temp.replace("_", " "))
+
+    def __call__(self, *args, **kwargs):
+        return self._feature_list()
+
+
+class AcquisitionMode(object):
+    def __init__(self, obj):
+        self.__obj_class = obj
+        self.__is_acquisition_mode = True
+
+    def __call__(self, *args):
+        return self.__obj_class(*args)
```

### Comparing `navigate-micro-0.0.4/src/navigate/tools/common_functions.py` & `navigate-micro-0.0.5/src/navigate/tools/common_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/decorators.py` & `navigate-micro-0.0.5/src/navigate/tools/common_dict_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,51 +26,59 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from time import time
 
+def update_nested_dict(d, find_func, apply_func):
+    """ Update a nested dictionary by applying a function to a value
 
-def function_timer(func):
-    """Decorator for evaluating the duration of time necessary to execute a statement.
+    Loops through a nested dictionary and if find_func() conditions are met,
+    run apply_func on that key.
+
+    TODO: It might be nice to make this non-recursive.
 
     Parameters
     ----------
-    func : function
-        The function to be timed.
+    d : dict
+        Dictionary to be updated
+    find_func : func
+        Accepts key, value pair and matches a condition based on these. Returns bool.
+    apply_func : func
+        Accepts a value returns the new value.
 
     Returns
     -------
-    wrap_func : function
-        The wrapped function.
+    d2 : dict
+        An version of d, updated according to the passed functions.
     """
+    d2 = {}
+    for k, v in d.items():
+        if find_func(k, v):
+            d2[k] = apply_func(v)
+        else:
+            d2[k] = v
+        if isinstance(v, dict):
+            d2[k] = update_nested_dict(v, find_func, apply_func)
+    return d2
 
-    def wrap_func(*args, **kwargs):
-        t1 = time()
-        result = func(*args, **kwargs)
-        t2 = time()
-        print(f"Function {func.__name__!r} executed in {(t2 - t1):.4f}s")
-        return result
-
-    return wrap_func
-
-
-class FeatureList(object):
-    def __init__(self, func):
-        self._feature_list = func
-        temp = func.__name__
-        self.feature_list_name = str.title(temp.replace("_", " "))
-
-    def __call__(self, *args, **kwargs):
-        return self._feature_list()
 
+def update_stage_dict(target, pos_dict):
+    """Update dictionary entries common to the model and controller.
 
-class AcquisitionMode(object):
-    def __init__(self, obj):
-        self.__obj_class = obj
-        self.__is_acquisition_mode = True
+    Parameters
+    ----------
+    target : navigate.model.Model or navigate.controller.Controller
+        The object that is being updated.
+    pos_dict : dict
+        The dictionary of positions to update.
 
-    def __call__(self, *args):
-        return self.__obj_class(*args)
+    Returns
+    -------
+    None
+    """
+    # Update our local experiment parameters
+    for axis, val in pos_dict.items():
+        ax = axis.split("_")[0]
+        target.configuration["experiment"]["StageParameters"][ax] = val
```

### Comparing `navigate-micro-0.0.4/src/navigate/tools/file_functions.py` & `navigate-micro-0.0.5/src/navigate/tools/file_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/image.py` & `navigate-micro-0.0.5/src/navigate/tools/image.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/linear_algebra.py` & `navigate-micro-0.0.5/src/navigate/tools/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/main_functions.py` & `navigate-micro-0.0.5/src/navigate/tools/main_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/multipos_table_tools.py` & `navigate-micro-0.0.5/src/navigate/tools/multipos_table_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/sdf.py` & `navigate-micro-0.0.5/src/navigate/tools/sdf.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/waveform_template_funcs.py` & `navigate-micro-0.0.5/src/navigate/tools/waveform_template_funcs.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/tools/xml_tools.py` & `navigate-micro-0.0.5/src/navigate/tools/xml_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/ArrowLabel.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/ArrowLabel.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/DockableNotebook.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/DockableNotebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/hover.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hover.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/hoverbar.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hoverbar.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/hovermixin.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hovermixin.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/popup.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/scrollbars.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/scrollbars.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/custom_widgets/validation.py` & `navigate-micro-0.0.5/src/navigate/view/custom_widgets/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 
         # Calls class that is mixed in with this class
         super().__init__(*args, **kwargs)
 
         # History for each widgets to undo and redo
         #: list: The undo history of the widget
         self.undo_history = []
+
         #: list: The redo history of the widget
         self.redo_history = []
 
         # Validation setup
         validcmd = self.register(self._validate)
         invalidcmd = self.register(self._invalid)
 
@@ -196,19 +197,19 @@
         self.error.set("")  # No error to start
         valid = True  # Again true means no error
         if event == "focusout":  # Leaving widget
             valid = self._focusout_validate(event=event)
             if valid:
                 self.add_history(event)
             else:
-               if self.undo_history:
-                   self.set(self.undo_history[-1])
-                   self.undo_history.pop()
-                   self._toggle_error(False)
-                   valid = True
+                if self.undo_history:
+                    self.set(self.undo_history[-1])
+                    self.undo_history.pop()
+                    self._toggle_error(False)
+                    valid = True
         elif event == "key":  # Keystroke into widget
             valid = self._key_validate(
                 proposed=proposed,
                 current=current,
                 char=char,
                 event=event,
                 index=index,
@@ -521,46 +522,46 @@
             if proposed == "":
                 self.is_fake_focusout = False
                 return True
             self._is_valid_proposed_value(proposed)
             return True
 
         return self._is_valid_proposed_value(proposed)
-    
+
     def _is_valid_proposed_value(self, proposed):
         """Validate a proposed value
-        
+
         Returns
         -------
         bool
             True if the proposed is valid, False if not
         """
         min_val = float(self.min)
         max_val = float(self.max)
 
-        if proposed == '-':
+        if proposed == "-":
             self._toggle_error(True)
             self.is_fake_focusout = False
             return min_val < 0
-        
-        if proposed == '.':
+
+        if proposed == ".":
             self._toggle_error(True)
             self.is_fake_focusout = False
             return True
 
         # Proposed value is a Decimal, so convert and check further
         try:
             proposed = Decimal(proposed)
         except InvalidOperation:
             self.is_fake_focusout = False
             return False
         proposed_precision = proposed.as_tuple().exponent
         if any([(proposed > max_val), (proposed_precision < self.precision)]):
             return False
-        
+
         if proposed < min_val:
             self._toggle_error(True)
             return True
 
         self._toggle_error(False)
 
         return True
@@ -720,20 +721,20 @@
             valid = self._focusout_validate(event=event)
             if self.is_fake_focusout:
                 self.is_fake_focusout = False
                 return valid
             if valid:
                 self.add_history(event)
             else:
-               if self.undo_history:
-                   self.is_fake_focusout = True
-                   self.set(self.undo_history[-1])
-                   self.undo_history.pop()
-                   self._toggle_error(False)
-                   valid = True
+                if self.undo_history:
+                    self.is_fake_focusout = True
+                    self.set(self.undo_history[-1])
+                    self.undo_history.pop()
+                    self._toggle_error(False)
+                    valid = True
         elif event == "key":  # Keystroke into widget
             valid = self._key_validate(
                 proposed=proposed,
                 current=current,
                 char=char,
                 event=event,
                 index=index,
@@ -754,15 +755,20 @@
         value = self.get()
         if value != "":
             min_val = float(self.min)
             max_val = float(self.max)
             # Don't add duplicates
             if self.undo_history and self.undo_history[-1] == value:
                 pass
-            elif value != "-" and value != "." and Decimal(value) >= min_val and Decimal(value) <= max_val:
+            elif (
+                value != "-"
+                and value != "."
+                and Decimal(value) >= min_val
+                and Decimal(value) <= max_val
+            ):
                 self.undo_history.append(value)
             if len(self.undo_history) > 3:
                 self.undo_history.pop(0)
 
     def undo(self, event):
         """Undo the last change to the widget.
 
@@ -928,33 +934,41 @@
         required : bool
             If True, the spinbox will require a value
         precision : int
             The number of decimal places allowed in the spinbox
 
         """
         super().__init__(*args, **kwargs)
+
         #: Decimal: The resolution of the spinbox
         self.resolution = str(kwargs.get("increment", "1.0"))  # Number put into spinbox
+
         #: int: The precision of the spinbox
         self.precision = self._get_precision()
+
         #: tk.StringVar: The variable to store the value of the spinbox in
         self.variable = kwargs.get("textvariable") or tk.DoubleVar()
+
         #: bool: Whether the spinbox requires a value
         self.required = required
 
         # Dynamic range checker
         if min_var:
             #: str: The minimum value of the spinbox
             self.min_var = min_var
             self.min_var.trace_add("write", self._set_minimum)
+
         if max_var:
             #: str: The maximum value of the spinbox
             self.max_var = max_var
             self.max_var.trace_add("write", self._set_maximum)
+
+        #: tk.StringVar: The variable to update when the spinbox loses focus
         self.focus_update_var = focus_update_var
+
         self.bind("<FocusOut>", self._set_focus_update_var)
 
     def set_precision(self, prec):
         """Set the precision of the spinbox in decimal places.
 
         Given a precision it will update the spinboxes ability to handle more or less
         precision for validation. This is separate from the increment value.
@@ -1017,18 +1031,18 @@
         if action == "0":
             if proposed == "":
                 return True
             self._is_valid_proposed_value(proposed)
             return True
 
         return self._is_valid_proposed_value(proposed)
-    
+
     def _is_valid_proposed_value(self, proposed):
         """Validate a proposed value
-        
+
         Returns
         -------
         bool
             True if the proposed is valid, False if not
         """
         min_val = self.cget("from")
         max_val = self.cget("to")
@@ -1042,15 +1056,15 @@
             proposed = Decimal(proposed)
         except InvalidOperation:
             return False
         proposed_precision = proposed.as_tuple().exponent
 
         if any([(proposed > max_val), (proposed_precision < self.precision)]):
             return False
-        
+
         if proposed < min_val:
             self._toggle_error(True)
             return True
 
         self._toggle_error(False)
 
         return True
@@ -1205,12 +1219,17 @@
         value = self.get()
         if value != "":
             min_val = self.cget("from")
             max_val = self.cget("to")
             # Don't add duplicates
             if self.undo_history and self.undo_history[-1] == value:
                 pass
-            elif value != "-" and value != "." and Decimal(value) >= min_val and Decimal(value) <= max_val:
+            elif (
+                value != "-"
+                and value != "."
+                and Decimal(value) >= min_val
+                and Decimal(value) <= max_val
+            ):
                 self.undo_history.append(value)
                 self.redo_history = []
             if len(self.undo_history) > 3:
                 self.undo_history.pop(0)
```

### Comparing `navigate-micro-0.0.4/src/navigate/view/icon/mic.ico` & `navigate-micro-0.0.5/src/navigate/view/icon/mic.ico`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/icon/mic.png` & `navigate-micro-0.0.5/src/navigate/view/icon/mic.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/icon/mic_orig.png` & `navigate-micro-0.0.5/src/navigate/view/icon/mic_orig.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/icon/splash_screen_image.png` & `navigate-micro-0.0.5/src/navigate/view/icon/splash_screen_image.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_application_window.py` & `navigate-micro-0.0.5/src/navigate/view/main_application_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/acquire_notebook.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/acquire_notebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/camera_tab.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/camera_tab.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/channels_tab.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/channels_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         #: QuickLaunchFrame: The frame that holds the quick launch buttons
         self.quick_launch = QuickLaunchFrame(self)
         self.quick_launch.grid(
             row=4, column=1, columnspan=2, sticky=tk.NSEW, padx=10, pady=10
         )
 
 
-
 class ChannelCreator(ttk.Labelframe):
     """Channel Creator
 
     This frame is used to create the channels for the stack acquisition.
     """
 
     def __init__(self, channels_tab, *args, **kwargs):
@@ -131,54 +130,54 @@
         self.title = "Channel Settings"
         ttk.Labelframe.__init__(self, channels_tab, text=self.title, *args, **kwargs)
 
         # Formatting
         tk.Grid.columnconfigure(self, "all", weight=1)
         tk.Grid.rowconfigure(self, "all", weight=1)
 
-        #: list: List of the variables for the channel checkbuttons
+        #: list: List of the variables for the channel check buttons
         self.channel_variables = []
 
-        #: list: List of the channel checkbuttons
+        #: list: List of the channel check buttons
         self.channel_checks = []
 
         #: list: List of the variables for the laser dropdowns
         self.laser_variables = []
 
         #: list: List of the laser dropdowns
         self.laser_pulldowns = []
 
         #: list: List of the variables for the laser power dropdowns
         self.laserpower_variables = []
 
         #: list: List of the laser power dropdowns
         self.laserpower_pulldowns = []
 
-        #: list: List of the variables for the filterwheel dropdowns
+        #: list: List of the variables for the filter  wheel dropdowns
         self.filterwheel_variables = []
 
         #: list: List of the filterwheel dropdowns
         self.filterwheel_pulldowns = []
 
         #: list: List of the variables for the exposure time dropdowns
         self.exptime_variables = []
 
         #: list: List of the exposure time dropdowns
         self.exptime_pulldowns = []
 
-        #: list: List of the variables for the time interval spinboxes
+        #: list: List of the variables for the time interval spin boxes
         self.interval_variables = []
 
-        #: list: List of the time interval spinboxes
+        #: list: List of the time interval spin boxes
         self.interval_spins = []
 
-        #: list: List of the variables for the defocus spinboxes
+        #: list: List of the variables for the defocus spin boxes
         self.defocus_variables = []
 
-        #: list: List of the defocus spinboxes
+        #: list: List of the defocus spin boxes
         self.defocus_spins = []
 
         #: list: List of the labels for the columns
         self.label_text = [
             "Channel",
             "Laser",
             "Power",
@@ -244,29 +243,29 @@
             self.laser_pulldowns.append(
                 ttk.Combobox(
                     self.frame_columns[1],
                     textvariable=self.laser_variables[num],
                     width=6,
                 )
             )
-            self.laser_pulldowns[num].config(state = "readonly")
+            self.laser_pulldowns[num].config(state="readonly")
             self.laser_pulldowns[num].grid(
                 row=num + 1, column=0, sticky=tk.NSEW, padx=1, pady=1
             )
 
             #  Laser Power Spinbox
             self.laserpower_variables.append(tk.StringVar())
             self.laserpower_pulldowns.append(
                 ValidatedSpinbox(
                     self.frame_columns[2],
                     from_=0,
                     to=100.0,
                     textvariable=self.laserpower_variables[num],
                     increment=5,
-                    width=3,
+                    width=5,
                     font=tk.font.Font(size=11),
                 )
             )
             self.laserpower_pulldowns[num].grid(
                 row=num + 1, column=0, sticky=tk.NS, padx=1, pady=1
             )
 
@@ -275,15 +274,15 @@
             self.filterwheel_pulldowns.append(
                 ttk.Combobox(
                     self.frame_columns[3],
                     textvariable=self.filterwheel_variables[num],
                     width=10,
                 )
             )
-            self.filterwheel_pulldowns[num].config(state = "readonly")
+            self.filterwheel_pulldowns[num].config(state="readonly")
             self.filterwheel_pulldowns[num].grid(
                 row=num + 1, column=0, sticky=tk.NSEW, padx=1, pady=1
             )
 
             #  Exposure Time Spin boxes
             self.exptime_variables.append(tk.StringVar())
             self.exptime_pulldowns.append(
```

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/display_notebook.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/display_notebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greydown.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greydown_disabled.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyleft.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyleft_disabled.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyright.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyright_disabled.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyup.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/greyup_disabled.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/images/wa_right.png` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/wa_right.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/menus.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/menus.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/multiposition_tab.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/multiposition_tab.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/settings_notebook.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/settings_notebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/main_window_content/stage_tab.py` & `navigate-micro-0.0.5/src/navigate/view/main_window_content/stage_tab.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/acquire_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/acquire_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/adaptiveoptics_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/adaptiveoptics_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/autofocus_setting_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/autofocus_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/camera_map_setting_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/camera_map_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/camera_view_popup_window.py` & `navigate-micro-0.0.5/src/navigate/view/popups/camera_view_popup_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/feature_list_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/feature_list_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/ilastik_setting_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/ilastik_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/microscope_setting_popup_window.py` & `navigate-micro-0.0.5/src/navigate/view/popups/microscope_setting_popup_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/plugins_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/plugins_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/tiling_wizard_popup.py` & `navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/tiling_wizard_popup2.py` & `navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup2.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate/view/popups/waveform_parameter_popup_window.py` & `navigate-micro-0.0.5/src/navigate/view/popups/waveform_parameter_popup_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,31 +225,32 @@
             self.buttons[galvo_labels[i] + " Freq"].grid(
                 row=prev + 2, column=2, sticky=tk.NSEW, pady=(20, 0)
             )
 
             prev = prev + 2
 
         # High/Low Resolution
-        hi_lo_labels = ["Percent Delay", "Percent Smoothing", "Settle Duration (ms)"]
-        dict_labels = ["Delay", "Smoothing", "Duty"]
-        for i in range(3):
+        hi_lo_labels = ["Delay (ms)", "Fly Back Time (ms)", "Settle Duration (ms)", "Percent Smoothing"]
+        dict_labels = ["Delay", "Ramp_falling" , "Duty", "Smoothing"]
+        for i in range(len(dict_labels)):
             self.inputs[dict_labels[i]] = LabelInput(
                 parent=self.high_low_frame,
                 input_class=ValidatedSpinbox,
                 label=hi_lo_labels[i],
                 input_var=tk.StringVar(),
                 label_args={"padding": (2, 5, 5, 0)},
                 input_args={"from_": 0, "to": 100, "increment": 0.1},
             )
             self.inputs[dict_labels[i]].grid(
                 row=i, column=0, sticky=tk.NSEW, padx=(2, 5)
             )
 
         # Padding Entry Widgets
-        self.inputs["Delay"].pad_input(60, 0, 0, 0)
+        self.inputs["Delay"].pad_input(75, 0, 0, 0)
+        self.inputs["Ramp_falling"].pad_input(30, 0, 0, 0)
         self.inputs["Smoothing"].pad_input(30, 0, 0, 0)
         self.inputs["Duty"].pad_input(25, 0, 0, 0)
 
     # Getters
     def get_variables(self):
         """Returns the variables of the inputs
```

### Comparing `navigate-micro-0.0.4/src/navigate/view/splash_screen.py` & `navigate-micro-0.0.5/src/navigate/view/splash_screen.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate_micro.egg-info/PKG-INFO` & `navigate-micro-0.0.5/src/navigate_micro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigate-micro
-Version: 0.0.4
+Version: 0.0.5
 Summary: Open source, smart, light-sheet microscopy control software.
 Author: The Dean Lab, UT Southwestern Medical Center
 License: Copyright (c) 2021-2023 The University of Texas Southwestern Medical Center.
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are
```

### Comparing `navigate-micro-0.0.4/src/navigate_micro.egg-info/SOURCES.txt` & `navigate-micro-0.0.5/src/navigate_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/src/navigate_micro.egg-info/requires.txt` & `navigate-micro-0.0.5/src/navigate_micro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/test/test_commit.py` & `navigate-micro-0.0.5/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.4/test/test_main.py` & `navigate-micro-0.0.5/test/test_main.py`

 * *Files identical despite different names*

