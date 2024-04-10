# Comparing `tmp/cnstd-1.2.3.5.tar.gz` & `tmp/cnstd-1.2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnstd-1.2.3.5.tar", last modified: Mon Oct  9 07:29:00 2023, max compression
+gzip compressed data, was "cnstd-1.2.3.6.tar", last modified: Wed Apr 10 13:56:00 2024, max compression
```

## Comparing `cnstd-1.2.3.5.tar` & `cnstd-1.2.3.6.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.728929 cnstd-1.2.3.5/
--rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnstd-1.2.3.5/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    29397 2023-10-09 07:29:00.725327 cnstd-1.2.3.5/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    28266 2023-10-09 07:26:24.000000 cnstd-1.2.3.5/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.596723 cnstd-1.2.3.5/cnstd/
--rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.3.5/cnstd/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      898 2023-10-09 07:01:32.000000 cnstd-1.2.3.5/cnstd/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.3.5/cnstd/app.py
--rw-r--r--   0 king       (501) staff       (20)    14425 2023-10-09 06:53:18.000000 cnstd-1.2.3.5/cnstd/cli.py
--rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.3.5/cnstd/cn_std.py
--rw-r--r--   0 king       (501) staff       (20)     9036 2023-10-09 06:55:15.000000 cnstd-1.2.3.5/cnstd/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.607039 cnstd-1.2.3.5/cnstd/datasets/
--rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/datasets/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.3.5/cnstd/datasets/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/datasets/util.py
--rw-r--r--   0 king       (501) staff       (20)    12290 2023-10-09 04:28:51.000000 cnstd-1.2.3.5/cnstd/detector.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.3.5/cnstd/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.616269 cnstd-1.2.3.5/cnstd/model/
--rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/model/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    15884 2023-06-30 10:13:21.000000 cnstd-1.2.3.5/cnstd/model/base.py
--rw-r--r--   0 king       (501) staff       (20)    10519 2023-06-30 10:27:24.000000 cnstd-1.2.3.5/cnstd/model/core.py
--rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/model/dbnet.py
--rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/model/fpn.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.626029 cnstd-1.2.3.5/cnstd/ppocr/
--rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.3.5/cnstd/ppocr/__init__.py
--rwxr-xr-x   0 king       (501) staff       (20)     7636 2023-10-09 04:30:59.000000 cnstd-1.2.3.5/cnstd/ppocr/angle_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.3.5/cnstd/ppocr/consts.py
--rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.3.5/cnstd/ppocr/img_operators.py
--rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.3.5/cnstd/ppocr/opt_utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.637551 cnstd-1.2.3.5/cnstd/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/cls_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/db_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/east_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pg_postprocess.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.639641 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/
--rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.641705 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
--rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.3.5/cnstd/ppocr/postprocess/sast_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    11682 2023-10-09 04:30:18.000000 cnstd-1.2.3.5/cnstd/ppocr/pp_detector.py
--rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.3.5/cnstd/ppocr/predict_rec.py
--rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.3.5/cnstd/ppocr/predict_system.py
--rw-r--r--   0 king       (501) staff       (20)    18879 2023-09-23 09:04:58.000000 cnstd-1.2.3.5/cnstd/ppocr/utility.py
--rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/trainer.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.650507 cnstd-1.2.3.5/cnstd/transforms/
--rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/transforms/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/transforms/base.py
--rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/transforms/process_data.py
--rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/cnstd/transforms/random_crop.py
--rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.3.5/cnstd/transforms/resize.py
--rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/transforms/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.656878 cnstd-1.2.3.5/cnstd/utils/
--rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     9475 2023-06-30 10:13:05.000000 cnstd-1.2.3.5/cnstd/utils/_utils.py
--rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/utils/common_types.py
--rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/utils/geometry.py
--rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/utils/metrics.py
--rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/cnstd/utils/repr.py
--rw-r--r--   0 king       (501) staff       (20)    17712 2023-10-09 06:58:18.000000 cnstd-1.2.3.5/cnstd/utils/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.700070 cnstd-1.2.3.5/cnstd/yolov7/
--rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.3.5/cnstd/yolov7/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.3.5/cnstd/yolov7/autoanchor.py
--rw-r--r--   0 king       (501) staff       (20)    85276 2023-09-21 03:10:05.000000 cnstd-1.2.3.5/cnstd/yolov7/common.py
--rw-r--r--   0 king       (501) staff       (20)     1300 2023-10-09 06:51:56.000000 cnstd-1.2.3.5/cnstd/yolov7/consts.py
--rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.3.5/cnstd/yolov7/datasets.py
--rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.3.5/cnstd/yolov7/experimental.py
--rw-r--r--   0 king       (501) staff       (20)    38670 2022-12-18 15:04:18.000000 cnstd-1.2.3.5/cnstd/yolov7/general.py
--rw-r--r--   0 king       (501) staff       (20)    15109 2023-10-09 04:29:44.000000 cnstd-1.2.3.5/cnstd/yolov7/layout_analyzer.py
--rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.3.5/cnstd/yolov7/loss.py
--rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.3.5/cnstd/yolov7/metrics.py
--rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.3.5/cnstd/yolov7/plots.py
--rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.3.5/cnstd/yolov7/torch_utils.py
--rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.3.5/cnstd/yolov7/yolo.py
--rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.3.5/cnstd/yolov7/yolov7-mfd.yaml
--rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.3.5/cnstd/yolov7/yolov7-tiny-layout.yaml
--rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.3.5/cnstd/yolov7/yolov7-tiny-mfd.yaml
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.603521 cnstd-1.2.3.5/cnstd.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    29397 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2256 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       40 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.3.5/cnstd.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      273 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-10-09 07:29:00.000000 cnstd-1.2.3.5/cnstd.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-10-09 07:29:00.729729 cnstd-1.2.3.5/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3366 2023-09-23 01:14:27.000000 cnstd-1.2.3.5/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-10-09 07:29:00.723711 cnstd-1.2.3.5/tests/
--rw-r--r--   0 king       (501) staff       (20)     1046 2022-07-06 06:05:27.000000 cnstd-1.2.3.5/tests/test_cnstd.py
--rw-r--r--   0 king       (501) staff       (20)     1411 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/tests/test_lr_schedulers.py
--rw-r--r--   0 king       (501) staff       (20)      986 2021-12-05 08:14:50.000000 cnstd-1.2.3.5/tests/test_models.py
--rw-r--r--   0 king       (501) staff       (20)      910 2021-08-26 09:54:14.000000 cnstd-1.2.3.5/tests/test_transforms.py
--rw-r--r--   0 king       (501) staff       (20)      456 2023-02-18 14:57:29.000000 cnstd-1.2.3.5/tests/test_utils.py
--rw-r--r--   0 king       (501) staff       (20)      281 2022-10-07 14:46:08.000000 cnstd-1.2.3.5/tests/test_yolov7.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.805409 cnstd-1.2.3.6/
+-rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnstd-1.2.3.6/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    29650 2024-04-10 13:56:00.804546 cnstd-1.2.3.6/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    28518 2024-02-02 07:26:36.000000 cnstd-1.2.3.6/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.786362 cnstd-1.2.3.6/cnstd/
+-rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.3.6/cnstd/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      898 2024-04-10 13:14:39.000000 cnstd-1.2.3.6/cnstd/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.3.6/cnstd/app.py
+-rw-r--r--   0 king       (501) staff       (20)    14425 2023-10-09 06:53:18.000000 cnstd-1.2.3.6/cnstd/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.3.6/cnstd/cn_std.py
+-rw-r--r--   0 king       (501) staff       (20)     9107 2024-04-10 13:22:57.000000 cnstd-1.2.3.6/cnstd/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.788011 cnstd-1.2.3.6/cnstd/datasets/
+-rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/datasets/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.3.6/cnstd/datasets/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/datasets/util.py
+-rw-r--r--   0 king       (501) staff       (20)    12290 2023-10-09 04:28:51.000000 cnstd-1.2.3.6/cnstd/detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.3.6/cnstd/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.789378 cnstd-1.2.3.6/cnstd/model/
+-rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/model/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    15884 2023-06-30 10:13:21.000000 cnstd-1.2.3.6/cnstd/model/base.py
+-rw-r--r--   0 king       (501) staff       (20)    10519 2023-06-30 10:27:24.000000 cnstd-1.2.3.6/cnstd/model/core.py
+-rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/model/dbnet.py
+-rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/model/fpn.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.791289 cnstd-1.2.3.6/cnstd/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.3.6/cnstd/ppocr/__init__.py
+-rwxr-xr-x   0 king       (501) staff       (20)     7636 2023-10-09 04:30:59.000000 cnstd-1.2.3.6/cnstd/ppocr/angle_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.3.6/cnstd/ppocr/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.3.6/cnstd/ppocr/img_operators.py
+-rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.3.6/cnstd/ppocr/opt_utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.793902 cnstd-1.2.3.6/cnstd/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/cls_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/db_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/east_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pg_postprocess.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.794351 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/
+-rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.794629 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.3.6/cnstd/ppocr/postprocess/sast_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    11682 2023-10-09 04:30:18.000000 cnstd-1.2.3.6/cnstd/ppocr/pp_detector.py
+-rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.3.6/cnstd/ppocr/predict_rec.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.3.6/cnstd/ppocr/predict_system.py
+-rw-r--r--   0 king       (501) staff       (20)    18879 2023-09-23 09:04:58.000000 cnstd-1.2.3.6/cnstd/ppocr/utility.py
+-rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/trainer.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.795472 cnstd-1.2.3.6/cnstd/transforms/
+-rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/transforms/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/transforms/base.py
+-rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/transforms/process_data.py
+-rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/cnstd/transforms/random_crop.py
+-rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.3.6/cnstd/transforms/resize.py
+-rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/transforms/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.796594 cnstd-1.2.3.6/cnstd/utils/
+-rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     9475 2023-06-30 10:13:05.000000 cnstd-1.2.3.6/cnstd/utils/_utils.py
+-rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/utils/common_types.py
+-rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/utils/geometry.py
+-rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/utils/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/cnstd/utils/repr.py
+-rw-r--r--   0 king       (501) staff       (20)    18273 2024-04-10 13:25:11.000000 cnstd-1.2.3.6/cnstd/utils/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.803208 cnstd-1.2.3.6/cnstd/yolov7/
+-rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.3.6/cnstd/yolov7/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.3.6/cnstd/yolov7/autoanchor.py
+-rw-r--r--   0 king       (501) staff       (20)    85276 2023-09-21 03:10:05.000000 cnstd-1.2.3.6/cnstd/yolov7/common.py
+-rw-r--r--   0 king       (501) staff       (20)     1300 2023-10-09 06:51:56.000000 cnstd-1.2.3.6/cnstd/yolov7/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.3.6/cnstd/yolov7/datasets.py
+-rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.3.6/cnstd/yolov7/experimental.py
+-rw-r--r--   0 king       (501) staff       (20)    38706 2024-04-10 13:05:59.000000 cnstd-1.2.3.6/cnstd/yolov7/general.py
+-rw-r--r--   0 king       (501) staff       (20)    15109 2023-10-09 04:29:44.000000 cnstd-1.2.3.6/cnstd/yolov7/layout_analyzer.py
+-rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.3.6/cnstd/yolov7/loss.py
+-rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.3.6/cnstd/yolov7/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.3.6/cnstd/yolov7/plots.py
+-rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.3.6/cnstd/yolov7/torch_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.3.6/cnstd/yolov7/yolo.py
+-rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.3.6/cnstd/yolov7/yolov7-mfd.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.3.6/cnstd/yolov7/yolov7-tiny-layout.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.3.6/cnstd/yolov7/yolov7-tiny-mfd.yaml
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.787430 cnstd-1.2.3.6/cnstd.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    29650 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2256 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       41 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.3.6/cnstd.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      273 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2024-04-10 13:56:00.000000 cnstd-1.2.3.6/cnstd.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-04-10 13:56:00.805462 cnstd-1.2.3.6/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3366 2023-09-23 01:14:27.000000 cnstd-1.2.3.6/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 13:56:00.804314 cnstd-1.2.3.6/tests/
+-rw-r--r--   0 king       (501) staff       (20)     1046 2022-07-06 06:05:27.000000 cnstd-1.2.3.6/tests/test_cnstd.py
+-rw-r--r--   0 king       (501) staff       (20)     1411 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/tests/test_lr_schedulers.py
+-rw-r--r--   0 king       (501) staff       (20)      986 2021-12-05 08:14:50.000000 cnstd-1.2.3.6/tests/test_models.py
+-rw-r--r--   0 king       (501) staff       (20)      910 2021-08-26 09:54:14.000000 cnstd-1.2.3.6/tests/test_transforms.py
+-rw-r--r--   0 king       (501) staff       (20)      456 2023-02-18 14:57:29.000000 cnstd-1.2.3.6/tests/test_utils.py
+-rw-r--r--   0 king       (501) staff       (20)      281 2022-10-07 14:46:08.000000 cnstd-1.2.3.6/tests/test_yolov7.py
```

### Comparing `cnstd-1.2.3.5/LICENSE` & `cnstd-1.2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/PKG-INFO` & `cnstd-1.2.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.3.5
+Version: 1.2.3.6
 Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
