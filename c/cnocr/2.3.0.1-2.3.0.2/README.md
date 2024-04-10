# Comparing `tmp/cnocr-2.3.0.1.tar.gz` & `tmp/cnocr-2.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnocr-2.3.0.1.tar", last modified: Tue Dec 26 09:05:42 2023, max compression
+gzip compressed data, was "cnocr-2.3.0.2.tar", last modified: Wed Apr 10 14:13:05 2024, max compression
```

## Comparing `cnocr-2.3.0.1.tar` & `cnocr-2.3.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.460714 cnocr-2.3.0.1/
--rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnocr-2.3.0.1/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    22852 2023-12-26 09:05:42.460572 cnocr-2.3.0.1/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    21779 2023-12-24 10:56:28.000000 cnocr-2.3.0.1/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.453196 cnocr-2.3.0.1/cnocr/
--rw-r--r--   0 king       (501) staff       (20)     1276 2023-12-15 14:22:44.000000 cnocr-2.3.0.1/cnocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      898 2023-12-26 09:03:58.000000 cnocr-2.3.0.1/cnocr/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     7026 2023-12-22 11:05:35.000000 cnocr-2.3.0.1/cnocr/app.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.454702 cnocr-2.3.0.1/cnocr/classification/
--rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.3.0.1/cnocr/classification/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.3.0.1/cnocr/classification/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.3.0.1/cnocr/classification/image_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.3.0.1/cnocr/clf_cli.py
--rw-r--r--   0 king       (501) staff       (20)    20063 2023-12-24 11:11:06.000000 cnocr-2.3.0.1/cnocr/cli.py
--rw-r--r--   0 king       (501) staff       (20)    17853 2023-12-22 11:08:08.000000 cnocr-2.3.0.1/cnocr/cn_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13733 2023-12-24 11:27:47.000000 cnocr-2.3.0.1/cnocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.455553 cnocr-2.3.0.1/cnocr/data_utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.3.0.1/cnocr/data_utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.3.0.1/cnocr/data_utils/aug.py
--rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.3.0.1/cnocr/data_utils/block_shuffle.py
--rw-r--r--   0 king       (501) staff       (20)    14928 2023-12-17 02:01:02.000000 cnocr-2.3.0.1/cnocr/data_utils/transforms.py
--rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.3.0.1/cnocr/data_utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     6380 2023-12-17 02:23:32.000000 cnocr-2.3.0.1/cnocr/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     3931 2023-12-15 14:07:55.000000 cnocr-2.3.0.1/cnocr/dataset_utils.py
--rw-r--r--   0 king       (501) staff       (20)     8873 2023-09-21 08:44:57.000000 cnocr-2.3.0.1/cnocr/gradio_app.py
--rw-r--r--   0 king       (501) staff       (20)     9676 2023-09-20 02:24:06.000000 cnocr-2.3.0.1/cnocr/gradio_app2.py
--rw-r--r--   0 king       (501) staff       (20)    26570 2023-11-04 12:25:59.000000 cnocr-2.3.0.1/cnocr/label_cn.txt
--rw-r--r--   0 king       (501) staff       (20)       19 2023-09-07 02:26:43.000000 cnocr-2.3.0.1/cnocr/label_number.txt
--rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.3.0.1/cnocr/line_split.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.3.0.1/cnocr/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.456304 cnocr-2.3.0.1/cnocr/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.3.0.1/cnocr/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.3.0.1/cnocr/models/ctc.py
--rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.3.0.1/cnocr/models/densenet.py
--rw-r--r--   0 king       (501) staff       (20)     6877 2023-05-11 02:09:18.000000 cnocr-2.3.0.1/cnocr/models/mobilenet.py
--rw-r--r--   0 king       (501) staff       (20)    12001 2023-12-22 09:32:41.000000 cnocr-2.3.0.1/cnocr/models/ocr_model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.457123 cnocr-2.3.0.1/cnocr/ppocr/
--rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.457611 cnocr-2.3.0.1/cnocr/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    10242 2023-12-22 11:10:08.000000 cnocr-2.3.0.1/cnocr/ppocr/pp_recognizer.py
--rw-r--r--   0 king       (501) staff       (20)    20282 2023-12-26 09:01:47.000000 cnocr-2.3.0.1/cnocr/ppocr/utility.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.458394 cnocr-2.3.0.1/cnocr/ppocr/utils/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/utils/chinese_cht_dict.txt
--rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/utils/en_dict.txt
--rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/cnocr/ppocr/utils/ppocr_keys_v1.txt
--rw-r--r--   0 king       (501) staff       (20)    17227 2023-12-22 11:08:36.000000 cnocr-2.3.0.1/cnocr/recognizer.py
--rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.3.0.1/cnocr/serve.py
--rw-r--r--   0 king       (501) staff       (20)    13168 2023-11-06 12:37:09.000000 cnocr-2.3.0.1/cnocr/trainer.py
--rw-r--r--   0 king       (501) staff       (20)    14898 2023-12-21 09:48:48.000000 cnocr-2.3.0.1/cnocr/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.454227 cnocr-2.3.0.1/cnocr.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    22852 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     1412 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       71 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.3.0.1/cnocr.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      294 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-12-26 09:05:42.000000 cnocr-2.3.0.1/cnocr.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-12-26 09:05:42.460761 cnocr-2.3.0.1/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3369 2023-12-15 14:09:20.000000 cnocr-2.3.0.1/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-12-26 09:05:42.460237 cnocr-2.3.0.1/tests/
--rw-r--r--   0 king       (501) staff       (20)     9469 2023-12-22 11:11:59.000000 cnocr-2.3.0.1/tests/test_cnocr.py
--rw-r--r--   0 king       (501) staff       (20)     1822 2023-09-19 11:58:02.000000 cnocr-2.3.0.1/tests/test_dataset.py
--rw-r--r--   0 king       (501) staff       (20)     4947 2021-11-05 14:17:16.000000 cnocr-2.3.0.1/tests/test_models.py
--rw-r--r--   0 king       (501) staff       (20)     3102 2022-07-20 02:15:52.000000 cnocr-2.3.0.1/tests/test_ppocr.py
--rw-r--r--   0 king       (501) staff       (20)     1298 2023-12-22 11:12:21.000000 cnocr-2.3.0.1/tests/test_pytorch.py
--rw-r--r--   0 king       (501) staff       (20)     1705 2023-12-22 11:12:28.000000 cnocr-2.3.0.1/tests/test_trainer.py
--rw-r--r--   0 king       (501) staff       (20)     5674 2023-09-23 15:24:13.000000 cnocr-2.3.0.1/tests/test_transforms.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.876387 cnocr-2.3.0.2/
+-rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnocr-2.3.0.2/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    23173 2024-04-10 14:13:05.876251 cnocr-2.3.0.2/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    22100 2024-03-16 05:12:51.000000 cnocr-2.3.0.2/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.868469 cnocr-2.3.0.2/cnocr/
+-rw-r--r--   0 king       (501) staff       (20)     1276 2023-12-15 14:22:44.000000 cnocr-2.3.0.2/cnocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      898 2024-04-10 14:06:19.000000 cnocr-2.3.0.2/cnocr/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     7026 2023-12-22 11:05:35.000000 cnocr-2.3.0.2/cnocr/app.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.870193 cnocr-2.3.0.2/cnocr/classification/
+-rw-r--r--   0 king       (501) staff       (20)      915 2023-02-11 15:48:37.000000 cnocr-2.3.0.2/cnocr/classification/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5430 2023-02-11 15:48:37.000000 cnocr-2.3.0.2/cnocr/classification/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     9801 2023-02-11 15:48:37.000000 cnocr-2.3.0.2/cnocr/classification/image_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     8314 2023-02-11 15:48:37.000000 cnocr-2.3.0.2/cnocr/clf_cli.py
+-rw-r--r--   0 king       (501) staff       (20)    20393 2024-01-01 13:45:43.000000 cnocr-2.3.0.2/cnocr/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    17853 2023-12-22 11:08:08.000000 cnocr-2.3.0.2/cnocr/cn_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13733 2024-04-10 13:51:17.000000 cnocr-2.3.0.2/cnocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.871117 cnocr-2.3.0.2/cnocr/data_utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2019-03-02 15:15:34.000000 cnocr-2.3.0.2/cnocr/data_utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4128 2023-02-11 15:48:37.000000 cnocr-2.3.0.2/cnocr/data_utils/aug.py
+-rw-r--r--   0 king       (501) staff       (20)     2221 2021-11-05 14:17:16.000000 cnocr-2.3.0.2/cnocr/data_utils/block_shuffle.py
+-rw-r--r--   0 king       (501) staff       (20)    14928 2023-12-17 02:01:02.000000 cnocr-2.3.0.2/cnocr/data_utils/transforms.py
+-rw-r--r--   0 king       (501) staff       (20)     4393 2021-08-26 09:54:36.000000 cnocr-2.3.0.2/cnocr/data_utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     6380 2023-12-17 02:23:32.000000 cnocr-2.3.0.2/cnocr/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     3931 2023-12-15 14:07:55.000000 cnocr-2.3.0.2/cnocr/dataset_utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8873 2023-09-21 08:44:57.000000 cnocr-2.3.0.2/cnocr/gradio_app.py
+-rw-r--r--   0 king       (501) staff       (20)     9676 2023-09-20 02:24:06.000000 cnocr-2.3.0.2/cnocr/gradio_app2.py
+-rw-r--r--   0 king       (501) staff       (20)    26570 2023-11-04 12:25:59.000000 cnocr-2.3.0.2/cnocr/label_cn.txt
+-rw-r--r--   0 king       (501) staff       (20)       19 2023-09-07 02:26:43.000000 cnocr-2.3.0.2/cnocr/label_number.txt
+-rwxr-xr-x   0 king       (501) staff       (20)     4596 2021-08-26 09:54:36.000000 cnocr-2.3.0.2/cnocr/line_split.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-11-05 14:17:16.000000 cnocr-2.3.0.2/cnocr/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.871879 cnocr-2.3.0.2/cnocr/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2021-08-26 09:54:36.000000 cnocr-2.3.0.2/cnocr/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     3788 2021-08-26 09:54:36.000000 cnocr-2.3.0.2/cnocr/models/ctc.py
+-rw-r--r--   0 king       (501) staff       (20)     5032 2021-11-05 14:17:16.000000 cnocr-2.3.0.2/cnocr/models/densenet.py
+-rw-r--r--   0 king       (501) staff       (20)     6877 2023-05-11 02:09:18.000000 cnocr-2.3.0.2/cnocr/models/mobilenet.py
+-rw-r--r--   0 king       (501) staff       (20)    12001 2023-12-22 09:32:41.000000 cnocr-2.3.0.2/cnocr/models/ocr_model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.872736 cnocr-2.3.0.2/cnocr/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)      222 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1782 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.873289 cnocr-2.3.0.2/cnocr/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     2088 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    26691 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    10242 2023-12-22 11:10:08.000000 cnocr-2.3.0.2/cnocr/ppocr/pp_recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)    20282 2023-12-26 09:01:47.000000 cnocr-2.3.0.2/cnocr/ppocr/utility.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.874166 cnocr-2.3.0.2/cnocr/ppocr/utils/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    33443 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/utils/chinese_cht_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)      190 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/utils/en_dict.txt
+-rw-r--r--   0 king       (501) staff       (20)    26249 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/cnocr/ppocr/utils/ppocr_keys_v1.txt
+-rw-r--r--   0 king       (501) staff       (20)    17227 2023-12-22 11:08:36.000000 cnocr-2.3.0.2/cnocr/recognizer.py
+-rw-r--r--   0 king       (501) staff       (20)     1797 2022-09-01 02:35:51.000000 cnocr-2.3.0.2/cnocr/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    13168 2023-11-06 12:37:09.000000 cnocr-2.3.0.2/cnocr/trainer.py
+-rw-r--r--   0 king       (501) staff       (20)    14898 2023-12-21 09:48:48.000000 cnocr-2.3.0.2/cnocr/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.869675 cnocr-2.3.0.2/cnocr.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    23173 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     1412 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       71 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-29 09:15:54.000000 cnocr-2.3.0.2/cnocr.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      294 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2024-04-10 14:13:05.000000 cnocr-2.3.0.2/cnocr.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-04-10 14:13:05.876450 cnocr-2.3.0.2/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3369 2023-12-15 14:09:20.000000 cnocr-2.3.0.2/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-10 14:13:05.875912 cnocr-2.3.0.2/tests/
+-rw-r--r--   0 king       (501) staff       (20)     9469 2023-12-22 11:11:59.000000 cnocr-2.3.0.2/tests/test_cnocr.py
+-rw-r--r--   0 king       (501) staff       (20)     1822 2023-09-19 11:58:02.000000 cnocr-2.3.0.2/tests/test_dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     4947 2021-11-05 14:17:16.000000 cnocr-2.3.0.2/tests/test_models.py
+-rw-r--r--   0 king       (501) staff       (20)     3102 2022-07-20 02:15:52.000000 cnocr-2.3.0.2/tests/test_ppocr.py
+-rw-r--r--   0 king       (501) staff       (20)     1298 2023-12-22 11:12:21.000000 cnocr-2.3.0.2/tests/test_pytorch.py
+-rw-r--r--   0 king       (501) staff       (20)     1705 2023-12-22 11:12:28.000000 cnocr-2.3.0.2/tests/test_trainer.py
+-rw-r--r--   0 king       (501) staff       (20)     5674 2023-09-23 15:24:13.000000 cnocr-2.3.0.2/tests/test_transforms.py
```

### Comparing `cnocr-2.3.0.1/LICENSE` & `cnocr-2.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/PKG-INFO` & `cnocr-2.3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.3.0.1
+Version: 2.3.0.2
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
@@ -28,14 +28,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
   <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
   <div>&nbsp;</div>
 
