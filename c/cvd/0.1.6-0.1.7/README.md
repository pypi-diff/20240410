# Comparing `tmp/cvd-0.1.6.tar.gz` & `tmp/cvd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvd-0.1.6.tar", max compression
+gzip compressed data, was "cvd-0.1.7.tar", max compression
```

## Comparing `cvd-0.1.6.tar` & `cvd-0.1.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0       12 2022-01-11 02:40:18.707451 cvd-0.1.6/README.md
--rw-r--r--   0        0        0       36 2023-04-25 10:27:33.418009 cvd-0.1.6/cvd/.uuid
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/__init__.py
--rw-r--r--   0        0        0      140 2022-12-12 04:16:54.905072 cvd-0.1.6/cvd/datasets/annotations/__init__.py
--rw-r--r--   0        0        0     1072 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/annotations/coco.py
--rw-r--r--   0        0        0     4584 2024-03-22 12:21:52.442709 cvd-0.1.6/cvd/datasets/annotations/image_annotation.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/annotations/importer/__init__.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/annotations/importer/images/__init__.py
--rw-r--r--   0        0        0     2781 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/annotations/importer/images/cvat.py
--rw-r--r--   0        0        0     5947 2022-10-05 14:59:10.579225 cvd-0.1.6/cvd/datasets/annotations/importer/images/toloka.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/annotations/importer/video/__init__.py
--rw-r--r--   0        0        0     5086 2024-03-04 12:25:54.880344 cvd-0.1.6/cvd/datasets/annotations/importer/video/cvat.py
--rw-r--r--   0        0        0    11617 2022-10-04 03:05:34.336960 cvd-0.1.6/cvd/datasets/annotations/objects.py
--rw-r--r--   0        0        0     2024 2022-10-11 04:27:56.519226 cvd-0.1.6/cvd/datasets/annotations/polygon.py
--rw-r--r--   0        0        0     5588 2023-01-09 09:02:52.091752 cvd-0.1.6/cvd/datasets/annotations/rbbox.py
--rw-r--r--   0        0        0     7973 2024-03-22 08:56:13.101898 cvd-0.1.6/cvd/datasets/annotations/sbbox.py
--rw-r--r--   0        0        0      643 2022-09-28 07:54:57.799412 cvd-0.1.6/cvd/datasets/annotations/type.py
--rw-r--r--   0        0        0     8714 2022-09-28 12:34:08.547768 cvd-0.1.6/cvd/datasets/annotations/video_annotation.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/augumentation/__init__.py
--rw-r--r--   0        0        0     1624 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/augumentation/crop.py
--rw-r--r--   0        0        0     8495 2022-09-28 12:34:44.679781 cvd-0.1.6/cvd/datasets/augumentation/filters.py
--rw-r--r--   0        0        0     1150 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/augumentation/flip.py
--rw-r--r--   0        0        0     1427 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/augumentation/rotate.py
--rw-r--r--   0        0        0     4254 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/augumentation/utils.py
--rw-r--r--   0        0        0       96 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/autoannotation/__init__.py
--rw-r--r--   0        0        0     1329 2022-12-12 04:16:31.600995 cvd-0.1.6/cvd/datasets/autoannotation/iautoannotator.py
--rw-r--r--   0        0        0     1451 2022-09-28 12:35:08.531789 cvd-0.1.6/cvd/datasets/autoannotation/retinafaceannotator.py
--rw-r--r--   0        0        0     6894 2022-09-28 12:35:03.079787 cvd-0.1.6/cvd/datasets/autoannotation/topbodyannotator.py
--rw-r--r--   0        0        0       65 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/common.py
--rw-r--r--   0        0        0     1838 2022-10-21 02:05:04.859931 cvd-0.1.6/cvd/datasets/converters.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/exporter/__init__.py
--rw-r--r--   0        0        0     8021 2022-09-28 12:27:26.759641 cvd-0.1.6/cvd/datasets/exporter/xml.py
--rw-r--r--   0        0        0     1710 2022-09-28 12:37:56.483849 cvd-0.1.6/cvd/datasets/filters.py
--rw-r--r--   0        0        0    20957 2023-01-24 06:27:25.298499 cvd-0.1.6/cvd/datasets/image_dataset.py
--rw-r--r--   0        0        0     1755 2023-02-15 06:01:38.717850 cvd-0.1.6/cvd/datasets/image_dataset_item.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/importer/__init__.py
--rw-r--r--   0        0        0     3008 2024-03-15 08:59:24.200843 cvd-0.1.6/cvd/datasets/importer/cocoimages.py
--rw-r--r--   0        0        0     2746 2022-12-12 04:14:18.736557 cvd-0.1.6/cvd/datasets/importer/rawimages.py
--rw-r--r--   0        0        0     2765 2023-03-09 05:48:06.123605 cvd-0.1.6/cvd/datasets/importer/rawvideo.py
--rw-r--r--   0        0        0       71 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/interfaces/__init__.py
--rw-r--r--   0        0        0      293 2022-09-28 12:37:56.327849 cvd-0.1.6/cvd/datasets/interfaces/iannotation.py
--rw-r--r--   0        0        0     3410 2024-03-21 10:34:39.476209 cvd-0.1.6/cvd/datasets/interfaces/idataset.py
--rw-r--r--   0        0        0      830 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/interfaces/interface.py
--rw-r--r--   0        0        0      502 2022-09-28 12:37:56.727849 cvd-0.1.6/cvd/datasets/merge.py
--rw-r--r--   0        0        0     6138 2022-10-10 08:12:47.752858 cvd-0.1.6/cvd/datasets/meta.py
--rw-r--r--   0        0        0        0 2023-01-20 09:31:09.015784 cvd-0.1.6/cvd/datasets/samplers.py
--rw-r--r--   0        0        0     1046 2022-10-04 05:32:12.321576 cvd-0.1.6/cvd/datasets/selection.py
--rw-r--r--   0        0        0     9568 2024-03-22 11:03:35.425577 cvd-0.1.6/cvd/datasets/torchdataset.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/transformations/__init__.py
--rw-r--r--   0        0        0      774 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/transformations/normalize.py
--rw-r--r--   0        0        0     2980 2022-10-21 03:32:31.588931 cvd-0.1.6/cvd/datasets/transformations/resize.py
--rw-r--r--   0        0        0     8811 2023-01-16 10:09:44.443886 cvd-0.1.6/cvd/datasets/transformers.py
--rw-r--r--   0        0        0    14982 2022-10-04 10:34:35.409280 cvd-0.1.6/cvd/datasets/video_dataset.py
--rw-r--r--   0        0        0     4256 2023-01-09 10:07:30.993442 cvd-0.1.6/cvd/datasets/video_dataset_item.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/__init__.py
--rw-r--r--   0        0        0    15045 2022-12-12 13:20:15.945724 cvd-0.1.6/cvd/datasets/zoo/datasets.py
--rw-r--r--   0        0        0     4087 2022-09-28 08:00:15.303375 cvd-0.1.6/cvd/datasets/zoo/internal_representation.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/__init__.py
--rw-r--r--   0        0        0     3922 2022-12-12 08:54:14.593767 cvd-0.1.6/cvd/datasets/zoo/raw/cepdof.py
--rw-r--r--   0        0        0     4799 2023-01-16 10:41:16.094113 cvd-0.1.6/cvd/datasets/zoo/raw/coco.py
--rw-r--r--   0        0        0     4495 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/crowdhuman.py
--rw-r--r--   0        0        0     3787 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/feeds.py
--rw-r--r--   0        0        0     3664 2022-12-12 07:01:01.528106 cvd-0.1.6/cvd/datasets/zoo/raw/habbof.py
--rw-r--r--   0        0        0     3144 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/mirrorworlds.py
--rw-r--r--   0        0        0     3886 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/mirrorworldsrotated.py
--rw-r--r--   0        0        0     4311 2022-12-12 08:54:31.373813 cvd-0.1.6/cvd/datasets/zoo/raw/mwr.py
--rw-r--r--   0        0        0     3692 2022-12-12 09:08:24.476689 cvd-0.1.6/cvd/datasets/zoo/raw/wepdtof.py
--rw-r--r--   0        0        0     5000 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/widerface.py
--rw-r--r--   0        0        0     3603 2022-09-12 07:30:32.634812 cvd-0.1.6/cvd/datasets/zoo/raw/widerperson.py
--rw-r--r--   0        0        0        0 2021-09-07 04:04:24.000000 cvd-0.1.6/cvd/models/__init__.py
--rw-r--r--   0        0        0     3834 2023-02-03 02:55:13.257830 cvd-0.1.6/cvd/models/interface.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/tools/__init__.py
--rw-r--r--   0        0        0      252 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/tools/hash.py
--rw-r--r--   0        0        0      501 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/tools/logger.py
--rw-r--r--   0        0        0     8519 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/tools/perception_benchmarks.py
--rw-r--r--   0        0        0     3280 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/tools/s3.py
--rw-r--r--   0        0        0        0 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/visualization/__init__.py
--rw-r--r--   0        0        0     1916 2023-01-20 02:56:08.689755 cvd-0.1.6/cvd/visualization/annotations.py
--rw-r--r--   0        0        0     3041 2023-01-20 06:00:32.843567 cvd-0.1.6/cvd/visualization/dataset.py
--rw-r--r--   0        0        0     3010 2023-02-03 02:48:31.665244 cvd-0.1.6/cvd/visualization/objects.py
--rw-r--r--   0        0        0     1081 2022-10-04 10:33:13.369245 cvd-0.1.6/cvd/visualization/tools.py
--rw-r--r--   0        0        0       52 2022-09-12 07:30:32.714812 cvd-0.1.6/cvd/visualization/type.py
--rw-r--r--   0        0        0      616 2024-03-25 11:50:00.547359 cvd-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 cvd-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       12 2022-01-11 02:40:18.707451 cvd-0.1.7/README.md
+-rw-r--r--   0        0        0       36 2023-04-25 10:27:33.418009 cvd-0.1.7/cvd/.uuid
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/__init__.py
+-rw-r--r--   0        0        0      140 2022-12-12 04:16:54.905072 cvd-0.1.7/cvd/datasets/annotations/__init__.py
+-rw-r--r--   0        0        0     1072 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/annotations/coco.py
+-rw-r--r--   0        0        0     4663 2024-04-01 15:22:08.274940 cvd-0.1.7/cvd/datasets/annotations/image_annotation.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/annotations/importer/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/annotations/importer/images/__init__.py
+-rw-r--r--   0        0        0     2781 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/annotations/importer/images/cvat.py
+-rw-r--r--   0        0        0     5947 2022-10-05 14:59:10.579225 cvd-0.1.7/cvd/datasets/annotations/importer/images/toloka.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/annotations/importer/video/__init__.py
+-rw-r--r--   0        0        0     5086 2024-03-28 15:12:20.041458 cvd-0.1.7/cvd/datasets/annotations/importer/video/cvat.py
+-rw-r--r--   0        0        0    11617 2022-10-04 03:05:34.336960 cvd-0.1.7/cvd/datasets/annotations/objects.py
+-rw-r--r--   0        0        0     2024 2022-10-11 04:27:56.519226 cvd-0.1.7/cvd/datasets/annotations/polygon.py
+-rw-r--r--   0        0        0     5588 2023-01-09 09:02:52.091752 cvd-0.1.7/cvd/datasets/annotations/rbbox.py
+-rw-r--r--   0        0        0     8020 2024-04-01 15:37:15.511555 cvd-0.1.7/cvd/datasets/annotations/sbbox.py
+-rw-r--r--   0        0        0      643 2022-09-28 07:54:57.799412 cvd-0.1.7/cvd/datasets/annotations/type.py
+-rw-r--r--   0        0        0     8714 2022-09-28 12:34:08.547768 cvd-0.1.7/cvd/datasets/annotations/video_annotation.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/augumentation/__init__.py
+-rw-r--r--   0        0        0     1624 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/augumentation/crop.py
+-rw-r--r--   0        0        0     8495 2022-09-28 12:34:44.679781 cvd-0.1.7/cvd/datasets/augumentation/filters.py
+-rw-r--r--   0        0        0     1150 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/augumentation/flip.py
+-rw-r--r--   0        0        0     1427 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/augumentation/rotate.py
+-rw-r--r--   0        0        0     4254 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/augumentation/utils.py
+-rw-r--r--   0        0        0       96 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/autoannotation/__init__.py
+-rw-r--r--   0        0        0     1329 2022-12-12 04:16:31.600995 cvd-0.1.7/cvd/datasets/autoannotation/iautoannotator.py
+-rw-r--r--   0        0        0     1451 2022-09-28 12:35:08.531789 cvd-0.1.7/cvd/datasets/autoannotation/retinafaceannotator.py
+-rw-r--r--   0        0        0     6894 2022-09-28 12:35:03.079787 cvd-0.1.7/cvd/datasets/autoannotation/topbodyannotator.py
+-rw-r--r--   0        0        0       65 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/common.py
+-rw-r--r--   0        0        0     2030 2024-03-29 05:32:52.932540 cvd-0.1.7/cvd/datasets/converters.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/exporter/__init__.py
+-rw-r--r--   0        0        0     8086 2024-04-02 12:41:34.348472 cvd-0.1.7/cvd/datasets/exporter/xml.py
+-rw-r--r--   0        0        0     1710 2022-09-28 12:37:56.483849 cvd-0.1.7/cvd/datasets/filters.py
+-rw-r--r--   0        0        0    21791 2024-04-02 11:29:30.116384 cvd-0.1.7/cvd/datasets/image_dataset.py
+-rw-r--r--   0        0        0     1755 2023-02-15 06:01:38.717850 cvd-0.1.7/cvd/datasets/image_dataset_item.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/importer/__init__.py
+-rw-r--r--   0        0        0     3008 2024-03-15 08:59:24.200843 cvd-0.1.7/cvd/datasets/importer/cocoimages.py
+-rw-r--r--   0        0        0     2746 2022-12-12 04:14:18.736557 cvd-0.1.7/cvd/datasets/importer/rawimages.py
+-rw-r--r--   0        0        0     2765 2023-03-09 05:48:06.123605 cvd-0.1.7/cvd/datasets/importer/rawvideo.py
+-rw-r--r--   0        0        0       71 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/interfaces/__init__.py
+-rw-r--r--   0        0        0      293 2022-09-28 12:37:56.327849 cvd-0.1.7/cvd/datasets/interfaces/iannotation.py
+-rw-r--r--   0        0        0     3409 2024-03-28 15:16:55.018403 cvd-0.1.7/cvd/datasets/interfaces/idataset.py
+-rw-r--r--   0        0        0      830 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/interfaces/interface.py
+-rw-r--r--   0        0        0      502 2022-09-28 12:37:56.727849 cvd-0.1.7/cvd/datasets/merge.py
+-rw-r--r--   0        0        0     6138 2022-10-10 08:12:47.752858 cvd-0.1.7/cvd/datasets/meta.py
+-rw-r--r--   0        0        0        0 2023-01-20 09:31:09.015784 cvd-0.1.7/cvd/datasets/samplers.py
+-rw-r--r--   0        0        0     1046 2022-10-04 05:32:12.321576 cvd-0.1.7/cvd/datasets/selection.py
+-rw-r--r--   0        0        0     9568 2024-03-22 11:03:35.425577 cvd-0.1.7/cvd/datasets/torchdataset.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/transformations/__init__.py
+-rw-r--r--   0        0        0      774 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/transformations/normalize.py
+-rw-r--r--   0        0        0     2980 2022-10-21 03:32:31.588931 cvd-0.1.7/cvd/datasets/transformations/resize.py
+-rw-r--r--   0        0        0     8836 2024-04-10 04:08:20.791423 cvd-0.1.7/cvd/datasets/transformers.py
+-rw-r--r--   0        0        0    14982 2024-03-28 15:16:48.194385 cvd-0.1.7/cvd/datasets/video_dataset.py
+-rw-r--r--   0        0        0     4324 2024-03-29 05:17:30.521609 cvd-0.1.7/cvd/datasets/video_dataset_item.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/__init__.py
+-rw-r--r--   0        0        0    15045 2022-12-12 13:20:15.945724 cvd-0.1.7/cvd/datasets/zoo/datasets.py
+-rw-r--r--   0        0        0     4087 2022-09-28 08:00:15.303375 cvd-0.1.7/cvd/datasets/zoo/internal_representation.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/__init__.py
+-rw-r--r--   0        0        0     3922 2022-12-12 08:54:14.593767 cvd-0.1.7/cvd/datasets/zoo/raw/cepdof.py
+-rw-r--r--   0        0        0     4799 2023-01-16 10:41:16.094113 cvd-0.1.7/cvd/datasets/zoo/raw/coco.py
+-rw-r--r--   0        0        0     4495 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/crowdhuman.py
+-rw-r--r--   0        0        0     3787 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/feeds.py
+-rw-r--r--   0        0        0     3664 2022-12-12 07:01:01.528106 cvd-0.1.7/cvd/datasets/zoo/raw/habbof.py
+-rw-r--r--   0        0        0     3144 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/mirrorworlds.py
+-rw-r--r--   0        0        0     3886 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/mirrorworldsrotated.py
+-rw-r--r--   0        0        0     4311 2022-12-12 08:54:31.373813 cvd-0.1.7/cvd/datasets/zoo/raw/mwr.py
+-rw-r--r--   0        0        0     3692 2022-12-12 09:08:24.476689 cvd-0.1.7/cvd/datasets/zoo/raw/wepdtof.py
+-rw-r--r--   0        0        0     5000 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/widerface.py
+-rw-r--r--   0        0        0     3603 2022-09-12 07:30:32.634812 cvd-0.1.7/cvd/datasets/zoo/raw/widerperson.py
+-rw-r--r--   0        0        0        0 2021-09-07 04:04:24.000000 cvd-0.1.7/cvd/models/__init__.py
+-rw-r--r--   0        0        0     3834 2023-02-03 02:55:13.257830 cvd-0.1.7/cvd/models/interface.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/tools/__init__.py
+-rw-r--r--   0        0        0      252 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/tools/hash.py
+-rw-r--r--   0        0        0      501 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/tools/logger.py
+-rw-r--r--   0        0        0     8519 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/tools/perception_benchmarks.py
+-rw-r--r--   0        0        0     3280 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/tools/s3.py
+-rw-r--r--   0        0        0        0 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/visualization/__init__.py
+-rw-r--r--   0        0        0     1916 2023-01-20 02:56:08.689755 cvd-0.1.7/cvd/visualization/annotations.py
+-rw-r--r--   0        0        0     3041 2023-01-20 06:00:32.843567 cvd-0.1.7/cvd/visualization/dataset.py
+-rw-r--r--   0        0        0     3010 2023-02-03 02:48:31.665244 cvd-0.1.7/cvd/visualization/objects.py
+-rw-r--r--   0        0        0     1081 2022-10-04 10:33:13.369245 cvd-0.1.7/cvd/visualization/tools.py
+-rw-r--r--   0        0        0       52 2022-09-12 07:30:32.714812 cvd-0.1.7/cvd/visualization/type.py
+-rw-r--r--   0        0        0      616 2024-04-10 04:09:33.323494 cvd-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 cvd-0.1.7/PKG-INFO
```

### Comparing `cvd-0.1.6/cvd/datasets/annotations/coco.py` & `cvd-0.1.7/cvd/datasets/annotations/coco.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/image_annotation.py` & `cvd-0.1.7/cvd/datasets/annotations/image_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         if objects:
             self.check_objects_type(objects)
             self._objects = tuple(itertools.chain(self._objects, objects))
             self._labels = tuple(set([obj.label for obj in self._objects]))
             self._markup_type = self.get_markup_type()
 
     def check_objects_type(self, objects):
