# Comparing `tmp/pyppbox-3.5b2.tar.gz` & `tmp/pyppbox-3.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.5b2.tar", last modified: Mon Mar 25 10:13:04 2024, max compression
+gzip compressed data, was "pyppbox-3.6b1.tar", last modified: Wed Apr 10 20:09:22 2024, max compression
```

## Comparing `pyppbox-3.5b2.tar` & `pyppbox-3.6b1.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.355253 pyppbox-3.5b2/
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-03-25 10:12:58.000000 pyppbox-3.5b2/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 10:12:58.000000 pyppbox-3.5b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-25 10:12:58.000000 pyppbox-3.5b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-03-25 10:13:04.355253 pyppbox-3.5b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-25 10:12:58.000000 pyppbox-3.5b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-03-25 10:12:58.000000 pyppbox-3.5b2/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.339253 pyppbox-3.5b2/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.339253 pyppbox-3.5b2/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.339253 pyppbox-3.5b2/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/cfg/cfg.7z
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.335253 pyppbox-3.5b2/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.343253 pyppbox-3.5b2/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.347252 pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.351252 pyppbox-3.5b2/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/standalone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52132 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/standalone/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.355253 pyppbox-3.5b2/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/mot2pyppbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.355253 pyppbox-3.5b2/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-03-25 10:13:04.000000 pyppbox-3.5b2/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-25 10:13:04.000000 pyppbox-3.5b2/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 10:13:04.000000 pyppbox-3.5b2/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-25 10:13:04.000000 pyppbox-3.5b2/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 10:13:04.000000 pyppbox-3.5b2/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-25 10:12:58.000000 pyppbox-3.5b2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 10:13:04.355253 pyppbox-3.5b2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-25 10:12:58.000000 pyppbox-3.5b2/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-25 10:12:58.000000 pyppbox-3.5b2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-25 10:12:58.000000 pyppbox-3.5b2/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 10:13:04.355253 pyppbox-3.5b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-03-25 10:12:58.000000 pyppbox-3.5b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-25 10:12:58.000000 pyppbox-3.5b2/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-10 20:09:15.000000 pyppbox-3.6b1/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 20:09:15.000000 pyppbox-3.6b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-10 20:09:15.000000 pyppbox-3.6b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-10 20:09:22.893230 pyppbox-3.6b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-10 20:09:15.000000 pyppbox-3.6b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-10 20:09:15.000000 pyppbox-3.6b1/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/cfg.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.873230 pyppbox-3.6b1/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52132 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/standalone/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/mot2pyppbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:09:22.893230 pyppbox-3.6b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-10 20:09:15.000000 pyppbox-3.6b1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-10 20:09:15.000000 pyppbox-3.6b1/setup_extra.yaml
```

### Comparing `pyppbox-3.5b2/GETSTARTED.md` & `pyppbox-3.6b1/GETSTARTED.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 # 🚀 Getting Started
 
-Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependencies or requirements for the modules you needs.
+Installing `pyppbox` is very easy and straightforward. You can install it from [PyPI](https://pypi.org/project/pyppbox/) directly or use the prebuilt `.whl` files on [GitHub releases](https://github.com/rathaumons/pyppbox/releases) or install from GitHub directly or build it from source on your own machine. However, in order to get it work, you need to install all the necessary dependencies or requirements for the modules you need.
 
-🆕 `pyppbox` `v3.0b2+` supports all Windows, Linux and macOS. ***Use the most recent version of `pyppbox` for smoother experience!***
 
 ## ⚙️ Requirements
 
 All requirements are not strictly limited. However, some specific modules might need some special dependencies. For example, `YOLO_Classic` (With `.weights` model) relies on [OpenCV DNN](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html) in order to make use of GPU power. In this case, you might need to build OpenCV from source by yourself or use our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) instead of the official `opencv-contrib-python` which does not include GPU support.
 
 * Prerequisite: 