+[![Discord](https://img.shields.io/discord/1200765964434821260?label=Discord)](https://discord.gg/GgD87WM8Tf)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
 [![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR)
 [![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
 [![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
@@ -318,14 +319,24 @@
 
 > **Warning** 
 >
 > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
 
 
 
+### Docker Image
+
+可以从 [Docker Hub](https://hub.docker.com/u/breezedeus) 直接拉取已安装好 CnOCR 的镜像使用。
+
+```bash
+$ docker pull breezedeus/cnocr:latest
+```
+
+更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
+
 
 
 ## HTTP服务
 
 CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
 
 ```bash
@@ -425,22 +436,22 @@
 更多说明见：[可用模型](https://cnocr.readthedocs.io/zh/latest/models/)。
 
 | `rec_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                            | 是否支持竖排文字识别 |
 | ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ----------------------------------- | -------------------- |
 | **densenet_lite_136-gru** 🆕                                  | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_136-gru** 🆕                            | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_136-gru** 🆕                              | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
-| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
 | **densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104812055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104815055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104820055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **number-densenet_lite_136-fc** 🆕                            | √            | √         | cnocr        | 2.7 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
-| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
+| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | **number-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104055055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 55 M         | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | ch_PP-OCRv3                                                  | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字                | √                    |
 | ch_ppocr_mobile_v2.0                                         | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字                | √                    |
 | en_PP-OCRv3                                                  | X            | √         | ppocr        | 8.5 M        | **英文**、数字                      | √                    |
 | en_number_mobile_v2.0                                        | X            | √         | ppocr        | 1.8 M        | **英文**、数字                      | √                    |
 | chinese_cht_PP-OCRv3                                         | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字            | X                    |
```

### Comparing `cnocr-2.3.0.1/README.md` & `cnocr-2.3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <div align="center">
   <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
   <div>&nbsp;</div>
 
+[![Discord](https://img.shields.io/discord/1200765964434821260?label=Discord)](https://discord.gg/GgD87WM8Tf)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
 [![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR)
 [![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
 [![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
@@ -288,14 +289,24 @@
 
 > **Warning** 
 >
 > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
 
 
 
+### Docker Image
+
+可以从 [Docker Hub](https://hub.docker.com/u/breezedeus) 直接拉取已安装好 CnOCR 的镜像使用。
+
+```bash
+$ docker pull breezedeus/cnocr:latest
+```
+
+更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
+
 
 
 ## HTTP服务
 
 CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
 
 ```bash
@@ -395,22 +406,22 @@
 更多说明见：[可用模型](https://cnocr.readthedocs.io/zh/latest/models/)。
 
 | `rec_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                            | 是否支持竖排文字识别 |
 | ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ----------------------------------- | -------------------- |
 | **densenet_lite_136-gru** 🆕                                  | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_136-gru** 🆕                            | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_136-gru** 🆕                              | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
-| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
 | **densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104812055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104815055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104820055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **number-densenet_lite_136-fc** 🆕                            | √            | √         | cnocr        | 2.7 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
-| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
+| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | **number-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104055055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 55 M         | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | ch_PP-OCRv3                                                  | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字                | √                    |
 | ch_ppocr_mobile_v2.0                                         | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字                | √                    |
 | en_PP-OCRv3                                                  | X            | √         | ppocr        | 8.5 M        | **英文**、数字                      | √                    |
 | en_number_mobile_v2.0                                        | X            | √         | ppocr        | 1.8 M        | **英文**、数字                      | √                    |
 | chinese_cht_PP-OCRv3                                         | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字            | X                    |
```

### Comparing `cnocr-2.3.0.1/cnocr/__init__.py` & `cnocr-2.3.0.2/cnocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/__version__.py` & `cnocr-2.3.0.2/cnocr/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '2.3.0.1'
+__version__ = '2.3.0.2'
```

### Comparing `cnocr-2.3.0.1/cnocr/app.py` & `cnocr-2.3.0.2/cnocr/app.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/classification/__init__.py` & `cnocr-2.3.0.2/cnocr/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/classification/dataset.py` & `cnocr-2.3.0.2/cnocr/classification/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/classification/image_classifier.py` & `cnocr-2.3.0.2/cnocr/classification/image_classifier.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/clf_cli.py` & `cnocr-2.3.0.2/cnocr/clf_cli.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/cli.py` & `cnocr-2.3.0.2/cnocr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,17 @@
 @click.option(
     '--det-model-backend',
     type=click.Choice(['pytorch', 'onnx']),
     default='onnx',
     help='检测模型类型。默认值为 `onnx`',
 )
 @click.option(
+    '--det-resized-shape', type=int, default=768, help='检测模型输入图像尺寸。默认值为 768',
+)
+@click.option(
     '-p',
     '--pretrained-model-fp',
     type=str,
     default=None,
     help='识别模型使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型',
 )
 @click.option(
@@ -248,28 +251,33 @@
 @click.option(
     "--draw-results-dir", default=None, help="画出的检测与识别效果图所存放的目录；取值为 `None` 表示不画图",
 )
 @click.option(
     "--draw-font-path", default='./docs/fonts/simfang.ttf', help="画出检测与识别效果图时使用的字体文件",
 )
 @click.option(
+    "--show-details", is_flag=True, default=False, help="是否打印识别结果详情。默认值为 `False`",
+)
+@click.option(
     "--verbose", is_flag=True, default=False, help="是否打印详细日志信息。默认值为 `False`",
 )
 def predict(
     rec_model_name,
     rec_model_backend,
     rec_vocab_fp,
     det_model_name,
     det_model_backend,
+    det_resized_shape,
     pretrained_model_fp,
     context,
     img_file_or_dir,
     single_line,
     draw_results_dir,
     draw_font_path,
+    show_details,
     verbose,
 ):
     """模型预测""",
     if verbose:
         logger = set_logger(log_level=logging.DEBUG)
     else:
         logger = set_logger(log_level=logging.INFO)
@@ -294,26 +302,32 @@
         det_model_name=det_model_name,
         det_model_backend=det_model_backend,
         rec_model_fp=pretrained_model_fp,
         context=context,
         # det_more_configs={'rotated_bbox': False},
     )
     ocr_func = ocr.ocr_for_single_line if single_line else ocr.ocr
+    ocr_kwargs = {}
+    if not single_line:
+        ocr_kwargs['resized_shape'] = det_resized_shape
 
     for fp in fp_list:
         start_time = time.time()
         logger.info('\n' + '=' * 10 + fp + '=' * 10)
         res = ocr_func(
             fp,
-            # resized_shape=2280,
+            **ocr_kwargs,
             # box_score_thresh=0.14,
             # min_box_size=20,
         )
         logger.info('time cost: %f' % (time.time() - start_time))
-        logger.info(res)
+        if show_details:
+            logger.info(res)
+        else:
+            logger.info('\n'.join([line_res['text'] for line_res in res]))
         if single_line:
             res = [res]
 
         if not single_line and draw_results_dir is not None:
             if not os.path.isfile(draw_font_path):
                 logger.error(
                     'can not find the font file {}, so stop drawing ocr results'.format(
@@ -325,18 +339,14 @@
                 out_draw_fp = os.path.join(
                     draw_results_dir, os.path.basename(fp) + '-result.jpg'
                 )
                 draw_ocr_results(
                     fp, res, out_draw_fp=out_draw_fp, font_path=draw_font_path
                 )
 
-        # for line_res in res:
-        #     preds, prob = line_res['text'], line_res['score']
-        #     logger.info('\npred: %s, with score %f' % (''.join(preds), prob))
-
 
 @cli.command('evaluate')
 @click.option(
     '-m',
     '--rec-model-name',
     type=str,
     default=DEFAULT_MODEL_NAME,
```

### Comparing `cnocr-2.3.0.1/cnocr/cn_ocr.py` & `cnocr-2.3.0.2/cnocr/cn_ocr.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/consts.py` & `cnocr-2.3.0.2/cnocr/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 # 模型版本只对应到第二层，第三层的改动表示模型兼容。
 # 如: __version__ = '2.2.*'，对应的 MODEL_VERSION 都是 '2.2'
 MODEL_VERSION = '.'.join(__version__.split('.', maxsplit=2)[:2])
-DOWNLOAD_SOURCE = os.environ.get('CNOCR_DOWNLOAD_SOURCE', 'CN')
+DOWNLOAD_SOURCE = os.environ.get('CNOCR_DOWNLOAD_SOURCE', 'HF')
 
 IMG_STANDARD_HEIGHT = 32
 CN_VOCAB_FP = Path(__file__).parent.absolute() / 'label_cn.txt'
 NUMBER_VOCAB_FP = Path(__file__).parent.absolute() / 'label_number.txt'
 
 ENCODER_CONFIGS = {
     'densenet': {  # 长度压缩至 1/8（seq_len == 35），输出的向量长度为 4*128 = 512
```

### Comparing `cnocr-2.3.0.1/cnocr/data_utils/aug.py` & `cnocr-2.3.0.2/cnocr/data_utils/aug.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/data_utils/block_shuffle.py` & `cnocr-2.3.0.2/cnocr/data_utils/block_shuffle.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/data_utils/transforms.py` & `cnocr-2.3.0.2/cnocr/data_utils/transforms.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/data_utils/utils.py` & `cnocr-2.3.0.2/cnocr/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/dataset.py` & `cnocr-2.3.0.2/cnocr/dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/dataset_utils.py` & `cnocr-2.3.0.2/cnocr/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/gradio_app.py` & `cnocr-2.3.0.2/cnocr/gradio_app.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/gradio_app2.py` & `cnocr-2.3.0.2/cnocr/gradio_app2.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/label_cn.txt` & `cnocr-2.3.0.2/cnocr/label_cn.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/line_split.py` & `cnocr-2.3.0.2/cnocr/line_split.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/lr_scheduler.py` & `cnocr-2.3.0.2/cnocr/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/models/ctc.py` & `cnocr-2.3.0.2/cnocr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/models/densenet.py` & `cnocr-2.3.0.2/cnocr/models/densenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/models/mobilenet.py` & `cnocr-2.3.0.2/cnocr/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/models/ocr_model.py` & `cnocr-2.3.0.2/cnocr/models/ocr_model.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/consts.py` & `cnocr-2.3.0.2/cnocr/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/postprocess/__init__.py` & `cnocr-2.3.0.2/cnocr/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/postprocess/rec_postprocess.py` & `cnocr-2.3.0.2/cnocr/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/pp_recognizer.py` & `cnocr-2.3.0.2/cnocr/ppocr/pp_recognizer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/utility.py` & `cnocr-2.3.0.2/cnocr/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/utils/chinese_cht_dict.txt` & `cnocr-2.3.0.2/cnocr/ppocr/utils/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/ppocr/utils/ppocr_keys_v1.txt` & `cnocr-2.3.0.2/cnocr/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/recognizer.py` & `cnocr-2.3.0.2/cnocr/recognizer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/serve.py` & `cnocr-2.3.0.2/cnocr/serve.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/trainer.py` & `cnocr-2.3.0.2/cnocr/trainer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr/utils.py` & `cnocr-2.3.0.2/cnocr/utils.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/cnocr.egg-info/PKG-INFO` & `cnocr-2.3.0.2/cnocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnocr
-Version: 2.3.0.1
+Version: 2.3.0.2
 Summary: Python3 package for Chinese/English OCR, with small pretrained models
 Home-page: https://github.com/breezedeus/cnocr
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
@@ -28,14 +28,15 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
   <img src="./docs/figs/cnocr-logo.jpg" width="250px"/>
   <div>&nbsp;</div>
 
+[![Discord](https://img.shields.io/discord/1200765964434821260?label=Discord)](https://discord.gg/GgD87WM8Tf)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnocr?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/cnocr)
 [![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR&label=Visitors&countColor=%23f5c791&style=flat&labelStyle=none)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fbreezedeus%2FCnOCR)
 [![license](https://img.shields.io/github/license/breezedeus/cnocr)](./LICENSE)
 [![Docs](https://readthedocs.org/projects/cnocr/badge/?version=latest)](https://cnocr.readthedocs.io/zh/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/cnocr.svg)](https://badge.fury.io/py/cnocr)
 [![forks](https://img.shields.io/github/forks/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
 [![stars](https://img.shields.io/github/stars/breezedeus/cnocr)](https://github.com/breezedeus/cnocr)
@@ -318,14 +319,24 @@
 
 > **Warning** 
 >
 > 如果电脑中从未安装过 `PyTorch`，`OpenCV` python包，初次安装可能会遇到问题，但一般都是常见问题，可以自行百度/Google解决。
 
 
 
+### Docker Image
+
+可以从 [Docker Hub](https://hub.docker.com/u/breezedeus) 直接拉取已安装好 CnOCR 的镜像使用。
+
+```bash
+$ docker pull breezedeus/cnocr:latest
+```
+
+更多说明可见 [安装文档](https://cnocr.readthedocs.io/zh/latest/install/)。
+
 
 
 ## HTTP服务
 
 CnOCR **V2.2.1** 加入了基于 FastAPI 的HTTP服务。开启服务需要安装几个额外的包，可以使用以下命令安装：
 
 ```bash
@@ -425,22 +436,22 @@
 更多说明见：[可用模型](https://cnocr.readthedocs.io/zh/latest/models/)。
 
 | `rec_model_name`                                             | PyTorch 版本 | ONNX 版本 | 模型原始来源 | 模型文件大小 | 支持语言                            | 是否支持竖排文字识别 |
 | ------------------------------------------------------------ | ------------ | --------- | ------------ | ------------ | ----------------------------------- | -------------------- |
 | **densenet_lite_136-gru** 🆕                                  | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_136-gru** 🆕                            | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_136-gru** 🆕                              | √            | √         | cnocr        | 12 M         | 简体中文、英文、数字                | X                    |
-| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
-| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **scene-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
+| **doc-densenet_lite_246-gru_base** 🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 25 M         | 简体中文、英文、数字                | X                    |
 | **densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104812055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **scene-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104815055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **doc-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104820055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 82 M         | 简体中文、英文、数字                | X                    |
 | **number-densenet_lite_136-fc** 🆕                            | √            | √         | cnocr        | 2.7 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
-| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享，2 月开源) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
+| **number-densenet_lite_136-gru**  🆕 <br /> ([星球会员](https://t.zsxq.com/FEYZRJQ)专享) | √            | √         | cnocr        | 5.5 M        | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | **number-densenet_lite_666-gru_large** 🆕 <br />（购买链接：[B站](https://gf.bilibili.com/item/detail/1104055055)、[Lemon Squeezy](https://ocr.lemonsqueezy.com/)） | √            | √         | cnocr        | 55 M         | **纯数字**（仅包含 `0~9` 十个数字） | X                    |
 | ch_PP-OCRv3                                                  | X            | √         | ppocr        | 10 M         | 简体中文、英文、数字                | √                    |
 | ch_ppocr_mobile_v2.0                                         | X            | √         | ppocr        | 4.2 M        | 简体中文、英文、数字                | √                    |
 | en_PP-OCRv3                                                  | X            | √         | ppocr        | 8.5 M        | **英文**、数字                      | √                    |
 | en_number_mobile_v2.0                                        | X            | √         | ppocr        | 1.8 M        | **英文**、数字                      | √                    |
 | chinese_cht_PP-OCRv3                                         | X            | √         | ppocr        | 11 M         | **繁体中文**、英文、数字            | X                    |
```

### Comparing `cnocr-2.3.0.1/cnocr.egg-info/SOURCES.txt` & `cnocr-2.3.0.2/cnocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/setup.py` & `cnocr-2.3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_cnocr.py` & `cnocr-2.3.0.2/tests/test_cnocr.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_dataset.py` & `cnocr-2.3.0.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_models.py` & `cnocr-2.3.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_ppocr.py` & `cnocr-2.3.0.2/tests/test_ppocr.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_pytorch.py` & `cnocr-2.3.0.2/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_trainer.py` & `cnocr-2.3.0.2/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `cnocr-2.3.0.1/tests/test_transforms.py` & `cnocr-2.3.0.2/tests/test_transforms.py`

 * *Files identical despite different names*