+        # TODO investigate is nessesary to check bbox_type
+        return True
         if not bool(objects):
             return
 
         if not self.is_empty():
             obj_type = type(self._objects[0])
             bbox_type = type(self._objects[0].bbox) if self.obj_type_is_bbox(self._objects[0]) else None
         else:
```

### Comparing `cvd-0.1.6/cvd/datasets/annotations/importer/images/cvat.py` & `cvd-0.1.7/cvd/datasets/annotations/importer/images/cvat.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/importer/images/toloka.py` & `cvd-0.1.7/cvd/datasets/annotations/importer/images/toloka.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/importer/video/cvat.py` & `cvd-0.1.7/cvd/datasets/annotations/importer/video/cvat.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/objects.py` & `cvd-0.1.7/cvd/datasets/annotations/objects.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/polygon.py` & `cvd-0.1.7/cvd/datasets/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/rbbox.py` & `cvd-0.1.7/cvd/datasets/annotations/rbbox.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/sbbox.py` & `cvd-0.1.7/cvd/datasets/annotations/sbbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         return BBoxXYXY(
             xmin=float(tag.attrib['xtl']),
             ymin=float(tag.attrib['ytl']),
             xmax=float(tag.attrib['xbr']),
             ymax=float(tag.attrib['ybr'])
         )
 