@@ -28,14 +28,15 @@
 License-File: LICENSE
 
 <div align="center">
 	<img src="./docs/logo.png" width="250px"/>
   <div>&nbsp;</div>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD)
 [![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
 [![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
 ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
@@ -303,15 +304,15 @@
 
 - `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
   
   - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
   
   - `score`：得分；`float` 类型；分数越高表示越可靠；
   
-  - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
+  - `cropped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
   
   - 示例:
     
     ```python
       [{'box': array([[416,  77],
                       [486,  13],
                       [800, 325],
@@ -626,7 +627,8 @@
 ## 给作者来杯咖啡
 
 开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
 
 ---
 
 官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
+
```

### Comparing `cnstd-1.2.3.5/README.md` & `cnstd-1.2.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <div align="center">
 	<img src="./docs/logo.png" width="250px"/>
   <div>&nbsp;</div>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD)
 [![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
 [![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
 ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
@@ -274,15 +275,15 @@
 
 - `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
   
   - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
   
   - `score`：得分；`float` 类型；分数越高表示越可靠；
   
-  - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
+  - `cropped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
   
   - 示例:
     
     ```python
       [{'box': array([[416,  77],
                       [486,  13],
                       [800, 325],
```

### Comparing `cnstd-1.2.3.5/cnstd/__init__.py` & `cnstd-1.2.3.6/cnstd/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/__version__.py` & `cnstd-1.2.3.6/cnstd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '1.2.3.5'
+__version__ = '1.2.3.6'
```

### Comparing `cnstd-1.2.3.5/cnstd/app.py` & `cnstd-1.2.3.6/cnstd/app.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/cli.py` & `cnstd-1.2.3.6/cnstd/cli.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/cn_std.py` & `cnstd-1.2.3.6/cnstd/cn_std.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/consts.py` & `cnstd-1.2.3.6/cnstd/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 
 
 # 模型版本只对应到第二层，第三层的改动表示模型兼容。
 # 如: __version__ = '1.0.*'，对应的 MODEL_VERSION 都是 '1.0'
 MODEL_VERSION = '.'.join(__version__.split('.', maxsplit=2)[:2])
 VOCAB_FP = Path(__file__).parent.parent / 'label_cn.txt'
 # Which OSS source will be used for downloading model files, 'CN' or 'HF'
-DOWNLOAD_SOURCE = os.environ.get('CNSTD_DOWNLOAD_SOURCE', 'CN')
+DOWNLOAD_SOURCE = os.environ.get('CNSTD_DOWNLOAD_SOURCE', 'HF')
+HF_ENDPOINT_LIST = ['https://huggingface.co', 'https://hf-mirror.com']
 
 MODEL_CONFIGS: Dict[str, Dict[str, Any]] = {
     'db_resnet50': {
         'backbone': resnet50,
         'backbone_submodule': None,
         'fpn_layers': ['layer1', 'layer2', 'layer3', 'layer4'],
         'fpn_channels': [256, 512, 1024, 2048],
```

### Comparing `cnstd-1.2.3.5/cnstd/datasets/__init__.py` & `cnstd-1.2.3.6/cnstd/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/datasets/dataset.py` & `cnstd-1.2.3.6/cnstd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/datasets/util.py` & `cnstd-1.2.3.6/cnstd/datasets/util.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/detector.py` & `cnstd-1.2.3.6/cnstd/detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/lr_scheduler.py` & `cnstd-1.2.3.6/cnstd/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/model/__init__.py` & `cnstd-1.2.3.6/cnstd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/model/base.py` & `cnstd-1.2.3.6/cnstd/model/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/model/core.py` & `cnstd-1.2.3.6/cnstd/model/core.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/model/dbnet.py` & `cnstd-1.2.3.6/cnstd/model/dbnet.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/model/fpn.py` & `cnstd-1.2.3.6/cnstd/model/fpn.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/__init__.py` & `cnstd-1.2.3.6/cnstd/ppocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/angle_classifier.py` & `cnstd-1.2.3.6/cnstd/ppocr/angle_classifier.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/consts.py` & `cnstd-1.2.3.6/cnstd/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/img_operators.py` & `cnstd-1.2.3.6/cnstd/ppocr/img_operators.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/opt_utils.py` & `cnstd-1.2.3.6/cnstd/ppocr/opt_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/__init__.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/cls_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/db_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/east_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/locality_aware_nms.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/pg_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/__init__.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/rec_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/postprocess/sast_postprocess.py` & `cnstd-1.2.3.6/cnstd/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/pp_detector.py` & `cnstd-1.2.3.6/cnstd/ppocr/pp_detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/predict_rec.py` & `cnstd-1.2.3.6/cnstd/ppocr/predict_rec.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/predict_system.py` & `cnstd-1.2.3.6/cnstd/ppocr/predict_system.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/ppocr/utility.py` & `cnstd-1.2.3.6/cnstd/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/trainer.py` & `cnstd-1.2.3.6/cnstd/trainer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/__init__.py` & `cnstd-1.2.3.6/cnstd/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/base.py` & `cnstd-1.2.3.6/cnstd/transforms/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/process_data.py` & `cnstd-1.2.3.6/cnstd/transforms/process_data.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/random_crop.py` & `cnstd-1.2.3.6/cnstd/transforms/random_crop.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/resize.py` & `cnstd-1.2.3.6/cnstd/transforms/resize.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/transforms/utils.py` & `cnstd-1.2.3.6/cnstd/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/__init__.py` & `cnstd-1.2.3.6/cnstd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/_utils.py` & `cnstd-1.2.3.6/cnstd/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/common_types.py` & `cnstd-1.2.3.6/cnstd/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/geometry.py` & `cnstd-1.2.3.6/cnstd/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/metrics.py` & `cnstd-1.2.3.6/cnstd/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/repr.py` & `cnstd-1.2.3.6/cnstd/utils/repr.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/utils/utils.py` & `cnstd-1.2.3.6/cnstd/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from tqdm import tqdm
 import cv2
 import numpy as np
 from PIL import Image, ImageOps
 import torch
 from huggingface_hub import hf_hub_download
 
-from ..consts import MODEL_VERSION, MODEL_CONFIGS, AVAILABLE_MODELS
+from ..consts import MODEL_VERSION, MODEL_CONFIGS, HF_ENDPOINT_LIST
 
 
 fmt = '[%(levelname)s %(asctime)s %(funcName)s:%(lineno)d] %(' 'message)s '
 logging.basicConfig(format=fmt)
 logging.captureWarnings(True)
 logger = logging.getLogger()
 
@@ -181,34 +181,46 @@
                 if total_length is None:  # no content length header
                     for chunk in r.iter_content(chunk_size=1024):
                         if chunk:  # filter out keep-alive new chunks
                             f.write(chunk)
                 else:
                     total_length = int(total_length)
                     for chunk in tqdm(
-                            r.iter_content(chunk_size=1024),
-                            total=int(total_length / 1024.0 + 0.5),
-                            unit='KB',
-                            unit_scale=False,
-                            dynamic_ncols=True,
+                        r.iter_content(chunk_size=1024),
+                        total=int(total_length / 1024.0 + 0.5),
+                        unit='KB',
+                        unit_scale=False,
+                        dynamic_ncols=True,
                     ):
                         f.write(chunk)
         else:
             HF_TOKEN = os.environ.get('HF_TOKEN')
-            logger.info('Downloading %s from HF Repo %s...' % (fname, url["repo_id"]))
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                local_path = hf_hub_download(
-                    repo_id=url["repo_id"],
-                    subfolder=url["subfolder"],
-                    filename=url["filename"],
-                    repo_type="model",
-                    cache_dir=tmp_dir,
-                    token=HF_TOKEN,
-                )
-                shutil.copy2(local_path, fname)
+            for hf_endpoint in HF_ENDPOINT_LIST:
+                try:
+                    logger.info(
+                        'Downloading %s from HF Repo %s/%s...'
+                        % (fname, hf_endpoint, url["repo_id"])
+                    )
+                    with tempfile.TemporaryDirectory() as tmp_dir:
+                        local_path = hf_hub_download(
+                            repo_id=url["repo_id"],
+                            subfolder=url["subfolder"],
+                            filename=url["filename"],
+                            repo_type="model",
+                            cache_dir=tmp_dir,
+                            token=HF_TOKEN,
+                            endpoint=hf_endpoint,
+                        )
+                        shutil.copy2(local_path, fname)
+                        break
+                except:
+                    logger.warning(
+                        'Failed to download %s from HF Repo %s/%s.'
+                        % (fname, hf_endpoint, url["repo_id"])
+                    )
 
         if sha1_hash and not check_sha1(fname, sha1_hash):
             raise UserWarning(
                 'File {} is downloaded but the content hash does not match. '
                 'The repo may be outdated or download may be incomplete. '
                 'If the "repo_url" is overridden, consider switching to '
                 'the default repo.'.format(fname)
@@ -242,21 +254,25 @@
     model_dir = os.path.expanduser(model_dir)
     par_dir = os.path.dirname(model_dir)
     os.makedirs(par_dir, exist_ok=True)
 
     zip_file_path = os.path.join(par_dir, url['filename'])
     if not os.path.exists(zip_file_path):
         try:
-            download(url, path=zip_file_path, download_source=download_source, overwrite=True)
+            download(
+                url, path=zip_file_path, download_source=download_source, overwrite=True
+            )
         except Exception as e:
             logger.error(e)
             message = f'Failed to download model: {url["filename"]}.'
-            message += '\n\tPlease open your VPN and try again. \n\t' \
-                       'If this error persists, please follow the instruction at ' \
-                       '[CnSTD/CnOCR Doc](https://www.breezedeus.com/cnocr) to manually download the model files.'
+            message += (
+                '\n\tPlease open your VPN and try again. \n\t'
+                'If this error persists, please follow the instruction at '
+                '[CnSTD/CnOCR Doc](https://www.breezedeus.com/cnocr) to manually download the model files.'
+            )
             raise ModelDownloadingError(message)
     with zipfile.ZipFile(zip_file_path) as zf:
         zf.extractall(par_dir)
     os.remove(zip_file_path)
 
     return model_dir
```

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/__init__.py` & `cnstd-1.2.3.6/cnstd/yolov7/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/autoanchor.py` & `cnstd-1.2.3.6/cnstd/yolov7/autoanchor.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/common.py` & `cnstd-1.2.3.6/cnstd/yolov7/common.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/consts.py` & `cnstd-1.2.3.6/cnstd/yolov7/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/datasets.py` & `cnstd-1.2.3.6/cnstd/yolov7/datasets.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/experimental.py` & `cnstd-1.2.3.6/cnstd/yolov7/experimental.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/general.py` & `cnstd-1.2.3.6/cnstd/yolov7/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,55 +114,55 @@
 def check_requirements(requirements='requirements.txt', exclude=()):
     # Check installed dependencies meet requirements (pass *.txt file or list of packages)
     import pkg_resources as pkg
     prefix = colorstr('red', 'bold', 'requirements:')
     if isinstance(requirements, (str, Path)):  # requirements.txt file
         file = Path(requirements)
         if not file.exists():
-            print(f"{prefix} {file.resolve()} not found, check failed.")
+            logger.warning(f"{prefix} {file.resolve()} not found, check failed.")
             return
         requirements = [f'{x.name}{x.specifier}' for x in pkg.parse_requirements(file.open()) if x.name not in exclude]
     else:  # list or tuple of packages
         requirements = [x for x in requirements if x not in exclude]
 
     n = 0  # number of packages updates
     for r in requirements:
         try:
             pkg.require(r)
         except Exception as e:  # DistributionNotFound or VersionConflict if requirements not met
             n += 1
-            print(f"{prefix} {e.req} not found and is required by YOLOR, attempting auto-update...")
+            logger.warning(f"{prefix} {e.req} not found and is required by YOLOR, attempting auto-update...")
             print(subprocess.check_output(f"pip install '{e.req}'", shell=True).decode())
 
     if n:  # if packages updated
         source = file.resolve() if 'file' in locals() else requirements
         s = f"{prefix} {n} package{'s' * (n > 1)} updated per {source}\n" \
             f"{prefix} ⚠️ {colorstr('bold', 'Restart runtime or rerun command for updates to take effect')}\n"
         print(emojis(s))  # emoji-safe
 
 
 def check_img_size(img_size, s=32):
     # Verify img_size is a multiple of stride s
     new_size = make_divisible(img_size, int(s))  # ceil gs-multiple
     if new_size != img_size:
-        print('WARNING: --img-size %g must be multiple of max stride %g, updating to %g' % (img_size, s, new_size))
+        logger.warning('--img-size %g must be multiple of max stride %g, updating to %g' % (img_size, s, new_size))
     return new_size
 
 
 def check_imshow():
     # Check if environment supports image displays
     try:
         assert not isdocker(), 'cv2.imshow() is disabled in Docker environments'
         cv2.imshow('test', np.zeros((1, 1, 3)))
         cv2.waitKey(1)
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         return True
     except Exception as e:
-        print(f'WARNING: Environment does not support cv2.imshow() or PIL Image.show() image displays\n{e}')
+        logger.warning(f'Environment does not support cv2.imshow() or PIL Image.show() image displays\n{e}')
         return False
 
 
 def check_file(file):
     # Search for file if not found
     if Path(file).is_file() or file == '':
         return file
@@ -175,24 +175,24 @@
 
 def check_dataset(dict):
     # Download dataset if not found locally
     val, s = dict.get('val'), dict.get('download')
     if val and len(val):
         val = [Path(x).resolve() for x in (val if isinstance(val, list) else [val])]  # val path
         if not all(x.exists() for x in val):
-            print('\nWARNING: Dataset not found, nonexistent paths: %s' % [str(x) for x in val if not x.exists()])
+            logger.warning('\nDataset not found, nonexistent paths: %s' % [str(x) for x in val if not x.exists()])
             if s and len(s):  # download script
-                print('Downloading %s ...' % s)
+                logger.info('Downloading %s ...' % s)
                 if s.startswith('http') and s.endswith('.zip'):  # URL
                     f = Path(s).name  # filename
                     torch.hub.download_url_to_file(s, f)
                     r = os.system('unzip -q %s -d ../ && rm %s' % (f, f))  # unzip
                 else:  # bash script
                     r = os.system(s)
-                print('Dataset autodownload %s\n' % ('success' if r == 0 else 'failure'))  # analyze return value
+                logger.info('Dataset autodownload %s\n' % ('success' if r == 0 else 'failure'))  # analyze return value
             else:
                 raise Exception('Dataset not found.')
 
 
 def make_divisible(x, divisor):
     # Returns x evenly divisible by divisor
     return math.ceil(x / divisor) * divisor
@@ -830,15 +830,15 @@
             weights = iou * scores[None]  # box weights
             x[i, :4] = torch.mm(weights, x[:, :4]).float() / weights.sum(1, keepdim=True)  # merged boxes
             if redundant:
                 i = i[iou.sum(1) > 1]  # require redundancy
 
         output[xi] = x[i]
         if (time.time() - t) > time_limit:
-            print(f'WARNING: NMS time limit {time_limit}s exceeded')
+            logger.warning(f'NMS time limit {time_limit}s exceeded')
             break  # time limit exceeded
 
     return output
 
 
 def strip_optimizer(f='best.pt', s=''):  # from utils.general import *; strip_optimizer()
     # Strip optimizer from 'f' to finalize training, optionally save as 's'
@@ -849,15 +849,15 @@
         x[k] = None
     x['epoch'] = -1
     x['model'].half()  # to FP16
     for p in x['model'].parameters():
         p.requires_grad = False
     torch.save(x, s or f)
     mb = os.path.getsize(s or f) / 1E6  # filesize
-    print(f"Optimizer stripped from {f},{(' saved as %s,' % s) if s else ''} {mb:.1f}MB")
+    logger.info(f"Optimizer stripped from {f},{(' saved as %s,' % s) if s else ''} {mb:.1f}MB")
 
 
 # def print_mutation(hyp, results, yaml_file='hyp_evolved.yaml', bucket=''):
 #     # Print mutation results to evolve.txt (for use with train.py --evolve)
 #     a = '%10s' * len(hyp) % tuple(hyp.keys())  # hyperparam keys
 #     b = '%10.3g' * len(hyp) % tuple(hyp.values())  # hyperparam values
 #     c = '%10.4g' * len(results) % results  # results (P, R, mAP@0.5, mAP@0.5:0.95, val_losses x 3)
```

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/layout_analyzer.py` & `cnstd-1.2.3.6/cnstd/yolov7/layout_analyzer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/loss.py` & `cnstd-1.2.3.6/cnstd/yolov7/loss.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/metrics.py` & `cnstd-1.2.3.6/cnstd/yolov7/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/plots.py` & `cnstd-1.2.3.6/cnstd/yolov7/plots.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/torch_utils.py` & `cnstd-1.2.3.6/cnstd/yolov7/torch_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/yolo.py` & `cnstd-1.2.3.6/cnstd/yolov7/yolo.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/yolov7-mfd.yaml` & `cnstd-1.2.3.6/cnstd/yolov7/yolov7-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/yolov7-tiny-layout.yaml` & `cnstd-1.2.3.6/cnstd/yolov7/yolov7-tiny-layout.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd/yolov7/yolov7-tiny-mfd.yaml` & `cnstd-1.2.3.6/cnstd/yolov7/yolov7-tiny-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/cnstd.egg-info/PKG-INFO` & `cnstd-1.2.3.6/cnstd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.3.5
+Version: 1.2.3.6
 Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
@@ -28,14 +28,15 @@
 License-File: LICENSE
 
 <div align="center">
 	<img src="./docs/logo.png" width="250px"/>
   <div>&nbsp;</div>
 
 [![Downloads](https://static.pepy.tech/personalized-badge/cnstd?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnstd)
+[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnSTD)
 [![license](https://img.shields.io/github/license/breezedeus/cnstd)](./LICENSE)
 [![PyPI version](https://badge.fury.io/py/cnstd.svg)](https://badge.fury.io/py/cnstd)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnstd)](https://img.shields.io/github/forks/breezedeus/cnstd)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnstd)](https://github.com/breezedeus/cnocr)
 ![last-releast](https://img.shields.io/github/release-date/breezedeus/cnstd?style=plastic)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/cnstd)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
@@ -303,15 +304,15 @@
 
 - `detected_texts`: `list`, 每个元素存储了检测出的一个框的信息，使用词典记录，包括以下几个值：
   
   - `box`：检测出的文字对应的矩形框；`np.ndarray`, shape: `(4, 2)`，对应 box 4个点的坐标值 `(x, y)`;
   
   - `score`：得分；`float` 类型；分数越高表示越可靠；
   
-  - `croppped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
+  - `cropped_img`：对应 "box" 中的图片patch（`RGB`格式），会把倾斜的图片旋转为水平。`np.ndarray`类型，`shape: (height, width, 3)`,  取值范围：`[0, 255]`；
   
   - 示例:
     
     ```python
       [{'box': array([[416,  77],
                       [486,  13],
                       [800, 325],
@@ -626,7 +627,8 @@
 ## 给作者来杯咖啡
 
 开源不易，如果此项目对您有帮助，可以考虑 [给作者来杯咖啡 ☕️](https://cnocr.readthedocs.io/zh/latest/buymeacoffee/) 。
 
 ---
 
 官方代码库：[https://github.com/breezedeus/cnstd](https://github.com/breezedeus/cnstd)。
+
```

### Comparing `cnstd-1.2.3.5/cnstd.egg-info/SOURCES.txt` & `cnstd-1.2.3.6/cnstd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/setup.py` & `cnstd-1.2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/tests/test_cnstd.py` & `cnstd-1.2.3.6/tests/test_cnstd.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/tests/test_lr_schedulers.py` & `cnstd-1.2.3.6/tests/test_lr_schedulers.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/tests/test_models.py` & `cnstd-1.2.3.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3.5/tests/test_transforms.py` & `cnstd-1.2.3.6/tests/test_transforms.py`

 * *Files identical despite different names*

