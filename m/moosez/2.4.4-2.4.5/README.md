# Comparing `tmp/moosez-2.4.4.tar.gz` & `tmp/moosez-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.4.tar", last modified: Wed Mar 20 14:37:23 2024, max compression
+gzip compressed data, was "moosez-2.4.5.tar", last modified: Wed Apr 10 09:25:55 2024, max compression
```

## Comparing `moosez-2.4.4.tar` & `moosez-2.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:37:23.992593 moosez-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-20 14:37:14.000000 moosez-2.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-20 14:37:23.992593 moosez-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-03-20 14:37:14.000000 moosez-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:37:23.988593 moosez-2.4.4/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:37:23.992593 moosez-2.4.4/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-03-20 14:37:14.000000 moosez-2.4.4/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:37:23.992593 moosez-2.4.4/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-20 14:37:23.000000 moosez-2.4.4/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:37:23.992593 moosez-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-20 14:37:14.000000 moosez-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.327526 moosez-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 09:25:47.000000 moosez-2.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 09:25:55.323526 moosez-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-04-10 09:25:47.000000 moosez-2.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-10 09:25:47.000000 moosez-2.4.5/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:25:55.323526 moosez-2.4.5/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 09:25:55.000000 moosez-2.4.5/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:25:55.327526 moosez-2.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-10 09:25:47.000000 moosez-2.4.5/setup.py
```

### Comparing `moosez-2.4.4/LICENSE` & `moosez-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/PKG-INFO` & `moosez-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.4
+Version: 2.4.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.4/README.md` & `moosez-2.4.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 </picture>
 </div>
 
 ## Star History 🤩
 
 <a href="https://star-history.com/#QIMP-Team/MOOSE&Date">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=QIMP-Team/MOOSE&type=Date&theme=dark" />
-    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=QIMP-Team/MOOSE&type=Date" />
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=ENHANCE-PET/MOOSE&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=ENHANCE-PET/MOOSE&type=Date" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=QIMP-Team/MOOSE&type=Date" />
   </picture>
 </a>
 
 
 
 ## Citations ❤️ 
@@ -294,16 +294,30 @@
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
 
 ## 🦌 MOOSE: A part of the [enhance.pet](https://enhance.pet) community
 
 ![Alt Text](https://github.com/QIMP-Team/MOOSE/blob/main/Images/Enhance.gif)
-<p align="right">Above image generated by Midjourney</p>
 
-## [![Repography logo](https://images.repography.com/logo.svg)](https://repography.com) / Recent activity [![Time period](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_badge.svg)](https://repography.com)
-[![Timeline graph](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_timeline.svg)](https://github.com/LalithShiyam/MOOSE/commits)
-[![Issue status graph](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_issues.svg)](https://github.com/LalithShiyam/MOOSE/issues)
-[![Pull request status graph](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_prs.svg)](https://github.com/LalithShiyam/MOOSE/pulls)
-[![Trending topics](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_words.svg)](https://github.com/LalithShiyam/MOOSE/commits)
-[![Top contributors](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_users.svg)](https://github.com/LalithShiyam/MOOSE/graphs/contributors)
-[![Activity map](https://images.repography.com/41227991/LalithShiyam/MOOSE/recent-activity/SyuBS4BfKPzTpJakc5ZBD8rkyz8nw0_fBA88YASAfEw/uDuGB8dDyAsfibx9qdNa6LulUe8EsIpMJhtV6nS3xc0_map.svg)](https://github.com/LalithShiyam/MOOSE/commits)
+## 👥 Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/LalithShiyam"><img src="https://github.com/LalithShiyam.png?s=100" width="100px;" alt="Lalith Kumar Shiyam Sundar"/><br /><sub><b>Lalith Kumar Shiyam Sundar</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=LalithShiyam" title="Code">💻</a> <a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=LalithShiyam" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Keyn34"><img src="https://github.com/Keyn34.png?s=100" width="100px;" alt="Sebastian Gutschmayer"/><br /><sub><b>Sebastian Gutschmayer</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=Keyn34" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/n7k-dobri"><img src="https://avatars.githubusercontent.com/u/114534264?v=4?s=100" width="100px;" alt="n7k-dobri"/><br /><sub><b>n7k-dobri</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=n7k-dobri" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mprires"><img src="https://avatars.githubusercontent.com/u/48754309?v=4?s=100" width="100px;" alt="Manuel Pires"/><br /><sub><b>Manuel Pires</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=mprires" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.meduniwien.ac.at/web/forschung/researcher-profiles/researcher-profiles/index.php?id=688&res=zacharias_chalampalakis1"><img src="https://avatars.githubusercontent.com/u/62066397?v=4?s=100" width="100px;" alt="Zach Chalampalakis"/><br /><sub><b>Zach Chalampalakis</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=zax0s" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dhaberl"><img src="https://avatars.githubusercontent.com/u/54232863?v=4?s=100" width="100px;" alt="David Haberl"/><br /><sub><b>David Haberl</b></sub></a><br /><a href="https://github.com/ENHANCE-PET/MOOSE/commits?author=dhaberl" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `moosez-2.4.4/moosez/constants.py` & `moosez-2.4.5/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/display.py` & `moosez-2.4.5/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/download.py` & `moosez-2.4.5/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/file_utilities.py` & `moosez-2.4.5/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/image_conversion.py` & `moosez-2.4.5/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/image_processing.py` & `moosez-2.4.5/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/input_validation.py` & `moosez-2.4.5/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/moosez.py` & `moosez-2.4.5/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.4.5/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.4.5/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/predict.py` & `moosez-2.4.5/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/moosez/resources.py` & `moosez-2.4.5/moosez/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         "directory": "Dataset600_Original_bones",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_all_bones_",
         "configuration": "3d_fullres"
     },
     "clin_ct_PUMA": {
-        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_PUMA_06112023.zip",
+        "url": "https://ucd-emic-muv.s3.us-west-2.amazonaws.com/moose/clin_ct_puma_04042024.zip",
         "filename": "Dataset002_PUMA.zip",
         "directory": "Dataset002_PUMA",
         "trainer": "nnUNetTrainer_2000epochs",
         "voxel_spacing": [1.5, 1.5, 1.5],
         "multilabel_prefix": "Clin_CT_PUMA_",
         "configuration": "3d_fullres"
     },
```

### Comparing `moosez-2.4.4/moosez.egg-info/PKG-INFO` & `moosez-2.4.5/moosez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.4
+Version: 2.4.5
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.4/moosez.egg-info/SOURCES.txt` & `moosez-2.4.5/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.4/setup.py` & `moosez-2.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.4',
+    version='2.4.5',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9.2',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