+    def toxyxy(self):
+        return self
+    
     def toxywh(self):
         return BBoxXYWH(
             x=self.xmin,
             y=self.ymin,
             width=self.xmax - self.xmin,
             height=self.ymax - self.ymin
         )
```

### Comparing `cvd-0.1.6/cvd/datasets/annotations/type.py` & `cvd-0.1.7/cvd/datasets/annotations/type.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/annotations/video_annotation.py` & `cvd-0.1.7/cvd/datasets/annotations/video_annotation.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/augumentation/crop.py` & `cvd-0.1.7/cvd/datasets/augumentation/crop.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/augumentation/filters.py` & `cvd-0.1.7/cvd/datasets/augumentation/filters.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/augumentation/flip.py` & `cvd-0.1.7/cvd/datasets/augumentation/flip.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/augumentation/rotate.py` & `cvd-0.1.7/cvd/datasets/augumentation/rotate.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/augumentation/utils.py` & `cvd-0.1.7/cvd/datasets/augumentation/utils.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/autoannotation/iautoannotator.py` & `cvd-0.1.7/cvd/datasets/autoannotation/iautoannotator.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/autoannotation/retinafaceannotator.py` & `cvd-0.1.7/cvd/datasets/autoannotation/retinafaceannotator.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/autoannotation/topbodyannotator.py` & `cvd-0.1.7/cvd/datasets/autoannotation/topbodyannotator.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/exporter/xml.py` & `cvd-0.1.7/cvd/datasets/exporter/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from copy import deepcopy
 from distutils.util import strtobool
 from pathlib import Path
 from typing import List, Any, Union
 from xml.etree.ElementTree import Element
 
 from cvd.datasets.annotations.image_annotation import ImageAnnotation