-  - (Optional) For NVIDIA GPU: [CUDA Toolkit 11.x/12.x](https://developer.nvidia.com/cuda-downloads) with default installation path
-  - (Optional) For NVIDIA GPU: [cuDNN 8.x.x](https://developer.nvidia.com/rdp/cudnn-download) with default installation path
   - Python [[3.9-3.12]](https://www.python.org/downloads/)
   - Local pyppbox repo: `git clone https://github.com/rathaumons/pyppbox.git`
 
 * Before you install dependencies/requirements:
   - For Linux, recommend changing `python3` to `python`: `sudo apt install python-is-python3`
   - If you prefer conda + Python [3.9-3.12]: `conda create --name pyppbox_env python=3.11`
-  - If you don't know whether to install only Tensorflow or PyTorch or both -> Check [Supported Modules](https://rathaumons.github.io/pyppbox/pyppbox/modules.html)
-  - For Tensorflow with GPU support -> [See here](https://www.tensorflow.org/install/pip)
+  - Upgrade `pip` and `setuptools`:
+    ```
+    python -m pip install --upgrade pip
+    pip install "setuptools>=67.2.0"
+    ```
+  - Recommend removing the official `ultralytics`:
+    ```
+    pip uninstall -y ultralytics
+    ```
 
 * Install dependencies/requirments under `pyppbox/requirements/`: 
   - On Windows, recommend using the `cmd` installer:
     - For GPU: `install_req_py3_cuda121.cmd` (Or `install_req_py3_cuda.cmd` for CUDA 11.8)
     - For CPU-only: `install_req_py3_cpu.cmd`
   - On Linux:
     - For GPU:
       ```
-      python -m pip install --upgrade pip
-      pip uninstall -y ultralytics # Remove the official ultralytics
-      pip install "setuptools>=67.2.0"
       pip install torch torchvision torchaudio
       pip install -r requirements.txt
       ```
     - For CPU-only:
       ```
-      python -m pip install --upgrade pip
-      pip uninstall -y ultralytics # Remove the official ultralytics
-      pip install "setuptools>=67.2.0"
       pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
       pip install -r requirements.txt
       ```
   - On macOS:
     - For GPU: Not available
     - For CPU:
       ```
-      python -m pip install --upgrade pip
-      pip uninstall -y ultralytics # Remove the official ultralytics
-      pip install "setuptools>=67.2.0"
       pip install torch torchvision torchaudio
       pip install -r requirements.txt
       ```
 
 * (Optional) For GPU-Only -> Verify the installed dependencies:
   - Execute the `test_gpu.py`
     - On Windows -> `test_gpu.cmd`
     - On Linux -> `python test_gpu.py`
   - If there is no error, then you are all good and ready to go.
   - For OpenCV, the official `opencv-contrib-python` (No GPU support) is set in the `requirements.txt` file. If you need GPU support, check our [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) or build one from source by yourself.
 
-* ⚠️ ***Notes:***
-  - For CPU-Only, YOLO Ultralytics uses GPU by default, you must set `cpu` as string for the parameter `device` in its configuration.
-  - For GPU on Windows, [Tensorflow 2.11+ no long provides native GPU support](https://www.tensorflow.org/install/pip#windows-native). 
+* ***ATTENTION*** ⚠️⚠️⚠️
+  - If you use YOLO Ultralytics without GPU, you need to set `cpu` as string for the parameter `device` in its configuration.
 
 
 ## 💽 Setup
 
 You need to install the main package which is `pyppbox` and the data for the modules you need `pyppbox-data-xxx`. If you want to have some fun for the demo on our [GTA_V_DATASET](https://github.com/rathaumons/PoseTReID_DATASET), you also need to install `pyppbox-data-gta5`.
 
 * Install `pyppbox`
@@ -75,19 +69,16 @@
     ``` 
   - Or install directly from GitHub:
     ```
     pip install git+https://github.com/rathaumons/pyppbox.git
     ```
   - Or build from source:
     ```
-    pip install "setuptools>=67.2.0"
     pip install wheel build PyYAML
     python -m build --wheel --skip-dependency-check --no-isolation
-    cd dist
-    pip install pyppbox-xxx.whl
     ```
 
 * Install [`pyppbox-data-xxx`](https://github.com/rathaumons/pyppbox-data/)
   - Download the latest from [releases](https://github.com/rathaumons/pyppbox-data/releases)
   - Or install the ones you need directly:
     ```
     pip install https://github.com/rathaumons/pyppbox-data/releases/download/v1.1.1/pyppbox_data_yolocls-1.1.1-py3-none-any.whl
@@ -100,23 +91,23 @@
 * Install [`pyppbox-data-gta5`](https://github.com/rathaumons/PoseTReID_DATASET#-introducing-pyppbox-data-gta5)
   - Download the latest from [releases](https://github.com/rathaumons/PoseTReID_DATASET/releases)
   - Or install directly:
     ```
     pip install https://github.com/rathaumons/PoseTReID_DATASET/releases/download/v2.0/pyppbox_data_gta5-2.0-py3-none-any.whl
     ```
 
-* (Optional) Quick Test
-  - On your terminal or CMD:
+* Quick Test
+  - In your Python terminal:
     ```
-    python
     import pyppbox
     pyppbox.launchGUI()
     ```
-  - Now you should see the GUI of pyppbox for easy demo.
-    <details><summary><ins>Show GUI example!</ins></summary><img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui.jpg"></details>
+    Now you should see the GUI demo like this screenshot:
+    <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/pyppbox/pyppbox_gui.jpg">
+  - For related GUI functions and other configurations, check the [Configurations page](https://rathaumons.github.io/pyppbox/pyppbox/config.html).
   - For ***Linux***, if the GUI does not work, you might need to install these:
     ```
     sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
     ```
   - For ***Ubuntu on WSL 2***, you need to install these:
     ```
     sudo apt-get install libgl1-mesa-glx
```

### Comparing `pyppbox-3.5b2/LICENSE` & `pyppbox-3.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/PKG-INFO` & `pyppbox-3.6b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.5b2
+Version: 3.6b1
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -51,16 +51,14 @@
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
 Requires-Dist: lapx
-Requires-Dist: pyunpack
-Requires-Dist: patool
 Requires-Dist: PyQt6
 Requires-Dist: pyppbox-torchreid
 Requires-Dist: pyppbox-ultralytics>=8.0.218
 
 # 🐍📦 [**pyppbox**](https://github.com/rathaumons/pyppbox)
 
 <div align="center">
@@ -75,12 +73,12 @@
 
 </div>
 
 ***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of code. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Integrate GUI for easy configurations and demo.
-* Support dictionary and YAML/JSON configurations.
+* Integrate GUI for easy configuration and demo.
+* Support dictionary and YAML/JSON configuration.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.5b2/README.md` & `pyppbox-3.6b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
 </div>
 
 ***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of code. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Integrate GUI for easy configurations and demo.
-* Support dictionary and YAML/JSON configurations.
+* Integrate GUI for easy configuration and demo.
+* Support dictionary and YAML/JSON configuration.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.5b2/RELEASENOTES.md` & `pyppbox-3.6b1/RELEASENOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Release Notes 
 
 ## **pyppbox V3 - Make Simpler and Faster**
 
+* `pyppbox` [v3.6b1](https://github.com/rathaumons/pyppbox/tree/v3.5b2)
+
+  - Replace `pyunpack` & `patool` with `shutil`
+  - Improve Example 9 - example_09_eva_offline.py
+  - Add `pyppbox.gui.guitools` to the documentations
+  - Fix `useInternalConfigDir()` in `pyppbox.gui.guitools`
+  - Fix sphinx-build warning for utils.rst
+  - Fix and improve documentations
+  - **Known issue/limitation**:
+    - You tell me :)
+
 * `pyppbox` [v3.5b2](https://github.com/rathaumons/pyppbox/tree/v3.5b2)
 
   - Increase default random ID range in evatools
   - Add exception to `generateStaticID()` in `pyppbox.utils.evatools.TKOReider`
   - Update documentations
   - **Known issue/limitation**:
     - You tell me :)
```

### Comparing `pyppbox-3.5b2/pyppbox/__init__.py` & `pyppbox-3.6b1/pyppbox/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.5b2'
+__version__ = '3.6b1'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.5b2/pyppbox/config/__init__.py` & `pyppbox-3.6b1/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.6b1/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.6b1/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.6b1/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/configtools.py` & `pyppbox-3.6b1/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/myconfig.py` & `pyppbox-3.6b1/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/config/unifiedstrings.py` & `pyppbox-3.6b1/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/__init__.py` & `pyppbox-3.6b1/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/assets/TReID.png` & `pyppbox-3.6b1/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/assets/icon.ico` & `pyppbox-3.6b1/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/assets/settings.ico` & `pyppbox-3.6b1/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/guidemo.py` & `pyppbox-3.6b1/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/guihub.py` & `pyppbox-3.6b1/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/guitools.py` & `pyppbox-3.6b1/pyppbox/gui/guitools.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 import os
 import sys
 import subprocess as sp
 
-from pyppbox.utils.logtools import add_warning_log, add_error_log
+from pyppbox.utils.logtools import add_info_log, add_warning_log, add_error_log
 from pyppbox.config.configtools import PYPPBOXStructure, loadDocument, loadListDocument
 from pyppbox.utils.commontools import getAbsPathFDS, joinFPathFull, isExist
 from pyppbox.gui.guihub import writeUITMP
 
 current_dir = os.path.dirname(__file__)
 pyppbox_struct = PYPPBOXStructure()
 __cfgdir__ =  pyppbox_struct.cfg_dir
@@ -48,16 +48,17 @@
     __cfgdir__ = getAbsPathFDS(cfg_dir)
     pyppbox_struct.setCustomCFG(cfg_dir)
     add_warning_log("FYI: This basic method only serves GUI submodule `pyppbox.gui`.")
 
 def useInternalConfigDir():
     """Use the internal config directory, :code:`{pyppbox root}/confog/cfg` inside pyppbox package.
     """
-    global pyppbox_struct
+    global pyppbox_struct, __cfgdir__
     pyppbox_struct = PYPPBOXStructure()
+    __cfgdir__ =  pyppbox_struct.cfg_dir
     add_warning_log("FYI: This basic method only serves GUI submodule `pyppbox.gui`.")
 
 def showMainConfig():
     """Print JSON dictionary of the configurations in main.yaml.
     """
     print(loadDocument(pyppbox_struct.main_yaml))
     add_warning_log("FYI: This basic method only serves GUI submodule `pyppbox.gui`.")
@@ -81,17 +82,18 @@
     add_warning_log("FYI: This basic method only serves GUI submodule `pyppbox.gui`.")
 
 def resetInternalConfig():
     """Reset the internal configurations.
     """
     global pyppbox_struct
     pyppbox_struct = PYPPBOXStructure()
-    from pyunpack import Archive
-    Archive(os.path.join(pyppbox_struct.cfg_dir, 'cfg.7z')).extractall(pyppbox_struct.cfg_dir)
-    print("Reset successfully!")
+    cfg_zip = os.path.join(pyppbox_struct.cfg_dir, 'cfg.zip')
+    import shutil
+    shutil.unpack_archive(cfg_zip, pyppbox_struct.cfg_dir)
+    add_info_log("Reset successfully!")
     add_warning_log("FYI: This basic method only serves GUI submodule `pyppbox.gui`.")
 
 def launchGUI():
     """Launch GUI configuration tool of pyppbox.
     """
     writeUITMP(__cfgdir__)
     p = sp.Popen([sys.executable, os.path.join(current_dir, 'ui_launcher.py')])
@@ -108,23 +110,20 @@
     ----------
     config_dir : str
         A path of configuration directory.
     auto_launch_gui : bool, default=True
         An indication of whether to load and launch GUI from the :obj:`config_dir`.
     """
     if isExist(cfg_dir):
-        abspath = getAbsPathFDS(cfg_dir)
         global pyppbox_struct
+        abspath = getAbsPathFDS(cfg_dir)
+        cfg_zip = os.path.join(pyppbox_struct.cfg_dir, 'cfg.zip')
         try:
-            from pyunpack import Archive
-            Archive(os.path.join(pyppbox_struct.cfg_dir, 'cfg.7z')).extractall(abspath)
-            try:
-                os.remove(joinFPathFull(abspath, 'strings.yaml'))
-            except Exception:
-                pass
+            import shutil
+            shutil.unpack_archive(cfg_zip, abspath)
             if auto_launch_gui:
                 useThisConfigDir(abspath)
                 launchGUI()
         except Exception as e:
             msg = "generateCFG() -> " + str(e)
             add_error_log(msg)
             raise print(msg)
```

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_centroid.py` & `pyppbox-3.6b1/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.6b1/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_facenet.py` & `pyppbox-3.6b1/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_gt.py` & `pyppbox-3.6b1/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_launcher.py` & `pyppbox-3.6b1/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_sort.py` & `pyppbox-3.6b1/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.6b1/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.6b1/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.6b1/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/standalone/__init__.py` & `pyppbox-3.6b1/pyppbox/standalone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/standalone/mt.py` & `pyppbox-3.6b1/pyppbox/standalone/mt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/__init__.py` & `pyppbox-3.6b1/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/commontools.py` & `pyppbox-3.6b1/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/evatools.py` & `pyppbox-3.6b1/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/gttools.py` & `pyppbox-3.6b1/pyppbox/utils/gttools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/logtools.py` & `pyppbox-3.6b1/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/mot2pyppbox.py` & `pyppbox-3.6b1/pyppbox/utils/mot2pyppbox.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/persontools.py` & `pyppbox-3.6b1/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/restools.py` & `pyppbox-3.6b1/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox/utils/visualizetools.py` & `pyppbox-3.6b1/pyppbox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.6b1/pyppbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.5b2
+Version: 3.6b1
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
@@ -51,16 +51,14 @@
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
 Requires-Dist: lapx
-Requires-Dist: pyunpack
-Requires-Dist: patool
 Requires-Dist: PyQt6
 Requires-Dist: pyppbox-torchreid
 Requires-Dist: pyppbox-ultralytics>=8.0.218
 
 # 🐍📦 [**pyppbox**](https://github.com/rathaumons/pyppbox)
 
 <div align="center">
@@ -75,12 +73,12 @@
 
 </div>
 
 ***pyppbox*** is an all-in-one Python toolbox which can be used for detecting, tracking, and re-identifying people with only a few lines of code. It is originally made for [***PoseTReID framework***](https://github.com/rathaumons/PoseTReID_DATASET) which can effectively track specific/certain people across multiple cameras or video scenes in distributed contexts of people interaction spaces such as malls or amusement parks, etc.
 
 * ` pyppbox = Python + People + Toolbox `
 * Design for both short and long term people detecting, tracking, and re-identifying.
-* Integrate GUI for easy configurations and demo.
-* Support dictionary and YAML/JSON configurations.
+* Integrate GUI for easy configuration and demo.
+* Support dictionary and YAML/JSON configuration.
 * Support [[GTA_V_Dataset]](https://github.com/rathaumons/PoseTReID_DATASET) -> Real-time online and offline evaluation.
 * Check our papers: 1 [[IEEE]](https://ieeexplore.ieee.org/document/9271712) | 2 [[IEEE]](https://ieeexplore.ieee.org/document/9946587) [[arxiv]](https://doi.org/10.48550/arxiv.2205.10086)
```

### Comparing `pyppbox-3.5b2/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.6b1/pyppbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 pyppbox.egg-info/dependency_links.txt
 pyppbox.egg-info/requires.txt
 pyppbox.egg-info/top_level.txt
 pyppbox/config/__init__.py
 pyppbox/config/configtools.py
 pyppbox/config/myconfig.py
 pyppbox/config/unifiedstrings.py
-pyppbox/config/cfg/cfg.7z
+pyppbox/config/cfg/cfg.zip
 pyppbox/config/cfg/detectors.yaml
 pyppbox/config/cfg/main.yaml
 pyppbox/config/cfg/reiders.yaml
 pyppbox/config/cfg/trackers.yaml
 pyppbox/config/strings/strings.yaml
+pyppbox/config/strings/strings.zip
 pyppbox/data/datasets/.gitignore
 pyppbox/data/logs/.gitignore
 pyppbox/data/modules/.gitignore
 pyppbox/data/res/.gitignore
 pyppbox/data/res/idmap.txt
 pyppbox/gui/__init__.py
 pyppbox/gui/guidemo.py
```

### Comparing `pyppbox-3.5b2/requirements/requirements.txt` & `pyppbox-3.6b1/requirements/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 # https://pytorch.org/get-started/
 torch
 torchvision
 torchaudio
 ### Tracker: SORT
 filterpy
 lapx
-### Compression
-pyunpack
-patool
 ### GUI
 PyQt6
 ### Customized pyppbox-torchreid
 pyppbox-torchreid
 ### Customized pyppbox-ultralytics
 pyppbox-ultralytics>=8.0.218
 ### Unused
```

### Comparing `pyppbox-3.5b2/requirements/test_gpu.py` & `pyppbox-3.6b1/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/setup.py` & `pyppbox-3.6b1/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.5b2/setup_extra.yaml` & `pyppbox-3.6b1/setup_extra.yaml`

 * *Files identical despite different names*