-from cvd.datasets.annotations.objects import DetectionObjectBBox, TrackGTObjectBBox, TrackGTObjectPolygon, \
-    DetectionObjectPolygon
+from cvd.datasets.annotations.objects import DetectionObjectBBox, TrackGTObjectBBox, \
+    TrackGTObjectPolygon, \
+    DetectionObjectPolygon, PredictedObject
 from cvd.datasets.annotations.polygon import Polygon
 from cvd.datasets.annotations.rbbox import RBBoxXYCenterWHA
 from cvd.datasets.annotations.sbbox import BBoxXYXY
 from cvd.datasets.annotations.video_annotation import VideoAnnotation, Frame
 from cvd.datasets.image_dataset import ImagesDataset
 from bs4 import BeautifulSoup
 
@@ -27,17 +28,18 @@
     'video_dataset': VideoDataset,
     'file_info': FileInfo,
     'image_file_info': ImageFileInfo,
     'video_file_info': VideoFileInfo,
     'image_annotation': ImageAnnotation,
     'video_annotation': VideoAnnotation,
     'detection_object_bbox': DetectionObjectBBox,
-    'detection_object_polygon':DetectionObjectPolygon,
+    'detection_object_polygon': DetectionObjectPolygon,
     'track_object_polygon': TrackGTObjectPolygon,
     'track_object': TrackGTObjectBBox,
+    'predicted_object': PredictedObject,
     'bboxxyxy': BBoxXYXY,
     'rbboxxycenterwh': RBBoxXYCenterWHA,
     'polygon': Polygon,
     'datasetmeta': DatasetMeta,
     'internal_datasets_meta': _InternalDatasetsMeta,
     'internal_dataset_meta': _InternalDatasetMeta,
     'internal_dataset': _InternalDataset,
```

### Comparing `cvd-0.1.6/cvd/datasets/filters.py` & `cvd-0.1.7/cvd/datasets/filters.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/image_dataset.py` & `cvd-0.1.7/cvd/datasets/image_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from typing import Optional, List, Dict, Union, Tuple, Iterable, Callable
 from xml.etree import ElementTree
 from xml.dom import minidom
 
 from IPython.core.display import display
 from matplotlib import pyplot as plt
 
-from cvd.datasets.annotations.objects import DetectionObjectBBox, DetectionObjectPolygon, RBBoxXYCenterWHA
+from cvd.datasets.annotations.objects import DetectionObjectBBox, \
+    DetectionObjectPolygon, RBBoxXYCenterWHA, TrackGTObjectBBox, PredictedObject
 from cvd.datasets.annotations.image_annotation import ImageAnnotation
 from cvd.datasets.annotations.coco import COCODataset, COCOInfo, COCOLicense, COCOImage, COCOAnnotation, COCOCategory
 import numpy as np
 
 from cvd.datasets.filters import ObjectsFilter
 from cvd.datasets.image_dataset_item import ImageDatasetItem
 from cvd.datasets.transformers import Transformer
@@ -240,24 +241,39 @@
             return new_datasets
 
     def rename_labels(self, rename_map: Dict[str, str], inplace: bool = False):
         _rename_map = dict(map(lambda x: (x, x), self.labels))
         _rename_map.update(rename_map)
 
         def _rename(_img_ann: ImageAnnotation):
-            return ImageAnnotation(
-                objects=list(map(
-                    lambda x: DetectionObjectBBox(
-                        bbox=x.bbox,
-                        label=_rename_map[x.label],
-                        attributes=x.attributes
-                    ),
-                    _img_ann.objects
-                )),
-            )
+            objects = []
+            for obj in _img_ann.objects:
+                if isinstance(obj, TrackGTObjectBBox):
+                    objects.append(TrackGTObjectBBox(
+                        bbox=obj.bbox,
+                        track_id=obj.track_id,
+                        label=_rename_map[obj.label],
+                        attributes=obj.attributes
+                    ))
+                elif isinstance(obj, PredictedObject):
+                    objects.append(PredictedObject(
+                        bbox=obj.bbox,
+                        label=_rename_map[obj.label],
+                        confidence=obj.confidence,
+                        attributes=obj.attributes
+                    ))
+                elif isinstance(obj, DetectionObjectBBox):
+                    objects.append(DetectionObjectBBox(
+                        bbox=obj.bbox,
+                        label=_rename_map[obj.label],
+                        attributes=obj.attributes
+                    ))
+                else:
+                    raise Exception(f"Unsupported object type: {type(obj)}")
+            return ImageAnnotation(objects=objects)
 
         if inplace:
             labels = []
             for id, ann in self._annotations.items():
                 self._annotations[id] = _rename(ann)
                 labels += self._annotations[id].labels
             self._labels = sorted(list(set(labels)))
```

### Comparing `cvd-0.1.6/cvd/datasets/image_dataset_item.py` & `cvd-0.1.7/cvd/datasets/image_dataset_item.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/importer/cocoimages.py` & `cvd-0.1.7/cvd/datasets/importer/cocoimages.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/importer/rawimages.py` & `cvd-0.1.7/cvd/datasets/importer/rawimages.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/importer/rawvideo.py` & `cvd-0.1.7/cvd/datasets/importer/rawvideo.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/interfaces/idataset.py` & `cvd-0.1.7/cvd/datasets/interfaces/idataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             if not items_filter.filter(ds_item):
                 new_ds.add_item(ds_item.file_info, ds_item.annotations)
         return new_ds
 
     def add_item(self, file_info: FileInfo, annotation: IAnnotation):
         if file_info.unique_id in self._annotations:
             raise DuplicationError(f"A file with a unique id `{file_info.abs_path} `exists in the dataset")
-
         self._files.append(file_info)
         unique_id = file_info.unique_id
         assert unique_id not in self._annotations, f"The unique_id in FileINfo isn't unique. " \
                                                    f"For the following id {unique_id} dataset contains following data:"\
                                                    f"file_info = {self._files_index[unique_id]} " \
                                                    f"and annotations = {self._annotations[unique_id]}"
         self._annotations[file_info.unique_id] = annotation
```

### Comparing `cvd-0.1.6/cvd/datasets/interfaces/interface.py` & `cvd-0.1.7/cvd/datasets/interfaces/interface.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/meta.py` & `cvd-0.1.7/cvd/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/selection.py` & `cvd-0.1.7/cvd/datasets/selection.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/torchdataset.py` & `cvd-0.1.7/cvd/datasets/torchdataset.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/transformations/normalize.py` & `cvd-0.1.7/cvd/datasets/transformations/normalize.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/transformations/resize.py` & `cvd-0.1.7/cvd/datasets/transformations/resize.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/transformers.py` & `cvd-0.1.7/cvd/datasets/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
+from pathlib import Path
 from typing import Union, Optional
 
 import cv2
 from scipy.spatial.distance import cosine
 from sklearn.metrics import euclidean_distances
 
 from cvd.datasets.annotations.objects import DetectionObjectPolygon, TrackGTObjectPolygon, DetectionObjectBBox
```

### Comparing `cvd-0.1.6/cvd/datasets/video_dataset.py` & `cvd-0.1.7/cvd/datasets/video_dataset.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/video_dataset_item.py` & `cvd-0.1.7/cvd/datasets/video_dataset_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
             raise StopIteration
         else:
             frame_img = self._load_frame(self._current)
             frame_ann = self.annotations[self._current]
             self._current += 1
             return frame_img, frame_ann
 
+    def __len__(self):
+        return self.file_info.frames_number
+
     def get_frame(self, number: int):
         return self._load_frame(number)
 
     def _load_frame(self, frame_number: int) -> np.ndarray:
         if frame_number > self._last_frame:
             while self._last_frame != frame_number:
                 self._cap.grab()
```

### Comparing `cvd-0.1.6/cvd/datasets/zoo/datasets.py` & `cvd-0.1.7/cvd/datasets/zoo/datasets.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/internal_representation.py` & `cvd-0.1.7/cvd/datasets/zoo/internal_representation.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/cepdof.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/cepdof.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/coco.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/coco.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/crowdhuman.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/crowdhuman.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/feeds.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/feeds.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/habbof.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/habbof.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/mirrorworlds.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/mirrorworlds.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/mirrorworldsrotated.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/mirrorworldsrotated.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/mwr.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/mwr.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/wepdtof.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/wepdtof.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/widerface.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/widerface.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/datasets/zoo/raw/widerperson.py` & `cvd-0.1.7/cvd/datasets/zoo/raw/widerperson.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/models/interface.py` & `cvd-0.1.7/cvd/models/interface.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/tools/perception_benchmarks.py` & `cvd-0.1.7/cvd/tools/perception_benchmarks.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/tools/s3.py` & `cvd-0.1.7/cvd/tools/s3.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/visualization/annotations.py` & `cvd-0.1.7/cvd/visualization/annotations.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/visualization/dataset.py` & `cvd-0.1.7/cvd/visualization/dataset.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/visualization/objects.py` & `cvd-0.1.7/cvd/visualization/objects.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/cvd/visualization/tools.py` & `cvd-0.1.7/cvd/visualization/tools.py`

 * *Files identical despite different names*

### Comparing `cvd-0.1.6/pyproject.toml` & `cvd-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvd"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["bogoslovskiy_nn <bogoslovskiy_nn@bw-sw.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 albumentations = "^1.3.0"
```

### Comparing `cvd-0.1.6/PKG-INFO` & `cvd-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvd
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: bogoslovskiy_nn
 Author-email: bogoslovskiy_nn@bw-sw.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

